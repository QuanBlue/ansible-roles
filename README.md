<h1 align="center">
  <img src="./assets/ansible-role-logo.png" alt="icon" height="150"></img>
  <br>
  <b>Ansible Roles</b>
</h1>

<p align="center">Reusable Ansible roles.</p>

<!-- Badges -->
<p align="center">
  <a href="https://github.com/quanblue/ansible-roles/graphs/contributors">
    <img src="https://img.shields.io/github/contributors/quanblue/ansible-roles" alt="contributors" />
  </a>
  <a href="">
    <img src="https://img.shields.io/github/last-commit/quanblue/ansible-roles" alt="last update" />
  </a>
  <a href="https://github.com/quanblue/ansible-roles/network/members">
    <img src="https://img.shields.io/github/forks/quanblue/ansible-roles" alt="forks" />
  </a>
  <a href="https://github.com/quanblue/ansible-roles/stargazers">
    <img src="https://img.shields.io/github/stars/quanblue/ansible-roles" alt="stars" />
  </a>
  <a href="https://github.com/quanblue/ansible-roles/issues/">
    <img src="https://img.shields.io/github/issues/quanblue/ansible-roles" alt="open issues" />
  </a>
  <a href="https://github.com/quanblue/ansible-roles/blob/master/LICENSE">
    <img src="https://img.shields.io/github/license/quanblue/ansible-roles.svg" alt="license" />
  </a>
</p>

<p align="center">
  <b>
      <a href="#introduction">Introduction</a> •
      <a href="https://github.com/quanblue/ansible-roles/issues/">Report Bug</a> •
      <a href="https://github.com/quanblue/ansible-roles/issues/">Request Feature</a>
  </b>
</p>

<br/>

<details open>
<summary><b>Table of Contents</b></summary>

- [Getting Started](#getting-started)
  - [System Requirements](#system-requirements)
- [Developer Guide](#developer-guide)
  - [Create a new role](#create-a-new-role)
  - [Test new role](#test-new-role)
- [:busts_in_silhouette: Contributors](#busts_in_silhouette-contributors)
- [:scroll: License](#scroll-license)
</details>

# Getting Started

## System Requirements

These roles have only been tested with:

- Ubuntu 20.04
- Ansible versions: 2.14.2

Each role contains a `README` describing its usage.

# Developer Guide

## Create a new role

**Step 1:** Create a new role skeleton

```sh
ansible-galaxy init rolename
```

This creates a directory structure like:

```
<rolename>/
├── defaults/         # <-- includes default variables.
│   └── main.yml      #
├── files/            # <-- store static files for remote hosts.
├── handlers/         # <-- include event-triggered tasks.
│   └── main.yml      #
├── meta/             # <-- defines role dependencies.
│   └── main.yml      #
├── tasks/            # <-- include tasks define the actions on the remote hosts.
│   └── main.yml      #
├── templates/        # <-- rendered templates for remote hosts.
├── tests/            # <-- role testing.
│   ├── inventory     #
│   └── test.yml      #
├── vars/             # <-- includes variables specific to the role
│   └── main.yml      #
└── README.md         # <-- role documentation
```

**Step 2:** Implement role functionality

The following links as guides for best practices in creating the role:

- https://galaxy.ansible.com/intro#share
- https://openedx.atlassian.net/wiki/display/OpenOPS/Ansible+Code+Conventions
- https://github.com/QuanBlue/tech-cheatsheets/tree/master/Infrastructure%20as%20Code%20(IaC)/Ansible

## Test new role

**Step 1:** Test syntax

```sh
ansible-playbook -i <rolename>/tests/inventory <rolename>/tests/test.yml --syntax-check
```

**Step 2:** Execute role and validate - this may not be possible locally and may require a container

```sh
ansible-playbook -i <rolename>/tests/inventory <rolename>/tests/test.yml --connection=local --sudo
```

# :busts_in_silhouette: Contributors

<a href="https://github.com/quanblue/ansible-roles/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=quanblue/ansible-roles" />
</a>

Contributions to this repository are always welcome! If you have any cheat sheets that you would.

# :scroll: License

Distributed under the MIT License. See <a href="https://github.com/quanblue/ansible-roles/blob/master/LICENSE">`LICENSE`</a> for more information.

---

> Bento [@quanblue](https://bento.me/quanblue) &nbsp;&middot;&nbsp;
> GitHub [@QuanBlue](https://github.com/QuanBlue) &nbsp;&middot;&nbsp; Gmail quannguyenthanh558@gmail.com
