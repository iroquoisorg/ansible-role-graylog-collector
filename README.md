# graylog-collector

[![Build Status](https://travis-ci.com/iroquoisorg/ansible-role-graylog-collector.svg?branch=master)](https://travis-ci.com/iroquoisorg/ansible-role-memcached)

Ansible role for graylog-collector

This role was prepared and tested for Ubuntu 16.04.

# Installation

`$ ansible-galaxy install iroquoisorg.graylog-collector`

# Default settings

```
graylog_server_url: "http://localhost:12900/"

graylog_collector_inputs: 
    - {id: "syslog", type: "file", path: "/var/log/syslog"}
    
graylog_collector_outputs: 
    - {id: "gelf-tcp", type: "gelf", host: "localhost", port: 12201}
    

```
