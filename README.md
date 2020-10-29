[![License](https://img.shields.io/badge/license-Apache%202-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
[![Build Status](https://travis-ci.org/grycap/ansible-role-storm.svg?branch=master)](https://travis-ci.org/grycap/ansible-role-storm)

Apache Storm Role
===================

Install [Apache Storm](https://storm.apache.org/).  
This role has been tested only with Ubuntu 16. Is not ensured that it will work with other systems.

Role Variables
--------------

Variables used in this role:

	zk_version: "3.6.2"
	zk_download_mirror: "https://archive.apache.org/dist/zookeeper"
	zk_system_user_name: zookeeper
	zk_system_group_name: zookeeper
	storm_download_mirror: "http://apache.rediris.es/storm"
	storm_version: "2.2.0"
	num_supervisors: 1
	storm_type_of_node: front # front or wn
	storm_system_user_name: storm
	storm_system_group_name: storm

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
