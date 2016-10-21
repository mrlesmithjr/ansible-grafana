Role Name
=========

An [Ansible] role to install/configure [Grafana]

Requirements
------------

Install all Ansible role requirements.
````
sudo ansible-galaxy install -r requirements.yml -f
````

Vagrant
-------
Spin up Environment under Vagrant to test.
````
vagrant up
````

Usage
-----

````
username: admin
password: admin
````  

#### Vagrant
http://127.0.0.1:3000

#### Non-Vagrant
http://iporhostname:3000

Role Variables
--------------

```
---
# defaults file for ansible-grafana
config_grafana: true
enable_grafana_plugins: true
enable_grafana_vsphere_support: false
grafana_analytics:
  check_for_updates: 'true'
  reporting_enabled: 'true'
  google_analytics_ua_id: ''
grafana_apt_key: 'https://packagecloud.io/gpg.key'
grafana_apt_repo: 'deb https://packagecloud.io/grafana/stable/debian/ wheezy main'
grafana_db_info: # Only required if not using sqlite3 as grafana_db_type
  host: '127.0.0.1:3306'
  name: 'grafana'
  user: 'root'
  password: 'root'
grafana_db_type: 'sqlite3' # Either "mysql", "postgres" or "sqlite3"
grafana_debian_pre_reqs:
  - 'default-jdk-headless'
  - 'git'
  - 'maven'
  - 'python-pip'
  - 'unzip'
grafana_paths: # Define paths for each grafana source
  data: '/var/lib/grafana'
  logs: '/var/log/grafana'
  plugins: '/var/lib/grafana/plugins'
grafana_plugins:
  - name: 'grafana-clock-panel'
    state: "present" # absent|present
grafana_security_info:
  admin_password: 'admin'
  admin_user: 'admin'
  cookie_remember_name: 'grafana_remember'
  cookie_username: 'grafana_user'
  data_source_proxy_whitelist: '' # data source proxy whitelist (ip_or_domain:port separated by spaces)
  disable_gravatar: 'false' # disable gravatar profile images
  login_remember_days: '7' # Auto-login remember days
  secret_key: 'SW2YcwTIb9zpOOhoPsMm' # used for signing
grafana_server_info:
  domain: 'localhost'
  enable_gzip: 'false'
  enforce_domain: 'false'
  http_addr: ''
  http_port: '3000'
  protocol: 'http'
  root_url: '%(protocol)s://%(domain)s:%(http_port)s/'
  router_logging: 'false'
  static_root_path: 'public'

# Provider config options
# memory: not have any config yet
# file: session dir path, is relative to grafana data_path
# redis: config like redis server e.g. `addr=127.0.0.1:6379,pool_size=100,db=grafana`
# mysql: go-sql-driver/mysql dsn config string, e.g. `user:password@tcp(127.0.0.1:3306)/database_name`
# postgres: user=a password=b host=localhost port=5432 dbname=c sslmode=disable
grafana_session_info: # Either "memory", "file", "redis", "mysql", "postgres", default is "file"
  cookie_name: 'grafana_sess' # Session cookie name
  cookie_secure: 'false' # If you use session in https only, default is false
  provider: 'file'
  provider_config: 'sessions' # File based
  # provider_config: 'addr=127.0.0.1:6379,pool_size=100,db=grafana' # Redis based
  session_life_time: '86400' # Session life time, default is 86400
```

Dependencies
------------

#### GitHub
````
ansible-collectd
ansible-snmpd
ansible-timezone
ansible-grafana
ansible-graphite
````
#### Galaxy
````
mrlesmithjr.collectd
mrlesmithjr.snmpd
mrlesmithjr.timezone
mrlesmithjr.grafana
mrlesmithjr.graphite
````

Example Playbook
----------------

#### GitHub
````
---
- name: provisions grafana
  hosts: all
  become: true
  vars:
  roles:
    - role: ansible-collectd
    - role: ansible-snmpd
    - role: ansible-timezone
    - role: ansible-grafana
    - role: ansible-graphite
  tasks:
````
#### Galaxy
````
---
- name: provisions grafana
  hosts: all
  become: true
  vars:
  roles:
    - role: mrlesmithjr.collectd
    - role: mrlesmithjr.snmpd
    - role: mrlesmithjr.timezone
    - role: mrlesmithjr.grafana
    - role: mrlesmithjr.graphite
  tasks:
````

License
-------

BSD

Author Information
------------------

Larry Smith Jr.
- @mrlesmithjr
- http://everythingshouldbevirtual.com
- mrlesmithjr [at] gmail.com

[Ansible]: <https://www.ansible.com/>
[Grafana]: <http://grafana.org/>
