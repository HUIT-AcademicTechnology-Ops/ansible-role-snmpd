# Ansible Role: snmpd

Installs and configures snmpd on supported Linux hosts.

## Requirements

None.

## Role Variables

The default values for the variables are set in `defaults/main.yml`.

## Dependencies

None.

## Example Playbook

```yaml
  - hosts: servers
    roles:
      - role: huit-academictechnology-ops.ansible-role-snmpd
        snmpd_auth:
            snmpv3_auth_pass: ""
            snmpv3_priv_pass: ""
            snmpv3_user: ""
        snmpd_syslocation: "AWS"
        snmpd_syscontact: "IT Helpdesk <ithelp@localhost>"
```

## License

MIT

## Author Information

This role was created in 2022 by Arthur Barrett as a member of the Harvard University IT Academic Technology group.