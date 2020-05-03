Role Name
=========

Install common packages on an Arch Linux based system via pacman.

Requirements
------------

- Arch Linux (pacman)
- Sudo permissions

Role Variables
--------------

No variables

Dependencies
------------

No dependencies

Example Playbook
----------------

```
---
- name: Playbook
  hosts: localhost
  connection: local
  roles:
    - ansible-role-packages
```

License
-------

MIT
