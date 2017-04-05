[![Build Status](https://travis-ci.org/godleon/ansible-role-linux_bonding.svg?branch=master)](https://travis-ci.org/godleon/ansible-role-linux_bonding)


Role Name
=========

**godleon.linux_bonding**

Requirements
------------

### Hardware

The target machine is going to be provisioned should have multiple NICs for the bonding interface.

### Software

- Python2.7 (**Ubuntu Xenial**)
> sudo apt-get update && sudo apt-get -y install python2.7



Role Variables
--------------

The variables that should be passed to this role and a brief description about them are as follows:

```yaml
# bonding interface name
linux_bonding_InterfaceName: 'bond0'
# Slave interfaces
linux_bonding_SlaveNics:
  - 'nic1'
  - 'nic2'
  - 'nic3'
  - 'nic4'
```

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yml
- hosts: servers
  roles:
    - { role: godleon.linux_bonding }
```

License
-------

MIT

Author Information
------------------

**Leon Tseng** 

-  [godleon@GitHub](https://github.com/godleon)
