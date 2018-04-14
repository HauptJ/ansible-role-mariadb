# ansible-role-mariadb
Ansible role to install MariaDB on Enterprise Linux 7 / CentOS7 and either create or import a database

The database to import goes in the ```databases``` folder. Imported databases can be
either uncompressed / ```.sql``` or compressed in a ```.bz2``` archive. **See:** https://docs.ansible.com/ansible/latest/modules/mysql_db_module.html

[![Build Status](https://travis-ci.org/HauptJ/ansible-role-mariadb.svg?branch=master)](https://travis-ci.org/HauptJ/ansible-role-mariadb)

**Ansible Galaxy:** HauptJ.mariadb


## Variables

### MariaDB

| Name 						                  | Default 							                    | Description 										        |
|-----------------------------------|-------------------------------------------|-----------------------------------------|
| mariadb_root_password             | password                                  | root user password to be set            |
| mariadb_open_port                 | 3306                                      | network port                            |
| mariadb_open_port                 | false                                     | allow MariaDB through firewalld         |
| mariadb_set_root_password         | true                                      | sets MariaDB root password              |
| mariadb_new_db                    | true                                      | create a new DB or use an existing one  |
| mariadb_db_name                   | testWP                                    | database name                           |
| mariadb_db_user                   | testWPuser                                | database user                           |
| mariadb_db_user_password          | 1337TestPass                              | database user password                  |
| mariadb_db_file_name              | testWP.sql                                | file name of DB to import               |
