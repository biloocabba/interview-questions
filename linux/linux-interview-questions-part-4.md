1. What is Unix?
Answer: UNIX is a computer operating system which is multi-user, multi-tasking and it is developed at Bell Laboratories by Ken Thompson and Dennis Ritchie. It is proprietary software with its code which is not available to the general public.
The different variants of UNIX are HP Unix, Solaris Unix, IBM AIX and BSD.

2. What is Linux?
Answer: Linux is an open source UNIX like operating system which is developed from scratch by Linus Trovald.  Linux is actually a different operating system but it is inspired from UNIX, therefore commands and syntax of UNIX and Linux programs are mostly similar.
Linux distributions are Ubuntu, RedHat, Fedora etc.

3. What are some basic features of Linux?
Answer: Following are the basic features of Linux:
1. Multiuser – The multiuser feature of Linux will provide the ability to let multiple users access the same computer resources such as memory, application programs, hard disk etc at the same time.
2. Multitasking – Multitasking will allow multiple applications or programs to run simultaneously.
3. Security – Linux will provide security feature by authentication means username-password for users, authorization by providing read-write-execute permissions to different files, encryption by encrypting files so that only the rightful owner can see the original content of the files.
4. Portable – Linux will support portability with the ability of the OS to get installed in different hardware platforms.
5. Open source – Its open source with its code available to general public.


5. What is a Linux Loader or LILO?
Answer: Linux loader or LILO is a boot loader for Linux which will load the operating system into memory. It is considered more of a legacy application which is superseded by GRUB(GRand Unified Boot loader) and GRUB2 bootloaders.

6. What is a Shell?
Answer: A shell is a program which will act as an interface between the user and operating system, which allow user for executing commands example for Bourne shell(sh), bash(Bourne Again Shell) etc.

7. What is a swap space? What are its advantages?
Answer: Swap space is a piece of hard-disk storage which is used when system required more memory but the RAM is full. If the inactive memory pages will be moved to swap space to free RAM.

8. What is a process in Linux?
Answer: A process is an instance of a program which is under execution. There are two kinds of processes-
1. Foreground processes – A foreground process when it is initiated by a user and will run in the foreground and user has to wait for it to get completed before issuing any other command example for running any command on the terminal.
2. Background processes – A background process will run on the background and the user will execute other commands also even before the background process will get executed completely. Adding ‘&’ after any command, will make it a background process. A background process will be brought to foreground using ‘fg’ command with jobId of the background job.

9. How can we list all the process running on a machine?
Answer: Using Top utility, we will list all the running processes. Running ‘top’, lists important attributes of the process such as PID(process id), user/userId, parent process id, virtual memory used, physical memory used, process status, CPU utilization, process start time, command initiating the process etc.

10. Mention the Command to stop or terminate a running process in Linux?
Answer: Kill command can be used to terminate a running process in Linux. There are two varients of killing a process-
1. Kill PId – This can generate a signal SIGTERM, specifying graceful termination of the process with process id – PId
2. Kill -9 PId – This can generate a signal SIGKILL specifying forceful termination of the process with process id – PId

11. What is the use of ‘ps’ command? How is it different from the top command?
Answer: Ps is stand for Process Status. It provides the information about the running processes.
#To display information about the process with PId – 13
ps -p 13
#To display all process
ps -ef
It is different from top command in the sense which top displays continuous interactive usage of the processes in real time.  ps displays a single snapshot of the processes and is mostly used for non-interactive usage in scripts.

12. What is a daemon?
Answer: Daemons are the processes which will run in background either at predefined time or in the event of a trigger. Daemons names in Linux end with the letter ‘d’ as a convention, .

13. What is the use of man command?
Answer: Man command will be used to know the usage of a command, config file or daemon using the man pages or user manual. Usage-
man ls
Output – It will Display the manual page for ls command.

14. How to print the current working directory in Linux?
Answer: Pwd command can be used for displaying the current directory (Print Working Directory)-
$ pwd
/c/Users/Kuldeep

15. How to create a directory in Linux and give full permission to it?
Answer: Using mkdir, we will create a directory and then with chmod we will provide permissions.
mkdir directoryName
chmod 777 directoryName
We will also use ‘-m’ or mode option of ‘mkdir’ command and perform the operation in single command-
mkdir -m 777 directoryName

16. How to delete a non-empty directory?
Answer: On trying to delete a non-empty directory with ‘rmdir directoryName’ command, we can get an error – “rmdir: Which is failed to remove ‘newFolder’: Directory not empty”.
To remove a non-empty directory, we required to use the ‘-r’ option of ‘rm’ command which is recursively delete the directory and its contents.
rm -r directoryName

17. How to change directory in Linux and move to parent directory, home directory and previous directory?
Answer: We can change directory in Linux using cd command.
Usage-
cd directoryName
1. Move to parent directory or one level up-
cd ..
2. Move to user’s home directory-
cd
Or
cd ~
3. Move to previous directory-
cd –

18. What is a root directory?
Answer: Linux will follow a hierarchical or tree based file system. Root directory is the parent directory of the hierarchy which will include all the other directories. It will be represented by a forward slash ‘/’.

19. What are absolute and relative paths?
Answer:
1. Absolute path – Absolute path is the path of a file or directory from the root directory example for from ‘/’.
2. Relative path – Relative path is the path of a file or directory from the present working directory.

20. Explain the method to login as a different user in Linux?
Answer: ‘Su’ command is used for login as different user in Linux. It will stand for substitute user or switch user.
#Switch to user2
su user2
Password:
#Switch to root
su root
Password:

21. What is a root account?
Answer: Root account is the account or a user which has access for each file and directory in Linux. Root account is called as superuser. A root user will also have access to run any command which includes adding users, grant or revoke permissions etc.

22. Explain the different file ownership in Linux?
Answer: Each file and directory in Linux will have following three owners:
1. User – The user or owner permission class will belong to the user who will be created the file.
2. Group – The group permission class will belong to the members of the file’s group.
3. Other – User or other permission class is refer to each user who will have access to the file.

23. Explain the usage of ‘ls -ltr’ command?
Answer: ‘ls’ is used for listing the directory contents. The options ‘-ltr’ stands for-
‘l’ – Use long listing format
‘t’ – Sort by modification time, newest first
‘r’ – Reverse order while sorting
Therefore, ‘ls -ltr’ can list the content of the directory in long listing format which is sorted oldest first.
$ ls
ebooks.zip  imp.txt Linux.png
$ ls -ltr
total 5072
-rw-r–r– 1 ram 197121 5170843 Mar 30  2017 ebooks.zip
-rw-r–r– 1 ram 197121    8695 Oct 28 14:06 Linux.png
-rw-r–r– 1 ram 197121    6883 Dec 28 19:37 imp.txt

24. What is the significance of file extensions like .txt, .png etc in Linux?
Answer: Unlike Windows, file extensions will have no significance in Linux. Linux will not rely on the file extensions instead the file type will be determined by the some content in the file header.

25. Explain the usage of ‘file’ utility.
Answer: The file utility is used for determining the file type of a file.
$ file imp.txt
imp.txt: ASCII text, with very long lines, with CRLF line terminators
$ file Linux.png
Linux.png: PNG image data, 521 x 177, 8-bit colormap, non-interlaced

26. What is the purpose of ‘touch’ command?
Answer: Touch command will serve two purposes in Linux-
1. With a new file name, touch is used for creating an empty file. touch newFile
2. For existing files or directories, touch can change the last access time to current time.

27. Explain the difference between ‘cp’ and ‘mv’ command?
Answer: The ‘cp’ command is used for copying content of one file to another. Whereas, ‘mv’ command will move a file from one location to another, deleting the source file. ‘mv’ command is also used to renaming files. Usage-
#Copies content of file1 to file2
cp file1 file2
#Moves/renames file1 to file2
mv file1 file2

28. List the usage of ‘head’ and ‘tail’ commands.
Answer: Head command is used for displaying first few lines (default 10) of a file. Tail is used for displaying last few lines (default 10) of a file. Usage-
#Display first 10 lines of a file
head fileA
#Display first 5 lines of a file
head -5 fileA
#Display last 10 lines of a file
tail fileA
#Display last 5 lines of a file
tail -5 fileA

29. What is ‘sed’ in Linux?
Answer: Sed stands for Stream Editor. It is used for editing a file or input from a pipeline. Example-
#Prints first 5 lines
sed -n 1,5p fileA.txt

30. How to print content of line 5 to 10 from one file to another?
Answer: Using ‘sed’
#’p’ to print and ‘-n’ to not print each line
sed -n 5,10p fileA.txt > fileB.txt

31. What is ‘awk’?
Answer: AWK named after the initials of its authors “Aho, Weinberger, and Kernighan”, and it is an interpreted programming language which is used for text processing. Usage-
#To display the content of file using awk
awk ‘{print}’ fileA.txt

32. How to count the number of words, lines and characters in a file?
Answer: Using wc command (word count)-
#Number of characters
wc -m fileA.txt
#Number of words
wc -w fileA.txt
#Number of lines
wc -l fileA.txt

33. How to combine the content of multiple files into a single file?
Answer: We can combine the content of multiple files into a single file Using ‘cat’ and redirection-
#merging content of fileA and fileB into mergedFile
cat file1 file2 > mergedFile

34. What is use of ‘tac’ command?
Answer: Tac is the reverse of ‘cat’ command. It will display the content of file in reverse order – line by line, displaying the last line first and moving up till the first line.
#Displays the content of fileA from the bottom line to top line
tac file!

35. State the difference between ‘more’ and ‘less’ command?
Answer: Both more and less commands are used to view large files page wise. Unlike any editor like vi, using these commands to open a file which will not load the whole file in memory. One limitation of more command is, we will only scroll down but not up. Whereas, using less command, we will scroll both upwards and downwards in a file.

36. How to find the top three space consuming file or directories within a directory?
Answer: We can find the disk usage of all directories and sub-directories using du(disk usage) command, .
Using du with -a option, can list the disk usage of all files along with the directories.
The ‘-h’ option will display the size in human readable form. Later, we will use this command along with sort and head command, to first sort the files/directories by size and then it will fetch the required number of files.
#Sorts the files and directories within artOfTesting directory by size
du -h -a artOfTesting/ | sort -n -r | head -n 3

37. How to create aliases in Linux?
Answer: Aliases are used for creating aliases or some abbreviated short-name for a command or a group of commands.
#Alias for some log directory
alias logs=“cd /user/application/logs”

38. What is the use of shred utility? How it is different from rm command?
Answer: Shred utility is used to delete the content of file in the way that the content will not be recovered using some data recovery tools/utilities. If we delete a file using rm command, the space used by the file is marked available for other files; therefore there is possibility to recover the content of the file. So, shred is better to delete files with sensitive data.
#Overwrites the content of the file to make it impossible to recover
shred file1

39. State the difference between find and locate command?
Answer: Both find and locate commands will be used to searched files on Linux. The ‘find’ command will be searched file in real time and thus take longer time for returning the search result in case there are too many files for scanning through. ‘locate’ command is much faster than find as instead of real time search it will look up in a database – updatedb. The updatedb will take snapshot of the file system only once a day output of locate will not always accurate or updated.
#Find all text files
find / *.txt
#Find all text files
locate “*.txt”

40. How to introduce wait time in scripts?
Answer: Sleep command will be used for introducing wait time in scripts. We will specify wait in terms of seconds, minutes, hours and days.
#Wait for 5 seconds
sleep 5s
#Wait for 5 minutes
sleep 5m
#Wait for 5 hours
sleep 5h
#Wait for 5 days
sleep 5d

41. How to compress and decompress files in Linux?
Answer: We will compress and decompress files in Linux using ‘zip’ and ‘unzip’ commands,
#Creates a file zipFile.zip with fileA and fileB compressed
zip zipFile fileA fileB
#Unzips zipFile.zip
unzip zipFile.zip

42. What are the different file permissions or access modes in Linux?
Answer: Each file and directory in Linux will have following three permissions which is represented by a three digit octal number-
1. Read – It will Provide the ability for reading the content of a file (It is represented by ‘r’ in first position – “r–“)
2. Write – It will Provide the ability for editing or deleting the content of a file (It is represented by ‘r’ in second position – “-w-“)
3. Execute -It will Provide the ability for executing or running a file (It will is represented by ‘x’ in third position – “–x”)

43. State the meaning of the permission mode “drwxr-x–x”.
Answer: The 10 characters of permission mode will be providing information about the permission to the user, group and other users.
1. 1st character will indicate whether the provided thing is file or directory, ‘-‘ for file and ‘d’ for directory.
2. Next 3 characters will indicate the read-write-execute permission to the user or owner of the file.
3. Next 3 characters will indicate the read-write-execute permission to the group belonging to the file.
4. Last 3 characters will indicate the read-write-execute permission to all the other users.
Therefore, the permission mode “drwxr-xr-x”, will mean a directory for that the user can have all the read-write-excute permission, group has read and execute permission and other users will only execute the file.

44. How to grant or remove access to a file in Linux?
Answer: The ‘chmod’ command will be used for granting permission to a file or directory in Linux. There are two modes for granting or removing permission using chmod-
1. Symbolic mode – We can grant permission to a file using ‘+’ operator, remove permission using ‘-‘ operator and set the required permission using ‘=’ operator with symbolic mode.
#Add read and execute permission to group
chmod g+rx fileA
#Remove execute permission to owner
chmod u-x fileA
#Set write and execute permission to other users
chmod o = wx fileA
2. Absolute mode – An octal number a used for specifying different permissions  absolute mode, a.
#852 will grant permission 8 to owner, 5 to group and 2 to other users
chmod 852 fileA
 

45. State the octal number representation for different permission types in Linux.
Answer: The absolute permission of chmod will use an octal number. The different octal numbers for different permission types are following:

Octal number	Permission granted
0	No permission (—) i.e. 0+0+0=0
1	Execute (–x) i.e. 0+0+1=1
2	Write (-w-) i.e. 0+2+0=2
3	Write and execute (-wx) i.e. 0+2+1=3
4	Read (r–) i.e. 4+0+0=4
5	Read and execute (r-x) i.e. 4+0+1=5
6	Read and write (rw-) i.e. 4+2+0=6
7	Read, write and execute (rwx) i.e. 4+2+1=7
46. How to change ownership and group ownership of a file in Linux?
Answer: The ‘chown’ command (change owner) will be used for changing the ownership of a file.
chown userK fileA
The ‘chgrp’ command will be used for changing the group ownership of a file.
chgrp group fileA

47. How to sort the contents of a file?
Answer: Sort command will be used for sorting the elements of a file line wise.
#File content – kuldeep, abc, 1India, zed each in separate line
sort file
Output-
1India
abc
kuldeep
zed

48. How can we remove the duplicates in a file?
Answer: We can remove the duplicate in a file using ‘uniq’ utility with ‘sort’ command.
#File content – bat, all, cat, all, cat, all, cat each in separate line
sort fileWithDuplicateContent | uniq
Output-
all
bat
cat

49. What are soft links in Linux? What are their advantages over cp command?
Answer: Soft links are also called as symbolic links or symlinks. These can be used for creating a symbolic links or pointers to a file. In Linux, soft links will be created using ‘ln’ command with ‘-s’ option.
#Creates a soft link ‘fileA’ to the file ‘fileA.txt’
#’-s’ option to create a soft link
ln -s fileA.txt fileA
It has advantage over cp command which will create a new copy of the file in the sense which in order for changing the permission to the files, with links only the permission of the original file required to be changed. The permission to all the copies of the file required to be changed with cp command.

