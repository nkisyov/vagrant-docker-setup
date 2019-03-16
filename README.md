# vagrant-docker-setup

A simple setup for runniung vagrant box with peinstalled Docker. For Windows hosts :)  
Will build Ubuntu 18.04 box and install docker.


# Requirements

Vagrant, VirtualBox and GitBash (or similar tool).


# Setup

Remove the `.gitignore` file from `source/` folder.  
Copy your project source in `source/` folder.  


# Usage

Build box
```bash
vagrant up
```

Log in the box and go to source folder
```bash
vagrant ssh
cd /source/
```

Switch off box
```bash
vagrant halt
```
