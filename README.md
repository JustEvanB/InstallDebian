# How to install Debian (Gnome)

## Step 1. Download

![DownloadPage](/DebianInstallPics/DownloadPage.png)

go to:
```
http://debian.osuosl.org/debian-cdimage/12.8.0-live/amd64/iso-hybrid/
```
and click on the "debian-live-12.8.0-amd64-gnome.iso" to download it, it's around 3.2GB
The page should look like:

## Step 2. Install

![ChooseISO](/DebianInstallPics/ChooseISO.png)

Open VMWare Workstation or an equivelant VM manager and open a new VM wizard (For VMWare it is inside File > New Virtual Machine)
Click Next and set the ISO image to the newly downloaded ISO
Click Next again and set the Guest Operation System to Linux and the version to "Debian 10.x 64-bit)
Click Next again and set the VM Name and Location
Now you can click Next until you are done with the wizard

## Step 3. Boot

![GRUB](/DebianInstallPics/GRUB.png)

Once done the installation you can boot the VM.
when you boot you will be put into the GRUB
Select "Start Installer"

Go through the install, selecting the language, location, keyboard map (I've left the defaults as they are all english)
You can then set the hostname to anything you like

For Domain Name you can just leave it blank

![Password](/DebianInstallPics/Password.png)

Then type in the admin password as shown above

After the password you need to enter the name of the user
Then the username of the account follows:

![Username](/DebianInstallPics/Username.png)

After the username you can enter the user account's password:

Click continue until you get to the Partition Disks, We will just be using "Guided"
Keep clicking continue, using the default options for everything until you reach "Write changes to disk"
We will press Yes.

Once the long process of copying the data to the disk is done, 
you can keep clicking continue, leaving the defaults of everything, until you get to entering a device to install GRUB bootloader to.
You will want to enter /dev/sda

![Boot Device](/DebianInstallPics/BootDev.png)

Click continue until the install process is done and the VM reboots.
NOTE: If using VMWare once the system is done rebooting you can click on the small Finished Installing from the pop-up at the bottom of the page.

Debian is now installed!

![Finish](/DebianInstallPics/Finish.png)
