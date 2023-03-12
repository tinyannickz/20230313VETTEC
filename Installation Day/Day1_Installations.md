# Installation Day

## WINDOWS ONLY!! Install Chocolatey

[Install Chocolatey](https://chocolatey.org/install)<br>

### Open Powershell as administrator and enter the following command `Set-ExecutionPolicy AllSigned`

<br>

### Run the following command to install Chocolatey `Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))`

---

## Install Virtual Box

[Virtual Box](https://www.virtualbox.org/wiki/Downloads)
![VBox Website](images/Screenshot%202023-03-12%20141113.png)

### Select the platform for your operating system

---

## WINDOWS ONLY!! Set up Windows environment to run Virtual Machines in Virtual box

We must ensure that windows Hyper-V is turned off, Run the following command: `Disable-WindowsOptionalFeature -Online -FeatureName Microsoft-Hyper-V-All
`
<br>
Also need to make sure that hypervisor launchtype is turned off: `bcdedit /set hypervisorlaunchtype off
`
<br>

## All commands must be run from an elevated prompt

## Install Vagrant

Windows:
<br>
`choco install vagrant`
<br>
Mac:
<br>
`brew install hashicorp/tap/hashicorp-vagrant`

---

## Install AWS CLI

For windows we will download the installer [here](https://awscli.amazonaws.com/AWSCLIV2.msi)
<br>
For Mac we will run a few commands from the terminal:
<br>
`curl "https://awscli.amazonaws.com/AWSCLIV2.pkg" -o "AWSCLIV2.pkg"`
<br>
`sudo installer -pkg AWSCLIV2.pkg -target /`
<br>
`aws --version`

---

## Install Python

run python --version, ensure a version 3.8 or higher is installed

For Mac, Python should already be installed
<br>
For Windows, If no python is installed, go to the Microsoft store ![store](images/Screenshot%202023-03-12%20142042.png) and search for python3.10
<br>
![Python3.10](images/Screenshot%202023-03-12%20142149.png)

---

## Install VS Code

Download the installer from [here](https://code.visualstudio.com/download)
<br>
For Mac, make sure you chose the correct chip
<br>
![chip](images/Screenshot%202023-03-12%20142516.png)

---

## Install Terraform

### Windows <br>`choco install terraform`

### Mac: <br> `brew tap hashicorp/tap`<br>`brew install hashicorp/tap/terraform`

---

## Install Node/NPM

Go [here](https://nodejs.org/en/download/) and install node based on your operating system
![NPM](images/Screenshot%202023-03-12%20142817.png)

---

## Install CDK

On all systems `npm install aws-cdk-lib`

---

## Install Docker Desktop

For Windows WSL is required to run docker desktop
<br>
Run powershell as admin and run the following command:
<br>
`wsl --install`
<br>
<br>

Windows: <br>
`choco install docker-desktop`
<br>
Mac:
<br>
Go [here](https://docs.docker.com/desktop/install/mac-install/) and follow the instructions based on the chip you have

---

## Install Git

Windows::
<br>
`choco install git`
<br>
Mac:
<br>
`brew install git`

---
