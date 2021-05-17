# Managing data
Data management is about collecting, storing and using data in a secure, efficient and cost-effective manner. The goal of data management is to help people, organizations and connected objects optimize the use of data within the confines of policy and regulation so that they can make decisions and take action. that maximize the benefits to the business. A good data management strategy is becoming more important than ever as organizations increasingly rely on intangibles to create value.
Managing digital data in an organization involves a wide range of tasks, policies, procedures and practices. The work of data management is extensive and covers factors such as:
Create, access and update data at a diverse data level
Store data across multiple clouds and on-premises
Provide high availability and disaster recovery
Use data in a growing variety of applications, analyzes and algorithms
Guarantee the confidentiality and security of data
Archive and destroy data in accordance with retention schedules and compliance requirements.
A formal data management strategy addresses the activity of users and administrators, the capabilities of data management technologies, the requirements of regulatory requirements, and the needs of the organization to derive value from its data.
# File permissions

Each file and directory on your UNIX / Linux system has the following 3 permissions set for the 3 owners mentioned above.

Read - This permission gives you the right to open and read a file. Read permission on a directory gives you the ability to list its contents.
Write: Write permission gives you the right to modify the content of a file. Write permission to a directory gives you the right to add, delete, and rename files stored in the directory. Consider a scenario where you must have write permission to the file, but you do not have write permission to the directory where the file is stored. You will be able to modify the contents of the file. But you will not be able to rename, move or delete the file in the directory.
Execute: In Windows, an executable program usually has an ".exe" extension and an extension that you can easily run. On Unix / Linux, you can only run a program if execute permission is set. If execute permission is not set, you can still view / edit program code (as long as read and write permissions are set), but not run it.

r = read permission
w = write permission
x = execute permission
" - " = no permission

We can use the 'chmod' command which stands for 'change mode'. Using the command, we can set permissions (read, write, execute) on a file/directory for the owner, group and the world. 
Syntax: chmod permissions filename

# Managing processes
The process is a program in execution. The process is created when a command is to be executed so, it can be called a running instance of a program in execution. Tuning or controlling a process is called Process Management.

The top command is the traditional way to view your system’s resource usage and see the processes that are taking up the most system resources

The htop command is an improved top. It’s not installed by default on most Linux distributions

The ps command lists running processes.

The pstree command is another way of visualizing processes

The kill command can kill a process, given its process ID. You can get this information from the ps -A, top or pgrep commands.

Given a search term, pgrep returns the process IDs that match it

The pkill and killall commands can kill a process, given its name.

The renice command changes the nice value of an already running process. The nice value determines what priority the process runs with. A value of -19 is very high priority, while a value of 19 is very low priority. A value of 0 is the default priority.