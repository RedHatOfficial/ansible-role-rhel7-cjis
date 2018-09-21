# Criminal Justice Information Services (CJIS) Security Policy

[![Build Status](https://travis-ci.org/RedHatOfficial/ansible-rhel7-cjis-role.svg?branch=master)](https://travis-ci.org/RedHatOfficial/ansible-rhel7-cjis-role)
[![Ansible Role](https://img.shields.io/ansible/role/29970.svg)](https://galaxy.ansible.com/RedHatOfficial/rhel7-cjis)
[![GitHub release](https://img.shields.io/github/release/RedHatOfficial/ansible-rhel7-cjis-role.svg)](https://github.com/RedHatOfficial/ansible-rhel7-cjis-role/releases/latest)

Ansible remediation role for profile cjis
Profile Title:  Criminal Justice Information Services (CJIS) Security Policy
Profile Description:
This profile is derived from FBI's CJIS v5.4
Security Policy. A copy of this policy can be found at the CJIS Security
Policy Resource Center:

https://www.fbi.gov/services/cjis/cjis-security-policy-resource-center
  
Benchmark ID:  RHEL-7  
 
XCCDF Version:  1.1  
  
This file was generated by OpenSCAP 1.2.17 using:  
	$ oscap xccdf generate fix --profile cjis --template urn:xccdf:fix:script:ansible xccdf-file.xml   
  
This script is generated from an OpenSCAP profile without preliminary evaluation.  
It attempts to fix every selected rule, even if the system is already compliant.  
  
How to apply this remediation role:  
$ ansible-playbook -i "192.168.1.155," playbook.yml  
$ ansible-playbook -i inventory.ini playbook.yml

# Requirements

- Ansible version 2.3 or higher

# Role Variables

To customize the role to your liking, check out the [list of variables](vars/main.yml).

# Dependencies

N/A

# Example Playbook

Run `ansible-galaxy install RedHatOfficial.rhel7-cjis` to
download and install the role. Then you can use the following playbook snippet.


    - hosts: all
      roles:
         - { role: RedHatOfficial.rhel7-cjis }


Then first check the playbook using (on the localhost):

    ansible-playbook -i "localhost," -c local --check playbook.yml

To deploy it, use (this may change configuration of your local machine!):

    ansible-playbook -i "localhost," -c local playbook.yml


# License

BSD-3-Clause

# Author Information

This Ansible remediation role has been generated from the body of security policies developed by the SCAP Security Guide project. Please see https://github.com/OpenSCAP/scap-security-guide/blob/master/Contributors.md for an updated list of authors and contributors.
