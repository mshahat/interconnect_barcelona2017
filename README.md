# PSG Event Oct 2017 @ Barcelona
As part of the event some deep dive sessions are planned, please go through this guide to get what is needed.

## Preparing for running the labs

Software you need to install or accounts you need to have to be able to carry on the labs during the workshops.

## Operating System
You should be able to run the labs if you are running on the following OS choices

* macOS
* Windows 10
  * Make sure to enable hardware virtualisation in BIOS
* Linux e.g. CentOS or Ubuntu

## Accounts

These accounts are needed to run through the labs:

* AWS
  * You will get assigned credentials by your instructor to access AWS to execute the relevant labs
  * AWS Username, AccessKeyId, SecretAccessKey

* Docker ID for Docker Hub
  * Create a Docker Hub account if you don't have one https://hub.docker.com/
  * Note your docker id and password

* TIBCO Cloud Integration
  * Sign up for trial EMEA - https://eu.account.cloud.tibco.com/signup/tci
  * Sign up for trial Americas - https://account.cloud.tibco.com/signup/tci
  * Sign up for trial Australia - https://au.account.cloud.tibco.com/signup/tci
  * If you have an expired trial - Google Hangout me for the form to request extension

<!-- insert docker login image -->
![Screenshot](https://github.com/mshahat/interconnect_barcelona2017/blob/master/graphics/Screen%20Shot%202017-10-11%20at%2018.53.55.png)

## Software

### TIBCO

Download TIBCO installers from https://edelivery.tibco.com 

install the following software on your machine. ( if you prefer to use a vm to leave your machine neat, make yourself at home ! )

* optional - BW5.13 including RV, TRA
* BWCE 2.3.1
* TCI Studio 1.0.5
* TCI CLI - follow install instructions https://integration.cloud.tibco.com/docs/getstarted/installation/installing-cli.html
* FTL 5.2.1
* optional - EMS 8.4 ( this is needed for jms libs, we're providing the libs, so no need to install if you don't need to )

### Thirdparty

For Linux users use your package manager for most of these, or follow the links provided below.
For macOS users homebrew is a decent option to install thirdparty software https://brew.sh/

I'm including the homebrew commands to download some sofware for those on macOS

If you fancy using a **vagrant box** which provides some of these components, [GO HERE](https://github.com/mshahat/interconnect_barcelona2017#option-b---vagrant-box)

* Text Editor, I use VS Code. TextMate, Notepad++ ...etc.
* Microsoft Powerpoint - to go through the labs instructions
* Docker CE 17.x, Docker for mac, Docker for Windows - https://www.docker.com/community-edition
* optional - Kitematic - to browse Docker Hub images - https://github.com/docker/kitematic/releases
* Java 1.8 or else

#### Option A - local installs
install the following to your machine 

* AWS cli - install from https://aws.amazon.com/cli/
  ```console
  brew update && brew install awscli
  ```
* kubectl - kubernetes cli - https://kubernetes.io/docs/tasks/tools/install-kubectl/
  ```console
  brew update && brew install kubectl
  ```
* kops - kubernetes operations
  ```console
  brew update && brew install kops
  ```
#### Option B - Vagrant box
use vagrant box to have the following preinstalled

* AWS cli
* kubectl
* kops

To have vagrant running, please install 

* Virtualbox - https://www.virtualbox.org/wiki/Downloads
  ```console
  brew cask install virtualbox
  ```
* Vagrant - https://www.vagrantup.com/downloads.html
  ```console
  brew cask install vagrant
  ```

## Operating System
You can decide to use macOS, Windows 10 or Linux ( any distro ). 
You can also use a virtual machine to run the labs. Please choose the operating system of choice 

* macOS 
* Windows 10
 * Make sure to enable hardware virtualisation in BIOS
* Linux e.g. CentOS or Ubuntu

*OR* 

We're providing a vagrant box to use, which includes this software 
* kubectl
* etc.

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
