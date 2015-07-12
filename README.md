Phabricator
=========

Phabricator installer to connect to an existing db or run mysql on the same box.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

    server_url: secure.vagrant.dev
    mysql_user: phabricator
    mysql_pass: secret
    web_root: /var/www
    install_localtion: localhost

Example Playbook
----------------

Simple playbook that is enabled for use of clustering. Never use the default key in production:

    ---
    - hosts: localhost
      connection: local
      sudo: yes
      roles:
        - phabricator

License
-------

MIT

Author Information
------------------

Produced by NoWait
