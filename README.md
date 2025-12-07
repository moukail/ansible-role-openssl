Ansible Role for OpenSSL
=========

Example Requirements
--------------------

```yml
---
roles:
  - name: ansible-role-openssl
    src: git+https://github.com/moukail/ansible-role-openssl.git
    version: main

```

Example Playbook
----------------

```yaml
---
- name: Install OpenSSL
  hosts: all
  become: true

  tasks:
    - name: Install OpenSSL
      ansible.builtin.include_role:
        name: ansible-role-openssl
      vars:
        openssl_ver: "3.6.0"

```