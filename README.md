Role Name
=========

An Ansible role for install GitLab Runners.

Requirements
------------

- Supported version of Ansible: 2.9 and highter.
- Supported platforms:
  - Debian
    - 10
    - 11
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

  ```yaml
  ---
  - name: 'Install gitlab-runner'
    hosts: all

    roles:
      - role: antmelekhin.gitlab_runner
  ```

License
-------

MIT

Author Information
------------------

Melekhin Anton.
