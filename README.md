GitLab Runner
=============

An Ansible role for install GitLab Runner.

Requirements
------------

- Supported version of Ansible: 2.12 and highter.
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

Role Variables
--------------

- `gitlab_runner_package_version` The specific version of Gitlab Runner to install (default: `''`).
- `gitlab_runner_repository_mirror` Mirror of `Gitlab` repository (default: `https://packages.gitlab.com/runner/gitlab-runner`).
- `gitlab_runner_repository_key_url` URL to `Gitlab's` GPG public key file (default: `https://packages.gitlab.com/runner/gitlab-runner/gpgkey`)

Dependencies
------------

None.

Example Playbook
----------------

- Install `Gitlab Runner`:

  ```yaml
  ---
  - name: 'Install gitlab-runner'
    hosts: all

    roles:
      - role: antmelekhin.gitlab_runner
  ```

- Install and configure `Gitlab Runner` with shell executor:

  ```yaml
  ---
  - name: 'Install gitlab-runner'
    hosts: all

    roles:
      - role: antmelekhin.gitlab_runner

    post_tasks:
      - name: 'Register gitlab-runner'
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
