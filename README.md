GitLab Runner
=============

An Ansible role to install [GitLab Runner](https://docs.gitlab.com/runner/).

Update to 2.x
-------------

The role version 1.x contains the task `Pin Gitlab Runner APT repository` that creates the pinning configuration file and actual for Debian Stretch only.
I've removed this task because it brakes package version selection in `Install Gitlab Runner package` task, and the role doesn’t support the Debian Stretch.
To continue using this role without side effects, you'll need to delete the pinning configuration file manually or add appropriate task in your ansible playbook file.

```yaml
- name: 'Install GitLab Runner'
  hosts: all

  pre_tasks:
    - name: 'Remove GitLab Runner APT pinning file'
      ansible.builtin.file:
        path: '/etc/apt/preferences.d/99-gitlab-runner'
        state: absent
      become: true

  roles:
    - role: antmelekhin.gitlab_runner
```

Update to 3.x
-------------

Since the 3.0.0 version of the role, some variables have changed. You will need to update them in your playbooks.

- `gitlab_runner_download_url` to `gitlab_runner_binary_download_url`
- `gitlab_runner_download_path` to `gitlab_runner_binary_download_path`
- `gitlab_runner_install_path` to `gitlab_runner_binary_install_path`

Requirements
------------

- Supported version of Ansible: 2.12 and higher. Systems with Python versions below than 3.7 are not compatible with ansible-core 2.17 (see [ansible/ansible#83357](https://github.com/ansible/ansible/issues/83357#issuecomment-2150254754)).
- `pywinrm` is a python library for connection Ansible to Windows hosts via [WinRM](https://docs.ansible.com/ansible/latest/user_guide/windows_winrm.html).
- Supported platforms:
  - Amazon Linux
    - 2
    - 2023
  - Debian
    - 10
    - 11
    - 12
  - Fedora
    - 39
    - 40
  - MacOSX
    - all
  - RHEL
    - 7
    - 8
    - 9
  - Ubuntu
    - 18.04
    - 20.04
    - 22.04
  - Windows
    - all

Role Variables
--------------

All variables that can be overridden are stored in the [defaults/main.yml](https://github.com/antmelekhin/ansible-role-gitlab-runner/blob/main/defaults/main.yml) file.
Please refer to the [meta/argument_specs.yml](https://github.com/antmelekhin/ansible-role-gitlab-runner/blob/main/meta/argument_specs.yml) file for a description of the available variables.
Similarly, descriptions and defaults for preset variables can be found in the [vars/main.yml](https://github.com/antmelekhin/ansible-role-gitlab-runner/blob/main/vars/main.yml) file.

Dependencies
------------

When using Ansible core, you will also need to install the following Ansible collections:

```yaml
---
collections:
  - name: community.general
  - name: community.windows
```

Example Playbook
----------------

Install GitLab Runner:

```yaml
---
- name: 'Install GitLab Runner'
  hosts: all

  roles:
    - role: antmelekhin.gitlab_runner
```

Install GitLab Runner v16.9.1:

```yaml
---
- name: 'Install GitLab Runner v16.9.1'
  hosts: all

  roles:
    - role: antmelekhin.gitlab_runner
      gitlab_runner_package_version: '16.9.1-1'
```

Install GitLab Runner and configure the shell executor:

```yaml
---
- name: 'Install GitLab Runner'
  hosts: all

  roles:
    - role: antmelekhin.gitlab_runner

  post_tasks:
    - name: 'Register GitLab Runner'
      ansible.builtin.copy:
        content: |
          concurrent = 1
          check_interval = 0
          shutdown_timeout = 0

          [session_server]
            session_timeout = 1800

          [[runners]]
            name = "{{ ansible_fqdn }}"
            url = "https://gitlab.com"
            token = "xxxxxxxxxxxx"
            executor = "shell"
        dest: '/etc/gitlab-runner/config.toml'
        owner: 'root'
        group: 'root'
        mode: 0600
```

License
-------

MIT

Author Information
------------------

Melekhin Anton.
