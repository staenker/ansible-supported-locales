staenker.supported-locales
=========
[![Ansible Galaxy](http://img.shields.io/badge/AnsibleGalaxy-staenker.supported-locales-blue.svg?style=flat)](https://galaxy.ansible.com/list#/roles/2124)

Ensures that a given list of locales is generated on a Debian based system.
Basically it's a simple abstraction over the Ansible locale_gen module which
allows the use of a list of supported locales.

Requirements
------------

A Debian based system is enough

Role Variables
--------------

 - locales, default: [ en_US.UTF-8, de_DE.UTF-8 ]

Dependencies
------------

none

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: staenker.supported-locales, locales: [ de_DE.UTF-8, ru_RU.UTF-8 ] }

License
-------

Apache License, Version 2.0

Author Information
------------------

Awesome dude
