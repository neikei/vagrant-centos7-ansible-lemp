# Vagrant-CentOS-Ansible-LEMP

This is just a simple LEMP setup with nginx, php7 and mariadb on a CentOS box from the bento project.

## Requirements
1. Virtualbox >= 5.1.14
2. Vagrant = 1.8.7
3. Vagrant Plugins:
 - vagrant-vbguest (recommended)
 - vagrant-winnfsd (only for Windows)

## Installation
1. git clone https://github.com/neikei/vagrant-centos7-ansible-lemp.git
2. cd vagrant-centos7-ansible-lemp
3. vagrant up
4. ... wait ...
5. Check the phpinfo(): http://192.168.56.123

## Playground access

 - Webserver: http://192.168.56.123
 - MariaDB: 192.168.56.123:3306
   - user: admin
   - password: changeme
   - root and vagrant are allowed to access the database from localhost without a password

Place your stuff in the subfolder web, because the folder is configured as share into the webserver root path in your VM.

## Changelog
24 January 2017
 - Implemented Windows support
 - Changed the provisioning to ansible_local

23 January 2017
 - Initial Commit
 - CentOS 7.3, Nginx, PHP7, MariaDB
