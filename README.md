# Ansible elasticsearch Role #

Ansible role to install and configure elasticsearch on RedHat/CentOS or Debian/Ubuntu. Feedback, bug-reports,
requests, is welcomed and can be done via
[github issues](https://github.com/New-Edge-Engineering/ansible-ansible/issues).

## Execution Requirements
- Tested on Mac OS X with Ansible 1.7.

## Dependencies
This role does not have a hard dependency on any other role to deploy but rundeck does require java to be installed. smola's
[ansible-java-role](https://github.com/smola/ansible-java-role) is a good choice with the following configuration:

 * **Debian:** Ensure java_packages has a debian java package in it, i.e. openjdk-7-jre-headless
 * **RedHat:** Ensure java_packages has a debian java package in it, i.e. java-1.7.0-openjdk, had to adjust role to include RedHat.yml in main.yml to work.

## Role Variables

 * `elasticsearch_version`: The major and minor version to be installed, defaults to `1.4`.
 * `elasticsearch_plugins`: Defaults to empty list but can be a list of plugin dictionaries containing; name, file or url

## Example Playbook

    - hosts: search
      roles:
        - { role: smola.java }
        - { role: neel.elasticsearch }

## License ##

Licensed under the MIT License. See the LICENSE file for details.

## Author Information

Created in 2014 by [Jeff Geerling](http://jeffgeerling.com/), author of [Ansible for DevOps](http://ansiblefordevops.com/).
Modified in 2015 by [Matthew Green](http://uk.linkedin.com/in/matthewgeraldgreen/en)
