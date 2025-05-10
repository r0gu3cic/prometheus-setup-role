# PROMETHEUS-SETUP-ROLE

=========

This Ansible role installs and configures the Prometheus service on an Ubuntu server. It prepares the system for production use, enabling metric collection and monitoring.

## Requirements

------------

This role is designed to work with Ubuntu distributions. It requires the following:

- Ansible 2.10.8 or higher
- `sshpass` for running the playbook with SSH password authentication.

## Role Variables

------------

The following variables can be configured for this role:

- **`prometheus.version`**: The version of Prometheus we want installed.

These variables can be defined in the playbook or in a `vars` file.

## Dependencies

------------

This role has no dependencies on other roles.

## License

------------

MIT Licence

## Testing Guide

------------

To run a local test for this role, use the following command:

```bash
ansible-playbook tests/test.yml -i tests/local_inventory.ini -u root -k --extra-vars "hosts=local_vm"
```

## Author Information

------------

This role was created by Stefan, aka enabler, aka r0gu3cic. For any inquiries or further information, please reach out via [GitHub](https://github.com/r0gu3cic).