50. What are hard links in Linux? How it is different from soft link?
Answer: Hard links are like another name to an existing file. Instead of pointing to a name such as soft link, hard links point to the content of the file directly point to inode – a table containing metadata about a file.
#Creates a hard link ‘fileA’ to the file ‘fileA.txt’
ln fileA.txt fileA
It is different from soft link in the sense which in case the original files required to be deleted its symbolic link will not point to anything and thus lead to “No such file or directory” error. The hard link will still point to the content of the original file even if the file will be deleted.
#Create hard-link to file1
ln file1 hardF1
#Create soft-link to file1
ln file1 softF1
#Delete original file
rm file1
#Check content of the hard link – hardF1
cat hardF1
#output -> valid content
#Check content of the soft link – softF1
cat softF1
#output -> “No such file or directory”

51. How can you make the file untouchable.txt to be immutable (un-alterable) so that it will not be able to be changed or deleted by any user including root?
Answer: This we can use attributes to change the file to be immutable using below command to achieve.
chattr +i untouchable.txt

52. How can you run a PHP statement from the command line without creating a file?
Answer: We can use the PHP interactive input run a PHP statement from the command line without creating a file.
php -r ‘echo “Hello World\r\n”;’

53. How can you find the usage time of all the users on the machine (individually)?
Answer: We will use the command ac in order to get login information about users
ac -p

54. How can you use variables as a part of your command? For example, set pipeline=”|” and run ps aux $pipeline grep root
Answer: We will use the eval command to use variables literally –
eval ps aux $pipeline grep root
will be the same as
eval ps aux | grep root

55. We want to create network statistics and graph for your server so which tool would you use (most common)?
Answer: The most common network statistics tool is called mrtg (Multi Router Traffic Grapher) and usually is the most recommended open-source tool.

56. How can you send the BIOS a query message directly from the command line?
Answer: We will send a message from the console by using the biosdecode tool in order to query the BIOS.

57. How can you manipulate partitions on a Linux system?
Answer: Linux will provide two applications for partition manipulation – fdisk and parted.

58. What is the result of the lsmod command?
Answer: The lsmod command will show the status of modules which are loaded into the Linux kernel.  This is a nice way for seeing /proc/modules.

59. How can you find your hardware configuration and description of the local machine?
Answer: We will see system hardware and configuration using the DMI table decoder (dmidecode).

60. How can you mount an NTFS partition on Linux?
Answer: We required to use an external application “ntfs-3g” which is also called “mount.ntfs” in order to mount ntfs.

61. What is the LD_LIBRARY_PATH environment variable?
Answer: It is an environment variable set to required the RT Shared library loader extra directories for looking  when searching for shared libraries. 

62. How can you get the Access, Modify and Change date & time of the file “myFile”?
Answer: We required to use stat myFile and look for the Access/Modify/Change information in order to get those times.

63. You want to save the mysql DB “mySQLDB” to a file “mySQLDB.sql” so how can you do it?
Answer: We will use the mysqldump command to dump a database:
mysqldump -u username -p mySQLDB > mySQLDB.sql

64. How can you prioritize system resources per running process?
Answer: The system will allocate and prioritize resources to processes on the system using nice levels, and to change the nice of a specific process, we required to run
renice level <process id>

65. How can you get the NS records of the domain “google.com” from the terminal command line?
Answer: The command dig will allow to get specific domain information, like A, AAAA, NS, etc’ records – we will use
dig google.com NS.

66. You are running a tail -f on /var/log/messages file and looking for specific error, you want only the log that you saw to be printed into a local file “found.log” in order to search it later on a smaller file so how can you do it?
Answer: The tee command will allow we to save data from the standard I/O to a file, we can use it as
tail -f /var/log/messages | tee found.log
and therefore it will save only the data that we saw on the tail. 

67. How do you check all the services that start/stop on each runlevel?
Answer: We required to use the chkconfig in order to check the runlevel services information for the run levels
chkconfig –list

68. How can you allow a user to run superuser commands without knowing the root password?
Answer: If we want to allow a user to run superuser commands without having superuser or root access then we will add him specific or all access using sudoers file after which the user can run all superuser commands using sudo.

69. How can you check which libraries are being used and needed for the binary file /bin/vi?
Answer: Running the tool “ldd /bin/vi” will show the shared libraries required to run the binary application /bin/vi.

70. You want to install a new PERL module, what is the correct way to do it?
Answer: PERL has its management console cpan which will allow we to install new modules using the command
install Group::Module

71. How can you enable jumbo-frame (9000) on a network interface eth0 in Linux?
Answer: We will use ifconfig eth0 mtu 9000, but to make it permanent we will require to add it to the ifcfg-eth0 file.

72. Explain the following command: “iptables -A OUTPUT -p icmp –icmp-type echo-request -j DROP”.
Answer: The command will add a rule to the iptables which will drop all PING requests to the server.

73. What does the wine application does on Linux system?
Answer: The wine application will allow to run windows applications on a Linux server/workstation.

74. What is the Nagios system?
Answer: The Nagios is an open-source monitoring tool/application which will help identify and will resolve infrastructure/network problems.

75. You need to generate a random number in the console so how can you do it without any random application?
Answer: It is required to generate a random number in the console. It can be  generated by a number string from the
/dev/urandom – od -N3 -tu2 -vAn < /dev/urandom | sed ‘s/ //g’

76. You have a very secret file “TOP-SECRET.txt”, which needs to be deleted “for good” so how can you do it?
Answer: We will use the shred tool for overwriting the file X times therefore it will not be able to recover –
shred -n 10 -z TOP-SECRET.txt

77. What are symbolic links?
Answer: Symbolic links will act similarly to shortcuts in Windows. Such links point to programs, files or directories. It will allow instant access to it without having to go directly to the entire pathname.

78. Does the Ctrl+Alt+Del key combination work on Linux?
Answer: Yes, it does. Just like Windows, we can use this key combination to perform a system restart. One difference is that we won’t be getting any confirmation message and therefore, a reboot is immediate.

79. How do you refer to the parallel port where devices such as printers are connected?
Answer: Whereas under Windows we refer to the parallel port as the LPT port, under Linux we refer to it as /dev/lp . LPT1, LPT2 and LPT3 would therefore be referred to as /dev/lp0, /dev/lp1, or /dev/lp2 under Linux.

80. Are drives such as hard drive and floppy drives represented with drive letters?
Answer: No. each drive and device have different designations in Linux. For example, floppy drives are referred to as /dev/fd0 and /dev/fd1. IDE/EIDE hard drives will be referred to as /dev/hda, /dev/hdb, /dev/hdc, and so forth.

81. How do you change permissions under Linux?
Answer: Assuming we are the system administrator or the owner of a file or directory, we can grant permission using the chmod command.
+ Symbol is used to add permission or – symbol is used to deny permission, along with any of the following letters: u (user),
g (group), o (others), a (all), r (read),   x (execute) and w (write).
For example, the command chmod go+rw FILE1.TXT will grant read and write access to the file FILE1.TXT, which will be assigned to groups and others.

82. In Linux, what names are assigned to the different serial ports?
Answer: Serial ports will be identified as /dev/ttyS0 to /dev/ttyS7. These will be the equivalent names of COM1 to COM8 in Windows.

83. How do you access partitions under Linux?
Answer: Linux will assign numbers at the end of the drive identifier. For example, if the first IDE hard drive will have three primary partitions, they would be named/numbered, /dev/hda1, /dev/hda2 and /dev/hda3.

84. What are hard links?
Answer: Hard links will point directly to the physical file on disk, and not on the pathname. This will mean that if we rename or move the original file, the link will not break since the link is for the file itself, not the path where the file is located.

85. What is the maximum length for a filename under Linux?
Answer: Any filename will have a maximum of 255 characters. This limit will not include the path name, therefore the entire pathname and filename can exceed 255 characters.

86. What are filenames that are preceded by a dot?
Answer: In general, filenames which are preceded by a dot are hidden files. These files will be configuration files will hold important data or setup info. Setting files as hidden will make it less likely to be accidentally deleted.

87. Explain virtual desktop.
Answer: This will serve as an alternative to minimize and maximize different windows on the current desktop. Using virtual desktops will clear the desktop when we will open one or more programs. Rather than minimizing/restoring all those programs as required, we can simply shuffle between virtual desktops with programs intact in each one.

88. How do you share a program across different virtual desktops under Linux?
Answer: For sharing a program across different virtual desktops, in the upper left-hand corner of a program window look for an icon that looks such a pushpin. Pressing this button will “pin” which application in place, making it will appear in all virtual desktops, in the same position onscreen.

89. What does a nameless (empty) directory represent?
Answer: This empty directory name will serve as the nameless base of the Linux file system. This will serve as an attachment for all other directories, files, drives, and devices.

90. What is the pwd command
Answer: The pwd command will be short for printing  working directory command.
Example:
pwd
Output:
/home/guru99/myDir

91. What are daemons?
Answer: Daemons will services which will provide several functions which will not be available under the base operating system. Its main task is for listening for service request and at the same time to act on these requests. After the service is done, it will be disconnected and will wait for further requests.

92. How do you switch from one desktop environment to another, such as switching from KDE to Gnome?
Answer: Suppose we have these two environments installed, it is log out from the graphical interface. Then at the login screen, type  login ID and password and choose that session type we wish to load. This choice will remain default until we change it to something else.

93. What are the kinds of permissions under Linux?
Answer: There are three kinds of permissions under Linux:
1. Read: users will read the files or list the directory.
2. Write: users will write to the file of new files to the directory.
3. Execute: users will run the file or lookup a specific file within a directory.

94. How does case sensitivity affect the way you use commands?
Answer: Commands will be considered identical only if every character is encoded it will include lowercase and uppercase letters. This means which CD, cd, and Cd are three different commands. If we enter a command using uppercase letters, where it shall be in lowercase, can produce different outputs.

95. What are environmental variables
Answer: Environmental variables are global settings which will control the shell’s function as well as which of other Linux programs. Another common term for environmental variables will be global shell variables.

96. Explain how you can view the text file using Terminal?
Answer: We will go to the specific folder where the text files which will be located by using the command cd and then type less filename.txt to view the text file.

97. Is it possible to use shortcuts for a long pathname?
Answer: Yes, there is a feature known as filename expansion will allows us do this using the TAB key.
For example: if we will have a path named /home/iceman/assignments directory, we will type as follows: /ho[tab]/ice[tab]/assi[tab] .
( sed command can be used )-use the result and use a grep command to look for occurrences of the word ORANGE in the files.

98. What is redirection?
Answer: Redirection will be the process of directing data from one output to another. It will also be used for directing an output as an input to another process.

99. What is grep command?
Answer: grep a search command which will make use of pattern-based searching. It will make use of options and parameters which are specified along with the command line and it can apply this pattern in searching the required file output.

100. What could be the problem when a command that was issued gave a different result from the last time it was used?
Answer: One highly possible reason to get different results for the same command due to case sensitivity issues.  Linux is case sensitive, a command which was previously used may have been entered in a different format from the present one.
For example, for listing all files in the directory, we should type the command ls, and not LS. If we type LS, it will result in an error message if no program exist by the name or it will produce a different output if a program named LS exists which will perform another function.

101. What are the contents of /usr/local?
Answer: It will contain locally installed files. This directory will matters in environments where files can be stored on the network. Specifically, locally-installed files will go to /usr/local/bin, /usr/local/lib, etc.).
This directory is used for software packages installed from source, or software not officially shipped with the distribution.

102. How do you terminate an ongoing process?
Answer: Every process in the system can be identified by a unique process id or pid. Use the kill command which is followed by the pid to terminate that process. For terminating all process at once, use kill 0.

103. How do you insert comments in the command line prompt?
Answer: Comments can be created by typing the # symbol before the actual comment text. This will tell the shell to completely ignore what will follow. For example “# This is just a comment which the shell will ignore.”

104. What is command grouping and how does it work?
Answer: We can use parentheses to group commands.
For example, if we want to send the current date and time along with the contents of a file named OUTPUT to a second file named MYDATES, we can apply command grouping as follows: (date cat OUTPUT) > MYDATES.

105. How do you execute more than one command or program from a single command line entry?
Answer: We will combine several commands by separating each command or program using a semicolon symbol.
For example, we will issue like a series of commands in a single entry:
ls –l cd .. ls –a MYWORK which is equivalent to 3 commands: ls -l cd.. ls -a MYWORK
**Note that this can be executed one after the other, in the order specified.

106. Write a command that will look for files with an extension “c”, and has the occurrence of the string “apple” in it.
Answer: A command that search for filewith an extension “c”, and has the occurrence of the string “apple” in it.
Find ./ -name “*.c” | xargs grep –i “apple”

107. Write a command that will display all .txt files, including its individual permission.
Answer: A command that will display all .txt files, including its individual permissionl
s -al *.txt

108. Write a command that will do the following:
-look for all files in the current and subsequent directories with an extension c,v-strip the,v from the result (you can use sed command)-use the result and use a grep command to search for all occurrences of the word ORANGE in the files.
Answer: Find ./ -name “*.c,v” | sed ‘s/,v//g’ | xargs grep “ORANGE”

109. What, if anything, is wrong with each of the following commands?
Answer: a) ls -l-s b) cat file1, file2 c) ls – s Factdir
Following is wrong with each of the following commands:
1. There should be space between the two options: ls -l -s
2. Do not use commas for separating arguments: cat file1 file2
3. There will be no space between hyphen and option label: ls
–s Factdir

110. What is the command to calculate the size of a folder?
Answer: Following is the Command to calculate the size of a folder:
To calculate the size of a folder will use the command du –sh folder1.

111. How can you find the status of a process?
Answer: To find the status of a process use the following command:
ps ux

112. How can you check the memory status?
Answer: We can check the memory status by using the command:
1. free -m to display output in MB
2. free -g to display output in GB

113.  Explain how to color the Git console?
Answer: To color the Git console, we will use the command git config—global color.ui auto. In the command, the color.ui variable will set the default value for a variable like color.diff and color.grep.

114. How can you append one file to another in Linux?
Answer: To append one file to another in Linux we will use command cat file2 >> file 1. The operator >> can append the output of the named file or creates the file if it will not be created. While another command cat file 1 file 2 > file 3 will append two or more files to one.

115. Explain how you can find a file using Terminal?
Answer: To find a file we have to use a command, find. –name “process.txt”.
It will look for the current directory for a file called process.txt.

116. Explain how you can create a folder using Terminal?
Answer: We have to use command mkdir to create a folder. It will be such as these: ~$ mkdir Guru99

117. Explain how to enable curl on Ubuntu LAMP stack?
Answer: To enable curl on Ubuntu, first, install libcurl, once it will be done use following command sudo/etc/init .d apache2 restart or sudo service apache2 restart.

118. Explain how to enable root logging in Ubuntu?
Answer: The command which will be enable root logging is
#sudo sh-c ‘echo “greater-show-manual-login=true” >>/etc/lightdm/lightdm.conf’

119. How can you run a Linux program in the background simultaneously when you start your Linux Server?
Answer: It will stop the process receiving the NOHUP signal and thus by terminating, it we will log out of the program which will invoked with and run the process in the background by using nohup.

120. Explain how to uninstall the libraries in Linux?
Answer: We will use command sudo apt-get remove library_name to uninstall the libraries in Linux.

121. What do you understand by Linux Kernal? Is it legal to edit it?
Answer: ‘Kernal’ basically will refer to which core component of the computer operating system which will provide basic services for the other parts and interacts with user commands.  It will come to ‘Linux Kernal’, it will be referred to as low-level system software providing an interface for user-level interactions.
Linux Kernal will be considered as free and open source software that will be capable of managing hardware resources for the users. It can be released under General Public Licenses (GPL), it will become legal for anyone to edit it.

