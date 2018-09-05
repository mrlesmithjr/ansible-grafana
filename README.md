# ansible-grafana

An [Ansible](https://www.ansible.com) role to install/configure [Grafana](https://grafana.com/)

## Requirements

Install all Ansible role requirements.

```bash
sudo ansible-galaxy install -r requirements.yml -f
```

## Information

Example dashboards are included in `dashboards/`. I would love to see some others
being added via PR's!

## Vagrant

Spin up Environment under Vagrant to test.

```bash
vagrant up
```

## Usage

```yaml
username: admin
password: admin
```

### Vagrant Login

<http://127.0.0.1:3000>

### Non-Vagrant Login

<http://iporhostname:3000>

## Role Variables

[defaults/main.yml](defaults/main.yml)

## Dependencies

Reference [Requirements](#Requirements)

## Example Playbook

```yaml
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
```

## License

MIT

## Author Information

Larry Smith Jr.

- [EverythingShouldBeVirtual](http://everythingshouldbevirtual.com)
- [@mrlesmithjr](https://www.twitter.com/mrlesmithjr)
- <mailto:mrlesmithjr@gmail.com>
