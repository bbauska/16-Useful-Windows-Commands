# 16-Useful-Windows-Commands
16 Useful Windows Commands

16 Useful Windows Commands (CMDs) You Should Know
1.1 ATTRIB: change the attributes of a file
1.2 ASSOC: display file associations
1.3 DRIVERQUERY: list the Windows drivers
Home
Windows 10
General
16 Useful CMD Commands You Should Know
16 USEFUL CMD COMMANDS YOU SHOULD KNOW
 Initial article: March 31, 2020
Last modification: March 31, 2020
 General , Windows 10
Windows Command Prompt is full of useful commands .
In this article, we gave the main ones: List of Windows Command Prompt (CMD) commands .
There are some things you can only do from the command line , even in Windows.
Indeed some tools do not have graphical equivalents, while others are simply faster to use than their graphical interfaces.
Some CMD commands are so useful and easy to use that even regular users see the Windows Command Prompt as a key part of the operating system.
Here are 16 of the best CMD commands you should know if you want to have more control over your Windows PC.
 
Contents
•	1 16 Useful Windows Commands (CMDs) You Should Know
o	1.1 ATTRIB: change the attributes of a file
o	1.2 ASSOC: display file associations
o	1.3 DRIVERQUERY: list the Windows drivers
o	1.4 FC: compare two text files
o	1.5 IPCONFIG: display the IP configuration
o	1.6 PING: check latency and connectivity
o	1.7 NETSTAT: display network connections
o	1.8 NET USE: create or delete Windows user accounts
o	1.9 NET USE: create a network drive
o	1.10 SFC: check and repair system files
o	1.11 SHUTDOWN: shutting down your PC with CMD
o	1.12 SYSTEMINFO: display system information
o	1.13 TASKLIST: list the processes
o	1.14 TASKKILL: kill a process
o	1.15 TRACERT: do a traceroute
o	1.16 XCOPY: copy files in command prompt
•	2 Links
•	3 Find the solution on the help forum
16 USEFUL WINDOWS COMMANDS (CMDS) YOU SHOULD KNOW
As a reminder, there is a full article that gives you all the methods to access the Command Prompt.
More information :
6 methods to open Command Prompt on Windows 10
From there, you can use the helpful commands provided in this article.
These useful CMD commands are available on Windows 7, 8, and 10.
ATTRIB: change the attributes of a file
The first CMD command we present is Attrib.
This gives the possibility to display or modify the attributes of a file .
For example to remove the reader attribute alone or hidden from a file.
Here we use -R to remove the read-only attribute and -H for hidden.
attrib -R -H nomdufichier
The + on the contrary allows to add the attribute to the file
attrib +R +H nomdufichier
For the list of attributes and more example attribute usage, follow this article:
File attributes on Windows: view and modify file attributes
ASSOC: show file associations
Next is the ASSOC command that can be used in the command prompt.
It allows you to list the file associations.
 
Finally ASSOC is also able to modify file associations.
For example to change the file association on the .doc extension
assoc .doc=Word.Document.8
For more information on these, read:
File associations and file extensions on Windows
DRIVERQUERY: list the Windows drivers
The driverquery command generates a list of all hardware drivers installed in Windows .
It generates a report of installed drivers that you can save for later reference or to find the version number of a currently installed driver so that you can make a better decision if you plan to update .
Here are some options and settings:
Home
Windows 10
General
16 Useful CMD Commands You Should Know
16 USEFUL CMD COMMANDS YOU SHOULD KNOW
 Initial article: March 31, 2020
Last modification: March 31, 2020
 General , Windows 10
Windows Command Prompt is full of useful commands .
In this article, we gave the main ones: List of Windows Command Prompt (CMD) commands .
There are some things you can only do from the command line , even in Windows.
Indeed some tools do not have graphical equivalents, while others are simply faster to use than their graphical interfaces.
Some CMD commands are so useful and easy to use that even regular users see the Windows Command Prompt as a key part of the operating system.
Here are 16 of the best CMD commands you should know if you want to have more control over your Windows PC.
 
Contents
•	1 16 Useful Windows Commands (CMDs) You Should Know
o	1.1 ATTRIB: change the attributes of a file
o	1.2 ASSOC: display file associations
o	1.3 DRIVERQUERY: list the Windows drivers
o	1.4 FC: compare two text files
o	1.5 IPCONFIG: display the IP configuration
o	1.6 PING: check latency and connectivity
o	1.7 NETSTAT: display network connections
o	1.8 NET USE: create or delete Windows user accounts
o	1.9 NET USE: create a network drive
o	1.10 SFC: check and repair system files
o	1.11 SHUTDOWN: shutting down your PC with CMD
o	1.12 SYSTEMINFO: display system information
o	1.13 TASKLIST: list the processes
o	1.14 TASKKILL: kill a process
o	1.15 TRACERT: do a traceroute
o	1.16 XCOPY: copy files in command prompt
•	2 Links
•	3 Find the solution on the help forum
16 USEFUL WINDOWS COMMANDS (CMDS) YOU SHOULD KNOW
As a reminder, there is a full article that gives you all the methods to access the Command Prompt.
More information :
6 methods to open Command Prompt on Windows 10
From there, you can use the helpful commands provided in this article.
These useful CMD commands are available on Windows 7, 8, and 10.
ATTRIB: change the attributes of a file
The first CMD command we present is Attrib.
This gives the possibility to display or modify the attributes of a file .
For example to remove the reader attribute alone or hidden from a file.
Here we use -R to remove the read-only attribute and -H for hidden.
attrib -R -H nomdufichier
The + on the contrary allows to add the attribute to the file
attrib +R +H nomdufichier
For the list of attributes and more example attribute usage, follow this article:
File attributes on Windows: view and modify file attributes
ASSOC: show file associations
Next is the ASSOC command that can be used in the command prompt.
It allows you to list the file associations.

DRIVERQUERY: list the Windows drivers
The driverquery command generates a list of all hardware drivers installed in Windows .
It generates a report of installed drivers that you can save for later reference or to find the version number of a currently installed driver so that you can make a better decision if you plan to update .
Here are some options and settings:
	/ s This option allows you to specify the name or IP address of a remote computer in order to find the drivers it has installed.
	/ si This option shows you the digital signature information for the drivers.
	/ fo This is really the key option that you will be using with driverquery . It allows you to specify the format in which the information is displayed so that you can save it more efficiently as a report. After typing / fo, add one of the following options: TABLE (the default view), LIST (which lists each driver with all of its information one after the other), and CSV (which displays the data as comma separated values).
driverquery /fo CSV > drivers.csv

1.4 FC: compare two text files
1.5 IPCONFIG: display the IP configuration
1.6 PING: check latency and connectivity
1.7 NETSTAT: display network connections
1.8 NET USE: create or delete Windows user accounts
1.9 NET USE: create a network drive
1.10 SFC: check and repair system files
1.11 SHUTDOWN: shutting down your PC with CMD
1.12 SYSTEMINFO: display system information
1.13 TASKLIST: list the processes
1.14 TASKKILL: kill a process
1.15 TRACERT: do a traceroute
1.16 XCOPY: copy files in command prompt
2 Links
3 Find the solution on the help forum