122. Enlist the basic components of LINUX
Answer: Linux operating system basically will consist of three components that are enlisted below
1. Kernel: This will be considered as the core part and will be responsible for all major activities of the Linux operating system. Linux Kernel can be considered as free and open-source software that is capable of managing hardware resources for the users. It will consist of various modules and will interact directly with the underlying hardware.
2. System Library: Most of the functionalities of the operating system will be implemented by System Libraries. These will act as a special function using that application programs can accesses Kernel’s features.
3. System Utility: These programs will be responsible to perform specialized, individual-level tasks.

123. How do you open a command prompt when issuing a command?
Answer: Press Ctrl-Alt-F1 to open the default shell which is where the command prompt can be found,  This can give a command line interface (CLI) from which we will run commands as needed.

124. How can you find out how much memory Linux is using?
Answer: For memory usage information, from a command shell, use the “concatenate” command: cat /proc/meminfo. We should see a line starting something such as Mem: 64655360, etc. This is the total memory Linux.
To see available to use memory, We can also use commands
free – m
vmstat
top
htop
To find current memory usage

125. What is a typical size for a swap partition under a Linux system?
Answer: The preferred size for a swap partition will be twice the amount of physical memory available on the system. If it is not possible, then the minimum size will be the same as the amount of memory installed.

126. Explain the virtual desktop?
Answer: When there are multiple windows available on the current desktop and It will appears the problem of minimizing and maximizing windows or restoring all the current programs, there ‘Virtual Desktop’ will serve as an alternative. It  will allow to open one or more programs on a clean slate. Virtual desktops can basically stored on a remote server and serve the following benefits:
Virtual desktops are basically stored on a remote server and serve the following benefits
Cost savings as the resources can be shared and allocated as and when required.
1. Resources and energy are more efficiently used.
2. Data integrity is improved.
3. Centralized administration
4. Fewer compatibility issues.

127. Differentiate between BASH and DOS?
Answer: The basic differences between BASH and DOS will be understood from the below table
Show 102550100 entries
Search:

BASH	DOS
BASH commands will case sensitive.	DOS commands will not case sensitive.
‘/’ character can be used as a directory separator.
‘\’ character  will be act as an escape character.

‘/’ character: serves as a command argument delimiter.
‘\’ character: serves as a directory separator.

File naming convention includes: 8 character file name followed by a dot and 3 characters for the extension.	No file naming convention is followed in DOS.
128. Explain the term GUI?
Answer: GUI will stand for the Graphical user interface. GUI can be considered as the most attractive and user-friendly because it is consist of the usage of images and icons. These images and icons will be clicked and being manipulated by the users for the purpose of communication with the system.
Advantages of GUI:
1. It will allow users for navigation and operation the software with the help of visual elements.
2. The more intuitive and rich interface will be possible to be created.
3. Occurrence of errors as complex, multi-step, dependent are easily grouped together.
4. Productivity can be enhanced with the means of multitasking  with a simple click of the mouse, the user will be able to maintain multiple open applications and transitions between them.
Disadvantages of GUI:
1. End-users will have less control over the operating system and file systems.
2. It will easier to use a mouse and keyboard for navigation and controlling the operating system, the whole process can be a bit slow.
3. It will require more resources because of the elements which are required to be loaded likeicons, fonts, etc.

129. Explain the term CLI?
Answer: CLI will stand for Command Line Interface. It is a way for humans to interact with computers and it is called as the Command-line user interface. It will depend on textual request and response transaction process where user types declarative commands to instruct the computer to perform operations.
Advantages of CLI
1. Very flexible
2. Can easily access commands
3. Much faster and easier to use by expert
4. It does not use much CPU processing time.
Disadvantages of CLI
1. Learning and remembering type commands is hard.
2. Have to be typed precisely.
3. Can be very confusing

130. Enlist some Linux distributors (Distros) along with its usage?
Answer: There are approx 600 Linux distributors. Following are some important Linux distributors:
1. UBuntu: It is a popular Linux Distribution. It has a lot of pre-installed apps and it is easy to use repositories libraries. It can be very easily used and it will work like a MAC operating system.
2. Linux Mint: It will use cinnamon and mates desktop. It will work on Windows and it will be used by newcomers.
3. Debian: It is very stable, quicker and user-friendly Linux Distributors.
4. Fedora: It is not much stable but it gives the latest version of the software. It will have a GNOME3 desktop environment by default.
5.  Red Hat Enterprise: It is commercially used and tested before release. It will usually provide a stable platform for a long time.
6. Arch Linux: Every package can be installed by us and is will not be suitable for beginners.

131. How can you determine the total memory used by LINUX?
Answer: It is need to keep a track on the memory usage for finding out whether the user will be able for accessing the server or the resources are adequate. There are five methods which will determine the total memory used by Linux.
This will be explained as following
1. Free command: This is the very simple and easy to use command for checking memory usage. For example: ‘$ free –m’, the option ‘m’ displays all the data in MBs.
2. /proc/meminfo: To determine memory usage is for reading /proc/meminfo file. For example: ‘$ cat /proc/meminfo’
3. Vmstat: This command will be basically lays out the memory usage statistics. For example: ‘$ vmstat –s’
4. Top command: This command will determine the total memory usage and monitors the RAM usage.
5. Htop: This command will display memory usage  with other details.

132. Explain the 3 kinds of file permissions under LINUX?
Answer: Every file and directory in Linux will assign three types of owners  ‘User’, ‘Group’, and ‘Others’.
1. Read: This permission will allow us for open and read the file list the contents of the directory.
2. Write: This permission will allow us to modify the contents of the file and adding, removing and renaming files and stored in the directories
3. Execute: User will access and run the file in the directory. We will not run a file unless the execute permission is set.

133. What is the maximum length for any file name under LINUX?
Answer: The maximum length for any filename under Linux will be 255 characters.

134. How permissions are granted under LINUX?
Answer: A system administrator or the owner of the file will grant permissions using the ‘chmod’ command.
Following symbols will be used while writing permissions
1. +’ for adding permission
2. ‘-‘ for denying permission
3. Permissions will include a single letter will denote.
u : user; g: group; o: other; a: all; r: read; w: write; x: execute.

135. What are the different modes when using the vi editor?
Answer: The three different kinds of modes in vi editor will be enlisted below:
1. Command Mode/ Regular Mode
2. Insertion Mode/ Edit Mode
3. Ex Mode/ Replacement Mode

136. Explain the Linux Directory commands along with the description?
Answer: Following are the directory commands along with descriptions
1. pwd: It is a built-in command which will stand for ‘print working  directory’. It will display the current working location, working path starting with / and directory of the user. It will  display the full path to the directory we are currently in.
2. Is: This command will list out all the files in the directed folder.
3. cd: This will stand to ‘change directory’. This command will be used to change to the directory we want to work from the present directory. We required to type cd followed by the directory name for accessing that particular directory.
4. mkdir: This command will be used for creating an entirely new directory.
5. rmdir: This command will be used for removing a directory from the system.

137. Differentiate between Cron and Anacron?
Answer: Difference between Cron and Anacron will be understood from the below table

Cron	Anacron
It will  allow the user for scheduling tasks to be executed every minute.	It will allow the user to schedule tasks to be run either on a specific date or the first available cycle after the date.
Tasks will be scheduled by any normal user and are  used when tasks have to be completed/executed at a particular hour or minute.	It can be used only by super users and it is used when a task will have to be executed irrespective of hour or minute.
It is ideal for servers	It is ideal for desktops and laptops
It will expect the system to be running 24×7.	It will not expect the system to be running 24×7.
138. Explain the work of Ctrl+Alt+Del key combination on Linux operating system?
Answer: The work of Ctrl+Alt+Del key combination on Linux operating system will be same as for Windows such as to restart the system. The only difference is that there is no confirmation message which is displayed and a system is rebooted directly.

139. Explain Linux Shell?
Answer: User will uses a program known as the shell for executing any commands. Linux  is a user interface used to execute the commands and communicate with Linux operating system. Shell will not use the kernel for executing certain programs, create files, etc. There will be several shells available with Linux which will include the following
1. BASH (Bourne Again SHell)
2. CSH ( C Shell)
3. KSH ( Korn Shell)
4. TCSH
There are two types of Shell commands
Built-in shell commands: These commands will call from the shell and will be executed directly within the shell. Examples: ‘pwd’, ’help’, ’type’, ’set’, etc.
External/ Linux commands: These commands are shell independent and it has their own binary and are located in the file system.

140. What is a Shell script?
Answer: The shell script is written for the shell. This is a program file or a flat text file where certain Linux commands will be executed one after another. The execution speed will be slow, Shell script are easy for debugging and will also simplify everyday automation processes.

141. Explain the features of a Stateless Linux server?
Answer: If no state exists for the centralized server on a single workstation it is called stateless Linux server.
Some of the features of Stateless Linux server will be explained below
1. Stores prototype of every machine
2. Store snapshots
3. Store home directories
4. Uses LDAP which determines the snapshot of state to be run on which system.

142. What is system calls used for process management in Linux?
Answer: Process management in Linux will use certain system calls. These are mentioned in below table with a brief explanation

System calls	Explanation
Fork()	To create a new process
Exec()	For execution of a new program
Wait()	To make the process to wait
Exit()	Exit/terminate the process
Getpid()	To find the unique process id
Getppid()	To find the parent process id
Nice()	To bias the currently running process property
143. Enlist some Linux to file content commands?
Answer: There will many commands which present in Linux are used to look at the contents of the file.
Some of them are enlisted below
1. head: Displays the beginning of the file
2. tail: Displays the last part of the file
3. cat: Concatenate files and print on the standard output.
4. more: Displays the content in pager form and will be used for viewing text in the terminal window one page or screen at a time.
5. less: Displays the content in pager form and allows backward and single line movement.

144. Explain Redirection?
Answer: It is called that every command will  take an input and displays output. Keyboard will be serve as the standard input device and the screen will serve as the standard output device. Redirection is the process of directing data from one output to another or even cases exist where output serves as input data for another process.
There will be basically three streams available in which input and output of Linux environment are distributed.
These are explained as below
Input Redirection: ‘<’ symbol can be used for input redirection and is numbered as (0). Therefore it is denoted as STDIN(0).
Output Redirection: ‘>’ symbol can be used for output redirection and is numbered as (1). Therefore it is denoted as STDOUT(1).
Error Redirection: It will be denoted as STDERR(2).

145. Why is Linux considered as more secured than other operating systems?
Answer: Linux is an open-source operating system and it will be growing rapidly in the tech world/market. The entire code is written in Linux will be read by anyone, it is considered as more secure because of the following reasons:
1. Linux will provide its user with limited default privileges that will restricted to the lower levels example for in the case of any virus attack, virus can impact only local files and folders.
2. It has a powerful auditing system which will include detailed logs.
3. Enhanced features of IPtables can be used in order for implementing a greater level of security for Linux machine.
4. Linux will have tougher program permissions before installing anything on machine.

146. Explain command grouping in Linux?
Answer: Command grouping will be done by the use of braces ‘()’ and parenthesis ‘{}’. Redirection can be applied to the entire group when the command is grouped.
When commands can be placed within the braces, then they will be executed by the current shell. Example for (list)
When the commands can be placed within the parenthesis, then they will be executed by a subshell. Example for {list;}

147. What is Linux pwd (print working directory) command?
Answer: Linux pwd command will be display the whole path of the current location, we are working in starting from the root ‘/’. For  printing the current working directory enter “$ pwd”.
It will be used for the bellow purposes.
1. For finding the full path of the current directory
2. Store the full path
3. Verify the absolute and physical path

148. Explain the Linux ‘cd’ command options along with the description?
Answer: ‘cd’ will stand for change directory and it is used for changing the current directory on which the user will
work.
cd syntax : $ cd {directory}
Following purposes will be served with ‘cd’ commands
1. Change from current to a new directory
2. Change directory by the absolute path
3. Change directory by the relative path
Few of the ‘cd’ options will be enlisted below
1. cd~: Brings us to the home directory
2. cd-: Brings us to the previous directory
3. . : Bring us to the parent directory
4. cd/: Takes us to the entire system’s root directory

149. What will you know about grep commands?
Answer: Grep is stand for global regular expression print. This command can be used for matching a regular expression against text in a file. This command will perform pattern-based searching and only the matching lines will be displayed as output. It will make use of options and parameters which are specified along with the command line.
Assume we required to locate the phrase “our orders” in HTML file which is named as “order-listing.html”. The command can be as follows:
$ grep “our orders” order-listing.html
The grep Command will output the entire matching line to the terminal.

150. How to create a new file and modify an existing file in vi editor? Also, enlist the commands used to delete information from vi editor.?
Answer: Following Command can be used to create a new file and modify an existing file in vi editor:
1. vi filename: This is the command used for creating a new file and modify an existing file.
2.View filename: This command can open an existing file in read-only mode.
3. X: This command can delete the character which is under the cursor or before the cursor location.
4. dd: This command can be used for deleting the current line

151. Enlist some Linux networking and troubleshooting commands?
Answer: Every computer can be connected to network internally or externally for the purpose of exchanging information. Network troubleshooting and configuration will be essential parts of and network administration. The networking commands enable us to quickly troubleshoot connection issues with another system, check the response of another host, etc.
A network administrator will maintain a system network which will include network configuration and troubleshooting.
Following are few commands along with their description
1. Hostname: This is used for viewing the hostname (domain and IP address) of the machine and for setting the hostname.
2. Ping: This will check if the remote server will be reachable or not.
3. ifconfig: This will display and manipulate route and network interfaces. It will display network configuration. ‘ip’ is the replacement of ifconfig command.
4. netstat: It will display network connections, routing tables, interface statistics. ‘ss’ is the replacement of netstat command which can be used for getting more information.
5. Traceroute: It is a network troubleshooting utility which will be used for finding the number of hops needed for a particular packet to reach the destination.
6. Tracepath: It is the same as traceroute with a difference that it will not need root privileges
7. Dig: This command can be used for querying the DNS name servers for any task related to the DNS lookup.
8. nslookup: To find DNS related query.
9. Route: It will show the details of the route table and manipulates the IP routing table.
10. mtr: This command will combine ping and track path into a single command.
11. Ifplugstatus: This command will inform us whether the network cable is plugged in or not.

152. What is the advantage of open source?
Answer: Open source will facilitates to distribute software, including source codes freely to anyone who is interested. So, It can  add features and even debug and correct errors of the source code.

153. Is it legal to edit Linux Kernel?
Answer: Yes. It is legal edit Linux Kernel cause Linux Kernel is released under General Public License (GPL) and anyone can edit it. It will come under the category of free and open source software.

154. What is Linux pwd (print working directory) command?
Answer: Linux pwd command will be display the whole path of the current location, we are working in starting from the root ‘/’. For  printing the current working directory enter “$ pwd”.
It will be used for the bellow purposes
1. For finding the full path of the current directory
2. Store the full path
3. Verify the absolute and physical path

155. Explain the Linux ‘cd’ command options along with the description?
Answer: ‘cd’ will stand for change directory and it is used for changing the current directory on which the user will work.
cd syntax : $ cd {directory}
Following purposes will be served with ‘cd’ commands
1. Change from current to a new directory
2. Change directory by the absolute path
3. Change directory by the relative path
Few of the ‘cd’ options will be enlisted below
1. cd~: Brings us to the home directory
2. cd-: Brings us to the previous directory
3. . : Bring us to the parent directory
4. cd/: Takes us to the entire system’s root directory

