# PSG Event Oct 2017 @ Barcelona
Some deep dive sessions are planned. This guide is to help prep yourself for the sessions.

## Preparing for running the labs
This guide is to provide a list of prerequisites which need to be installed on your machine before the Workshops on Friday October 13th 

## Accounts

* AWS
 * You will get assigned credentials by your instructor to access AWS to execute the relevant labs

```
1. Download the Private key for AWS account from AWS Web Console and save it on to your workstation.
2. Follow steps below to get public key. 
i. Login into your EC2 instance and see what's inside the ~/.ssh folder 
ii. $ ls -la ~/.ssh
You should find an authorized_keys file
iii. Cat the file (is the corresponding public key):
 $ cat ~/.ssh/authorized_keys
 Outuput:
 ssh-rsa SAGsg43 (....) sd53ySGS aws_machines 
	Please notice the string at the end of the output: "aws_machines". That's there because I chose 	it when created the .pem file. For you it may be different.

iv. Now, return to your workstation and save that last output into a file to create your copy of the public key:
$ echo ssh-rsa SAGsg43 (....) sd53ySGS aws_machines >> ~/.ssh/aws_machines.pub
Now, if you want, you can copy the .pem file without the extension to create a proper private key file:
$ cp ~/.ssh/aws_machines.pem ~/.ssh/aws_machines 
```

* Docker Hub
 * Create a Docker Hub account

## Operating System 
You can decide to use macOS, Windows 10 or Linux ( any distro ). 
You can also use a virtual machine to run the labs. Please choose the operating system of choice 

* macOS 
* Windows 10
 * Make sure to enable hardware virtualisation in BIOS
* Linux e.g. CentOS or Ubuntu

## TIBCO software

* BW 5.13 - RV, TRA
* FTL 5.2.1
* BWCE 2.3.1
* TCI Studio 

## Thirdparty

* Microsoft Office - will need to go through some slides for the labs instructions
* Text editor of choice - e.g. Microsoft VS Code, Notepad++
* Docker CE - Docker for macOS, Docker for Widnows, Docker on linux using yum or apt-get
* Java 1.8
* golang

* AWS CLI
* Kubectl
* Kobs
* Oracle VirtualBox
* Vagrant
* Putty - for Windows users
