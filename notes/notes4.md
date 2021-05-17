## Managing files and directories
In Linux, most operations are performed on files. And to manage these files, Linux has directories also called folders which are kept in a tree structure. However, these directories are also a type of file in themselves. Linux has 3 types of files:
Normal Files: This is the common file type in Linux. includes files such as: text files, images, binary files, etc. These files can be created using the touch control. They consist of most of the Linux / UNIX system files. The normal file contains ASCII or human readable text, executable binary files, program data and much more.
Directories: Windows calls these directories folders. These are the files that store the list of file names and associated information. The root (/) directory is the base of the system, / home / is the default location for user home directories, / bin for essential user binaries, / boot - static boot files, and so on. We could create new directories with the mkdir command.
Special Files - Represents an actual physical device, such as a printer, used for I / O operations. The device or special files are used for device input / output (I / O) on systems UNIX and Linux. You can view them in a file system like a directory or a regular file.
## Getting help
The help command is a command prompt command that is used to provide more information about another command. You can use the help command at any time to learn more about the usage and syntax of a command, such as the available options and how to structure the command to use its various options.
Launch the terminal by pressing Ctrl + Alt + T or just click the terminal icon on the taskbar. Just type your command whose usage you should know in the terminal with –h or –help after a space and hit enter.
## Working with wildcards
Wildcards are special characters that can stand in for unknown characters in a text value and are handy for locating multiple items with similar, but not identical data. Wildcards can also help with getting data based on a specified pattern match. For example, finding everyone named John on Park Street.
For more information about queries, see introduction to queries.
Here are some examples of wildcard characters for Access queries:

* "*" Matches any number of characters. You can use the asterisk (*) anywhere in a character string.
wh* finds what, white, and why, but not awhile or watch.

* ?
Matches a single alphabet in a specific position.
b?ll finds ball, bell, and bill.

* [ ]
Matches characters within the brackets.
b[ae]ll finds ball and bell, but not bill.

* !
Excludes characters inside the brackets.
b[!ae]ll finds bill and bull, but not ball or bell.
Like “[!a]*” finds all items that do not begin with the letter a.

* "-" Matches a range of characters. Remember to specify the characters in ascending order (A to Z, not Z to A).
b[a-c]d finds bad, bbd, and bcd.
* "#" Matches any single numeric character.
1#3 finds 103, 113, and 123.

## Shell Expansion
When a command is entered on the command line, it expands to its displayed output.
This is called expansion.
The command you type will be printed using the echo command in the terminal. This command will come in handy when you want to check what your command is doing in the shell.