156. How to create a new file and modify an existing file in vi editor? Also, enlist the commands used to delete information from vi editor.?
Answer: Following Command can be used to create a new file and modify an existing file in vi editor:
1. vi filename: This is the command used for creating a new file and modify an existing file.
2.View filename: This command can open an existing file in read-only mode.
3. X: This command can delete the character which is under the cursor or before the cursor location.
4. dd: This command can be used for deleting the current line.

157. Enlist some Linux networking and troubleshooting commands?
Answer: Every computer can be connected to network internally or externally for the purpose of exchanging information. Network troubleshooting and configuration will be essential parts of and network administration. The networking commands enable us to quickly troubleshoot connection issues with another system, check the response of another host, etc.
A network administrator will maintain a system network which will include network configuration and troubleshooting.
Following are few commands along with their description
1. Hostname: This is used for viewing the hostname (domain and IP address) of the machine and for setting the hostname.
2. Ping: This will check if the remote server will be reachable or not.
3. ifconfig: This will display and manipulate route and network interfaces. It will display network configuration. ‘ip’ is the replacement of ifconfig command.
4. netstat: It will display network connections, routing tables, interface statistics. ‘ss’ is the replacement of netstat command which can be used for getting more information.
5. Traceroute: It is a network troubleshooting utility which will be used for finding the number of hops needed for a particular packet to reach the destination.
6. Tracepath: It is the same as traceroute with a difference that it will not need root privileges.
7. Dig: This command can be used for querying the DNS name servers for any task related to the DNS lookup.
8. nslookup: To find DNS related query.
9. Route: It will show the details of the route table and manipulates the IP routing table.
10. mtr: This command will combine ping and track path into a single command.
11. Ifplugstatus: This command will inform us whether the network cable is plugged in or not.

158. Is it legal to edit Linux Kernel?
Answer: Yes. It is legal edit Linux Kernel because Linux Kernel is released under General Public License (GPL) and anyone can edit it. It will come under the category of free and open source software.

159. What is the advantage of Linux?
Answer: Linux gives a free downloading facility for all codes and every aspect has additional features.

160. Which Linux is specially designed by the Sun Microsystems?
Answer: Solaris is designed by the Linux of Sun Microsystems.

161. Name the Linux loader.
Answer: LILO is the Linux loader.

162. If you have saved a file in Linux. And again you wish to rename the file, what command will be used for it?
Answer: mv Command is used to rename a saved file.

163. Write about an internal command.
Answer: internal commands is built in the shells.

164. Define inode.
Answer: Each file has a unique name which is given by the operating system which is called as the inode.

165. If the programmer is willing to execute an instruction at the specified time. Which command is used?
Answer: The ‘at’ command is used to execute an instruction at the specified time.

166. Explain process id.
Answer: The operating system can identify each process by a unique id called as the process id.

167. Which popular office suite is available free for both Microsoft and Linux?
Answer: Open Office Suite is available free for both.

168. Suppose a company is recently switched from Microsoft to Linux and they have some MS Word document to save and work in Linux, what can be done?
Answer: Install Open Office Suite on Linux. It will facilitate us to work with Microsoft documents.

169. What is SMTP?
Answer: SMTP is stand for Simple Mail Transfer Protocol. It is an internet standard for mail transmission.

170. What is Samba? Why is it used?
Answer: Samba service is used for connecting Linux machines to Microsoft network resources by giving Microsoft SMB support.

171. What are the basic commands for user management?
Answer:
1. last,
2. chage,
3. chsh,
4. lsof,
5. chown,
6. chmod,
7. useradd,
8. userdel,
9. newusers

172. Is Linux Operating system virus free?
Answer: No, Linux is not virus free but it will have less number of viruses.

173. Which partition stores the system configuration files in Linux system?
Answer: /stc partition.

174. Which command is used to uncompress gzip files?
Answer: gunzip Command

175. Why do developers use MD5 options on passwords?
Answer: MD5 is an encryption method, therefore it is used for encrypting the passwords before saving.

176. What is the difference between soft and hard mounting points?
Answer: In the soft mount, if the client will fail to connect the server, it will provide an error report and will close the connection But in the hard mount, if the client will fail to access the server, the connection will hang; and once the system is up, it will again accesses the server.

177. What is LILO?
Answer: LILO is a boot loader for Linux. It will be used mainly for loading the Linux operating system into main memory so that it will begin its operations.

178. What are the modes used in VI editor?
Answer: There are following types of modes in vi Editor:
Regular mode or command mode
Insertion mode or edit mode
Replacement mode or Ex-mode

179. How to exit from vi editors?
Answer: The following commands can be used for exiting from vi editors.
:wq will save the current work and will exit the VI.
:q! will exit the VI without saving current work.

180. You wish to print a file ‘draft’ with 60 lines on a page. What command would you use?
Answer: The command used to print a file ‘draft’ with 60 lines on a page:
pr -l60 draft
The default page length if we are using pr is 66 lines.
The -l option specifies a different length.

181. What is LD_LIBRARY_PATH?
Answer: LD_LIBRARY_PATH is an environment variable. It will be used for debugging a new library or a non-standard library. It can  also be used to identify which directories required to be searched for; to do this the path to search for the directories required to specified.
The variable will be set using:
setenv—LD_LIBRARY_PATH–$PATH
It is used for searching for the shared objects/dynamic libraries by the operating system for extendable functionality at the runtime.
1.Name a service that you should disable (which acts both as web and FTP servers) on a Linux server.
The finger service can be disabled on a Linux server because a remote user will get important information about the system by using this command.

182. What does Sar provide? Where are Sar logs stored?
Answer: Sar will collect, report, or save system activity information, and it will serve to log and it will evaluate a variety of information regarding system activity.  Sar will permit retroactive analysis of the load values for various sub-systems like CPUs, memory, disks, interrupts, network interfaces, and so on and for the limitation of problems in this manner. If CPU utilization is approximately 100 percent (user + nice + system), the workload sampled is CPU-bound.
By default, the log files of Sar command are located at the /var/log/sa/sadd file, where the dd parameter will indicate the current day.

183. How to check memory stats and CPU stats as a Linux Admin?
Answer: Using the free and vmstat commands, we will display the physical and virtual memory statistics, respectively. With the help of the sar command, we will see the CPU utilization and other stats.

184. How to reduce or shrink the size of the LVM partition?
Answer: Following are the logical steps for reducing the size of the LVM partition:
Unmount the file system using the unmount command
Use the resize2fs command as
resiz2fs /dev/mapper/myvg-mylv 10G
3.use the lvreduce command as lvreduce -L 10G /dev/mapper/myvg-mylv
The above commands shrink the size of the LVM partition and fix the size of the file system to 10 GB.

185. What are the different modes of Network Bonding in Linux?
Answer: Following are the modes used in Network Bonding:
1. balance-rr or 0: The round-robin mode for fault tolerance and load balancing
2. active-backup or 1: Sets the active-backup mode for fault tolerance
3. balance-xor or 2: Sets an XOR (exclusive-or) mode for fault tolerance and load balancing
4. broadcast or 3: Sets a broadcast mode for fault tolerance. All transmissions are sent on all slave interfaces
5. 802.3ad or 4: Sets an IEEE 802.3ad dynamic link aggregation mode and creates aggregation groups that share the same speed and duplex settings
6. balance-tlb or 5: Sets a Transmit Load Balancing (TLB) mode for fault tolerance and load balancing
7. balance-alb or 6: Sets an Active Load Balancing (ALB) mode for fault tolerance and load balancing.

186. How can you enhance the security of a password file?
Answer: Linux will keep the user account information in a text file called /etc/passwd. This file can store the one-way encrypted password. It will be accessed by several tools for receiving user information that is a security risk. For minimizing security risk, we will use a shadow password format. This method can save account information in the regular file, /etc/passwd.
However, the password will store as a single ‘x’ character not actually stored in this file. A second file is called /etc/shadow which contains the encrypted password, and other information like account or password expiration values, etc. The /etc/shadow file can be read only by the root account and therefore it has fewer security risks.

187.What command can you use to make a tape archive file of /home directory and send it to the /dev/tape device?
Answer: The following is correct command:
tar -cvf /dev/tape /home
The -xvf option is used to extract files from an archive.

188.Suppose, FTP Server is hacked and the entire server needs to
be restored. How can we restore the original Kernel system files?
Answer: We cannot restore the entire operating system from the tape backup device. Therefore, we should reinstall the core operating system and restore the system configuration files and user data from the tape backup device.

189. Why will we avoid Telnet to administer a Linux system remotely?
Answer: Telnet will use the most insecure method to communicate. It will send data across the network in plain text format, and anybody can easily find out the password by the network tool. It will include the passing of the login credentials in plain text, example for anyone running a sniffer on our network can find the information required to have control of the device in a few seconds by eavesdropping on a Telnet login session.

190.What is Puppet Server?
Answer: Puppet is open-source and enterprise software for configuration management toll in UNIX-like operating systems. It is IT automation software which is used to push configuration to its client’s puppet agents using its code. Puppet code will do multiple tasks from installing new software for checking file permissions to updating user accounts.

191. Which command is used to check the number of files, the disk space, and each user’s defined quota?
Answer: The repquota command can be used for checking the status of a user’s defined quota, with the disk space and the number of files used.
This command will provide a summary of the user’s quota, example for how much space and files will be left for the user. Each user has a defined quota in Linux. This will be done mainly for security as some users will have only limited access to files. This will provide security to files from unwanted access. The quota will be given to a single user or to a group of users.

192. What is the name and path of the main system log?
Answer: By default, the main system log is /var/log/messages. This file will contain all messages and will script written by a user. By default, all scripts can be saved in this file. This is the standard system log file, which will contain messages from all system software, non-kernel boot issues, and messages which go to dmesg. The dmesg file is a system file which is written upon the system boot.

193. Can a Linux computer be made a router so that several machines can share a single Internet connection and how?
Answer: Yes, a Linux machine will be made a router. This can be called IP Masquerade. IP Masquerade is a networking function in Linux similar to the one-to-many (1:Many) NAT (Network Address Translation) servers will found in various commercial firewalls and network routers.
The IP Masquerade feature will allow other ‘internal’ computers connected for this Linux box via PPP, Ethernet, etc. to connect to the Internet. Linux IP Masquerading will allow this functionality even if the internal computers will not have IP addresses.
IP masquerading will be done through the following steps:
1. The Linux PC will have an Internet connection and a connection to the LAN. Typically, a Linux PC will have two network interfaces: an Ethernet card for the LAN and a dial-up PPP connection to the Internet (through an ISP).
2. All other systems on our LAN will use the Linux PC as the default gateway for TCP/IP networking. Use the same ISP-provided DNS addresses on all systems.
3. Enable IP forwarding in the Kernel. By default, the IP forwarding will not be enabled. For ensuring that IP forwarding will be enabled, when we reboot system, place this command in the /etc/rc.d/rc.local file.
4. Run /sbin/iptables—the IP packet filter administration program—to set up the rules that enable the Linux PC to masquerade for your LAN.

194.How to change window manager by editing your home directory?
Answer: The /.xinitrc file will allow changing the window manager we required for using when logging into X from that account. The dot in the file name shows that the file is a hidden file and will not show when do a normal directory listing. To set a window manager, we will have for saving a command in this file.
The syntax of this command is:
exec window manager
It will save the file. Next time when run a startx, a new window manager can open and become the default.
The commands to start some popular window managers and desktop environments are:
KDE = startkde
Gnome = gnome-session
Blackbox = blackbox
VWM = fvwm
Window Maker = wmaker
IceWM = icewm

195. How are shadow passwords given in Linux?
Answer: The pwconv command will be used to give shadow passwords. Shadow passwords will be given for better system security. The pwconv command will create the file /etc/shadow and will change all passwords to ‘x’ in the /etc/passwd file.
First, the entries in the shadowed file, which will not exist in the main file, can be removed. Then, the shadowed entries which will not have ‘x’ as the password in the main file are updated. Any missing shadowed entries can also added. Finally, passwords in the main file will be replaced with ‘x’. These programs will be used for initial conversion as well to update the shadowed file if the main file will edited by hand.

196. What daemon is used for scheduling the commands?
Answer: The crontab command will be used for scheduling the commands to run at a later time.
Syntax:
crontab [ -u user ] file
crontab [ -u user ] { -l | -r | -e }
Options:
-l List: It will Display the current crontab entries
-r: It will Remove the current crontab
-e: Edits the current crontab using the editor specified by the VISUAL or EDITOR environment variables.
When a user will exit from the editor, the modified crontab can be installed automatically. Each user will have their own crontab, and though these will files in /var, it is not intended to be edited directly.
If the -u option is provided, and then the crontab will provide the name of the user whose crontab are to be tweaked. If it is given without this option, then it can be displayed the crontab of the user who will execute the command.

197. What shell does assign to a POP3 mail-only account?
Answer: A Linux Administrator can assign a POP3 mail-only account to the /bin/false shell. It will assign a bash shell for a POP3 mail-only account provides the user login access that is avoided. The /bin/nologin shell will also be used. This shell can be provided to the user when we don’t want to provide shell access to the user. The user will not access the shell and it will reject shell login on the server as in Telnet. It is for the security of the shells.
POP3 can basically used for downloading mail-to-mail programs. It is for the illegal downloading of emails on the shell, this account can be assigned to the /bin/false shell or the /bin/nologin shell. Both shells will be the same as they do the same work of rejecting the user login to the shell.
The main difference between these two shells is the the false shell shows the incorrect code and any unusual coding when a user logs in to it, but the nologin shell simply inform that no such account is available. Therefore, the nologin shell can be used often in Linux.

198. If a volume group named VG0 already exists and we need to extend this volume group up to 4 GB, how would you do it?
Answer: First, we  required to create a physical volume (/dev/sda7) of size 4 GB.
We would run the following command:
vgextend VG0 /dev/sda7

199. Is there any relation between the modprobe.conf file and network devices?
Answer: Yes, this file will assign a Kernel module to each network device.
Example:
[root@localhost ~]# cat /etc/modprobe.conf
alias eth0 b44
Here, b44 is the kernel module for network device eth0.
We will confirm whether this module “b44” can be presented or not by the following command
[root@localhost ~]# lsmod |grep b44
b44 29005 0

200. What is YUM?
Answer: YUM will stand for Yellow dog Updater, Modified because it can be based on YUP, the Yellow dog Updater. Yellow Dog can a version of Linux for the Power Architecture hardware and is RPM-based, just such as Red Hat Enterprise Linux and Fedora. YUP, and later YUM, were can be written by the Linux community as a way to maintain an RPM-based system.

201. What is the role of Kudzu?
Answer: Kudzu can be used for detecting new hardware. Red Hat Linux will run a hardware discoverer, called Kudzu. When we will attempt to identify a serial port, Kudzu resets the serial port. This will stop the serial console. Kudzu can be configured from the file:
/etc/sysconfig/kudzu
Kudzu will be prevented from resetting hardware, by setting the configuration parameter SAFE to ‘yes.’

202. What is the difference between ext2 and ext3 file systems?
Answer: The ext3 file system is developed version of the ext2 file system.
The difference between ext2 and ext3 is that ext3 will support journaling.
After an unexpected power failure or system crash also called an unclean system shutdown, each mounted ext2 file system on the machine can be checked for consistency by the e2fsck program. This is a time-consuming process and during this time, any data on the volumes can be unreachable.
The journaling can be provided by the ext3 file system means this sort of a file system check is no longer necessary after an unclean system shutdown. The only time a consistency check will occur while using ext3 is in certain rare hardware failure cases, like hard drive failures. The time for recovering an ext3 file system after an unclean system shutdown will not depend on the size of the file system or on the number of files. Rather, it will depend on the size of the journal used for maintaining consistency. The default journal size will take almost a second for recovering, depending on the speed of the hardware.

