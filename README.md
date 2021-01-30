ansible-role-packages
=========

Install applications on an Arch or Ubuntu based systems via its package manager. Optionally, install an AUR package manager on Arch based systems.

Requirements
------------

- Arch Linux or Ubuntu based OS
- Sudo permissions

Role Variables
--------------

- `aur`: set tot true to install an [AUR helper](https://aur.archlinux.org/)

Dependencies
------------

ansible-role-basic

Example Playbook
----------------

```
---
- name: Playbook
  hosts: localhost
  connection: local
  pre_tasks:
    - set_fact:
      laptop: true
      aur: true
  roles:
    - ansible-role-packages
```

License
-------

MIT
