## A list and provide a brief description of the resources that are being used to complete the project. 

## Device Used
* Name         UbuntuVM
* Processor	   AMD Ryzen 5 4500U with Radeon Graphics 2.38 GHz
* Graphics     SVGA3D;build:RELEASE;LLVM;
* Disk Capacity     109 GB
* RAM          32GB
* Memory Used  1.9 GiB
  
## OS type
* OS Name           Ubuntu 20.04.2 LTS
* OS Type           64-bit
* GNOME Version     3.36.8
* Windowing System  X11
* Virtualization    Oracle

## What is NFS (Network File System)?
NFS, or Network File System protocol allows a user on a client computer to access files over a network in the same way they would access a local storage file. Because it is an open standard, anyone can implement the protocol. NFS started in-system as an experiment but the second version was publicly released after the initial success.

## Setting up a Firewall
Ubuntu 20.04 servers can use the UFW firewall to make sure only connections to certain services are allowed. We can set up a basic firewall very easily using this application.
* First, to check the firewall status: sudo ufw status
* Next, to list all applications that have register their profiles with UFW: sudo ufw app list
To make sure that the firewall allows SSH connections so that allow these connections by typing:
* ufw allow OpenSSH
Next,enable the firewall by typing:
* ufw enable
Type y and press ENTER to proceed. You can see that SSH connections are still allowed by typing
* ufw status

## How does NFS work?
To access data stored on another machine (i.e. a server) the server would implement NFS daemon processes to make data available to clients. The server administrator determines what to make available and ensures it can recognize validated clients.
From the client's side, the machine requests access to exported data, typically by issuing a mount command. If successful, the client machine can then view and interact with the file systems within the decided parameters.

## Directory
The directory that you want to share. It may be an entire volume though it need not be. If you share a directory, then all directories under it within the same file system will be shared as well. 

## Client machines that will have access to the directory. 
The machines may be listed by their DNS address or their IP address. Using IP addresses is more reliable and more secure. If you need to use DNS addresses, and they do not seem to be resolving to the right machine.

## Some of the command used that describe what kind of access user's will have
* ro: The directory is shared read only; the client machine will not be able to write to it. This is the default.
* rw: The client machine will have read and write access to the directory.
* no_root_squash: By default, any file request made by user root on the client machine is treated as if it is made by user nobody on the server. (Excatly which UID the request is mapped to depends on the UID of user "nobody" on the server, not the client.) If no_root_squash is selected, then root on the client machine will have the same level of access to the files on the system as root on the server. This can have serious security implications, although it may be necessary if you want to perform any administrative work on the client machine that involves the exported directories. You should not specify this option without a good reason.
* no_subtree_check: If only part of a volume is exported, a routine called subtree checking verifies that a file that is requested from the client is in the appropriate part of the volume. If the entire volume is exported, disabling this check will speed up transfers. 