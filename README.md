Apple TV Ansible
================

This repo is nothing more than a simple Ansible playbook to provision my
first generation Apple TV running
[Kinos](https://forum.kodi.tv/showthread.php?tid=313407) by Soli. Right now
it's not much, but there are planned improvements for Kinos to run Ubuntu 10.04,
at which point I expect it to be more capable, and so I'll probably expand on
this playbook then.

## Prerequisites
To run this, you simply need Ansible and its dependencies installed on your
local "master" machine. In my case, I run it from Ubuntu in WSL:

~~~bash
$ sudo apt-get install -y ansible
~~~

## Usage
Once you have Ansible installed, simply run the playbook using
`ansible-playbook`:

~~~bash
$ ansible-playbook -i "${APPLE_TV_HOSTNAME}," --ask-pass
~~~
