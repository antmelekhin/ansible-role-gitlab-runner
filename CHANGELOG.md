# Changelog

## [2.2.2](https://github.com/antmelekhin/ansible-role-gitlab-runner/compare/v2.2.1...v2.2.2) (2024-05-12)


### Documentation

* **README:** update documentation ([600a19d](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/600a19dfdc11159737556235ed76396f02e777d7))


### Fixes

* add `ca-certificates` package ([1d0622c](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/1d0622c9d89b2ff1b0237fe76b9fd253a4d9ecb7))
* use apt source config and gpgkey names from GitLab installation script ([9b2d98c](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/9b2d98cb6f1524c34261513736ec99bb0b5e21ba))


### Styles

* minor changes ([58260d2](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/58260d26f5bc3dd5d28819b7dac02871b89d11ee))

## [2.2.1](https://github.com/antmelekhin/ansible-role-gitlab-runner/compare/v2.2.0...v2.2.1) (2024-05-11)


### Documentation

* **README:** update variables documentation ([5006406](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/5006406c604bc8faf06849c5f3d5c6554940f522))


### Styles

* rename tasks ([2e422a0](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/2e422a00c82c1f4f10f0a53d192d4beca47e1980))

## [2.2.0](https://github.com/antmelekhin/ansible-role-gitlab-runner/compare/v2.1.0...v2.2.0) (2024-05-09)


### Features

* add windows support ([#8](https://github.com/antmelekhin/ansible-role-gitlab-runner/issues/8)) ([6ef0022](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/6ef0022c0c038ae6924bc14d1fde54afb859ddcc))

## [2.1.0](https://github.com/antmelekhin/ansible-role-gitlab-runner/compare/v2.0.4...v2.1.0) (2024-05-05)


### Improvements

* add architecture for debian-based distros ([d82ef98](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/d82ef98f26636b09679db77fba61ea0ada9117e1))

## [2.0.4](https://github.com/antmelekhin/ansible-role-gitlab-runner/compare/v2.0.3...v2.0.4) (2024-04-28)


### Documentation

* **README:** fixed examples view for Ansible Galaxy ([d12c965](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/d12c965e81c33b6621ef818af44b2b4e38d01edd))


### Fixes

* fixed running a role in check_mode ([03182d9](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/03182d92fc4a4d2e4acda07337cb77eb6e1e97bf))


### Styles

* add newline to end of file ([4fc69c7](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/4fc69c7b5c8f0b49c49e887e3e02eda626d133b2))
* use double underline in register variable ([71536ff](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/71536fff0171d71bb028b4a080a6acd02d51a35f))


### Tests

* add .tox as ignore ([1a6a4c6](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/1a6a4c6abeda4509cc12f5ab757488f52d7b5461))
* add role_name prefix to instance name ([e557118](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/e557118fa14e26d3018ff2492959031490ba3e16))
* run linters in its own workflow ([5b64a88](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/5b64a88486f4e7fa278c9ceda56c14e41d752a9a))

## [2.0.3](https://github.com/antmelekhin/ansible-role-gitlab-runner/compare/v2.0.2...v2.0.3) (2024-04-20)


### Documentation

* **README:** update role variables description ([0f8fec6](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/0f8fec657ff890ba0b30eb02f4f834f0ba8312ea))

## [2.0.2](https://github.com/antmelekhin/ansible-role-gitlab-runner/compare/v2.0.1...v2.0.2) (2024-04-20)


### Code Refactoring

* update variable names, rm conditional expression, quote strings and rm loop for `include_vars` ([#7](https://github.com/antmelekhin/ansible-role-gitlab-runner/issues/7)) ([3acb973](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/3acb9735bc438138d13d7daad528b8bf495a52d5))


### Continuous Integration

* update workflows ([9904b65](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/9904b65b459eaf9193f81d511da9a33c93ec2374))

## [2.0.1](https://github.com/antmelekhin/ansible-role-gitlab-runner/compare/v2.0.0...v2.0.1) (2024-04-10)


### Fixes

* gpgkey value for redhat-based distros ([#6](https://github.com/antmelekhin/ansible-role-gitlab-runner/issues/6)) ([5f0558b](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/5f0558bf3a0cb0192e290ec00bcdca6e94fdc5e7))

## [2.0.0](https://github.com/antmelekhin/ansible-role-gitlab-runner/compare/v1.2.0...v2.0.0) (2024-03-31)


### ⚠ BREAKING CHANGES

* rm `Pin Gitlab Runner APT repository` task and add minor changes (#5)

### Continuous Integration

* fix publish workflow ([9d74d0d](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/9d74d0d7b87b3db1bfaada7fd0b2bce44f19cf94))
* update release rules ([6819e51](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/6819e5165df3812716d5ff4b98309b6149c2b2dd))


### Fixes

* rm `Pin Gitlab Runner APT repository` task and add minor changes ([#5](https://github.com/antmelekhin/ansible-role-gitlab-runner/issues/5)) ([83f90e9](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/83f90e95aba6645d597355a7be3bbf22fa05c999))


### Styles

* add `_gitlab_runner_apt_local_gpgkey` variable ([ffd3c88](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/ffd3c88efc14a294684ebce65a8d8d87e5a7fa12))
* update description and rename some task names ([#4](https://github.com/antmelekhin/ansible-role-gitlab-runner/issues/4)) ([1c0aa2f](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/1c0aa2fdc9b0a4698ba3a30a5606a44061b92571))

## [1.2.0](https://github.com/antmelekhin/ansible-role-gitlab-runner/compare/v1.1.1...v1.2.0) (2024-01-05)


### Improvements

* update variable names and rm useless repo ([#3](https://github.com/antmelekhin/ansible-role-gitlab-runner/issues/3)) ([47109b1](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/47109b162b9dec2e5c02061e90d1ea2b40b78a8c))

## [1.1.1](https://github.com/antmelekhin/ansible-role-gitlab-runner/compare/v1.1.0...v1.1.1) (2023-11-15)


### Code Refactoring

* code minor fixes ([#2](https://github.com/antmelekhin/ansible-role-gitlab-runner/issues/2)) ([1d16841](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/1d16841c1b1091f3ec25828a615c0d1bd15b60c2))


### Documentation

* add extra example ([03d0a25](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/03d0a25d307d9163a60f32e57c34200bfb654470))


### Tests

* add tox ([5f062f0](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/5f062f0bac1a9969f7083135953e6bf4ad4ad69a))

## [1.1.0](https://github.com/antmelekhin/ansible-role-gitlab-runner/compare/v1.0.0...v1.1.0) (2023-08-15)


### Continuous Integration

* update distros matrix ([1ae6871](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/1ae68711fa88d223a2132b5de08cb984eb2db14f))


### Documentation

* fix README ([5af25ee](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/5af25ee9abdd426323f11e66d9386df1655ea58b))


### Fixes

* package version selection ([f8e324f](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/f8e324fb6c14ce270e7a4bb8b8abab0344e53fb3))


### Improvements

* distribution select ([1d6f490](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/1d6f49038ae7843685b96b7237bada6ec7fd2d95))


### Tests

* add version check ([31dbc9f](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/31dbc9ffd73958f02b4a9f7d06371b8df337f71a))
* fix task name ([94c62ec](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/94c62ec722ac1c1bfe70b5446754642a32e1fce3))

## [1.0.0](https://github.com/antmelekhin/ansible-role-gitlab-runner/compare/...v1.0.0) (2023-08-14)


### Features

* initial commit ([c88f006](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/c88f006b6ff66fe0753ebffef5f44402c0d77e49))
