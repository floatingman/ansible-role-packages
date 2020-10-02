ansible-role-packages
=========

Install applications on an Arch or Ubuntu based systems via its package manager. Optionally, install yay as AUR package manager on Arch based systems.

Requirements
------------

- Arch Linux or Ubuntu based OS
- Sudo permissions

Role Variables
--------------

- `yay`: set tot true to install [yay](https://github.com/Jguer/yay)

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
  roles:
    - ansible-role-packages
```

License
-------

MIT
