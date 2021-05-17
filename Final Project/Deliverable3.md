# Setup an NFS Server
## Table of Content
* Setup an NFS Server
    * Table of content
    * Hardware Requirements
    * Software Specifications
    * How to Install NFS Kernel Server
    * How to Create Root NFS Directory
    * Define Access for NFS Clients in Export File
    * How to Make NFS share Available to Clients
    * Configure NFS
    * Setting Up NFS on Client Machine and Mounting an NFS   Share
    * How to Install NFS Client Packages
    * Creating Local Directory
    * Mounting the NFS File Share Temporarily
    * Mounting NFS File Shares Permanently
    * Verify NFS is running
    * Work Cited
## Hardware Requirements
The NFS have the following hardware requirements: 
* 16 GB RAM
* 8 CPU cores
* 100 GB free disk space.

## Software Specifications
Ubuntu 21.04 is being used as the OS to complete this project.
The latest version of the Ubuntu 21.04 comes with nine months, until January 2022, of security and maintenance updates.

## Install NFS Server
* NFS Kernel is the server component that enables a machine to expose directories as NFS shares
* Before Installing, run the update command.
![Image1](../imgs/FinalProject/StepOne-Update.png)

* Next, run the following command to install NFS Kernel Server
![Image2](../imgs/FinalProject/Step2.png)  
## Create Root NFS Directory
* Next, create the root directory of the NFS shares
![image3](../imgs/FinalProject/step3.png)

* Set permissions so that public / any user on the client machine can access the folder 
![Image4](../imgs/FinalProject/step4.png)
## Define Access for NFS Clients in Export File
* To grant access to NFS clients, define an export file
![image5.1](../imgs/FinalProject/step5.png)

* Next, edit the /etc/exports file in a text editor
![image5.2](../imgs/FinalProject/step5.2.png)
## Make NFS share Available to Clients
* After that, make the shared directory available to clients using the exportfs command
![image6](../imgs/FinalProject/step6.png)
## Configure NFS server
* Configure the NFS server
![image7](../imgs/FinalProject/step7.png)
## Setting Up NFS on Client Machine and Mounting an NFS   Share
* Now set up the NFS server, with a Linux computer by mounting it on the local machine.
## Installing NFS Client Packages
* NFS client Packages need to install to enable mounting an NFS share on a local Linux machine.
![image8](../imgs/FinalProject/step8.png)
## Creating Local Directory
* This will be the mount point for the NFS share
![image10](../imgs/FinalProject/step10.png)
## Mounting the NFS File Share Temporarily
* To mount the file share temporarily, run the following command
![image11.1](../imgs/FinalProject/step11.1.png)

* Here, it shows the command have been successful
![image11.2](../imgs/FinalProject/step11.2.png)
## Mounting NFS File Shares Permanently
* To mount the file server permanently, first Edit the /etc/fstab file using nano command
![image12.1](../imgs/FinalProject/step12.1.png)

* Now, add a line defining the NFS share. Insert a tab character between each parameter. It should appear as one line with no line breaks.The last three parameters indicate NFS options (which is set to default), dumping of file system and filesystem check (these are typically not used so keep them to 0).
![image12.2](../imgs/FinalProject/step12.2.png)

* Now, mount the files, using sudo mount -a ( which will mount all folders )
![image12.3](../imgs/FinalProject/step13.1.png)

* Here, it shows that the folders mounted successfully
![image12.4](../imgs/FinalProject/step13.2.png)
## Verify NFS is running
* To do this, query the portmapper with the command rpcinfo -p to find out what services it is providing
![image13](../imgs/FinalProject/step14.png)

## Work Cited
* VITUX- Linux Compendium, Author- Karim Buzdar
https://vitux.com/install-nfs-server-and-client-on-ubuntu/

* Linux NFS Server: How to Set Up Server and Client
Posted by Jeff Whitaker, Cloud Data Services
https://cloud.netapp.com/blog/azure-anf-blg-linux-nfs-server-how-to-set-up-server-and-client#H_H5

