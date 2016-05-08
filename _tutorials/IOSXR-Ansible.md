---
title: "IOS-XR-Ansible"
published: true
author: Mike Korshunov
---
## Introduction
In this tutorial we are going to cover XRv4 configuration with Ansible. We will setup and try simplest configuration with Unix machine connected to XRv64.

## Prerequisites
- Computer with with 4-5GB free RAM;
- Vagrant;
- Ansible;
- [XRv64 image](http://engci-maven-master.cisco.com/artifactory/appdevci-snapshot/);

### Vagrant pre-setup

To add XR box, image should be downloaded, after this issue the command:
	
    $ vagrant box add xrv64 iosxrv-fullk9-x64.box_2016-05-07-19-04-50

Image for Ubuntu will be downloaded from official source:
	
    $ vagrant box add ubuntu/trusty64
    
Let's check for result, we should have box available, box ubuntu/trusty64 and xrv64 should be displayed:
![Box validation]({{site.baseurl}}/images/xr_ansible_01_box_list.png)

Next step to create Vagrantfile and boot up boxes:


mkorshun@MKORSHUN-2JPYH MINGW64 ~/Documents/workCisco/tutorial
$ vagrant up




sudo apt-get install python-setuptools python-dev build-essential git
sudo easy_install pip
git clone http://gitlab.cisco.com/aermongk/iosxr-ansible.git

conf t
interface GigabitEthernet0/0/0/0
 ipv4 address 10.1.1.20 255.255.255.0
 no shutdown
!
commit
end