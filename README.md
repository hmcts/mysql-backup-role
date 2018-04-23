Role Name
====================

This ansible role runs a playbook to configure a backup job to be added to a crontab to configure MySQL backups to be backed up to a folder locally.


Requirements
------------

The new server needs to be created and in the correct network.
Please make sure the new server has the correct tags, verify from jenkins server.


Role Variables
-------------
Configure the following variables, the following is an example

```yaml
mysql_use_credentials: true
mysql_admin_user: mysqladminlogin
mysql_admin_password: Y0urT3stP@ssW0rd
scripts_backup_dir: "/usr/backups/scripts/"
mysql_backup_dir: "/usr/backups/mysql/"
mysql_backup_dir_owner: root
mysql_backup_dir_group: root

Dependencies
------------

Example Playbook
----------------
```yaml
- hosts: role_monitor
  roles:
    - role: devops.mysql-backup
```

License
-------
MIT


Author Information
------------------
HMCTS Reform Programme
