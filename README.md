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

Requirements
------------

- Supported version of Ansible: 2.12 and highter.
- `pywinrm` is a python library for connection Ansible to Windows hosts via [WinRM](https://docs.ansible.com/ansible/latest/user_guide/windows_winrm.html).
- Supported platforms:
  - Debian
    - 10
    - 11
    - 12
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

- `gitlab_runner_package_version` The version of the GitLab Runner package. By default, GitLab Runner is installed with the latest available version.
- `gitlab_runner_repository_mirror_url` The GitLab repository mirror (default: `https://packages.gitlab.com/runner/gitlab-runner`).
- `gitlab_runner_repository_gpgkey_url` URL to GitLab repository GPG key file (default: `https://packages.gitlab.com/runner/gitlab-runner/gpgkey`).
- `gitlab_runner_binary_version` The version of the GitLab Runner binary (default: `17.1.0`).
- `gitlab_runner_binary_name` The GitLab Runner binary name (default: `gitlab-runner-windows-amd64`).
- `gitlab_runner_download_url` URL to download the GitLab Runner binary (default: `https://gitlab-runner-downloads.s3.amazonaws.com/v17.1.0/binaries`).
- `gitlab_runner_download_path` Local path to download and extract the binary (default: `/tmp`).
- `gitlab_runner_install_path` GitLab Runner installation folder (default: `C:\Program Files\gitlab-runner`).

Dependencies
------------

None.

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
