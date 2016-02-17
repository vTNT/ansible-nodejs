# Ansible role for Nodejs 

This role will install nodejs on ubuntu 14.04

## Tested On

  * Ubuntu 14.04

## Defaults

The `defaults/main.yml` should be pretty clear on the usage and values.  

## Usage

The tests in the respository should be pretty straight forward, but here are
some examples:

### Nodejs

playbook.yml:

```
- name: Install and run Nodejs
  hosts: all
  sudo: True

  vars:
    nodejs_global_packages: grunt
  
  roles:
    - { role: ansible-nodejs }

```

## TODO

  * Extract supervisor to it's own role
  * Extend to other distros

