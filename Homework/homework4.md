## Explain the difference between absolute path and relative path:
* An absolute path is defined as the specifying the location of a file or directory from the root directory(/).
To write an absolute path-name:
Start at the root directory ( / ) and work down.
Write a slash ( / ) after every directory name.
* Relative path is defined as the path related to the present working directly(pwd). It starts at your current directory and never starts with a / .
## Why Linux uses / instead of \ for its directory paths?
For a path to a web resource or file located on a UNIX based machine (includes Linux), use a slash. The reason . NET's URI uses forward slashes is because it's formatting for use in a webbrowser. The server will do all the necessary work to link web resources to files on a hard driveIn Linux and other Unix-like operating systems, a forward slash is used to represent the root directory, which is the directory that is at the top of the directory hierarchy and that contains all other directories and files on the system
## In Windows, these files are all the same: File FILE file and FiLE. But in Linux this is not the case, Why?
On Windows, you can't have a file named file and another file named FILE in the same folder. The Windows file system isn't case sensitive, so file / FILE / File will be name as the same file. On Linux, the file system is case sensitive. This means that you could have files named file, File, and FILE in the same folder

# What is the Filesystem Hierarchy Standard (FHS) and who maintains it?
Linux uses the Filesystem Hierarchy Standard (FHS) file system structure, which defines the names, locations, and permissions for many file types and directories. The Filesystem Hierarchy Standard (FHS) defines the directory structure and directory contents in Linux distributions. It is maintained by the Linux Foundation.

## Explain what type of files are stored in the following directories:

## Directory	What is it used for?
* /bin	/bin is a standard subdirectory of the root directory 
* /dev	/dev is the location of special or device files
* /etc	/etc is a folder which contain all your system configuration    files in it
* /home	/home directory for each user takes the form /home/username (where username is the name of the user account
* /lib	/lib directory contains kernel modules and those shared library images 
* /opt	/opt is a directory for installing unbundled packages
* /tmp	/var/tmp is used for persistent files (as it may be preserved over reboots), and /tmp is for more temporary files.
* /var	/var is a standard subdirectory of the root directory in Linux 
* /proc	/proc filesystem is a pseudo-filesystem which provides an interface to kernel data structures
* /usr	/usr is where user-land programs and data (as opposed to ' system land' programs and data) are
## How does a period at the beginning of a file name means (example .bashrc)?
A dot at the beginning of a file name hides the file in common file managers and for common shell programs. The reason is historical, when ls hid the special directories and hide anything that begins with a period.

## Which command would you use to list all the files inside the /usr/share/ directory?
ls command. ls is one of the basic commands that every Linux user should know. The ls command lists files and directories in the file system and displays detailed information about them.

## If you are working in the /usr/share/icons directory and want to move to your home directory, which command would you use?
To navigate to your home directory, use "cd" or "cd ~".

## Explain what these commands do:

cd .config/.htop; cd ../; ls -lX
* Is used to navigate inside the .config and then inside .htop directory.
* It is used to move up one directory or simply up to go back one directory for example,Suppose you are currently in the /usr/local/share directory, to switch to the /usr/local directory (one level up from the current directory), you would type:cd ../
* ls -lX is used for long listing and then sorting entries by file extension rather than the filename.
* ls to list files
* -l for long listing
* -X for sorting entries by filename rather than the filename.

## John has a lot of files in the directory /var/www/html/webapp. He wants to long list all the files, including hidden files, by modification time (newest first), and with human-readable file sizes. Which command should he use conjuring that his current working directory is:
## /home/john/.git/
* ls -lath /var/www/html/webapp

here, -l is for long listing , -a for hidden files, -t for modification time(-r can be used to change the order), -h for human-readable file sizes.