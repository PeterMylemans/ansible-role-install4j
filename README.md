Role Name
=========

Installs [install4j](https://www.ej-technologies.com/products/install4j/overview.html) on RHEL/CentOS and Debian/Ubuntu servers.

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

The url of the timestamp server that is for code signing. 

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
