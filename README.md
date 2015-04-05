<<<<<<< HEAD
# Ansible elasticsearch Role #

Ansible role to install and configure elasticsearch. Feedback, bug-reports, 
requests, is welcomed and can be done via
[github issues](https://github.com/New-Edge-Engineering/ansible-ansible/issues).

## Requirements & Dependencies ##
- Tested on Mac OS X with Ansible 1.5.

## License ##

Licensed under the MIT License. See the LICENSE file for details.
=======
# Ansible Role: Elasticsearch

[![Build Status](https://travis-ci.org/geerlingguy/ansible-role-elasticsearch.svg?branch=master)](https://travis-ci.org/geerlingguy/ansible-role-elasticsearch)

An Ansible Role that installs Elasticsearch on RedHat/CentOS or Debian/Ubuntu.

## Requirements

None.

## Role Variables

None.

## Dependencies

  - geerlingguy.java

## Example Playbook

    - hosts: search
      roles:
        - { role: geerlingguy.java }
        - { role: geerlingguy.elasticsearch }

## License

MIT / BSD

## Author Information

This role was created in 2014 by [Jeff Geerling](http://jeffgeerling.com/), author of [Ansible for DevOps](http://ansiblefordevops.com/).
>>>>>>> origin/master
