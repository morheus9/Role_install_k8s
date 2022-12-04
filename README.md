install_k8s
=========

Installs k8s.

Requirements
------------

You have to rename your nodes, then check defaults and just start this role!

Role Variables
--------------

Defaults:
```
nodes:
  - 192.168.1.110 k8smaster.example.net k8smaster
  - 192.168.1.111 k8sworker1.example.net k8sworker1
  - 192.168.1.112 k8sworker2.example.net k8sworker2

cni_link: https://github.com/containernetworking/plugins/releases/download/v1.1.1/cni-plugins-linux-amd64-v1.1.1.tgz
```
Example Playbook
----------------
```
- hosts: servers
  roles:
     - role: install_k8s
```
Author Information
------------------

nodegopher@gmail.com
Nagornov Vyacheslav
