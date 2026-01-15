BOLID installation
=========

Ansible role for installation the BOLID programs (APVC2000, PPROG, UPROG). Allows you to install all software products for working with panel APMC2000 configurations and Modbus devices. Supports Windows

Requirements
------------

Before launching, you need to activate WinRM.

Role Variables
--------------

| Variable | Default | Description |
|----------|---------|-------------|
| `APMC2000_url` | `https://bolid.ru/files/373/566/arm_s2.exe` | URL for installation the APMC2000 program |
| `PPROG_url` | `https://bolid.ru/files/373/566/instpprog_3.15.1.zip` | URL for installation the PPROG program |
| `UPROG_url` | `https://bolid.ru/files/373/566/InstallUProg_4.1.9.zip` | URL for installation the UPROG program |

Example Playbook
----------------

```yml
- hosts: servers
  become: yes
  roles:
    - role: ansible-role-win-BOLID-installation
```

License
-------

MIT License