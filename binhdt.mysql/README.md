MySQL
=========

Ansible role for installing mysql 5.7. Tested platforms are:
* Debian 8
* Debian 9
* Ubuntu 16

Requirements
------------

Debian 8 (jessie)
Debian 9 (stretch)
Ubuntu 16 (xenial)
CentOS 7 (RHEL)

Role Variables
--------------

Available variables are listed below, along with default values (see defaults/main.yml):

| Parameter | Required | Default | Choices | Comments |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| default_mysql_root_password | yes | access | | Sets MySQL user root password |
| default_mysql_user_login | yes | user | | Sets default MySQL user name |
| default_mysql_user_password | yes | access | | Sets default MySQL user password |
| default_mysql_port | yes | 3306 | | Sets MySQL server port |


Dependencies
------------

None

Example
----------------
    ---
    - hosts: all
      roles:
         - { role: binhdt.mysql }

License
-------

MIT / BSD

Author Information
------------------

This role was created in 2021 by [BINH DO](https://github.com/binhdt2611).
