WELCOME!!!

This is my first attempt at creating a Android Hacking viritual image.

I was VERY inspired by Android Tamer Twitter handle - @androidtamer, creator - @anantshri

Note: I do not have all of the features as Android Tamer such as ROM Development and Forensics.

The image is built on top of Linux 18.04 LTE (Bionic Beaver) minimal installation. 

Now without further ado, what is on the image...

1/29/2021 - Removed Android-InsecureBankv2. Included ig learner and UnCrackable series apks.
1/23/2021 - Added GoatDroid APK to the Documents folder. I also removed Android Studio
as it was not needed. I also updated MobSF from 1.1 to 3.3. There's a new user interface
and more functionality. Note the dynamic analysis will not work as MobSF is inside of a virtual
machine.

Opening the menu option I added six subitems:
1. Dynamic Analysis which has settings to start MobSF Server and UI, Frida, and Drozer
2. Manual Analysis - apktool
3. Penetration Testing which has Nikto, Nmap, Burpsuite (free), SSLscan, Wireshark, w3af console and gui, ZAP
4. Reporting - Cherrytree and Keepnote
5. Reverse Engineering - baksmali, dex2jar, jadx, jadx-gui, jd-gui, smali

To use MobSF, first start the server, you will need to enter the password (security) as this app runs as root.
Once the server is started then start the UI. The website is http://localhost:8000. 

Note: You can't change the port.

In the /home/android/Documents folder I included some Android apps to play with.
1. MSTG-Hacking-Playground. The apk (application) is located at the following location:
/Documents/MSTG-Hacking-Playground/MSTG-Hacking-Playground/Android/MSTG-Android-Java-App/app
In this folder there are different apks based on the architecture of your computer.
2. DIVA (diva-beta.apk)
3. IG Learner (ig-learner.apk)
5. UnCrackable Series (Levels 1-4). NOTE: the fourth level have two files (r2pay-v0.0.apk and r2pay-v1.0apk)

You will need an Android emulator (I used android-x86 which is free), and from there you can install above apps onto the emulator (using adb install) and hack away :-)

For most of the files on this image I have done a git clone. I have also removed the .git and .github folder(s) to save space and make the VM as lean as possible.

I have built this image on VirtualBox. The image should work on VMWare.

If you feel adventureous and want to modify the image most of the files are saved in the following locations:
1. /opt - burp, zap, gradle
2. /usr/bin - scripts to make applications run
3. /usr/share/ - applications are saved in this location

To change the Menu options. Right click on the Menu option and select Edit Menus.
From there you will be presented with all of the applications on the OS.

If there are any issues please hit me up on twitter @thefluffy007. I will try my best to remediate the issue. 

Please note, this is my first image, so be patient for a response.

I hope you, user, have as much fun using this image as I did creating it.
