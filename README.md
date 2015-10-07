Ansible role/standalone to install latest s3cmd via pip.
===========================

Ansible role -and standalone- to install and configure latest version of s3cmd (via pip).

Using
--------------
Use role directly:
```bash
ansible-playbook ansible-latest-s3cmd.yml
```

Use role in a playbook:
```
- name: Ansible role to install and configure latest version of s3cmd (via pip).
  hosts: s3cmd-servers
  sudo: true
  gather_facts: no
  roles:
    - ansible-latest-s3cmd
```

Variables
--------------

```
s3cmd:
  - key: 'AWS_KEY'
  - secret: 'AWS_SECRET'
```

Dependencies
--------------
None

License
--------------
Licensed under one of the following license: GPLv3, GPLv2, LGPLv2.

Maintainers
--------------
[Ahmed AbouZaid](https://github.com/AAbouZaid)
