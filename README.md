nginx
=========

Add ngnix to your machine.

Requirements
------------

Systems running this playbook should have access to a repository containing nginx.

Role Variables
--------------

- appport - You can specify what port should be used to listen on. The default (defaults/main.yml) is port 80.

Dependencies
------------

- robertdebock.ansible-role-epel

Example Playbook
----------------

```
- hosts: all

  roles:
    - role: robertdebock.ansible-role-nginx

  tasks:
    - name: place some content
      copy:
        src: files/index.html
        dest: /usr/share/nginx/html/index.html
```

License
-------

Apache License, Version 2.0

Author Information
------------------

Robert de Bock <robert@meinit.nl>
