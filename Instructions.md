WELCOME!!!

This is the second version of this virtual machine.

I was inspired by Android Tamer Twitter handle - @androidtamer, 
creator - @anantshri

As well as the @TryHackMe Android room created by @stuxnet. I added more
Dynamic Analysis tools after seeing their room.

Note: I do not have all of the features as Android Tamer such as ROM Development 
and Forensics.

The image is built on top of a vagrant Linux 18.04 (Bionic Beaver) 
minimal installation. 

Some of the below items need to run as root - password: security

Opening the menu option I added six subitems:
1. Dynamic Analysis which has settings to start MobSF Server and UI, Frida, Drozer, 
QARK, PIDCat, and MARA Framework
2. Manual Analysis - apktool
3. Penetration Testing which has Nikto, Nmap, Burpsuite-Community Edition, SSLscan, 
Wireshark, w3af console and gui, ZAP, FireBase Scanner, Metasploit
4. Programming - Python2.7, Python3.6, Sqlite3, Sqlite3 Browser
5. Reporting - Cherrytree and Keepnote
6. Reverse Engineering - baksmali, dex2jar, jadx, jadx-gui, jd-gui, smali

Note: MobSF is in a docker container
Need to start MobSF Server (under Dynamic Analysis)
Next, start to MobSF UI (under Dynamic Analysis)

I've included the commands if you want to enter on the command line

To start the docker:
sudo service docker start

To start MobSF docker container:
sudo docker run -p 8000 opensecurity/mobile-security-framework-mobsf

To see the current status of the docker (active, inactive):
sudo service docker status

To see the running processes enter the command (docker needs to be started):
sudo docker ps

To remove the current process enter the command:
sudo docker rm -f <container id>

To stop the docker container:
sudo service docker stop

When executing MobSF, first start the server.
Once the server is started then start the UI. 
The website is http://172.17.0.2:8000. 

In the /home/android/Documents folder I included some Android apps to play with.
1. MSTG-Hacking-Playground. The apk (application) is located at the following location:
/Documents/MSTG-Hacking-Playground/MSTG-Hacking-Playground/Android/MSTG-Android-Java-App/app
In this folder there are different apks based on the architecture of your computer.
2. DIVA (diva-beta.apk)
3. IG Learner (ig-learner.apk)
4. UnCrackable Series (Levels 1-4). NOTE: the fourth level have two files 
(r2pay-v0.0.apk and r2pay-v1.0apk)

You will need an Android emulator (I used android-x86 which is free), and from 
there you can install above apps onto the emulator (using adb install) and 
hack away :-)

I have built this image on VirtualBox. The image should work on VMWare.

If there are any issues please hit me up on twitter @thefluffy007. I will try 
my best to remediate the issue. 

Please note, this is my first image, so be patient for a response.

I hope you, user, have as much fun using this image as I did creating it.
