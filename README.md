Icingaweb
=========

Installs and configures Icinga 2 and Icinga Web on Debian systems.

Requirements
------------

None.

Role Variables
--------------

 * icingaweb2_timezone: default timezone that is used in the web interface
 * icingaweb2_admin_username: username of the default admin account
 * icingaweb2_graphite: do you want to use graphite graphs
 * icingaweb2_graphite_url: URL to your graphite web installation
 * icingaweb2_certificate_dir: directory where your TLS certificates are installed
 * icingaweb2_graphite_version: git version to use for https://github.com/Icinga/icingaweb2-module-graphite

Dependencies
------------

* icinga2
* geerlingguy.git
* ajsalminen.mysql_database
* ajsalminen.mysql_sync
* ajsalminen.apache_ssl

Example Playbook
----------------

```
- hosts: icinga
  roles:
    - role: icingaweb2
```

License
-------

MIT

Author Information
------------------

Libraries.fi
