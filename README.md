Chef Setup notes
================

Install VirtualBox

Setup internal network

Install CentOS 7

Setup networking
----------------
Modify `/etc/sysconfig/network-scripts/ifcfg-enp0s8`(for interface enp0s8) Change ONBOOT=no to ONBOOT=yes

`ifup enp0s8`

Download Chef server core
-------------------------
`yum install wget`
`wget https://packages.chef.io/files/stable/chef-server/12.16.2/el/7/chef-server-core-12.16.2-1.el7.x86_64.rpm`

Install Chef server
-------------------