203. Explain the /proc file system?
Answer: The /proc file system is a virtual file system which will provide detailed information about Linux Kernel, hardware, and running processes. Files under the /proc directory can be named as virtual files.
Since /proc will contain virtual files, it can be called a virtual file system. These virtual files will have unique qualities. They are listed as zero bytes in size.
Virtual files like /proc/interrupts, /proc/meminfo, /proc/mounts, and /proc/partitions provide an up-to-the-moment glimpse of the system’s hardware. Others: The /proc/filesystems file and the /proc/sys/ directory will provide system configuration information and interfaces.

204. How would you create an ext4 file system?
Answer: We will create an ext4 file system with the following command:
# mke2fs -t ext4 /dev/DEV

205. How to enable ACLs for the /home partition?
Answer:  Add the following entry in /etc/fstab:
LABEL=/home /home ext3 acl 1 2
Then, remount the /home partition with the acl option:
mount -t ext3 -o acl /dev/sda3 /home

206. Explain the history of Linux?
Answer: In 1991, Linus Torvalds was a student at the University of Helsinki, Finland. He has started writing code to get the academic version of Unix for free. Later, it was popular as Linux Kernel.

207. How many types of Shells are there in Linux?
Answer: They are five Shells in Linux:
1. C Shell (csh): It has C syntax and it will provide spelling checking and job control.
2.Korn Shell (ksh): It is a high-level programming language shell.
3. Z Shell (Zsh): It will provide some unique nature such as it will observes login/logout watching, file name generating, startup files, closing comments.
4.  Bourne Again Shell (bash): default to Linux distributions.
5. Friendly Interactive Shell (Fish): It will provide web-based configuration,  auto-suggestions, etc.

208. What are the basic components of Linux?
Answer: Following are the Basic components of Linux
1. Kernel: it is as an interface between software and hardware.
2. Shell: It is as an interface between the user and the Kernel.
3. GUI: It will stand for Graphic User Interface that is another way for the user to interact with the system.  It is unlike images, buttons, text boxes for interaction.
4. System Utilities: These are the software functions which will allow users to manage the computer.
5. Application Programs: Set of functions designed for performing a set of tasks.

209. What are the environmental variables?
Answer: They are dynamic values which will affect the process of programs on a computer. They are available in every operating system and their types can vary. They will be created, edited, saved and deleted and they will provide the information about the system behavior.

210. What is the advantage of Open Source?
Answer: Linux was one of the first open-source technologies which many programmers added software which is completely open for the users, that means we can download the file and change the code as per need. It has a wide range of options for the users and increased security.

211. What is the disadvantage of Open Source?
Answer: Disadvantages of Open Source Operating System which is mentioned below
1. Difficulty of use
2. Compatibility Issues
3. Liabilities and warranties
4. Hidden costs

212. What are the symbolic links?
Answer:  Symbolic links can be redirected to another file using its path. Target files will not contain any data. Symbolic links can redirect to another entry in the file system. If the target file can be deleted, link to that file will be removed, but not the file.

213.  What are hard links?
Answer: A hard link is an existing file on Linux. So many numbers of hard links can be created, for any file. It can create links for other hard links.

214. Explain Process Management System Calls in Linux?
Answer: The process management system calls in Linux:
1. fork(): Used for creating a new process.
2. exec(): Execute new process.
3. wait(): wait until process execution.
4. exit(): exit from the process.
System calls to get the Process id :
1. getpid(): to find the unique process id.
2. getppid(): to find the unique parent process id.

215.What is a File system in Linux?
Answer: Linux file system will stores and handles the data. Without a file system, it will not know where the file will start from and where the file will end.

216. Explain different file system types in Linux?
Answer: There are many file systems in a Linux:Ext, Ext2, Ext3, Ext4, JFS, XFS, btrfs, ufs, autofs, devpts, ntfs and swap.

217. Why LVM is required?
Answer: LVM will stand for Large Volume Management, it will manage Storage in device. User will create, resize and delete LVM partitions. It will increase the abstraction, flexibility and control. LVM can be used for gathering existing storage devices into the group and allocate logical units.

218. What is umask?
Answer: unmask is stand for user file creation mode and the user will creates any file, which has default file permissions. Therefore unmask can specify few restrictions to the newly created file. It will control the file permissions.
umask [-S] [mask]

219. How to set the mask permanently for a user?
Answer: If the unmask command will invoke without any arguments, that will mean it can display the current mask.
For setting the unmask permanently, we have following types.
They are:
1. Ocotal representation.
2.Symbolic representation.

220. What is network bonding in Linux?
Answer: Network Bonding is a process for combining more than two network interfaces to form a single network interface. It can offer performance improvement and redundancy by increasing network throughput and bandwidth. There is no requirement to worry, if one interface is down or unplugged because the other will work. The behavior of the bonded interface will depend on the bonding method.

221. What are the different modes of Network bonding in Linux?
Answer: Mode-0(balance-rr): default mode and based on Round-Robin policy. It will offer fault tolerance and load balancing features. It will use round-robin fashion for transmitting the packets.
Mode-1(active-backup): Based on Active Backup policy and only one slave can act in the band and another one can act when the others will fail in the band. It will also provide fault tolerance.
Mode-2(balance-xor): It will sets a xor mode between the source Mac address and destination MAC address for providing fault tolerance.
Mode-3(broadcast): Based on broadcast policy and transmitted everything in the slave interface. It will provide fault tolerance and it will be used only for a particular purpose.
Mode-4(802.3ad): A dynamic aggregation mode, it will be created aggregation groups that are having the same speed. It can use transmit hashing method for selecting the slaves for outgoing traffic.
Mode-5(balance-tlb): The outgoing traffic is according to the current load on the slave, and the incoming traffic can be received by the slave. It will called an adaptive transmit load balancing mode.
Mode-6(balance-alb): An adaptive load balancing mode. It will not require any switch support.

222. How to check the default route and routing table?
Answer: We can use the following commands to display the default route and routing table,
$ route-n
$ nestat-rn
$ ip

223. How to check which ports are listening in my Linux Server?
Answer: We have two commands for checking which ports are in listening in Linux Server. Following are the commands 
# netstat –listen
# netstat –l

224.Where the kernel modules are located?
Answer: lib/modules/kernel-version/, this directory can store all the information about the compiled drives under the Linux system. Using lsmod command also we will see the installed kernel modules.

225. How to change the default run level in Linux?
Answer: To change the default run level in Linux use init command.

226.How to share a directory using nfs?
Answer: To share a directory using NFS, 
1. edit the configuration file and ‘/etc/exports’
2. add an entry like directory name ‘/’.
3.  restart the NFS service.

227. What are the default ports used for SMTP, DNS, FTP, DHCP, SSH, and squid?
Answer:

Service	Port
SMTP	25
DNS	53
FTP	20(Data Transfer) 21(Connections Established)
DHCP	68(dhcp client), 67(DHCP server)
SSH	22
Squid	3128
228.How to lock user account in Linux?
Answer: Locking user account is done for the security purpose therefore that unauthorized users will not login. Therefore, we will have a few ways to lock the user account. Few of them are listed below.
1.Lock or disable the password using passwd command.
2. Expire the user account using usermod command or chage command.
3. Changing the shell using nologin command ( /sbin/nologin ).

229. What is env command in Linux?
Answer: env is a shell command which is  used for printing a list of current environmental variables and it will run another process in another environment without any modification of the current environment.
env [OPTION]… [-] [NAME=VALUE]… [COMMAND [ARG]…]
Options

Tag	Description
-i, –ignore-environment	Start with an empty environment.
-0, –null	output line End with a 0 (null) byte rather than a newline.
-u, –unset=NAME	removes variable NAME from the environment
–help	Display a help message and exit.
230. What is top Command in Linux?
Answer: top command is used for showing the system process and it will display and update the sorted process information. 

231. What is netstat command in Linux?
Answer: netstat command will give various information regarding the network and routing tables, interface statics and more about the system.

232. What is lsof command in Linux?
Answer: lsof means List of file, we will know which file is opened by which process.
#lsof

233. Explain about chmod command?
Answer: This command can be used for changing the permission of files and directories.  On the whole, there are three ty0pe of permission, read, write and execute and are represented by numbers as shown below.
4 – read permission
2 – write permission
1- execute permission
syntax:
$ chmod options permissions file name
$ chmod [OPTION]… MODE[,MODE]… FILE…
$ chmod [OPTION]… OCTAL-MODE FILE…
$ chmod [OPTION]… –reference=RFILE FILE

234. Explain about chown command?
Answer: The command “chown” will stand for change file owner and Group. This command is used for changing the ownership of one or more files or folders for a specified user or group.
syntax:
$chown [OPTION]… [OWNER][:[GROUP]] FILE…
                                Or
$ chown [OPTION]… –reference=RFILE FILE…

235. What is cp command in Linux?
Answer: cp command will be used for copying files and directories. It can also used for backup files or directories.
$ cp file name

236. How to remove file or directory from the system in Linux?
Answer: The rm command will used for removing directory or file specified on the command line.
Syntax:
rm filename— 

Command	Description
rm filename	Removes single file.
rm filename1, filename2, filename 3	Removes multiple files.
 rm * .pdf	Removes all pdf files in the current directory. 
 rm -i filename(s)	-i means to confirm before deleting the file
 rm -i filename(s)	Removes files without prompting
rm -fv *.txt	Remove all .txt files in the current directory without prompting
237. What is mkdir in Linux?
Answer: mkdir command will allow users to create directories in the Linux. User will create multiple directories and will set the permissions for  the directories.
Syntax:
mkdir [options…] [directories …]
mkdir [options…] [directories …]

Option	Description
Directory	name of the directory to be created
-m=mode, –mode=mode	to set a file mode permissions, etc. for the created directories
-p, –parents	create parent directories
–v, –verbose	Verbose output. Print a message for created directory.
–Z= context, –context=context	If we will use  SELinux, this option sets the security context of each created directory to context.
–help	shows help message and exit
–version	It shows version information and exit
238. Explain rmdir command in Linux?
Answer: The rmdir will be used for removing each directory specified on the command line.
Syntax:
rmdir [-p] [-v | –verbose] [–ignore-fail-on-non-empty] directories

239. Enlist some Linux file content commands?
Answer: File content commands
1. head: Display top lines of the file.
2. tail: Display last lines of the file.
3. cat: Concatenate more than 2 files.
4. more: Displays the content in pager form to view in the terminal.

240. What is meant by internal commands and external commands?
Answer: Internal Commands: Commands will directly run by the shell is called as internal commands and there will be no separate process to run the commands.
External Commands: External Commands are run by the kernel is called as external commands and for every single command has its own unique process id.

241. What is meant by PIPE in Linux?
Answer: It is a form of redirection which will be used in Linux, it is used for combining more than two commands and the output of one command will take as input to the next command.
Syntax:
command_1 | command_2 | command_3 | …. | command_N

242. Describe how a parent and child process communicates each other?
Answer: Parent process will communicate with the child process by using pipes, sockets, messages queues and more.

243. Explain features of Stateless Linux Server?
Answer: Features of stateless Linux Server:
1. Stores the prototype of every system.
2. Stores the snapshot was taken.
3. Stores the home directories.
4. Uses LDAP, which will contain the information about which snapshot should run on which system.

244. What is Zombie Process?
Answer: It is a process whose execution will be completed but even the information will exist in the process table. It will occur for the child process because the parent process requires to read the child process status. Once it will be completed using the wait system call, then the zombie process can be removed from the process table. This is called as Zombie Process.

245. What is tail command in Linux?
Answer: tail command will display the last part of a file. Generally, users will require every logline to troubleshoot. Instead, we want to check what  logs state about the most recent request to your application.
tail Example:
$ tail -n 100 /var/log/httpd/access_log

246. What is cat command in Linux?
Answer: In Linux cat Command will  concatenate and print files. Users may use cat to check the contents of  dependencies file or to confirm the version of the application that we have already built locally.
cat Example:
$cat requirements.txt
flask
flask_pymongo.

247. What is df command in Linux?
Answer: Users will use df command for troubleshooting disk space issues.  df will stand for display free disk space.
df Command Example:
df -h

