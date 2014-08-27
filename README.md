Centos7 Vagrant box
===================

Minimal (Core from NetInstall ISO) CentOS 7.0 install,
built using kickstart and the ansible-local provisioner.

Only supports Virtualbox provider for now.

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
