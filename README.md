# HomeServer-Guide
This is a guide for those individuls who want to convert their old PC into a HomeServer using free and open source tools.

## Purpose for creating this repository
- It took a lot of my time finding the right resources and services which can be integrated easily and are really useful.
  
- I want to help people save time and give them a step by step guide.

## Requirements
1. Old PC or any pc you want to convert into a server
2. Pendrive >= 16GB
3. Wifi Router

## Setup 
### Step1: Setting up UBUNTU SERVER OS
1. Download Ubuntu server ISO 
2. Make bootable pendrive with Rufus
3. Boot from the pendrive and start setting up the ubuntu server on your system  

Reference Video [HERE](https://youtu.be/0-T7af_lRF8?feature=shared)

### Step2: DHCP IP Binding / Static IP


> [!TIP]
> Every router has little different admin settings so names can be like IP Reserve , Static IP , etc.  
- Open your routers Setting 
- by entering default gateway ip adderess in a browser 
- to check your routers ip address enter this command in terminal 
- for windows 
- ipconfig 
- for linux 
- ifconfig 
  
### Step3: Configuring SSH

=> A network protocol that allows users to securely access and manage remote computers.

- Install OpenSSH by following command 
```Shell
sudo apt install openssh
```
- Remotely Access Terminal from another device by entering 

```sudo ssh device_name@device_ipaddress``` <br>

Eg:
`sudo ssh adserver@192.168.1.9`

Reference Video :[HERE](https://youtu.be/3FKsdbjzBcc?feature=shared)
  
### Step4: Setting up CasaOS

=> Gives a good dashboard to manage your server.<br>
=> Provides apps in form of docker container. 

- Setup casaos by simply typing this command:

```
curl -fsSL https://get.casaos.io | sudo bash
```
Reference Github: https://github.com/IceWhaleTech/CasaOS

=> After Setup , Enter the server IP in any browser to access the CasaOs dashboard


<div align="center"><table><tr>CasaOS</tr><tr><td>
<img src="Screenshots/CasaL.png"/></td><td>
<img src="Screenshots/CasaD.png"/></td></tr></table></div>

### Step5: File Sharing
=> CasaOS made samba protocol very simple just one click 
- select the folder which you want to share and click share
- Copy the path and paste it in windows file explorer 

<div align="center"><table><tr>CasaOS</tr><tr><td>
<img src="Screenshots/CasaShare.png"/></td><td>
<img src="Screenshots/SharePath.png"></td></tr></table></div>
 

---

 <kbd>Ctrl</kbd>

<a id="installation"></a>
<img src="https://readme-typing-svg.herokuapp.com?font=Lexend+Giga&size=25&pause=1000&color=CCA9DD&vCenter=true&width=435&height=25&lines=INSTALLATION" width="450"/>
---
[Arch Linux](https://wiki.archlinux.org/title/Arch_Linux)


> [!IMPORTANT]
> The install script will auto-detect an NVIDIA card and install nvidia-dkms drivers for your kernel.
> Please ensure that your NVIDIA card supports dkms drivers in the list provided [here](https://wiki.archlinux.org/title/NVIDIA).

> [!CAUTION]
> The script modifies your `grub` or `systemd-boot` config to enable NVIDIA DRM.


```shell
cd ~/HyDE/Scripts
git pull origin master
./install.sh -r
```
<!-- comment -->
<img alt="TailscaleD" src="Screenshots/TailscaleD.png">