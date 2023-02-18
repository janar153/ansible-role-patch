Ansible Role: (Ubuntu) System Upgrade
=========

** Perform Ubuntu upgrade **

This Ansible role will perform Ubuntu upgrade. After which it will reboot host (only if required). 
  
Example requirements.yml
------------------------

```
---
- src: https://github.com/janar153/ansible-role-patch.git
  scm: git
  version: main
  name: patch

```


Example Playbook
----------------

```
- hosts: all
  gather_facts: true
  become: true

  roles:
    - role: patch
```

License
-------

MIT
