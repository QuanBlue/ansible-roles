<div align="center">
<h1> NodeJS role </h1>

This Ansible role installs and configures Node.js on remote hosts.

</div>

## Requirements

- Ansible 2.10 or higher
- Supported operating systems:
  - Debian-based distributions (e.g., Ubuntu)

## Role Variables

- `nodejs_version`: version of Node.js to install

## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yml
- name: Install and configure NodeJS
  become: true
  become_method: sudo
  hosts: nodejs_servers
  roles:
    - role: nodejs
```

## Additional Information

For additional information about NodeJS and its configuration options, please refer to the [**NodeJS documentation**](https://nodejs.org/en).

---

Feel free to customize this document with additional details relevant to your Node.js Ansible role, such as specific features, configuration options, or any other information that may be useful for users of the role.
