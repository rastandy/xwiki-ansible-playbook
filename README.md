XWiki Playbook
==============

Ansible playbook to install XWiki Enterprise with PostgreSQL as Database backend.

## Installation

First of all, you need to install the dependencies for this playbook
by issuing this command:

```shell
ansible-galaxy install -p roles --role-file=requirements.yml

```

You also need to install some git submodules through this commands:

```shell
git submodule init
git submodule update

```

## Configuration

The playbook variables and default values.



## Testing

This playbook ships with a Vagrant file for testing puropuse. If you
want to install quickly an XWiki instance in a virtual machine, you
need Vagrant and Virtualbox installed on your machine.

After installing them throw a:

```shell
vagrant up

```

in your shell from the directory where the playbook resides and after
Vagrant and Ansible finish their job, you should have your XWiki
instance up and running at this url:

http://192.168.88.22:18080

Also, if you install the Vagrant landrush plugin, you can access your
instance by pointing your browser to this url:

http://xwiki.vagrant.test:18080

Enjoy it.

## Licence

GPLv3
