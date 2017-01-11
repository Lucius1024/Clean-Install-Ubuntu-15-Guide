# Install Ubuntu 16

![alt text](http://core0.staticworld.net/images/article/2014/08/logo-ubuntu-100372440-primary.idge.png "Ubuntu 16.04")

#Performing a Clean Install of Ubuntu 16.04

**Total Estimated time: 30-45 minutes**

**Required items:**

USB drive with at least 6GB of storage

**Index:**

1. Backing up Files and Settings
2. Mounting Ubuntu on a USB drive
3. Installing Ubuntu
4. Additional software

#1. Backing up Files and Settings

1. Click on the Start Menu > All Programs > Accessories > System Tools backup.
2. Click next and select the Back up files and settings.
3. Select what to backup from the options listed.
4. Choose where to back up the files and name it.
*Note: back up sizes will vary.* 


#2. Mounting Ubuntu on a USB drive

1. Download the appropriate Ubuntu file and place it on your desktop.

    [32-bit](http://www.ubuntu.com/download/desktop/thank-you/?version=15.10&architecture=i386) (2GB RAM or less)
    
    [64-bit](http://www.ubuntu.com/download/desktop/thank-you/?version=15.10&architecture=amd64) (Recommended)
    
2. Click [here](http://www.pendrivelinux.com/downloads/Universal-USB-Installer/Universal-USB-Installer-1.9.6.3.exe) to install a Universal USB Installer and move it to your desktop.
3. Run the USB installer and select Ubuntu from the first dropdown menu.
4. Select the Ubuntu .iso file you had saved from earlier.
5. Select the flash drive you will be using to install Ubuntu and click the create button.
6. Wait for the file to extract to the USB drive.
7. Safely eject the USB drive from your task bar and plug the USB drive into the machine you will be installing Ubuntu on.


#3. Installing Ubuntu

1. Insert the USB drive into the computer that you will be installing Ubuntu on.
2. Restart the computer. As soon as the first text appears on the screen, press the appropriate button to enter your BIOS/system setup which is usually one of the following keys: F1, F2, Del, Esc, F10, F11, or F12.
3. Once inside the BIOS Enter administaror password to change boot sequence from the HD to the USB drive you installed Ubunutu on.
4. Once the boot order is changed restart your computer.
5. Wait a minute or two, an install window will appear.
6. Select "Install Ubuntu" and wait for it to load.
7. Select English from the list to the left of the screen and click continue.
8. Connect to Wi-Fi, if available, by selecting the connect to this network option and clicking connect and then continue (this will not show up if you are connected with an ethernet cable).
9. Select the checkbox "download updates while installing" and click continue.
10. When you get to the installation type, choose which option best suits your needs, I chose to erase Windows completely.
11. If installing alongside windows boot manager, allocate space and select install now.
12. Follow the instructions to choose your location, language and keyboard settings, name, computer name, a username and a password.
13. Click Install. The installation will begin, and should take 10-20 minutes to complete. When it is finished, choose to restart the computer and then remove your USB drive. Ubuntu should start to load on restart.

#4. Recommended Software (Optional)

Click the launcher in the top left corner of the screen and type Terminal. Click the icon that pops up. Commands will be entered here.

###Chromium
Chromium is an open-source version of Chrome. 

1. Change to root directory:

    ```bash
$ cd ~
```

2. Add the Chromium PPA:
    
    ```bash
$ sudo add-apt-repository ppa:chromium-daily/ppa
```

3. Download the package lists from the repositories and "update" them to get information on the newest versions of packages and their dependencies. It will do this for all repositories and PPAs.

    ```bash
$ sudo apt-get update
```

4. Install Chromium:
    
    ```bash
$ sudo apt-get install chromium-browser
```

###Sublime Text 3
Sublime Text is a sophisticated text editor for code, html and prose. 

1. Change to root directory:

    ```bash
$ cd ~
```

2. Add the WebUpd8 Sublime Text 3 (beta) PPA:
    
    ```bash
$ sudo add-apt-repository ppa:webupd8team/sublime-text-3
```

3. Download the package lists from the repositories and "update" them to get information on the newest versions of packages and their dependencies. It will do this for all repositories and PPAs.

    ```bash
$ sudo apt-get update
```

4. Install Sublime Text 3:
    
    ```bash
$ sudo apt-get install sublime-text-installer
```

5. Add in drupal specific preferences [https://drupal.org/node/1346890](https://drupal.org/node/1346890)

###IRC (HexChat)
1. Add the HexChat PPA:
    
    ```Bash
$ sudo add-apt-repository ppa:gwendal-lebihan-dev/hexchat-stable
```

2. Download the package lists from the repositories and "update" them to get information on the newest versions of packages and their dependencies. It will do this for all repositories and PPAs
    
    ```Bash
$ sudo apt-get update
```

3. Install HexChat:
    
    ```Bash
$ sudo apt-get install hexchat
```

###Terminator

1. Change to root directory:

    ```bash
$ cd ~
```

2. Add the Terminator Nightly Builds PPA:
    
    ```bash
$ sudo add-apt-repository ppa:gnome-terminator/nightly
```

3. Download the package lists from the repositories and "update" them to get information on the newest versions of packages and their dependencies. It will do this for all repositories and PPAs.

    ```bash
$ sudo apt-get update
```

4. Install Terminator:
    
    ```bash
$ sudo apt-get install terminator
```
# HELP/TROUBLESHOOTING

1. Forgotten Bios Password
    In the Event that the Bios Screen has an administrator password, and the user is unable to recover it.
    1. turn the computer off
    2. locate the motherboards documentation 
    3. open the computers chasie and locate the the mother board jumper to reset the bios.
    4. remove the jumper pin for 2-3 seconds and replace back to its original state.
    5. Power the computer ON and then proceed with the installation. 


