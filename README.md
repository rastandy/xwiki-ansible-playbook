XWiki Playbook
==============

Ansible playbook to install XWiki Enterprise in the Apache Tomcat
container with PostgreSQL as Database backend.

## Installation

First, you need to install the dependencies for this playbook by
issuing this command:

```shell
ansible-galaxy install -p roles --role-file=requirements.yml

```

You also need to install some git submodules through this commands:

```shell
git submodule init
git submodule update

```

## Testing

This playbook ships with a Vagrant file for testing purpouse. If you
want to take advantage of it, just install Vagrant and Virtualbox on
your machine and you should be able to setup a VM with XWiki up and
running by just issuing this shell command from the playbook
directory:

```shell
vagrant up

```

After that, you should be able to browse your XWiki instance at the
following url:

http://192.168.88.22:18080

Also, if you install the Vagrant landrush plugin, you can access your
instance by pointing your browser to this url:

http://xwiki.vagrant.test:18080

## Customization

The playbook variables and default values.

## Licence

GPLv3
