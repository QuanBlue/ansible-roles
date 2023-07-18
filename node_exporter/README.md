<div align="center">
<h1> Node Exporter role </h1>

The Node Exporter Ansible role sets up and configures Prometheus Node Exporter on target hosts. Prometheus Node Exporter is a lightweight exporter for machine metrics that can be scraped by Prometheus monitoring system.

</div>

## Requirements

- Ansible 2.10 or higher
- Supported operating systems:
  - Debian-based distributions (e.g., Ubuntu)

## Role Variables

- `version`: version of Node_exporter to install
- `port`: port on which Node_exporter will listen

## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yml
- name: Install and configure Node_exporter
  become: true
  become_method: sudo
  hosts: monitoring_hosts
  roles:
    - role: node_exporter
```

## Additional Information

For additional information about NodeJS and its configuration options, please refer to the [**Node_exporter documentation**](https://prometheus.io/docs/guides/node-exporter/).

---

Feel free to customize this document with additional details relevant to your Node_exporter Ansible role, such as specific features, configuration options, or any other information that may be useful for users of the role.
