### Ansible Role for OpenSSL
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