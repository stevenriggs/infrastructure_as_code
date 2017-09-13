Chef Setup notes
================

Install VirtualBox

Setup internal network

Install CentOS 7

Setup networking
----------------
Modify `/etc/sysconfig/network-scripts/ifcfg-enp0s8`(for interface enp0s8) Change ONBOOT=no to ONBOOT=yes

`ifup enp0s8`

`systemctl disable firewalld`
Disable selinux `/etc/selinux/config`

per: https://learn.chef.io/modules/manage-a-node-chef-server/rhel/bring-your-own-system/set-up-your-workstation#/

Install Chef DK
---------------
`wget https://packages.chef.io/files/stable/chefdk/2.1.11/el/7/chefdk-2.1.11-1.el7.x86_64.rpm`

Install Chef server core
------------------------
`yum install wget`
`wget https://packages.chef.io/files/stable/chef-server/12.16.2/el/7/chef-server-core-12.16.2-1.el7.x86_64.rpm`

LEFT OFF HERE
https://docs.chef.io/install_server.html#standalone
https://getchef.zendesk.com/hc/en-us/articles/204205284-Why-am-I-receiving-a-warning-about-exceeding-the-number-of-licensed-nodes-
