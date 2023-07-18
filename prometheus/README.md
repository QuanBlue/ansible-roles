<div align="center">
<h1> Prometheus role </h1>

The Prometheus role is an Ansible role that facilitates the installation and configuration of Prometheus, an open-source monitoring and alerting tool.

</div>

## Requirements

- Ansible 2.10 or higher
- Supported operating systems:
  - Debian-based distributions (e.g., Ubuntu)

## Role Variables

- `userId`: userId of the user that will run Prometheus
- `groupId`: groupId of the user that will run Prometheus
- `version`: version of Prometheus to install
- `port`: port on which Prometheus will listen

## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yml
- name: Install and configure Prometheus
  become: true
  become_method: sudo
  hosts: monitoring_servers
  roles:
    - role: prometheus
```

## Additional Information

For additional information about Prometheus and its configuration options, please refer to the [**Prometheus documentation**](https://prometheus.io/).

---

Feel free to customize this document with additional details relevant to your Prometheus Ansible role, such as specific features, configuration options, or any other information that may be useful for users of the role.
