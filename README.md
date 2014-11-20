Ansible Role: Nginx
===================

Installs minimal latest Nginx version (using packages directly from nginx.org) on CentOS 6.5

Requirements
------------

None.

Role Variables
--------------

Default values:

* nginx_user: nginx
* nginx_worker_processes: 1
* nginx_pid: /var/run/nginx.pid
* nginx_access_log: /var/log/nginx/access.log
* nginx_error_log: /var/log/nginx/error.log
* nginx_worker_connections: 1024

You can override these values on your playbook.

Dependencies
------------

* tcosta84.yum

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: tcosta84.nginx }

License
-------

BSD

Author Information
------------------

This role was created by [Thiago Costa](http://thiagocostapy.com)
