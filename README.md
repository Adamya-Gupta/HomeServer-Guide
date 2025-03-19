# HomeServer-Guide
This is a guide for those individuls who want to convert their old PC into a HomeServer using free and open source tools.

## Purpose for creating this repository
- It took a lot of my time finding the right resources and services which can be integrated easily and are really useful.
  
- I want to help people save time and give them a step by step guide.

## Requirements
1. Old PC or any pc you want to convert to a server
2. Pendrive >= 16GB
3. Wifi Router

## Setup 
### Step1: Setting up UBUNTU SERVER OS
1. Download Ubuntu server ISO 
2. Make bootable pendrive with Rufus
3. Boot from the pendrive and start setting up the ubuntu server on your system  

### Step2: DHCP IP Binding / Static IP
- Open your routers Setting 
- by entering default gateway ip adderess in a browser 
- to check your routers ip address enter this command in terminal 
- for windows 
- ipconfig 
- for linux 
- ifconfig 
  

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