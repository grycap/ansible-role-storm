[![License](https://img.shields.io/badge/license-Apache%202-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
[![Build Status](https://travis-ci.org/grycap/ansible-role-storm.svg?branch=master)](https://travis-ci.org/grycap/ansible-role-storm)

Apache Storm Role
===================

Install [Apache Storm](https://storm.apache.org/).  
This role has been tested only with Ubuntu 16. Is not ensured that it will work with other systems.

Role Variables
--------------

Variables used in this role:

	# Install info
	storm_version: "1.0.2"
	## System info
	storm_system_user_name: storm
	storm_system_group_name: storm
	storm_system_comment: Storm system user
	storm_system_shell: /bin/false
	storm_system_user_home: "/var/lib/{{ storm_system_user_name }}"

Example Playbook
----------------
```
- hosts: server
  roles:
  - { role: 'grycap.storm' }
```

Contributing to the role
========================
In order to keep the code clean, pushing changes to the master branch has been disabled. If you want to contribute, you have to create a branch, upload your changes and then create a pull request.  
Thanks
