Role Name
=========

Installs grafana http://grafana.org/

Requirements
------------

None

Role Variables
--------------

````
graphite_host: localhost
````

Dependencies
------------

````
mrlesmithjr.snmpd
mrlesmithjr.timezone
mrlesmithjr.graphite
````

Example Playbook
----------------

---
- hosts: grafana-servers
  remote_user: remote
  sudo: yes
  roles:
    - mrlesmithjr.collectd
    - mrlesmithjr.snmpd
    - mrlesmithjr.timezone
    - mrlesmithjr.grafana
    - mrlesmithjr.graphite

License
-------

BSD

Author Information
------------------

Larry Smith Jr.
- @mrlesmithjr
- http://everythingshouldbevirtual.com
- mrlesmithjr [at] gmail.com
