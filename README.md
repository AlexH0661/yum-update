# yum-update

This Ansible role will update and optionally reboot systems if required

```bash
ansible-playbook playbook.yaml -Kkv
```

## Example Playbook

```yaml
---
- name: Update and reboot hosts (if required)
  hosts: all
  vars:
    reboot: true
  roles:
    - yum-update
```
