## What is Virtualization?
Virtualization creates a virtual version, rather than an actual version, of something, such as an operating system (OS), server, storage device, or network resources.
Virtualization uses software that simulates the functionality of hardware to create a virtual system. This practice enables IT organizations to operate multiple operating systems, multiple virtual systems, and multiple applications on a single server. The benefits of virtualization include greater efficiency and economies of scale.
Operating system virtualization is the use of software to allow a piece of hardware to run multiple images of the operating system at the same time. The technology started on mainframes decades ago, allowing administrators to avoid wasting expensive processing power.
## Using Virtualbox (optional)
Oracle VM VirtualBox is a cross-platform virtualization application. On the one hand, it installs on your existing Intel or AMD computers, whether they run on Windows, Mac OS X, Linux or Oracle Solaris operating systems (OS). Second, it expands the capabilities of your existing computer, allowing you to run multiple operating systems simultaneously within multiple virtual machines. For example, you can run Windows and Linux on your Mac, run Windows Server 2016 on your Linux server, run Linux on your Windows PC, etc., all in addition to your existing apps. You can install and use as many virtual machines as you want. The only practical limits are disk space and memory.
## Installing Ubuntu In a virtual machine
First, open VirtualBox, then click "New" to create a virtual machine.Enter "Ubuntu" as the name, select "Linux" as the type, and select Ubuntu (64-bit) as the version.
NOTE: Select any amount of memory you wish, but don't add more than 50 percent of your total RAM.
Check the "Create a virtual hard disk now" option so we can later define our Ubuntu OS virtual hard disk size.
Now, we want to select "VHD (Virtual Hard Disk)".
Next, we'll dynamically allocate storage on our physical hard disk.
We want to specify our Ubuntu OS's size. The recommended size is 10 GB, but you can increase the size if you wish.
After creating a virtual hard disk, you'll see Ubuntu in your dashboard.
Now, we have to set up the Ubuntu disk image file (.iso).
The Ubuntu disk image file can be downloaded here: Ubuntu OS download
To set up the Ubuntu disk image file, go to settings and follow these steps:
1.	Click "Storage"
2.	In storage devices, click "Empty"
3.	In attributes, click the disk image and "Choose Virtual Optical Disk File"
4.	Select the Ubuntu disk image file and open it
Click OK.
Your Ubuntu OS is ready to install in VirtualBox. Let's start!
NOTE: Ubuntu VirtualBox installation and actual OS installation steps may vary. This guide helps you to install Ubuntu in VirtualBox only.
Let's install Ubuntu!
Click Install Ubuntu.
Select your keyboard layout.
In the "Updates and other software" section, check "Normal installation" and continue.
In "Installation type", check "Erase disk and install Ubuntu".
Click "Continue".
Choose your current location.
Now, set up your profile.
You'll see Ubuntu installing.
After the installation, restart it.
After logging in, you'll see the Ubuntu desktop.
We have successfully installed Ubuntu in VirtualBox. It's ready to use for your future development projects.
Let's verify the installation.
Open your terminal (Press Ctrl+Alt+T) and type in the commands below and check if they work.
1.	pwd: This will print the current working directory
2.	ls: This will list all items in your current directory
After checking those, power off your machine by using the following command.
poweroff

## What is a Raspberry Pi (optional)
The Raspberry Pi is an inexpensive computer the size of a credit card that plugs into a computer monitor or TV and uses a standard keyboard and mouse. It's a capable little device that allows people of all ages to explore computers and learn to program in languages like Scratch and Python. It is capable of doing everything you expect from a desktop computer, from surfing the web and playing HD videos, creating spreadsheets, word processing and playing games.