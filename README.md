Role Name
=========

Installs grafana http://grafana.org/

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

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

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
        - { role: mrlesmithjr.snmpd }
        - { role: mrlesmithjr.timezone }
        - { role: mrlesmithjr.graphite }
        - { role: mrlesmithjr.grafana }

License
-------

BSD

Author Information
------------------

Larry Smith Jr.
- @mrlesmithjr
- http://everythingshouldbevirtual.com
- mrlesmithjr [at] gmail.com
