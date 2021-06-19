Ansible Role: grafana

```yaml
- hosts: all
  roles:
    - role: cloudalchemy.grafana
      vars:
        grafana_security:
          admin_user: admin
          admin_password: enter_your_secure_password
```
