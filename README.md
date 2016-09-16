# ansible-newrelic-nginx
[![Build Status](https://travis-ci.org/jimbydamonk/ansible-newrelic-nginx.svg?branch=master)](https://travis-ci.org/jimbydamonk/ansible-newrelic-nginx)

Install and configure newrelic-nginx.

Requirements
------------

NA

Role Variables
--------------

The default variables for this role are listed below. They are defined in defaults/main.yml`.

```yml
---
newrelic_nginx_sources: []
newrelic_nginx_log_file: /var/logs/nginx-nr-agent/nginx-nr-agent.log

```

Dependencies
------------

None

Example Playbook
----------------

Simple Playbook:

    - hosts: servers
      vars:
        newrelic_nginx_sources:
          - title: Source1
            name: source_one
            url: http://localhost
      roles:
        - ansible-newrelic-nginx


License
-------

Apache

Author Information
------------------
Mike Buzzetti
