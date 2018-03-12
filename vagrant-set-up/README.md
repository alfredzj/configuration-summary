## How to set up your own vagrant in a scientific way?

### Introduction

* what is virtual box?

  - It supports the creation and management of guest virtual machines running versions and derivations of Windows, Linux, etc.
  
* what is vagrant?

  - Vagrant is an open-source software product for building and maintaining portable virtual software development environments (VirtualBox,...)
  - Vagrant allows you to bring up a virtual machine, which will behave the same way on your computer.
  
* why we want to use virtual box?

  - Multiple Operating Systems at a time without restarting the single computer.
  - Completely isolated virtual environment from host OS. 
 
* why we want to use vagrant?
  - Easy to set up the environment

### Get started!

1. Click this [link](https://www.vagrantup.com/downloads.html) and download corresponding version of vagrant. If you are using ubuntu, you don't want to use apt-get to install since the version is too old.

2. Assuming you are using ubuntu 16.04, you need to download the Debian version since [Ubuntu is Debian-based OS](https://unix.stackexchange.com/questions/28324/how-is-ubuntu-based-on-debian)

        ```sudo dpkg -i vagrant_2.0.2_x86_64.deb``` . 

3. Install VirtualBox.

        ```sudo apt-get install virtualbox```

4. Create a new directory for your configuration scripts. e.g. Websites, or Work-environments. This folder will not contain the VirtualBox binary files, just the Vagrant configuration scripts. 
Yu can orefer to this [Vagrantfile](https://github.com/alfredcoder/configuration-summary/blob/master/vagrant-set-up/Vagrantfile) as an example

5. Now you are free to start it. From the command line, run the following commands:

        ``` $ vagrant up```
        ``` $ vagrant ssh```
        
6. To return to your host machine, run the command:

        ``` $ exit```
        
7. To destroy the VM and remove the binary disk image:

        ``` $ vagrant destroy``` 
        
Note: This command must be run from the directory which contains the Vagrantfile for the box you wish to destroy. It will not remove any of your configuration files. To recreate the machine, use the commands in (5).
