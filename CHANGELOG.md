# Changelog

## [3.0.6](https://github.com/antmelekhin/ansible-role-gitlab-runner/compare/v3.0.5...v3.0.6) (2024-11-27)


### Documentation

* **README:** updated requirements and dependencies ([09e8381](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/09e83815e90bd4802ede59afb000335e2e0bd6d3))


### Fixes

* normalize `ansible_architecture` for windows ([fbf50ea](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/fbf50ea4974ae8d701763a85e84055885672d0a7))

## [3.0.5](https://github.com/antmelekhin/ansible-role-gitlab-runner/compare/v3.0.4...v3.0.5) (2024-11-04)


### Fixes

* **version:** gitlab-runner updated to `17.5.3` release ([#25](https://github.com/antmelekhin/ansible-role-gitlab-runner/issues/25)) ([44a0447](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/44a0447dc329c1591b383d92cc697a8dbbcbba07))

## [3.0.4](https://github.com/antmelekhin/ansible-role-gitlab-runner/compare/v3.0.3...v3.0.4) (2024-10-29)


### Code Refactoring

* update `vars/main.yml` file ([097ed59](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/097ed59d9ddea1426bf6434cd1091adb275f520e))

## [3.0.3](https://github.com/antmelekhin/ansible-role-gitlab-runner/compare/v3.0.2...v3.0.3) (2024-10-29)


### Fixes

* **version:** gitlab-runner updated to `17.5.2` release ([#24](https://github.com/antmelekhin/ansible-role-gitlab-runner/issues/24)) ([5957c6b](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/5957c6b63e05a19f3612110561d48bfb973542ff))

## [3.0.2](https://github.com/antmelekhin/ansible-role-gitlab-runner/compare/v3.0.1...v3.0.2) (2024-10-22)


### Fixes

* **version:** gitlab-runner updated to `17.5.1` release ([#23](https://github.com/antmelekhin/ansible-role-gitlab-runner/issues/23)) ([cd2453b](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/cd2453ba4d4a7af8f888a5c065281637ad235789))

## [3.0.1](https://github.com/antmelekhin/ansible-role-gitlab-runner/compare/v3.0.0...v3.0.1) (2024-10-05)


### Continuous Integration

* reverted runner image to `ubuntu-22.04` ([f109795](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/f109795157e6e1353c25b7b282a56bfa87866a9a))
* updated runner image to `ubuntu-24.04` ([8327ce6](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/8327ce6b52dc1e57ba535bac88bff6acc427a6a2))


### Fixes

* add `become: false` to localhost delegated tasks ([2c0e0e9](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/2c0e0e947711cacf4db9967023189780db7febff))


### Styles

* minor fixes ([204804f](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/204804f1c3b9fc6c50ad4d558ddb37b2c3cca86f))

## [3.0.0](https://github.com/antmelekhin/ansible-role-gitlab-runner/compare/v2.7.0...v3.0.0) (2024-09-30)


### ⚠ BREAKING CHANGES

* rename variables used for installation from the binary (#22)

### Continuous Integration

* use `ubuntu-22.04` instead of `ubuntu-latest` ([4489246](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/448924602a5e122d9841a9c73e5d392fa426e7ce))


### Styles

* minor fixes in task names ([ac5f7fe](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/ac5f7fef84f0db72d9b1e4779b577adc0b0aee2e))
* rename some binary vars ([f71044e](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/f71044e4f2e1c4e7a9bd34fe9760b2328928709c))
* rename variables used for installation from the binary ([#22](https://github.com/antmelekhin/ansible-role-gitlab-runner/issues/22)) ([7a8c428](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/7a8c428f7a9895d89525ad821bf70693238a6afb))

## [2.7.0](https://github.com/antmelekhin/ansible-role-gitlab-runner/compare/v2.6.2...v2.7.0) (2024-09-24)


### Features

* add `darwin` support ([#19](https://github.com/antmelekhin/ansible-role-gitlab-runner/issues/19)) ([beecbf0](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/beecbf0f73344aaf5709bc8763fa3b4915e035a5))

## [2.6.2](https://github.com/antmelekhin/ansible-role-gitlab-runner/compare/v2.6.1...v2.6.2) (2024-09-23)


### Fixes

* **version:** gitlab-runner updated to `17.4.0` release ([#20](https://github.com/antmelekhin/ansible-role-gitlab-runner/issues/20)) ([2bb26c9](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/2bb26c969eaeba4f454fdee715cc2c7131ea627f))

## [2.6.1](https://github.com/antmelekhin/ansible-role-gitlab-runner/compare/v2.6.0...v2.6.1) (2024-08-22)


### Fixes

* **version:** gitlab-runner updated to `17.3.1` release ([#18](https://github.com/antmelekhin/ansible-role-gitlab-runner/issues/18)) ([3a0d5e3](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/3a0d5e32651af3021e1be65b8c822d44a121562d))

## [2.6.0](https://github.com/antmelekhin/ansible-role-gitlab-runner/compare/v2.5.0...v2.6.0) (2024-08-22)


### Features

* add `meta/argument_specs.yml` file ([#17](https://github.com/antmelekhin/ansible-role-gitlab-runner/issues/17)) ([3c837bf](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/3c837bf57917f598ed80c377b88dd3819372cdf9))

## [2.5.0](https://github.com/antmelekhin/ansible-role-gitlab-runner/compare/v2.4.1...v2.5.0) (2024-08-21)


### Improvements

* merge OS-specific variables into the `vars/main.yml` file ([#16](https://github.com/antmelekhin/ansible-role-gitlab-runner/issues/16)) ([846eccd](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/846eccd83a90edb18a3a322d19f7155358106ceb))

## [2.4.1](https://github.com/antmelekhin/ansible-role-gitlab-runner/compare/v2.4.0...v2.4.1) (2024-08-20)


### Fixes

* **version:** gitlab-runner updated to `17.3.0` release ([#15](https://github.com/antmelekhin/ansible-role-gitlab-runner/issues/15)) ([4a5f06d](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/4a5f06d38fd84802f92ccf80a0ee8515a2e0ea40))


### Tests

* clean version output in the default scenario ([ce1836c](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/ce1836c0fc40af975aca4dbdaef8324f7fb7bddd))

## [2.4.0](https://github.com/antmelekhin/ansible-role-gitlab-runner/compare/v2.3.3...v2.4.0) (2024-08-05)


### Features

* add `fedora` and `amazonlinux` support ([#14](https://github.com/antmelekhin/ansible-role-gitlab-runner/issues/14)) ([cebd97b](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/cebd97b8b3f3c72e55dea2c52a659e0b7fbe488a))

## [2.3.3](https://github.com/antmelekhin/ansible-role-gitlab-runner/compare/v2.3.2...v2.3.3) (2024-07-30)


### Fixes

* **version:** gitlab-runner updated to `17.2.1` release ([#13](https://github.com/antmelekhin/ansible-role-gitlab-runner/issues/13)) ([22351fa](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/22351faee20948df7819b003f5a41bbf121d2057))

## [2.3.2](https://github.com/antmelekhin/ansible-role-gitlab-runner/compare/v2.3.1...v2.3.2) (2024-07-23)


### Continuous Integration

* fix updater script ([28c5a32](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/28c5a32d33efb44851d9e41c418f149f990b268d))


### Fixes

* **version:** gitlab-runner updated to `17.2.0` release ([#12](https://github.com/antmelekhin/ansible-role-gitlab-runner/issues/12)) ([49bf8dd](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/49bf8dd7b353a69ff01f525242dfc77106153de2))


### Tests

* fix assert task ([e9c47b6](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/e9c47b6fb1148cf2b6eb0e3d4862574ed6ad61d7))

## [2.3.1](https://github.com/antmelekhin/ansible-role-gitlab-runner/compare/v2.3.0...v2.3.1) (2024-07-02)


### Continuous Integration

* add `update-version` workflow ([5955a61](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/5955a6121989f43156a1972426e33530a6c5b853))
* fix `update-version` workflow ([90b19c5](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/90b19c59dc067958c22e89039df44c1b80f12097))
* fix PR_MESSAGE in `update-version` script ([48d760f](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/48d760f425e52bd016f27a443d248e2c4c5c6833))


### Fixes

* **version:** gitlab-runner updated to `17.1.0` release ([#10](https://github.com/antmelekhin/ansible-role-gitlab-runner/issues/10)) ([592cee0](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/592cee00fe48def6aee5cf1fb2e11fe4daa542ed))

## [2.3.0](https://github.com/antmelekhin/ansible-role-gitlab-runner/compare/v2.2.2...v2.3.0) (2024-06-05)


### Improvements

* update variables and common role style ([#9](https://github.com/antmelekhin/ansible-role-gitlab-runner/issues/9)) ([e7514e9](https://github.com/antmelekhin/ansible-role-gitlab-runner/commit/e7514e92a8a1ad39b8cfbbc2288dd3949354f396))

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
