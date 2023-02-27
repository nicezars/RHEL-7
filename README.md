# RHEL 7 CIS

[![N|Solid](https://www.rededucation.com/wp-content/uploads/2019/08/red-hat-logo-c-sample_1-1.png)](https://gitlab.consulting.redhat.com/tsel)

Configure RHEL 7 machine to be CIS compliant.

# Requirements
------------
You should carefully read through the remediation tasks to make sure these changes will not break your systems before running the playbooks.

# Role Variables
--------------
Refer defaults/main.yml for more info on role variables defined.

# Installation
--------------

```sh
$ yum install ansible,git -y
$ git clone ssh://git@gitlab.consulting.redhat.com:2222/tsel/tsel-rhel7-cis.git
```

# Dependencies
--------------
Ansible latest

# Example Playbook
--------------
```sh
- name: Execute CIS benchmark Scan for RHEL 7
  include_role:
    name: rhel7scanning
  tags: always
```

# Tags
--------------
Some of the example tags are
```sh
ansible-playbook playbook-rhel7scanning.yml --tags rule_1.1.1.1
ansible-playbook playbook-rhel7scanning.yml --tags rhel7
ansible-playbook playbook-rhel7scanning.yml --tags level2
ansible-playbook playbook-rhel7scanning.yml --tags section4
```

# License
------------------
All rights reserved.

# Author Information
------------------
None
