Install4j
=========

Installs [install4j](https://www.ej-technologies.com/products/install4j/overview.html) on RHEL/CentOS and Debian/Ubuntu servers.

[![CI](https://github.com/petermylemans/ansible-role-install4j/workflows/CI/badge.svg)](https://github.com/petermylemans/ansible-role-install4j/actions)
[![Version](https://img.shields.io/github/v/release/petermylemans/ansible-role-install4j)](https://github.com/petermylemans/ansible-role-install4j/releases/)
[![galaxy downloads](https://img.shields.io/ansible/role/d/52985?label=galaxy%20downloads)](https://galaxy.ansible.com/petermylemans/install4j)
[![galaxy score](https://img.shields.io/ansible/quality/52985?label=galaxy%20quality%20score)](https://galaxy.ansible.com/petermylemans/install4j)

Typically, this is used in build servers that need to generate installers.

Requirements
------------

The IDE and the compiler of install4j require at least a 1.8 JRE to run.

You can combine this role with e.g. `geerlingguy.java`.

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

`install4j_version: 8.0.10`

The version of install4j to install. This defaults to the latest released version.

`install4j_timestamp_server_url: http://timestamp.digicert.com`

The url of the timestamp server that is used for code signing. 

Dependencies
------------

None.

Example Playbook
----------------

```
- hosts: all
  roles:
    - petermylemans.install4j
```

License
-------

Apache 2.0
