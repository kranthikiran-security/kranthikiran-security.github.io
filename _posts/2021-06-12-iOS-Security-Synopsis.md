---
layout: post
title: Part-1 : Setting up Lab for iOS App Pen testing
categories: [iOS , iOS Penetration Testing ,Security]
---

### Need for jailbreaking 

iOS itself has a lot of security features. Neither installing any app outside of AppStore nor accessing its file system by default is allowed by iOS.
To conduct a security assessment of an iOS application, we will need to access the iDevice file system and keychain data, hook debuggers to application, and so on.It is not possible to perform,iOS pen testing with so many restrictions and this is the point where we need to jailbreak the iDevice 
in order to bypass security restrictions provided by iOS.

### What is jailbreak?
Jailbreaking is the privilege escalation from mobile user to root user.
Jailbreaking is exploiting the iOS vulnerability and maintaining root access on the device by 
installing utilities on it. Finding a jailbreak is itself an in-depth topic and beyond the scope.

Jailbreaking allow us to do the following:
-Access complete file system on iDevice
-Install any app from outside App store

### Types of Jailbreaks
Basically, there are three types of jailbreak, described as follows:

#### Tethered:
In this type, Jailbreak is temporary. When you turn off your device you can’t boot your 
device up without connect it to PC to delete the Jailbreak and then you are able to boot the device. 
In this Jailbreak you have to install it every time you turn off your device.

#### Semi Tethered:
It looks like tethered jailbreak with addition thing that here you can turn off your device and 
boot it again without any problem. The features are limited.

##### Untethered:
It is the common jailbreak and the new one. It gives the user ability to run all the tools and 
applications they downloaded anytime they want. In this type, you can turn off your device without 
fear of losing the jailbreak.

### How jailbreak works
#### bootchain
The bootchain (also called chain of trust) is the system by Apple which can tries to ensure 
that only signed or trusted code is loaded on an iOS device.
The bootchain consist couple of deferent modules that load each other and between the 
loadings there are check points that Apple put it in order to prevent unauthorized access to the 
code.

![image](https://user-images.githubusercontent.com/85728232/121724433-81546980-cb05-11eb-8b33-fda29c4aece7.png)

#### Boot ROM 
it is the first significant code that starts in the device. It is read-only which means it 
can’t be modified by Apple when they release a device. This part is hard to Jailbreak because it 
connects with the hardware not the software it in the chip inside the device, but if someone 
Jailbreak this part, Apple can’t stop the Jailbreak and they have to change the hardware next 
time they publish a new device.

#### Low level Bootloader (LLB)
which is a part of the software. It runs several setup routines. On 
firmware versions 2.0 and higher it checks the signature of Boot ROM before jumping to it. If 
someone found vulnerabilities and Jailbreak this part, Apple can close the vulnerabilities by 
releasing new software version (iOS firmware).

#### iBoot
it is Apple’s stage 2 bootloader for all of the devices. It runs what is known as Recovery 
Mode. It has an interactive interface which can be used over USB or serial.

#### IOS Kernel
it is using page verification. When you start application the Kernel will verify if the 
application has the code singing in tagged. If it has “SHA1” verification it will pass the application 
to AMFI which is a Kernel extension. The Kernel doesn’t verify if the application’s signature is 
valid, it is only verified if the signature is exist.

#### IOS apps
These are the phase after the Kernel boot. It goes hand to and with iOS Kernel. For iOS all 
applications have to be signed since the launch of the App Store (iOS 2.0), this includes all 
system binaries that come with iOS. For the end user. This code signing enforcement cannot be 
disabled, which makes that an end user can only install applications from the App Store.

##### what else ?
/private/etc/fstabis is where all the iOS files are stores and must be patched. fstab is like a 
switch that is giving you the ability to control the media partitions and the permissions. By default, 
fstab is setting as a read-only mode that letting you to read or view only without making any 
changes. To be able to make any modifications, you have to set the fstab as “read-write” mode. It is 
very important for your Apple device because it is controlling the permission of the media partition 
and the root.The big problem is to pass in all the files you need through the various 

The big problem is to pass in all the files you need through the various checkpoints. The 
checkpoint is what Apple does in order to ensuring the file is legit or coming from a third party. Every 
file is signed by a key. The file will be through a way and be unusable if this file without kay.

In short, we can access to the door if we either find a back door entry (bypass) or unlock the 
lock (patch all checkpoints). Patching is a difficult and mostly not worth the effort. So, most people 
who make the jailbreak will try to find a backdoor entry or a bypass

### Hardware and Software requirements
The hardware that is required to perform a jailbreak is an iDevice running iOS versions up to 
8.x, 9.x. Also, the software required are Windows or macOS jailbreak utility and iTunes software.

### Jailbreaking iDevice
As a first step you have to know the version of your IOS system. Then search on Internet if 
this version has a Jailbreak or not. The best way to search is to get into the Jailbreak teams websites. 
Since Jailbreak is published by one team other teams published their copies too.

All jailbreaking tools available to install in application called Cydia, which is similar to the 
Apple App Store but applications available on Cydia are not checked by Apple and developers can 
submit their applications to distribute through Cydia


### History of Cydia
Cydia is a third-party installer application for all Apple devices. Developed by Jay Freeman 
(Saurik), Cydia is similar to the official App Store. Cydia is a manager mobile application for IOS, 
which enables the user to find and install tools or software packages on jailbroken device.

It’s important for you to jailbreak your IOS device to get the Cydia. With Cydia everyone has the option 
of customizing their devices

### Jailbreak Methods
##### Jaibreak using Computer software
COMPATIBLE JAILBREAK TOOLS FOR IOS 10 - IOS 10.3.4
Here is a table with all iOS 10 versions and compatible jailbreak tools for each version.

|Jailbreak Tools       | iOS Version Compatiability |
|--------------------- | ---------------------------|
|H3LIX  Jailbreak      | iOS 10.3.4, iOS 10.3.3, iOS 10.3.2, iOS 10.3.1, iOS 10.3, iOS 10.2.1, iOS 10.2, iOS 10.1.1, iOS 10.1, iOS 10.0.3, iOS 10.0.2, iOS 10.0.1, iOS 10 (supports only 32 bit devices)|
|G0blin Jailbreak      | iOS 10.3, iOS 10.3.1, iOS 10.3.2, iOS 10.3.3 (supports 64 bit devices) |
|Meridian Jailbreak    | iOS 10.3.4, iOS 10.3.3, iOS 10.3.2, iOS 10.3.1, iOS 10.3, iOS 10.2.1, iOS 10.2, iOS 10.1.1, iOS 10.1, iOS 10.0.3, iOS 10.0.2, iOS 10.0.1, iOS 10 (supports 64 bit devices)|
|Yalu102 Jailbreak     | iOS 10.2, iOS 10.1, iOS 10.1.1, iOS 10.0.3, iOS 10.0.2, iOS 10.0.1, iOS 10 (supports 64 bit devices) |
|Houdini Semi Jailbreak| iOS 10.3.2, iOS 10.3.1, iOS 10.3, iOS 10.2.1, iOS 10.2, iOS 10.1.1, iOS 10.1, iOS 10.0.3, iOS 10.0.2, iOS 10.0.1, iOS 10
|Saigon Jailbreak      | iOS 10.2.1 |

 
 
 
 






