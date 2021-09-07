# ansible-role-packages

Install applications on an Arch or Ubuntu based systems via its package manager. Optionally, install an AUR package manager on Arch based systems.

## Test

Run `molecule test` to test this role in a docker container

## Requirements

- Arch Linux or Ubuntu based OS
- Sudo permissions

## Role Variables

- `aur`: set to true to install an [AUR helper](https://aur.archlinux.org/)

## Dependencies

ansible-role-basic

## Example Playbook

```
---
- name: Playbook
  hosts: localhost
  connection: local
  pre_tasks:
    - set_fact:
        aur: true
  roles:
    - ansible-role-packages
```

## License

MIT
