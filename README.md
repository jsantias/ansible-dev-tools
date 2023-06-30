Ansible Development Tools
==============================

- cloudcli - install various cloud CLIs (aws, helm, azure, oc, kubectl, ibmcloud, etc.)
- languages - install various programming languages (.net, python, node, etc.)

Tested on:
----------

- CentOS 7
- RHEL 8
- Fedora 30
- Ubuntu 18.04
- Debian 10

Example
-------


### playbook.yml example

```yaml
- name: setup a development environment
  hosts: all
  connection: local
  become: yes
  gather_facts: yes
  roles:
    - role: cloudcli
```
