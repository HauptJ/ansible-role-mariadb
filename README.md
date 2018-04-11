# ansible-role-mariadb
Ansible role to install MariaDB on Enterprise Linux 7 / CentOS7 and either create or import a database

The database to import goes in the ```databases``` folder. Imported databases can be
either uncompressed / ```.sql``` or compressed in a ```.bz2``` archive. **See:** https://docs.ansible.com/ansible/latest/modules/mysql_db_module.html

[![Build Status](https://travis-ci.org/HauptJ/ansible-role-mariadb.svg?branch=master)](https://travis-ci.org/HauptJ/ansible-role-mariadb)

**Ansible Galaxy:** HauptJ.mariadb
