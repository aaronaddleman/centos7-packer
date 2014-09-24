Centos7 Vagrant box
===================

Minimal (Core from NetInstall ISO) CentOS 7.0 install,
built using kickstart and the ansible-local provisioner.

Only supports Virtualbox provider for now.

This takes about 15 minutes to build, so if you're short
on time you can just grab it from:

https://github.com/rasputnik/centos7-packer/releases/download/v0.1/CentOS-7.0-1406-x86_64-v20140721-virtualbox.box

## config

see 

* http/bootstrap-ks.cfg for the initial kickstart
* ansible/bootstrap.yml for the Ansible build
* centos7.json for exact details of build steps

## notes

As a side effect of the build, you'll have the (beta)
EPEL7 repo installed and a copy of Ansible installed
(since they're both needed to use the ansible-local
provisioner).

These could easily be removed if you wanted, personally
I find them both indispensible.
