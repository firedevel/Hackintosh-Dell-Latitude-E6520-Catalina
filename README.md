# Hackintosh Dell Latitude E6520  

<p align="center">
  <img src="https://github.com/firedevel/Hackintosh-Dell-Latitude-E6520-Catalina/blob/main/e6520.png">
</p>

## macOS Catalina -  
I've no idea how to make HD3000 work in BigSur +, It only supports Catalina -

## Hardware

Type | Spec
:---------|:---------
Model Name      | Dell Latitude E6520
CPU              | Intel(R) Core(TM) i7-2620M CPU @ 2.70GHz Sandy Bridge
RAM           | 4 GB 1333 MHz DDR3
Internal Graphics Card | Intel® HD Graphics 3000
Has External Graphics Card | No
Wi-Fi             | Intel Centrino Advanced-N 6205 AGN
Ethernet          | Intel 82579LM
Audio       | IDT IDT92HD90BXX


![Hardware-1](https://github.com/firedevel/Hackintosh-Dell-Latitude-E6520-Catalina/blob/main/config-1.png)

![Hardware-2](https://github.com/firedevel/Hackintosh-Dell-Latitude-E6520-Catalina/blob/main/config-2.png)

## What's not working 
Type | Problem | Status
:---------|:---------|:----------
IGPU | OCLP not working with this machine, so BigSur + is not supported |  ❌  
AppleALC.kext | Soundcard only work with VoodooHDA |  ⚠️  
Touchpad | acidanthera/VoodooPS2 only work with BigSur + |  ⚠️  

## What's you have to do 
  
Type | Info | Status
:---------|:---------|:----------
SMBIOS Settings  | With [GenSMBIOS] you should definitely set your SMBIOS settings and ROM value for iCloud and Apple services. ROM value is your ethernet MAC address. Be sure your ethernet is en0 in Hackintool. |  ⚠️
Patching IGPU  | Patching HD3000 in Catalina by using [chris1111/Legacy-Video-patch](https://github.com/chris1111/Legacy-Video-patch) |  ⚠️
  