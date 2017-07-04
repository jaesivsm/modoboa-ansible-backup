Modoboa Ansible Backup
======================

A simple script to backup datas from a modoboa instance.

The script will backup:
* any database listed in the Django configurations (aka: ```/srv/modoboa/instance/instance/settings.py```)
* the /srv/vmail folder

Role Variables
--------------

* ```modoboa_ab_dump_dir```:
  default to ```~/.local/share/modoboa_dump_dir/```
  The remote path on the servers where the datas will be dumped.

* ```modoboa_ab_local_backup_storage```:
  default to ```~/modoboa_backups/```
  The local path where the dumps will be retrieved.

* ```modoboa_ab_remove_after```:
  default to ```false```
  If set to ```true```, will remove the distant dump dir at the end.

License
-------

GPL v3.0

Author Information
------------------

jaesivsm (https://1pxsolidblack.pl)
