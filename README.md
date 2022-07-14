Ubuntu desktop setup automation with Ansible

This repository contains configuration files for setting up all development tools on Ubuntu desktop using Ansible playbooks.

### Steps to follow:
1. Install `git` and `ansible` using following commands:
```shell
sudo apt install git ansible
git config --global user.email "dhiraj.pathania@gfk.com"
git config --global user.name "Pathania, Dhiraj"
```
2. Run `ansible-pull` to apply the ansible configuration:
```shell
sudo ansible-pull -U https://github.com/edhipat/ansible_desktop.git ubuntu.yml
```


### Optional steps:
If Ubuntu desktop is installed on VirtualBox, then
1. Install VBox Guest addition on Guest OS.
2. Resolve the NumLock toggle issue by running this command on Host CLI:
```commandline
cd "C:\Program Files\Oracle\VirtualBox"
VBoxManage setextradata "Ubuntu-2004" GUI/HidLedsSync "0"
```
