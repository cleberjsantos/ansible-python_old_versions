python_old_versions
===================

[![Ansible Role](https://img.shields.io/ansible/role/5751.svg)](https://galaxy.ansible.com/list#/roles/5751)


Installs older and newer Python versions for Debian likes.

Currently supported releases — 2.3, 2.4, 2.5, 2.6, 2.7, 3.1, 3.2, 3.3, 3.4, 3.5


Requirements
------------

* This role requires Ansible 1.6 or higher.

* python-apt

* python-keyczar (on the remote side)


Role Variables
--------------

The variables that can be passed to this role with default values are as follows.

    # Python Version
    python_version: 2.3 # Default: 2.4

    # Installs easy_install
    easy_install: false # Default: true

    # If yes, force installs (Use with caution)
    force_install: yes # Default: no

    # Virtualenv version, If python 2.4, not change this value for higher version.
    python_virtualenv: 1.7.2 # Default: 1.7.2


Example Playbook
-----------------

Example of usage:

    - hosts: servers
      roles:
        - { role: cleberjsantos.python_old_versions, tags: [python] }

License
-------

GPLv2

Author Information
------------------

Cleber J Santos
