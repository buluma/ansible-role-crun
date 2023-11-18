# [Ansible role crun](#crun)

Ansible Role for crun Installation

|GitHub|GitLab|Downloads|Version|Issues|Pull Requests|
|------|------|-------|-------|------|-------------|
|[![github](https://github.com/buluma/ansible-role-crun/actions/workflows/molecule.yml/badge.svg)](https://github.com/buluma/ansible-role-crun/actions/workflows/molecule.yml)|[![gitlab](https://gitlab.com/shadowwalker/ansible-role-crun/badges/master/pipeline.svg)](https://gitlab.com/shadowwalker/ansible-role-crun)|[![downloads](https://img.shields.io/ansible/role/d/4678)](https://galaxy.ansible.com/buluma/crun)|[![Version](https://img.shields.io/github/release/buluma/ansible-role-crun.svg)](https://github.com/buluma/ansible-role-crun/releases/)|[![Issues](https://img.shields.io/github/issues/buluma/ansible-role-crun.svg)](https://github.com/buluma/ansible-role-crun/issues/)|[![PullRequests](https://img.shields.io/github/issues-pr-closed-raw/buluma/ansible-role-crun.svg)](https://github.com/buluma/ansible-role-crun/pulls/)|

## [Example Playbook](#example-playbook)

This example is taken from [`molecule/default/converge.yml`](https://github.com/buluma/ansible-role-crun/blob/master/molecule/default/converge.yml) and is tested on each push, pull request and release.

```yaml
---
- name: converge | all
  hosts: all
  remote_user: root
  become: true
  gather_facts: true
  roles:
    - role: buluma.crun
```

The machine needs to be prepared. In CI this is done using [`molecule/default/prepare.yml`](https://github.com/buluma/ansible-role-crun/blob/master/molecule/default/prepare.yml):

```yaml
---
- name: Prepare
  hosts: all
  become: yes
  gather_facts: no

  roles:
    - role: buluma.bootstrap
```

Also see a [full explanation and example](https://buluma.github.io/how-to-use-these-roles.html) on how to use these roles.


## [Requirements](#requirements)

- pip packages listed in [requirements.txt](https://github.com/buluma/ansible-role-crun/blob/master/requirements.txt).

## [State of used roles](#state-of-used-roles)

The following roles are used to prepare a system. You can prepare your system in another way.

| Requirement | GitHub | GitLab |
|-------------|--------|--------|
|[buluma.bootstrap](https://galaxy.ansible.com/buluma/bootstrap)|[![Build Status GitHub](https://github.com/buluma/ansible-role-bootstrap/workflows/Ansible%20Molecule/badge.svg)](https://github.com/buluma/ansible-role-bootstrap/actions)|[![Build Status GitLab](https://gitlab.com/shadowwalker/ansible-role-bootstrap/badges/master/pipeline.svg)](https://gitlab.com/shadowwalker/ansible-role-bootstrap)|

## [Context](#context)

This role is a part of many compatible roles. Have a look at [the documentation of these roles](https://buluma.github.io/) for further information.

Here is an overview of related roles:

![dependencies](https://raw.githubusercontent.com/buluma/ansible-role-crun/png/requirements.png "Dependencies")

## [Compatibility](#compatibility)

This role has been tested on these [container images](https://hub.docker.com/u/buluma):

|container|tags|
|---------|----|
|[Ubuntu](https://hub.docker.com/repository/docker/buluma/ubuntu/general)|jammy, focal, bionic|
|[EL](https://hub.docker.com/repository/docker/buluma/enterpriselinux/general)|9, 8, 7|
|[Debian](https://hub.docker.com/repository/docker/buluma/debian/general)|all|
|[Fedora](https://hub.docker.com/repository/docker/buluma/fedora/general)|36, 35|

The minimum version of Ansible required is 4.10, tests have been done to:

- The previous version.
- The current version.
- The development version.

If you find issues, please register them in [GitHub](https://github.com/buluma/ansible-role-crun/issues)

## [Changelog](#changelog)

[Role History](https://github.com/buluma/ansible-role-crun/blob/master/CHANGELOG.md)

## [License](#license)

[Apache-2.0](https://github.com/buluma/ansible-role-crun/blob/master/LICENSE).

## [Author Information](#author-information)

[buluma](https://buluma.github.io/)

Please consider [sponsoring me](https://github.com/sponsors/buluma).

### [Special Thanks](#special-thanks)

Template inspired by [Robert de Bock](https://github.com/robertdebock)
