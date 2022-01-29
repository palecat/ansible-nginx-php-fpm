Role Name
=========

Ansible role which installs / configures nginx + php-fpm


Role Variables
--------------

```
php_version: "7.4"
nginx_document_root: "/var/www/html/"
nginx_index: "index.php"
nginx_port: "80"
fastcgi_index: "index.php"
unix_socket: "/run/php/php7.4-fpm.sock"
```


Example Playbook
----------------

```
---
- hosts: servers
  become: yes

  roles:
    - role: "nginx-php-fpm"
      nginx_document_root: /opt/nginx/ansible/

```
