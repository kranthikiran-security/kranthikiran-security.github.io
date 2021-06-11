---
layout: post
title: 2.Setting up Lab for iOS App Pen testing
categories: [iOS , iOS Penetration Testing ,Security]
---
In Continuation...to the post [Setting up Lab for iOS App Pentesting](https://kranthikiran-security.github.io/iOS-Security-Synopsis/). If you are reading this blog for the first time 
please read the first post and come back , as it is a series of posts.[click here for Part -1](https://kranthikiran-security.github.io/iOS-Security-Synopsis/).

Check the suitable tool as per your iOS version compatiablity.(Table which is given in the last Part of this series). 

Download ipa file according to your iOS version and install it in iDevice, Follow this steps

we will use some software to install IPA files on iOS It also can help you exploit.

#### I. Cydia Impactor:
Cydia Impactor is a GUI tool for working with mobile devices. It has features already, but is 
still very much a work-in-progress. It is developed by Saurik

#### How to install H3lix Jailbreak for iOS 10.0.1 - 10.3.4 with Alt Deploy:
Step 01 – Download H3lix jailbreak IPA.
Step 02 – Download Cydia impactor.
Step 03 – Connect your iOS device to Computer.
Step 04 – Launch Cydia Impactor and drag and drop H3lix jailbreak IPA to Cydia Impactor to start 
side loading.
Step 05 – Cydia Impactor now requires your Apple ID details and submit the details.
Step 06 – Wait for side loading complete and once complete it you will have a H3lix app on your 
device home screen.
Step 07 – Now you can disconnect the device from the computer.
Step 08 – You cannot launch the app until you trust the app. Go to Settings > General > Profiles 
& Device Management and trust the app.
Step 09 – Launch the H3lix app and tap the jailbreak button.Step 10 – Wait for the already jailbroken message.
Step 11 – Now you should see Cydia on your home screen.

#### II. Alt Deploy:
Alt Deploy is a macOS solution for signing and side loading IPA files to your iPhone or iPad, 
including some jailbreak tools, without worrying about app certificates being revoked – this tends to 
happen with alternative download methods, such as third-party app stores but AltDeploy fixes that 
issue.

It is based on Riley Testut’s AltStore installer app and provides a number of preinstalled apps 
to choose from, as well as signing any other IPA file. It looks and works the same as Cydia Impactor, 
requiring your Apple ID credentials.

With Alt Deploy, you will get a Mail app add-on; this must be enabled in client preferences 
for the app. Once enabled, AltDeploy will work, but you must ensure your Mail app is open all the 
time you use AltDeploy.

#### How to install H3lix Jailbreak for iOS 10.0.1 - 10.3.4 with Alt Deploy:
Step 1: Download the H3lix Jailbreak for iOS 10.0.1 - 10.3.4 IPA file onto your computer.
Step 2: Download Alt Deploy from here.
Step 3: Open the AltDeploy and sign in with you Apple Id first; you can do it by clicking AltDeploy at 
the top of your screen; there you’ll see it add Apple Id option. You can add multiple Apple Ids as 
well; you can select through dropdown on the interface. This looks similar to Cydia Impactor with 
some improved features.

![image](https://user-images.githubusercontent.com/85728232/121729253-deebb480-cb0b-11eb-9e80-f260a2f89d74.png)

Step 4: Connect your device to your computer using a USB cable.

![image](https://user-images.githubusercontent.com/85728232/121729334-fa56bf80-cb0b-11eb-9256-7b354d0f11e1.png)

Step 5: Drag and drop the IPA file on to the AltDeploy, and press the start button. A process will start 
to do everything for you, like registering stuff and downloading stuff as well.
If you’re not comfortable providing it, then create an alternative Apple ID and use that instead.

![image](https://user-images.githubusercontent.com/85728232/121729438-1bb7ab80-cb0c-11eb-92c3-897978e3f068.png)

Step 6: After the app is installed, go to Settings -> General -> Profiles (or “Device Management” / 
“Profiles & Device Management”). Find the profile with your Apple ID and open it.

![image](https://user-images.githubusercontent.com/85728232/121729575-44d83c00-cb0c-11eb-95b1-402cb3d41db6.png)

Step 7: Tap on the Trust button. After this process application found to main springboard. Run or 
open application to jailbreak idevice.

![image](https://user-images.githubusercontent.com/85728232/121729750-70f3bd00-cb0c-11eb-94df-7ce7df40f290.png)

#### Jaibreaking online (Direct):
IOS 10 - IOS 10.3.4 JAILBREAK
Old iPhone and iPad users still use old iOS versions such as iOS 10 and iOS 9. iOS 10 is still a 
well performed iOS version for old devices and jailbreak available for iOS 10 - iOS 10.3.4.
Spyware contains bootstraps for both doubleh3lix and Meridian jailbreak tools.

If you are running any of these tools, it will automatically load your jailbreak via Safari. 
However, if you have no jailbreak running on your device, you can choose any one of them.

#### Why is a Safari jailbreak useful?

Firstly, a Safari jailbreak lets you jailbreak your device without Cydia Impactor or a computer. 
Generally, you need to install the IPA file on your device using Cydia Impactor on a Windows or Mac 
but this is a non-issue with a browser-based tool.

Secondly, it negates the need to use third-party signing utilities such as ReProvision or 
Ext3nder Installer.

Thirdly, it turns an existing semi-untethered jailbreak into a quasi-fully untethered jailbreak. 
Whenever the certificate of your jailbreak app expires, you can easily open Safari and load the 
exploit in a jiffy. Just make sure you have an internet connection and you will be good to go.

Step 1:  Launch Safari web browser and open Spyware’s website totally-not.spyware.lol. Don’t be 
fooled by the dated skeuomorphic design of this website, it’s the real deal and can jailbreak your 
device in an instant.

Step 2:  Slide the “slide for spyware” all the way to the right.

Step 3:  The website will now display the “Running exploit…” message. Wait and allow it to complete 
the exploitation.

Step 4:  Wait for your device to respring.

Step 5:  That’s all there’s to it! You can now run Cydia like you normally do.






























