ansible-role-packages
=========

Install applications on an Arch or Ubuntu based systems via its package manager.

Requirements
------------

- Arch Linux or Ubuntu based OS
- Sudo permissions

Role Variables
--------------

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
  pre_tasks:
    - set_fact:
      laptop: true
  roles:
    - ansible-role-packages
```

License
-------

MIT
