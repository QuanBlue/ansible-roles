<div align="center">
<h1> Grafana role </h1>

This Ansible role installs and configures Grafana, a popular open-source analytics and monitoring platform, on target hosts.

</div>

## Requirements

- Ansible 2.10 or higher
- Supported operating systems:
  - Debian-based distributions (e.g., Ubuntu)

## Role Variables

- `grafana_admin_password`: set the Grafana admin password
- `port`: set the port on which Grafana will listen

## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yml
- name: Install and configure Grafana
  become: true
  become_method: sudo
  hosts: grafana_servers
  roles:
    - role: grafana
```

## Additional Information

For additional information about Grafana and its configuration options, please refer to the [**Grafana documentation**](https://grafana.com/docs/).

---

Feel free to customize this template to include any additional information or specific instructions relevant to your Grafana Ansible role.
