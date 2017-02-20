# Setup Observium on CentOS 7

[![Codacy Badge](https://api.codacy.com/project/badge/Grade/9743715950ea48ae896fe34258ec0d4b)](https://www.codacy.com/app/Findarato/ansible-CentOS7-Observium?utm_source=github.com&utm_medium=referral&utm_content=Findarato/ansible-CentOS7-Observium&utm_campaign=badger)
[![Build Status](https://travis-ci.org/Findarato/ansible-CentOS7-Observium.svg?branch=master)](https://travis-ci.org/Findarato/ansible-CentOS7-Observium) [![Code Climate](https://codeclimate.com/github/Findarato/ansible-CentOS7-Observium/badges/gpa.svg)](https://codeclimate.com/github/Findarato/ansible-CentOS7-Observium) [![Test Coverage](https://codeclimate.com/github/Findarato/ansible-CentOS7-Observium/badges/coverage.svg)](https://codeclimate.com/github/Findarato/ansible-CentOS7-Observium/coverage)

This ansible role will setup Observium on Centos 7

To remove the monitoring from installing just comment out or remove it from site.yml

```yaml
- hosts: all
  remote_user: root
  roles:
  - common
  - observium
```

## NTP

With out any alteration NTP is installed and configured by default. This is done in the common role. This can also be removed from this by removing the common role.
