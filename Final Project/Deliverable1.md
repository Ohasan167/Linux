# Deliverable 1

## Which project will you be completing?
The project i will be completing is from Networking and Technical Support, which is Build a NFS file Server.
## Why have you chosen this project?
The reason I chose this project. because we all know that files should be stored on a central server for added security and ease of backup. Network File Sharing (NFS) is a protocol that allows you to share directories and files with other Linux clients over a network.
## What are the possible problems, roadblocks, or difficulties you anticipate during the process of completing the project?
There are some commonly occurring NFS issues. 
Error: "Server Not Responding"
Error: "No Route to Host"
## How are you planning to overcome these difficulties?
To resolve Error: "Server Not Responding", I will use common tools such as ping, traceroute or tracepath to verify that the client and server machines can reach each other. If not I will examine the network interface card (NIC) settings using either ifconfig or ethtool to verify the IP settings.
To resolve Error: "No Route to Host" As a quick test I switch the firewall off, by "service iptables stop" on both the client and the server. I will try mounting the NFS directory again, then switch it back on and configure it correctly to allow NFS traffic.
## How do you think completing this project will help you in your career?
This project will definitely help me in my career. By completing the project, I got to know more about the NFS. I got know, how to create one, how to troubleshoot and sovlve  the problems. A Network File System (NFS) allows remote hosts to mount file systems on a network and interact with those file systems as if they were mounted locally. This allows system administrators to consolidate resources on centralized servers on the network.  Provides centralized administration. Provides security,The server-side file system is also simply called the file server.The NFS mount protocol helps obtain the directory handle for the root directory in the file system.