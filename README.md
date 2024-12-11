---
Filename: 16-Useful-Windows-Commands
Date Created: 		12/10/2024 @9:22pm
Date Last Editted: 	12/10/2024
---

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~ readme.md of 16-useful-windows-commands ~~~~~~~~~~~~~~~~~~~~~~~~~~-->

Windows Command Prompt is full of useful commands. In this article, we gave the main 
ones: List of Windows Command Prompt (CMD) commands.

There are some things you can only do from the command line, even in Windows.

Indeed some tools do not have graphical equivalents, while others are simply faster 
to use than their graphical interfaces.

Some CMD commands are so useful and easy to use that even regular users see the Windows 
Command Prompt as a key part of the operating system.

Here are 16 of the best CMD commands you should know if you want to have more control 
over your Windows PC.

### Contents

## 16 Useful Windows Commands (CMDs) You Should Know;

	1 ATTRIB: change the attributes of a file
	2 ASSOC: display file associations
	3 DRIVERQUERY: list the Windows drivers
	4 FC: compare two text files
	5 IPCONFIG: display the IP configuration
	6 PING: check latency and connectivity
	7 NETSTAT: display network connections
	8 NET USE: create or delete Windows user accounts
	9 NET USE: create a network drive
	10 SFC: check and repair system files
	11 SHUTDOWN: shutting down your PC with CMD
	12 SYSTEMINFO: display system information
	13 TASKLIST: list the processes
	14 TASKKILL: kill a process
	15 TRACERT: do a traceroute
	16 XCOPY: copy files in command prompt
	
As a reminder, there is a full article that gives you all the methods to access the Command Prompt.

More information:

6 methods to open Command Prompt on Windows 10;

From there, you can use the helpful commands provided in this article.
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
### 1. ATTRIB: change the attributes of a file
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
The first CMD command we present is Attrib.

This gives the possibility to display or modify the attributes of a file.

For example to remove the reader attribute alone or hidden from a file.

Here we use -R to remove the read-only attribute and -H for hidden;
```
attrib -R -H fname.ext
```

The + on the contrary allows to add the attribute to the file;
```
attrib +R +H fname.ext
```

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
### 2. ASSOC: For the list of attributes and more example attribute usage, follow this article:
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

File attributes on Windows: view and modify file attributes;
```
ASSOC: show file associations
```
Next is the ASSOC command that can be used in the command prompt.
It allows you to list the file associations.
 
Finally ASSOC is also able to modify file associations.
For example to change the file association on the .doc extension
```
assoc .doc=Word.Document.8
```
For more information on these, read:

File associations and file extensions on Windows
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
### 3. DRIVERQUERY: list the Windows drivers
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
The driverquery command generates a list of all hardware drivers installed in Windows.

It generates a report of installed drivers that you can save for later reference or to 
find the version number of a currently installed driver so that you can make a better 
decision if you plan to update.

Here are some options and settings:

DRIVERQUERY: list the Windows drivers.

The driverquery command generates a list of all hardware drivers installed in Windows.
It generates a report of installed drivers that you can save for later reference or to 
find the version number of a currently installed driver so that you can make a better 
decision if you plan to update.

Here are some options and settings:

	/ s - This option allows you to specify the name or IP address of a remote computer in 
  order to find the drivers it has installed.
	/ si - This option shows you the digital signature information for the drivers.
	/ fo - This is really the key option that you will be using with driverquery. It allows 
  you to specify the format in which the information is displayed so that you can save 
  it more efficiently as a report. After typing / fo, add one of the following options: 
  TABLE (the default view), LIST (which lists each driver with all of its information 
  one after the other), and CSV (which displays the data as comma separated values).

driverquery /fo CSV \> drivers.csv

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
### 4 FC: compare two text files
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->


<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
### 5 IPCONFIG: display the IP configuration
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
### 6 PING: check latency and connectivity
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
### 7 NETSTAT: display network connections
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
### 8 NET USE: create or delete Windows user accounts
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
### 9 NET USE: create a network drive
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
### 10 SFC: check and repair system files
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
### 11 SHUTDOWN: shutting down your PC with CMD
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
### 12 SYSTEMINFO: display system information
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
### 13 TASKLIST: list the processes
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
### 14 TASKKILL: kill a process
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
### 15 TRACERT: do a traceroute
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
### 16 XCOPY: copy files in command prompt
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

