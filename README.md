# Ansible role: ansible.rssh

Debian - Restricted shell for scp/sftp

## Role Variables

Available variables are listed below, along with default values:

    rssh_allowcvs: False
    rssh_allowrdist: False
    rssh_allowrsync: False
    rssh_allowscp: False
    rssh_allowsftp: False
    rssh_logfacility: LOG_USER
    rssh_umask: '022'

Additional variables available, not set by default:

    rssh_chrootpath: /usr/local/chroot
    rssh_users:
      mrtango:
        umask: '077'
        access_bits: '00001'
        path: /usr/local/chroot

## Example Playbook

    - hosts: scpserver
      roles:
        - role: ansible.rssh

## License

BSD

## Author Information

This role was created by [Maik Derstappen | MrTango](http://derico.de).

## Creadits

Originally based on: https://github.com/linuxhq/ansible-role-rssh