248. What is du command in Linux?
Answer: du command in Linux is used for retrieving detailed information about which files can use the disk space in a directory.
du Command Example:
$du -sh /var/log/*
1.8M  /var/log/anaconda
384K  /var/log/audit
4.0K  /var/log/boot.log
0 /var/log/chrony
4.0K  /var/log/cron
4.0K  /var/log/maillog
64K /var/log/messages

249.What is iptables command in Linux?
Answer: iptables command will block or allow traffic on a Linux host, similar to a network firewall. This iptables command will prevent certain applications from receiving or transmitting requests.

250. What does cd – command do?
Answer: cd- command go to the previous directory.

251. What does cd command do?
Answer: cd go to $HOME directory

252. What does (cd dir && command) do?
Answer: cd dir && command will go to the dir, execute the command and return to the current directory.

253. What does pushd command do?
Answer: pushd will command put current dir on the stack so we can pop back to it.

254. What is ls -lSr command?
Answer: ls – ISr command will show files by size, biggest file can be displayed last.

255. What is du -s * | sort -k1,1rn | head command used for?
Answer: This command will show top disk users in current dir.

256. What does this du -hs /home/* | sort -k1,1h command do?
Answer: easy to interpret disk usage.

257. What is df -h command?
Answer: This command will show free space on mounted file systems.

258. What is df -i command?
Answer: df -I Command will show free inodes on mounted filesystems.

259. What is fdisk -l command used for?
Answer: fdisk -I command will show disks partitions sizes and types run as root.

260. How do you kill the program using one port in Linux?
Answer: Use this command for kills the program using one port: sudo fuser -k 8000/tcp

261. How do you limit memory usage for commands?
Answer: Limit memory usage for commands
ulimit -Sv 2000       # 2000 KBs = 2 MB
ulimit -Sv unlimited  # Remove limit

262. How do you get full path of a file in Linux?
Answer: <strong style=”font-family: -apple-system, BlinkMacSystemFont, ‘Segoe UI’, Roboto, Oxygen, Ubuntu, Cantarell, ‘Open Sans’, ‘Helvetica Neue’, sans-serif; color: #e74c3c;”>Ans:</strong> Use this command: readlink -f file.txt

263. How do you list contents of tar.gz and extract only one file?
Answer: Use these commands:
tar tf file.tgz
tar xf file.tgz filename

264. How do you find who is logged in?
Answer: Use this command for finding who logged in: w

265. How do you check permissions of each directory to a file?
Answer: It is useful for detecting permissions errors, for example when configuring a web server.
namei -l /path/to/file.txt

266. How to copy text to the clipboard?
Answer: Use this command: cat file.txt | xclip -selection clipboard

267. How do you check resources usage?
Answer: Use this command to check resource usage: /usr/bin/time -v ls

268. How do you run a command for a limited time?
Answer: Use this command: timeout 10s ./script.sh
# Restart every 30 minutes
while true; do timeout 30m ./script.sh; done

269. How do you combine two lines from two sorted files in Linux?
Answer: Use this command: comm file1 file2.

270. Where is password file located in Linux and how can you improve the security of password file?
Answer: To improve the security of the password file, we will use shadow password format. Therefore, in shadow password format, the password can be stored as single “x” character that is not the same file (/etc/passwd). This information can be stored in another file instead with a file name /etc/shadow. Therefore, for enhancing the security,  this file is readable only by the root user. Thus security risks will be overcome to a great extent by using the shadow password format.

271. What is Key-based authentication? Explain.
Answer: There are various methods for entering into the servers. One of the ways to log in is using password-based authentication, but that will not secure. Therefore, we required a method which is secured.
The way to achieve the security is to use Key-based authentication. To use this type of authentication, we required to disable the password-based authentication. Therefore, there is a procedure to set up this authentication that is as below:
We have to get the SSH key pair using following command:
$ ssh-keygen -t rsa
It can generate the public/private rsa key pair.
Enter file where required to save this generated key (/home/username/.ssh/id_rsa):
It can prompt  for the same location, i.e. ~/.ssh/id_rsa for the key pair. Press enter if required to confirm the same location. Else, if  want to provide any other location, enter that and confirm the same.
Now copy ~/.ssh/id_rsa.pub into the ~/.ssh/authorized_keys which will be located where we have to connect.
Now, we have to provide the permissions to the file as per below command:
$ chmod 600 ~/.ssh/authorized_keys
Now try to sshthe machine we want to connect, and we will see that we are able to login to the machine without a password.
If we are confirmed that key-based authentication is working fine, disable the password-based authentication.
Go to the path /etc/ ssh/sshd_config
set the following property as no.
PasswordAuthentication no

272. How can your track events on your system?
Answer: We can able to track events by using a daemon. It should be a specific daemon for it to work. 

273. How do you run the command every time a file is modified?
Answer: Use this command to do:
while inotifywait -e close_write document.text

274. How can you grant permission?
Answer: If we are a system administrator, then we can grant permission. We can do it by using the “chmod” command, followed by a “+”. If we ever wanted to revoke the permission, the process will look the same. The only thing that we have to replace is the “+” – you’d insert a “–” in its place.

275. What is a ‘whoami’ command?
Answer: This command is used on both Windows and Linux.
“who am I?” This is the meaning of the command – it shows current login and user information.

276. What is a ‘partial backup’?
Answer: Partial back up will allow us to choose specific files that we want to back up, instead of doing so with the entire system.

277. What is “comm” used for?
Answer: “Comm” can compare two files and will search for both common and exclusive features.

278. What command would you use to have your processor use less time?
Answer: This is  the “nice” command.
We have to also set different priority numbers for the task. CPU will perform the tasks in order of priority, thus it will make it run faster and smoother.

279. What does ls -R do?
Answer: The Is-R option or command is used for flagging the lists of the directory in a recursive manner.

280. What are the Linux boot files?
Answer: The Linux boot files are the configuration files, that will be accessed and called during the system booting operation. The usage of this /boot/directory will be standardized in the File System Hierarchy as it can hold all the files used in booting the system- it is the first file to be called during the system boot. It will contain Linux kernel files or boot loader files.

281. What is Samba? Why is it used?
Answer: Samba is software suite with open source. It will run on Linux OS and Unix/Linux based platforms. It is a reimplementation of the Common Internet File System (CIFS) and the more central Server Message Block (SMB) protocol. It will be the standard Windows interoperability suite, that will mean, the software is able to communicate the programs of Linux to the Windows clients like a native application

282. What is SSH? what is the method to connect a remote server via SSH?
Answer: SSH will stand for Secure Shell, which will be a protocol for securely logging onto remote systems. It is the most common and simple way for accessing the remote Linux based servers. We must own a domain name and IP address

283. What is a shebang line?
Answer: The shebang or bang line is the absolute path from the root to the Bash interpreter. In a text file, the program loader will parses the text in the initial line following the shebang as an interpreter directive.

284. What does the command env do?
Answer: The env command is a shell command, that will be used for printing out a list of the existing environment variables, or to run another program in a custom environment without changing the current one.

285. What is the basic difference between BASH and DOS?
Answer: The key differences between the BASH and DOS console lie in three areas:
1. BASH commands are case sensitive but DOS commands are not;
2. Under BASH, / character is a directory separator and \ acts as an escape character and under DOS, / serves as a command argument delimiter and \ is the directory separator
3. DOS will follow a convention in naming files, that is 8 character file name which is followed by a dot and three characters for the extension. BASH follows no such convention.

286. What is the importance of the GNU project?
Answer: This so-called Free software movement which will allow several advantages, like the freedom to run programs for any purpose and freedom of study and modify a program to  requirement. It will also allow us to redistribute copies of software to other people, and the freedom for improving software and have it released for the public.

287. What does chmod +x FILENAMEdo?
Answer: The chmod command is an abbreviation for Change Mode. This command will be extremely useful to change the permission for Files and folders located in Linux/Unix. File/Directory permission, that is generally Write, Read or executable for any user, group or others.

288. What is the difference between Telnet and SSH?
Answer: SSH is basically a network protocol, that is used for remotely access and manage any device distantly. The chief difference between SSH and Telnet is that SSH will make use of encryption, that will implies  the entire data is transmitted over a network which is secure from snooping. Telnet is not as secure but like Telnet, a user who will want to access a remote device must install an SSH client.

289. What does set -o do?
Answer: Set is an inbuilt shell, that will display all the shell variables including the environment variables.

290. State the difference between swap partition and a swap file?
Answer: The Linux Operating System will use reserved disk block in the hard drive to swap. This is called as Swap Partition as no other files will be traced in the swap partition. In Windows OS, the swap space or partition will be called swap file or page file.

291. What is an A record, an NS record, a PTR record, a CNAME record, an MX record?
Answer: An NS record will be operated for providing a subdomain to a set of name servers. A user will delegate a domain to DNSimple, the TLD authorities will automatically place NS records for which domain in the TLD name servers.
The PTR record will  be basically used as a spam filter and will be used for authenticating the incoming messages. A record will always exist for the PTR records.
CNAME will stand for Canonical Name, that is this record will provide to an alias name.
MX will stand for Mail Exchanger and the MX record will be a special type of resource record in the DNS (Domain Name System). It will specify a mail server, that is completely responsible to accept the messages via email on behalf of the recipient’s domain. A preference value will be used for prioritizing the mail delivery in case of multiple servers.

292. What is a Split-Horizon DNS?
Answer: This is the facility of the DNS implementation for providing the user with DNS information. It will provide a strong mechanism for privacy management and overall security. 

293. What is a typical size for a swap partition under a Linux system?
Answer: The recommended swap size is of 20% of RAM for modern systems. If hibernation will be used, the swap will have a minimum of the same amount of space as the physical RAM.

294. What is SSH port forwarding?
Answer: SSH port forwarding will create a secure connection between a remote machine through that services will be relayed and the local computer, which will provides the commands. It will also called SSH tunneling and will be used for transmission of information, that is not necessarily require an encrypted protocol. 

295. What does the immutable bit do to a file?
Answer: Making the file immutable by associating the immutable bit attribute to it will prohibit even the root user from deleting it.

296. Describe the mknod command and when you’d use it.
Answer: The mknod command will be employed for creating device files which will act strangely as compared with normal files. Device files will be kept in the directory /dev, and unlike normal files, these device files are ones that the kernel called about, and reads or writes to.

297. What is the TCP handshake?
Answer: This is a three-way handshake  of the transmission control protocol, that will use the SYN-SYN-ACK method.

298. How to increase the size of LVM partition ?
Answer: Below are the Logical Steps :
1. Use the lvextend command (lvextend -L +100M /dev/<Name of the LVM Partition> , we will extend the size by 100MB.
2. resize2fs /dev/<Name of the LVM Partition>
check the size of partition using ‘df -h’ command

299. How to reduce or shrink the size of LVM partition ?
Answer: Below are the logical Steps for reducing size of LVM partition :
1. Umount the filesystem using umount command,
2. use resize2fs command , example for resiz2fs /dev/mapper/myvg-mylv 10G
3. use the lvreduce command , example for lvreduce -L 10G /dev/mapper/myvg-mylv
Above Command can shrink the size and can make the filesystem size 10GB.

300. How to create partition from the raw disk ?
Answer: We will able to create partitions from the raw disk using fdisk utility. Following are the steps for creating partition from the raw dsik :
1. fdisk  /dev/hd* (IDE) or /dev/sd* (SCSI)
2. Type n to create a new partition
3. After creating partition , type w command to write the changes to the partition table.

301. Where the kernel modules are located ?
Answer: The ‘/lib/modules/kernel-version/’ directory will store all kernel modules or compiled drivers in Linux operating system. With ‘lsmod’ command we we will able to see all the installed kernel modules.

302. Does it help for a Linux system to have multiple desktop environments installed?
Answer: One desktop environment, such as KDE or Gnome, is good enough to operate without issues. It will be all a matter of preference for the user, although the system will allow switching from one environment to another. Some programs can work in one environment and will not work on the other, therefore it will also be considered a factor in selecting which environment to use.

303. How to set the umask permanently for a user?
Answer: For setting this value permanently for a user, it required to be put in the appropriate profile file that will depend on the default shell of the user.

304.  How to change the default run level in linux ?
Answer: We have to edit the file “/etc/inittab” to change the run level and change initdefault entry ( id:5:initdefault:). We change the run level temporary such as ‘init 3’ using ‘init’ command.  This command will move the system in runlevl 3.

305. How to share a directory using nfs ?
Answer: For sharing a directory using nfs ,  edit the configuration file ‘/etc/exportfs’ , add a entry like
‘/<directory-name>  <ip or Network>(Options)’ and then restart the nfs service.

306. How to check and mount nfs share ?
Answer: We will able to see what directories are shared via nfs example for ‘showmount -e <ip address of nfs server>’ using ‘showmount’ command. We can mount the nfs share on linux machine using mount command .

307. What are the default ports used for SMTP,DNS,FTP,DHCP,SSH and squid ?
Answer:  Service      Port
SMTP          25
DNS            53
FTP             20 data transfer,
                    21 Connection established
DHCP        67/UDP(dhcp server) ,
                    68/UDP(dhcp client)
SSH            22
Squid         3128

308. What are the basic components of Linux?
Answer: Linux will have all of these components: kernel, shells and GUIs, system utilities, and an application program.

309. What are the different modes of Network bonding in Linux?
Answer: Following are list of modes used in Network Bonding :
1 .balance-rr or 0 – round-robin mode for fault tolerance and load balancing.
2. active-backup or 1 – Sets active-backup mode for fault tolerance.
3. balance-xor or 2 – Sets an XOR (exclusive-or) mode for fault tolerance and load balancing.
4. broadcast or 3 – Sets a broadcast mode for fault tolerance. All transmissions will be sent on all slave interfaces.
5. 802.3ad or 4  – Sets an IEEE 802.3ad dynamic link aggregation mode. Creates aggregation groups which will share the same speed and duplex settings.
6. balance-tlb or 5 –  Sets a Transmit Load Balancing (TLB) mode for fault tolerance and load balancing.
7. balance-alb or 6 –  Sets an Active Load Balancing (ALB) mode for fault tolerance and load balancing.

310. How to check and verify the status the bond interface.
Answer: We will able to check which mode is enabled and what lan cards are used in this bond  the command ‘cat /proc/net/bonding/bond0’. We have one only one bond interface but we will have multiple bond interface such as bond1,bond2 and so on.

311. How to check default route and routing table ?
Answer: We can see the default route and routing tables using the Commands ‘netstat -nr’ and ‘route -n’

312. How to check which ports are listening in my Linux Server ?
Answer: Use the Command ‘netstat –listen’ and ‘lsof -i’

313. List the services that are enabled at a particular run level in linux server ?
Answer: We will able to list all the service which are enabled in run level5. For other run levels just replace five with the respective run level.

314. How to enable a service at a particular run level ?
Answer: We will enable a service by using the Command ‘chkconfig <Service-Name> on –level 3’ at a particular run level.

315. How To scan newly asssigned luns on linux box without rebooting ?
Answer:  There are two ways for scanning newly assigned luns :
1. Method1: if sg3 rpm is installed , then run the command ‘rescan-scsi-bus.sh’
2. Method2: Run the Command ,  echo ” – – – ” > /sys/class/scsi_host/hostX/scan

316. How  to find WWN numbers of HBA cards in Linux Server ?
Answer: We can  find the WWN numbers of HBA cards by using the command ‘systool -c fc_host -v | grep port_name’ in Linux server.

317. How to add & change the Kernel parameters ?
Answer: First edit the file ‘/etc/sysctl.conf’ to Set the kernel parameters in linux. After making the changes,  we can save the file and can run the command ‘sysctl -p’ . This command can make the changes permanently without rebooting the machine.

318. What is Puppet Server ?
Answer:  Puppet is an open-source and enterprise software for configuration management toll in UNIX such as operating system.  Puppet is a  IT automation software will be used to push configuration to its clients puppet agents using code. Puppet code will install new software,  check file permissions, or update user accounts and lots of other tasks.

319. What are manifests in Puppet ?
Answer: Manifests in Puppet are the files in that the client configuration is specified.

320. Which Command is used to sign requested certificates in Puppet Server ?
Answer: ‘puppetca  –sign hostname-of-agent’ in (2.X)  & ‘puppet ca  sign hostname-of-agent’ in  (3.X)

321. At which location  Puppet Master Stores Certificates ?
Answer: /var/lib/puppet/ssl/ca/signed

322. How to find all the regular files in a directory  ?
Answer: using the command ‘find /<directory -type f’.

323. What is load average in Linux ?
Answer: Load  Average will be defined as the average sum of the number of process waiting in the run queue and number of process currently will execute over the period of 1,5 and 15  minutes. We find the load average of a Linux sever using the ‘top’ and ‘uptime’ command

324. Torvalds, Wrote most of the Linux Kernel in C++ programming Language, do you agree?
Answer: No! Linux Kernel will contain 12,020,528 Lines of codes out of which 2,151,595 Lines are comments. Therefore remaining 9,868,933 lines will be codes and out of 9,868,933 Lines of codes 7,896,318 can be written in C Programming Language.
The remaining Lines of code 1,972,615 is written in C++, Assembly, Perl, Shell Script, Python, Bash Script, HTML, awk, yacc, lex, sed, etc.
The Number of Lines of codes varies on daily basis and an average of more than 3,509 lines are being added to Kernel.

325. Do you agree with Linux was developed for intel X86 architecture but has been ported to other hardware platform than any other Operating System?
Answer: Yes, I do agree. Linux will be written for x86 machine, and has been ported for all kind of platform. Linux has a very promising future in mobile phone, Tablets.We are surrounded by Linux in remote controls, space science, Research, Web, Desktop Computing.
The list is endless.

326.Which Syntax of any Linux command is:
Answer:  command [options] [arguments]
command options [arguments]
command [options] [arguments]
command options arguments
The correct Syntax of is Command [options] [arguments].

327. Choose the odd one out.
Answer: Vi
vim
cd
nano
The odd one in the list is cd. Vi, vim and nano are editors that is useful in editing files, and cd command is used to change directory.

328. What is YUM?
Answer:  YUM stands for Yellowdog Updater Modified Which is an open source command-line and graphical based package management tool for RPM (RedHat Package Manager) based Linux systems. It will allow users and system administrator to easily install, update, remove or search software packages on a systems. It will be developed and released by Seth Vidal under GPL (General Public License) as an open source, which means anyone will allowed to download and access the code to fix bugs and develop customized packages. YUM can use numerous third party repositories to install packages automatically by resolving their dependencies issues.

329. What are the ways to implement Virtual Desktop?
Answer: There are following ways to implement Virtual Desktop:
Switching Desktops: In the case of Switching Desktops, we will create discrete virtual desktops to run programs. Each virtual desktop can behave as an individual desktop and the programs will be running on each of these desktops is accessible only to the users who will be using that particular desktop.
Oversized Desktops: Oversized Desktops will not offer a discrete virtual desktop but it will allow the user to pan and scroll around the desktop which is larger in size than the physical screen.

330. Explain Process Management System Calls in Linux
Answer: Following are the process Management  System Calls in Linux:
1. fork () : Used to create a new process
2. exec() : Execute a new program
3. wait() : Wait until the process finishes execution
4. exit() : Exit from the process
The System Calls used for getting Process ID are:
1. getpid():- get the unique process id of the process
2. getppid():- get the parent process unique id

331. Explain the ‘ls’ command in Linux
Answer: The ls command is used for listing the files in a specified directory. The general syntax is:
$ ls <options> <directory>
For example, if we want to list all the files in the Example directory, then the command can be as follows:
$ ls Example/
There are different options which will be used with the ls command. These options will provide additional information regarding the file/ folder.
For example:

-l	 lists long format shows the permissions of the file
-a	 lists all files including hidden files
-i	 lists files with their inode number
-s	 lists files with their size
-S	 lists files with their size and sorts the list by file size
-t	 sorts the listed files by time and date
332. What is a Latch?
Answer:  A Latch is a temporary storage device which is  controlled by timing signal that can either store 0 or 1. A Latch will have two stable states (high-output or 1, and low-output or 0) and can be used to store state information. A Latch will store one bit of data as long as it is powered on. 

333. What is a Microprocessor?
Answer:  A Microprocessor is a device which will execute instructions. It will be a single-chip device which fetches the instruction from the memory, decodes it and executes it. A Microprocessor will carry out three basic functions:
Mathematical operations
Move data from one memory location to another
Make decisions based on conditions and jump to new different instructions based on the decision.

334. What is the minimum number of disk partitions required to install Linux?
Answer: The minimum number of partitions required is two.
One partition can be used as the local file system where all the files will be stored. This will includes files of the OS, files of applications and services, and files of the user. The other partition can be used as Swap Space which will acts as an extended memory for RAM.

335. How to copy a file in Linux?
Answer:  We can use the cp command to copy a file in Linux. The general syntax is:
$ cp <source> <destination>
Suppose we want to copy a file named questions.txt from the directory /new/linux to /linux/interview, then the command can be:
$ cp questions.txt /new/linux /linux/intervie

336. How to find the difference in two configuration files?
Answer: We can use the diff command for this:
$ diff abc.conf xyz.conf

337. How would you create a text file without opening it?
Answer: The touch command will be used to create a text file without opening it. The touch command can create an empty file. The syntax is as follows:
$ touch <filename>
Suppose to create a file named sample.txt, then the command would be:
$ touch sample.txt

338. How would you delete a directory in Linux?
Answer: There are two commands that can be used to delete a directory in Linux.
rmdir
$ rmdir <directory name>
rm -rf
$ rm -rf <directory name>
Note: The command rm -rf should be used carefully because it will delete all the data without any warnings.

339. How would you schedule a task in Linux?
Answer: There are two commands for schedule tasks in Linux: cron and at.
The cron command is used for repeatedly scheduling a task at a specific time. The tasks will be stored in a cron file and then executed using the cron command. The cron Command can read the string from this file and schedules the task.
Syntax
<minute> <hour> <day> <month> <weekday> <command>
Suppose we want to run a command at 4 pm every Sunday, then the string would be:
0 16 * * 0 <command>
The at command is used for schedule a task only once at the specified time.
Suppose we want to shut down the system at 6 pm today, then the command for this would be:
$ echo “shutdown now” | at -m 18:00

340. Suppose you try to delete a file using the rm command and the deletion fails. What could be the possible reason?
Answer: The path specified to the file or the file name mentioned might be wrong
The user trying to delete the file might not have permissions to delete the file.

341. How do you look at the contents of a file named sample.z?
Answer: The .z extension means that the file is compressed. To look at the contents of the compressed file, we will  use the zcat command. Example:
$ zcat sample.z

342. How to copy files to a Floppy Disk safely?
Answer: Steps to copy files to a Floppy Disk safely:
1. Mount the floppy disk
2. Copy the files
3. Unmount the floppy disk
If We don’t unmount the floppy disk, then the data might become corrupted.

343. How to identify which shell you are using?
Answer:  Open the terminal and run:
$ echo $SHELL
This can print the name of the Shell being used. 

344. How can you login to another system in your network from your system?
Answer: SSH will be used to login to another system in network.
Syntax
ssh <username>@<ip address>
Suppose we want to login into a system with IP address 192.168.5.5 as a user “Jon”, then the command would be:
$ ssh Jon@192.168.5.5

345. How would you open a file in read-only mode using the vim editor?
Answer: $ vim -R <filename>

346. How would you search for a specific Employee ID in a file using the vim editor?
Answer: $ vim +/<employee id to be searched> <filename>

347. How to jump to a particular line in a file using vim editor?
Answer: $ vim +<line number> <filename>

348. How do you sort the entries in a text file in ascending order?
Answer: We can sort the entries in a text file in ascending order by sort Command.
$ sort sample.txt

349. How do you check the status of all the services?
Answer: $ service –status-all

350. How do you start and stop a service?
Answer: To start:
$ service <servicename> start
To stop:
$ service <servicename> start

351. Explain the free command.
Answer: This command can be used to display the free, used, swap memory available in the system.
Typical free command output. The output will be displayed in bytes.
$ free

352. Which file will we examine for determining the levels of messages written in system log files?
Answer: – kernel.h

353. You are logged on as a regular user. Without logging off and logging on as root, we will required to create a new user account immediately. How would you do it?
Answer:
1. This will be achieved by issuing the su command.
2. This will prompt  for the password of the root account.
3. Providing the password, logs  in as root. Now, we can perform any administrative duties.

354. You are required to restore the file memo.ben. It was backed up in the tar file MyBackup.tar. Which command would you use to do it?
Answer: The command Which we will  use is: tar xf MyBackup.tar memo.ben
It will use the x switch to extract a file.

355. What is partial backup?
Answer: When we will select only a portion of  file hierarchy or a single partition to back up, it will called partial backup.

356. What is the fastest way to enter a series of commands from the command-line?
Answer:
1. Write the commands, each separated by a semi-colon.
2. Press enter after the last command.
3. The semi-colon would inform the shell that multiple commands are being entered at the command line, are executed serially.

357. Which command is used to check the number of files and disk space used and the each user’s defined quota?
Answer: repquota command can be used to check the status of the user’s quota along with the disk space and number of files used.
This command will provide a summary of the user’s quota that how much space and files will be left for the user. Every user will have a defined quota in Linux. This can be done mainly for the security, as some users will have only limited access to files. This will provide a security to the files from unwanted access. The quota will be provided to a single user or to a group of users.

358. What is the name and path of the main system log?
Answer: By default, the main system log is ‘/var/log/messages’. This file will contain all the messages and the script will be written by the user. By default all scripts can be saved in this file. This is the standard system log file, that will contain messages from all system software, non-kernel boot issues, and messages which go to ‘dmesg’. dmesg is a system file which is written upon system boot.

359. Which utility is used to make automate rotation of a log?
Answer: logrotate command will be used for making automate rotation of log.
Syntax of the command is:
logrotate [-dv] [-f|] [-s|] config_file+
It will allow automatic rotation, compression, removal, and mailing of log files. This command will be mainly used to rotate and compressed log files. This job will be done every day when a log file will become too large. This command will also be run by giving on command line. We can done force rotation by providing –f option with this command in command line. This command can also used for mailing. We can provide –m option for mailing with this command. This option will take two arguments subject and recipient name.

360. What are the partitions created on the mail server hard drive?
Answer: The main partitions will be done firstly that are root, swap and boot partition.
But for the mail server three different partitions will be also done that are as follows:
1. /var/spool – This will be done so that if something is wrong with the mail server or spool than the output will not overrun the file system.
2. /tmp – Putting this on its own partition will prevent any user item or software from overrunning the system files.
3. /home – Putting this on its own is useful for system will upgrade or reinstalls. It will allow not to wipe off the /home hierarchy along with other areas.

361. What are the fields in the/etc/passwd file?
Answer: It will contain all the information of the users who log into the system. It will contains a list of the system’s accounts, providing for each account some useful information such as user ID, group ID, home directory, shell, etc. It will have general read permission as many utilities, like ls use it to map user IDs to user names, but it will write access only for the superuser (root).
The main fields of /etc/passwd file are:
1. Username: It will be used when user logs in. It should be between 1 and 32 characters in length.
2. Password: An x character will indicate that encrypted password which is stored in /etc/shadow file.
3. User ID (UID): Each user must be assigned a user ID (UID). UID 0 (zero) can be reserved for root and UIDs 1-99 will be reserved for other predefined accounts. Further UID 100-999 will be reserved by system for administrative and system accounts/groups.
4. Group ID (GID): The primary group ID (stored in /etc/group file)
5. User ID Info: The comment field. It will allow  to add extra information about the users like user’s full name, phone number etc. This field can be used by finger command.
6. Home directory: The absolute path to the directory the user can be in when they log in. If this directory will not exists then users directory becomes /
7. Command/shell: The absolute path of a command or shell (/bin/bash). Typically, this will a shell.

362. Which commands are used to set a processor-intensive job to use less CPU time?
Answer: nice command will be used for changing priority of the jobs.
Syntax: nice [OPTION] [COMMAND [ARG]…]
Range of priority will goes from -20 (highest priority) to 19 (lowest). Priority will be  provided to a job therefore that the most important job will be executed first by the kernel and then the other least important jobs. This will take less CPU times as the jobs will be scheduled and are provided priorities therefore the CPU will execute fast. The priority is provided by numbers such as -20 describe the highest priority and 19 describe the least priority.

363. How to change window manager by editing your home directory?
Answer: We want to use when logging into X from that account “/.xinitrc file” will allow changing the window manager.  The dot in the file name will show that the file is a hidden file and will not show when do a normal directory listing. To set a window manager we will have to save a command in this file. The syntax of command is: exec windowmanager. Save the file. Next time when  run a startx a new window manager can open and become default.
The commands for starting some popular window managers and desktop environments are:
-KDE = startkde
-Gnome = gnome-session
-Blackbox = blackbox
-FVWM = fvwm
-Window Maker = wmaker
-IceWM = icewm

364. How documentation of an application is stored?
Answer: When a new application will be installed its documentation can also be installed. This documentation will be stored under the directory named for application. For example if application name is App1 then the path of the documentation can be /user/doc/App1. It will contain all the information about the application. It will contain date of creating application, name of application and other important module of the application. We will get the basic information of application from the documentation

365. How can your track events on your system?
Answer: We track events by using a daemon. It has to be a specific daemon for it to work. It would be the “syslogd” daemon.

366. How can you grant permission?
Answer: If we are a system administrator, then we can grant permission. We would have to do therefore by using the “chmod” command, followed by a “+”. If we ever wanted for revoking the permission, the process will look the same. The only thing that would have to replace is the “+” – we would insert a “–” in its place.

367. Which shell do you assign to a POP3 mail-only account?
Answer: POP3 mail only account will be assigned to the /bin/false shell. However, assigning bash shell to a POP3 mail only provides user login access, that is avoided. /bin/nologin will be also be used. This shell can provided to the user when we will not want to give shell access to the user. The user will not access the shell and it will reject shell login on the server such as on telnet. It will mainly for the security of the shells. POP3 will be basically used to download mail to mail program. Therefore for illegal downloading of emails on the shell this account will be assigned to the /bin/false shell or /bin/nologin. These both shells can be same they both do the same work of rejecting the user login to the shell. The main difference between these two shells is that false shell will show the incorrect code and any unusual coding when user login with it.

368. Which daemon is responsible for tracking events on Linux system?
Answer: syslogd will be responsible to track system information and can save it to the desired log files. It will provide two system utilities that give system logging and kernel message trapping. Internet and UNIX domain sockets will support enable this utility package for supporting both local and remote logging. Every logged message will contain at least a time and a hostname field, a program name field, too. Therefore to track these information this daemon will be used.
syslogd mainly will react to the set of signals provided by the user.
These are the signals provided to syslogd:
1. SIGHUP: This syslogd perform a re-initialization. All open files can be closed, the configuration file, default is /etc/syslog.conf can  read again and the syslog facility can be started again.
2. SIGTERM: The syslogd can die.
3. SIGINT, SIGQUIT: If debugging will be enabled these can be ignored. Otherwise syslogd can die.
4. SIGUSR1: Switch debugging on/off. This option will only be used if syslogd can be started with the – d debug option.
5. SIGCHLD: Wait for Childs if some were born, because of waiting messages.

369. Which daemon will be used for scheduling of the commands?
Answer: The crontab command can be used to schedule of the commands to run at a later time.
SYNTAX:
crontab [ -u user ] file
crontab [ -u user ] { -l | -r | -e }
Options:
1. l List – display the current crontab entries.
2. r- Remove the current crontab.
3. e- Edit the current crontab using the editor specified by the VISUAL or EDITOR environment variables.
When user will exit from the editor, the modified crontab can be installed automatically. Each user will have their own crontab, and though these will be files in /var, they will not intended to be edited directly.
If the –u option is provided than the crontab will provide the name of the user whose crontab will be tweaked. If it is provided without this then it can display the crontab of the user who will be executing the command.

370. How environment variable is set so that the file permission can be automatically set to the
newly created files?
Answer: umask command will be used to set file permission on newly created files automatically.
Syntax: umask [-p] [-S] [mode]
It will be represented in octal numbers. We will simply use this command without arguments for seeing the current file permissions. To change the permissions, mode is provided in the arguments. The default umask will be used for normal user is 0002. The default umask used for  the root user is 0022. For calculating the original values, the values shown by the umask must be subtracted by the default values. It will be mainly used to mask of the file and directory permission. The /etc/profile script will be where the umask command will be usually set for all users. The –S option will be used for seeing the current default permissions displayed in the alpha symbolic format. For example, umask 022 will ensure that new files can have at most 755 permissions (777 NAND 022).
The permissions will be calculated by taking the NAND of original value with the default values of files and directories.

371. What is the difference between home directory and working directory?
Answer: Home Directory: Every user can have one home directory and can have complete control over it. On login, home is the default working directory for the user. It will contain the configuration files and responsible for login and logout of the user.
Working directory: The directory in which the user will be working currently is called as working directory. The home can  be the working directory, if the user will not be working in it.

372. What is initrd image and what is its function in the linux booting process?
Answer: The initial RAM disk (initrd) will an initial root file system which is mounted prior to when the real root file system will be available.The initrd can be bound to the kernel and loaded as part of the kernel boot procedure. The kernel will mount this initrd as part of the two-stage boot process for loading the modules for making the real file systems available and get at the real root file system. Thus initrd image will play a vital role in linux booting process.

373. Explain the terms suid, sgid and sticky bit?
Answer: There are few special permissions which are available for executable files and directories.
1. SUID: If setuid bit is set, when the file will be executed by a user, the process can have the same rights as the owner of the file being executed.
2. SGID: Same as above, but it will inherit group privileges of the file on execution, not user privileges. Similar way when we will create a file within the directory, it can inherit the group ownership of the directories.
3. Sticky bit: Sticky bit will be used on executables in linux therefore that they will remain in the memory more time after the initial execution, hoping they will be required in the near future. It is on folders, to imply that a file or folder will be created inside a stickybit which is enabled folder will only be deleted by the owner. A very good implementation of sticky bit is /tmp , where every user will write permission but only users who own a file will delete them.

374. What is Static library and dynamic library?
Answer: Static libraries are loaded when the program will be compiled and dynamically-linked libraries will be loaded in while the program is running. Dynamic libraries will save the RAM space as against the static library because linking to static libraries will include the actual code for the library function(s)/procedure(s) with the executable. DLL code will be kept at one location and will be usually shared among all the processes which use the DLL.

375. Explain RPM (Red Hat Package Manager) features.
Answer: RPM is a package managing system which is a collection of tools to manage software packages.
Features:
1. RPM will verify software packages.
2. RPM will be served as a powerful search engine to search for software’s.
3. Components, software’s etc will be upgraded using RPM without having to reinstall them
4. Installing, reinstalling will be done with ease using RPM
5. During updates RPM will handle configuration files carefully, therefore that the customization will not lost.

376. How do you sent a mail attachment via bash console?
Answer: Mutt is an opensource tool to send emails with attachments from the linux bash command line. We will install “mutt” from the binary rpm or via package manager.
For Ubuntu / Debian based destros.
# apt-get install mutt
For Redhat / Fedor based destros,
# yum install mutt
Usage:
# mutt -s “Subject of Mail” -a “path of attachment file” “email address of recipient” < “message text containing body of the message”
Example for : mutt -s “Backup Data” -a /home/backup.tar.gz admin@mywebsite.com < /tmp/message.txt

377. What is the difference between umask and ulimit?
Answer: Umask will stand for ‘User file creation mask’, that will determine the settings of a mask which will control which file permissions will be set for files and directories when they will be created. While ulimit will be a linux built in command which will provide control over the resources available to the shell and/or to processes started by it.
We limit user to specific range by editing /etc/security/limits.conf at the same time system wide settings will be updated in /etc/sysctl.conf

378. What are the run levels in linux and how to change them?
Answer: A run level is a state of init and the whole system which will define what system services will be operating and they will be identified by numbers.There are seven different run levels present which is 0-6 in Linux system for the different purpose.
The descriptions are provided below.
0: Halt System (To shutdown the system)
1: Single user mode
2: Basic multi user mode without NFS
3: Full multi user mode (text based)
4: unused
5: Multi user mode with Graphical User Interface
6: Reboot System
To change the run level, edit the file “/etc/inittab” and change initdefault entry ( id:5:initdefault:). If we want to change the run level on the fly, it will be done using ‘init’ command.
For example, when we type ‘init 3′ in the command line , this will move the system from current runlevel to runlevl 3. Current level can be listed by typing the command ‘who -r’

379. What is SeLinux?
Answer: SELinux is an acronym for Security-enhanced Linux Which is an access control implementation and security feature for the Linux kernel. It will be designed to protect the server against misconfigurations and/or compromised daemons. It will put limits and instructs server daemons or programs what files they will access and what will actions they will take by defining a security policy.

380. Why should I use DAS either NAS or SAN?
Answer: There are some solutions that will exist but before choosing one solution , we required to know their role:
1. DAS is a block device from a disk that is physically attached for the host machine like a /dev/sda or /dev/sda1) . We must place a filesystem upon it before it will be used. There will be limitations like the number of servers which will access it. Storage device, or DAS storage has to be near to the server storage and the resources will be dedicated but generally, we will not able to dedicate the hard disks to multiple computers. DAS solution will be inexpensive and simple to configure. Technologies to do this will include IDE, SCSI, SATA, etc.
2. NAS  will authenticate clients and provide shared to other computers and users will over a network so it will require a dedicated ip address to be accessible. NAS devices will generally run an embedded operating system on simplified hardware and lack peripherals such as a monitor or keyboard. Network file systems will be considered safe enough to be used in a concurrent way, the protocol implementation can take care of problems due for concurrent accessing to the same resource (file), normally by locking the file to a single user/requester. We will set up automatic or manual will backup and file copies between the NAS and all other connected devices by using a software program. It will be an easy way for providing RAID redundancy to mass amount of users, it will allows users permissions, folder priv
leges, restricted access to documents, etc
3. SAN has the particularity to be a block level storage solution that NAS will not provide. It will be optimized for high volume of block level data transfer. SAN will performed best when used with fiber channel medium (optical fibers, and a fiber channel switch). It will provide synchronous replication and it is an architecture for attaching remote storage for making it will appear as though it will be locally attached. There will be highly scalable, both from a capacity and performance perspective. It will offer centralized storage management. It will be a solution for terabytes of storage and multiple simultaneous access to files example for streaming audio/video and it will allow virtual environments, cloud computing, etc.

381. What is drop cache in Linux and how do you clear it?
Answer: Cache in Linux memory will be where the Kernel can store the information it will required later, as memory will be incredible faster than disk.
It will be great which the Linux Kernel will take care about that.Linux Operating system will be very efficient in managing  computer memory, and will automatically free the RAM and drop the cache if some application requires memory.
Kernels 2.6.16 and newer provide a mechanism to have the kernel will drop the page cache and/or inode and dentry caches on command, which will help free up a lot of memory. We will throw away which script that will be allocated a ton of memory will to get rid of the cache.
To free pagecache:
# echo 1 > /proc/sys/vm/drop_caches
To free dentries and inodes:
# echo 2 > /proc/sys/vm/drop_caches
To free pagecache, dentries and inodes:
echo 3 > /proc/sys/vm/drop_caches
This will be a non-destructive operation in normal scenarios and will only free things which are completely unused.  It will always be preferred to run “sync” first to flush useful things out to disk.

382. Password based authentication is disabled in your infrastructure. So how do you login to the servers?
Answer: Most of the organizations will be turned to use key based authentications instead of Password based authentication to improve the system security even further.
We will enforce the key-based authentication by disabling the standard password authentication, that will involve a public key private key pair. The public key will be added in the server configuration file while private key will be kept confidential on the client side.
To set up password less authentication.
1) Generating Key Pairs
A)Generate an RSA key pair at a shell prompt by typing following:
$ ssh-keygen -t rsa
Generating public/private rsa key pair.
Enter file in which to save the key (/home/steve/.ssh/id_rsa):
B)Press Enter to confirm the default location (that is, ~/.ssh/id_rsa) for the newly created key.
C)Enter a passphrase, and confirm it by entering it again when prompted to do so.
D)Copy the content of ~/.ssh/id_rsa.pub into the ~/.ssh/authorized_keys on the machine to which you want to connect,
Appending to its end, if the file already exists.
E)Change the permissions of the ~/.ssh/authorized_keys file using the following command:
$ chmod 600 ~/.ssh/authorized_keys
2) Now on client side, open the remote connection agent like putty and browse  public key and try SSH to the server, we should be able to login without a password now.
# ssh server1.myserver.com
The authenticity of host ‘server1.myserver.com (192.168.44.2)’ will not be established.
RSA key fingerprint is e3:c3:89:37:4b:94:37:d7:0c:d5:6f:9a:38:62:ce:1b.
To continue connecting (yes/no)? yes
Warning: Permanently added ‘server1.myserver.com’ (RSA) to the list of known hosts.
Last login: Tue July 13 12:40:34 2014 from server2.myserver.com
3) Public key authentication can prevent brute force SSH attacks, but only if all password-based authentication methods are disabled. Once public key authentication has been confirmed to work, disable regular password authentication by editing /etc/ssh/sshd_config and set the following option to “no”.
PasswordAuthentication no

383. Explain the different Scenarios involved in TCP 3 way handshake?
Answer: The TCP three way handshake is for establishing a TCP connection.We will explain three way handshake with a simple scenario where we can assume a client computer will be contacting a server for sending it some information.
a) The client can send a packet with the SYN bit set and a sequence number of N.
b) The server can send a packet with an ACK number of N+1, the SYN bit set and a sequence number of X.
c) The client can send a packet with an ACK number of X+1 and the connection will be established.
d) The client can send the data.
The a, b, c  steps in the above process will called the three way handshake.

384. As the disk space utilization was so high in the server, the Administrator has removed few files from the server but still, the disk utilization is showing as high. What would be the reason?
Answer: In Linux,  even if we will remove a file from the mounted file system, it can still be in use by some application and for this application, it will remain available. Because file descriptor in /proc filesystem will held open..Therefore if there are such open descriptors to files already removed, space will be occupied by them considered as used. We find this difference by checking them using the “df” and “du” commands. While df will to show the file system usage, du will  report the file space usage. du will work from files while df will work at filesystem level, reporting what the kernel state it is available.
We will find all unlinked but held open files with:
# lsof | grep ‘(deleted)’
This can list the filename that is open with the pid in which it will be running. We will kill those Pids and which can stop these process and can recover the disk space responsible for this file.

385. What is sosreport, how do you generate it while working with your Redhat Support Team in production?
Answer: Sosreport is a command-line utility in Redhat based linux destros (RHEL / CentOS) that will collect system configuration and diagnostic information of  linux box such as running kernel version, loaded modules, and system and service configuration files. This command will also run external programs for collecting further information, and will store this output in the resulting archive. Sosreport will be required when we have open a case with redhat for technical support. Redhat support Engineers can needed sosreport of  server for troubleshooting purpose. To run sosreport, sos package will be installed. Sos package will be part of default installation in most of linux. If for any reason this package will not be installed , then use below yum command to install it manually:
# yum install sos
Generate the report
Open the terminal type sosreport command :
# sosreport
This command can complete within a few minutes. Depending on local configuration and the options specified in some cases the command will take longer to finish. Once completed, sosreport can generate a compressed a file under /tmp folder. The file will be provided to Redhat support representative as an attachment to open a support case.

386. What is swappiness in Linux Memory Management and how do we configure that?
Answer: The swappiness parameter will control the tendency of the kernel for moving processes out of physical memory and onto the swap disk. Because disks will be much slower than RAM, this will lead to slower response times for system and applications if processes will be too aggressively moved out of memory.
swappiness will have a value of between 0 and 100
swappiness=0 can explain the kernel for avoiding swapping processes out of physical memory for as long as possibleswappiness=100 state the kernel to aggressively swap processes out of physical memory and move them to swap cache
The default setting in Redhat/Ubuntu based Linux distros is swappiness=60. By reducing the default value of swappiness can probably improve overall performance for a typical Ubuntu desktop installation.
~$ cat /proc/sys/vm/swappiness
60
If we will have enough RAM, we will turn which is down to 10 or 15. The swap file can then only be used when the RAM usage  will be around 80 or 90 percent.
open /etc/sysctl.conf as root to change the system swappiness value. Modify or add this line to the file:
vm.swappiness = 10
Reboot for the change to take effect
We can also change the value while system is still running
sysctl vm.swappiness=10
We can also clear swap by running swapoff -a and then swapon -a as root instead of rebooting to achieve the same effect.

387. What is the difference between CTRL-C and CTRL-Z?
Answer: When we have a process in progress that will handle  prompt, there will be some signals (orders) which we will send to theses process for indicating what we required:
Control+C sends SIGINT that will interrupt the application. Usually causing to abort, but a process will be able for intercepting the signal and do whatever it likes: for instance, from  Bash prompt, try hitting Ctrl-C. In Bash, it just will cancel whatever we have typed and provides a blank prompt as opposed to quitting Bash.
Control+Z will send SIGTSTP to a foreground application, effectively put it in the background on suspended mode. This will very useful when we required the application to continue its process while we are doing another job in the current shell. When we will finish the job, we can go back into the application by running fg (or %x where x is the job number as shown in jobs).

390. How can I redirect both stderr and stdin at once?
Answer: command > file.log 2>&1 : Redirect stderr to “where stdout is currently going”. In this case, It is a file opened in append mode. The &1 will reuse the file descriptor that stdout currently uses.
command 2>&1 | tee -a file.txt

391. If you have to choose 5 commands, what will be your choices?
Answer:
1) rsync command
The rsync command will be used for synchronizing two directories or directory trees, if they are on the same or different computer. rsync will create or update the target directory to be identical to the source directory.
rsync -aH sourcedir targetdir
The -a option can preserve permissions, ownerships and symbolic (soft) links in archive mode . The -H is for preserving hard links.
2) sed command
If we required for selecting specific lines of a file, Sed command can be used.  Sed will be short for stream editor, is one way to do this. We required for combining multiple files which all had headers or to do a bulk find and replace a file.
insert a blank line above every line that will matches “regex”
$ sed ‘/regex/{x;p;x;}’
change “scarlet” or “ruby” or “puce” to “red”
$ sed ‘s/scarlet/red/g;s/ruby/red/g;s/puce/red/g’
change “scarlet” or “ruby” or “puce” to “red
3) awk command
Awk is a programming language which can  easily manipulate of structured data and the generation of formatted reports.  It will search one or more files for seeing if they will contain lines which will match with the specified patterns and then perform associated actions. It will like sed command.
Print Specific Field
$ awk -F’:’ ‘{ print $1 }’ /etc/group
$ date | awk ‘{print $2 ” ” $6}’
4) lsof command
lsof will a command line utility that will be used to list the information about the files which are opened by various processes.  By using lsof, we will get the information about any opened files.
List processes, which can open a specific file
# lsof /var/log/syslog
 Files belonging to processes owned by the user will be listed
# lsof -u username
Kill all process which will belong to a particular user
# kill -9 `lsof -t -u username
All network connection are listed
# lsof -i|
List all network files in use by a specific process
# lsof -i -a -c ssh
List processes which will be listening on a particular port
# lsof -i :25
5) grep command
It is a command used for searching text. it can search the provided file for lines containing a match to the  strings or words. By default, grep will display the matching lines.
print network connection used by firefox
# netstat -pltnu | grep firefox
print the line which will contain “root” on /etc/passwd file
# cat /etc/passwd | grep root

392. What is the difference between name based virtual hosting and IP based virtual hosting?
Answer: It can be used to host multiple domains on a single apache instance. We will have one virtual host for each IP your server has, or the same IP but different ports, or the same IP, the same port but different host names. The latter will be called “name based vhosts”.
We will run more than one web site on the same server machine in n IP-based virtual hosting but each web site has its own IP address.  We will host multiple websites on the same IP address in Name-based virtual hosting. We have to keep more than one DNS record for IP address in the DNS database.

393. Describe briefly the procedure for re-installing Grub in Linux.
Answer: Following is the procedure to re-install Grub in Linux:
1.Download Ubuntu Installation / Live cd
2. Boot from Ubuntu Installation / Live cd – usb, burned cd etc.
3. While Booting select “Try Ubuntu”. Don’t select install.
4. Mount  Linux root partition
sudo mount /dev/sda6 /mnt ( Assuming /dev/sda6 is the Linux root partition)
5. Install / reinstall grub
$ sudo grub-install –root-directory=/mnt/ /dev/sda ( where /dev/sda is your primary disk)
Installation finished. No error reported.
6. Reboot  system, remove bootable CD and we should keep the boot menu ready when the system starts.



395. You are in a directory /home/user/downloaded/ and you want to share the files in this directory quickly over web without configuring an httpd server so how can you do it with python?
Answer: The Python script language will allow a quick httpd service which is called SimpleHTTPServer using which we will share the local directory we are using the command, for example
python -m SimpleHTTPServer

396. While running a command interactively so how do you send the command into background?
Answer: Click Ctrl+Z to send a command to the background, it sends  to the command line and pause the application, then type bg to send that command to background.

397. How can you compile a regular c application “myprog.c” and create a binary “myprog”?
Answer: The most common way to compile is with the “gcc” compiler, and to compile a c file to a binary file we run
gcc myprog.c -o myprog

398. What is BASH?
Answer: BASH is short for Bourne Again SHell. It is written by Steve Bourne as a replacement to the original Bourne Shell Which is represented by /bin/sh.  It will combine all the features from the original version of Bourne Shell, plus additional functions for making it easier and more convenient to use. 

399.What is Linux Kernel?
Answer: The Linux Kernel is a low-level systems software which will manage hardware resources for the user. It will be also used for providing an interface for user-level interaction.

400. What is the export command used for?
Answer: The export command can be used to set and reload the environment variables. For example, if we want to set the Java path, then the command would be:
$ export JAVA_HOME = /home/user/Java/bin

401. How do you check if a particular service in running?
Answer: $ service <servicename> status.