---
Filename: 16-Useful-Windows-Commands
Date Created: 		12/10/2024 @9:22pm
Date Last Editted: 	12/10/2024
---

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~ readme.md of 16-useful-windows-commands ~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p>Windows Command Prompt is full of useful commands. In this article, we gave the main 
ones: List of Windows Command Prompt (CMD) commands.</p>

<p>There are some things you can only do from the command line, even in Windows.</p>

<p>Indeed some tools do not have graphical equivalents, while others are simply faster 
to use than their graphical interfaces.</p>

<p>Some CMD commands are so useful and easy to use that even regular users see the Windows 
Command Prompt as a key part of the operating system.</p>

<p>Here are 16 of the best CMD commands you should know if you want to have more control 
over your Windows PC.</p>

<h3 id="toc">Contents</h3>

<h2 id="cmds">16 Useful Windows Commands (CMDs) You Should Know;</h2>
<ol>
  <li>ATTRIB: change the attributes of a file</li>
  <li>ASSOC: display file associations</li>
  <li>DRIVERQUERY: list the Windows drivers</li>
  <li>FC: compare two text files</li>
  <li>IPCONFIG: display the IP configuration</li>
  <li>PING: check latency and connectivity</li>
  <li>NETSTAT: display network connections</li>
  <li>NET USE: create or delete Windows user accounts</li>
  <li>NET USE: create a network drive</li>
  <li>SFC: check and repair system files</li>
  <li>SHUTDOWN: shutting down your PC with CMD</li>
  <li>SYSTEMINFO: display system information</li>
  <li>TASKLIST: list the processes</li>
  <li>TASKKILL: kill a process</li>
  <li>TRACERT: do a traceroute</li>
  <li>XCOPY: copy files in command prompt</li>
</ol>

<p>As a reminder, there is a full article that gives you all the methods to access the Command Prompt.</p>

<p>More information:</p>

<p>6 methods to open Command Prompt on Windows 10;</p>

<p>From there, you can use the helpful commands provided in this article.</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="attrib">1. ATTRIB: change the attributes of a file</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p>The first CMD command we present is Attrib.</p>

<p>This gives the possibility to display or modify the attributes of a file.</p>

<p>For example to remove the reader attribute alone or hidden from a file.</p>

<p>Here we use -R to remove the read-only attribute and -H for hidden;</p>
<pre>
attrib -R -H fname.ext
</pre>

<p>The + on the contrary allows to add the attribute to the file;</p>
<pre>
attrib +R +H fname.ext
</pre>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="assoc">2. ASSOC: For the list of attributes and more example attribute usage, follow this article:</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p>File attributes on Windows: view and modify file attributes;</p>

<pre>
ASSOC: show file associations
</pre>

<p>Next is the ASSOC command that can be used in the command prompt.</p>
<p>It allows you to list the file associations.</p>
 
<p>Finally ASSOC is also able to modify file associations.</p>
<p>For example to change the file association on the .doc extension</p>
<pre>
assoc .doc=Word.Document.8
</pre>
<p>For more information on these, read:</p>

<p>File associations and file extensions on Windows.</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="driverquery">3. DRIVERQUERY: list the Windows drivers</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p>The driverquery command generates a list of all hardware drivers installed in Windows.</p>

<p>It generates a report of installed drivers that you can save for later reference or to 
find the version number of a currently installed driver so that you can make a better 
decision if you plan to update.</p>

<p>Here are some options and settings:</p>

<h4>DRIVERQUERY: list the Windows drivers.</h4>

<p>The driverquery command generates a list of all hardware drivers installed in Windows.
It generates a report of installed drivers that you can save for later reference or to 
find the version number of a currently installed driver so that you can make a better 
decision if you plan to update.</p>

<p>Here are some options and settings:</p>

<ul>
  <li>/ s - This option allows you to specify the name or IP address of a remote computer in 
  order to find the drivers it has installed.</li>
  <li>/ si - This option shows you the digital signature information for the drivers.</li>
  <li>/ fo - This is really the key option that you will be using with driverquery. It allows 
  you to specify the format in which the information is displayed so that you can save 
  it more efficiently as a report. After typing / fo, add one of the following options: 
  TABLE (the default view), LIST (which lists each driver with all of its information 
  one after the other), and CSV (which displays the data as comma separated values).</li>
</ul>
<pre>
driverquery /fo CSV \> drivers.csv
</pre>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="fc">4 FC: compare two text files</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p>Now you will need to open up an elevated command prompt window. Open the start menu in 
Windows 7 and 10 or open the search function in Windows 8 and search for CMD.  Next, 
right-click on it and then press $ Run as administrator. While you don't need to open an 
elevated command prompt window, it will help you to avoid any pesky confirmation dialog 
boxes.</p>

<p>There is a great command line tool that can be used to compare files to see if there are 
any content or binary code differences that you can access if you are using a PC. File 
Compare or FC as we will refer to is from here on out, is a simple program that will 
compare the contents of text or binary files and is capable of comparing both ASCII and 
Unicode text. You can use this tool to display any lines from two files or two sets of 
files that do not match up with the others.</p>

<ul>
  <li>/B – This switch will perform a binary comparison.</li>
  <li>/C – If you need to do a case insensitive comparison, use this switch.</li>
  <li>/A – This switch will make FC show only the first and last lines for each group of differences.</li>
  <li>/U – Use this switch to compare files as Unicode text files.</li>
  <li>/L – This will compare your files as ASCII text.</li>
  <li>/N – This switch can only be used with ASCII but it will show all the corresponding line numbers.</li>
  <li>/LBn – Replace the “n” with a number to limit the amount of consecutive different lines that FC will read before it will abort. The default, if you do not specify a number is 100 lines of mismatched text.</li>
  <li>/nnnn – Replacing the “n’s” here will tell FC that when it finds mismatched lines, it can only continue if it finds “n” consecutive matching lines after the mismatch. This is useful if you want to prevent two files from becoming extremely out of sync.</li>
  <li>/T – This switch will tell FC not to expand tabs to spaces.</li>
  <li>/W – If you use this switch, FC will compress white space (tabs and spaces) during its comparison of your files.</li>
</ul>
<pre>
FC [pathname1] [pathname2]
FC [switches] [pathname1] [pathname2]
</pre>

<p>Depending on your command, you will receive one of four %errorlevel% responses.</p>
<ul>
  <li>-1 – Your syntax is incorrect.</li>
  <li>0 – Both files are identical.</li>
  <li>1 – The files are different.</li>
  <li>2 – At least one of the files can’t be found.</li>
</ul>




<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="iponfig">5 IPCONFIG: display the IP configuration</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ping">6 PING: check latency and connectivity</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="netstat">7 NETSTAT: display network connections</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="netuse">8 NET USE: create or delete Windows user accounts</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="netuse2">9 NET USE: create a network drive</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="sfc">10 SFC: check and repair system files</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="shutdown">11 SHUTDOWN: shutting down your PC with CMD</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="systeminfo">12 SYSTEMINFO: display system information</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="tasklist">13 TASKLIST: list the processes</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="taskkill">14 TASKKILL: kill a process</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="tracert">15 TRACERT: do a traceroute</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="xcopy">16 XCOPY: copy files in command prompt</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
Why are MS-Dos Commands used?
File Management: MS-Dos commands enable users to navigate through directories and create, delete, or copy files, enabling efficient file management.
System Configuration: Users can configure system settings, manage drives, and analyze hardware issues using MS Dos commands, providing a robust toolkit for system customization.
Program Execution: MS-Dos for commands facilitate the execution of programs and scripts, offering a streamlined approach to launching applications without the need for graphical interfaces.
List of MS-Dos Commands
Here's a table of some of the essential and commonly used commands MS-Dos for Commands for quick reference:

| Command | Syntax            | Description                                            |
|---------|-------------------|--------------------------------------------------------|
| CD      | CD [drive:][path] | Changes the current directory to the specified folder. |
| DIR     | DIR [drive:][path] | Displays a list of files and subdirectories in a directory. |
| COPY | COPY [source] [destination] | Copies files from one location to another. |
| DEL | DEL [drive:][path]  | Deletes one or more files. |
| REN | REN [drive:][path][filename1] [filename2]  | Renames a file or directory.  |
| MKDIR | MKDIR [drive:][path]  | Creates a new directory. |
| RMDIR | RMDIR [drive:][path]  | Removes an existing directory. |
| TYPE | TYPE [drive:][path] filename | Displays the contents of a text file. |
| EDIT | EDIT [drive:][path]filename  | Opens the MS-DOS text editor for editing a specified file. |
| CHKDSK | CHKDSK [volume:][[path]filename] [/F] [/V] [/R] [/X] [/I] [/C] [/L[:size]] [/B] | Scans and fixes errors on a disk. |
| FORMAT | FORMAT volume [/FS:file-system] [/V:label] [/Q] [/L[:size]] [/A:size] [/C] [/X] | Prepares a storage medium for data storage. |
| XCOPY | XCOPY [source] [destination] [/E] [/C] [/H] [/R] [/Y] | Copies files and directories, including subdirectories. |
| TREE | TREE [drive:][path] | Graphically displays the folder structure of a drive or path. |
| DATE | DATE [MM-DD-YYYY]  | Displays or sets the system date. |
| TIME | TIME [HH: MM: SS] | Displays or sets the system time. |
| HELP | HELP [command]  | Provides help information for MS-DOS commands. |
| EXIT | EXIT | Exits the MS-DOS command prompt or a batch file.
| ATTRIB | ATTRIB [+ R &vert; -R] [+A &vert; -A] [+H &vert; -H] [+S &vert; -S] [d:][path]filename [/S]  | Sets or clears file attributes (Read-Only, Archive, System, Hidden), managing file visibility and access in MS-DOS. |
| MODE | MODE [device] [BAUD=b] [PARITY=p] [DATA=d] [STOP=s]  | Configures system devices. |
| DISKCOPY | DISKCOPY [drive1:][path1][filename1] [drive2:][path2][filename2] | Copies the contents of one disk to another. |
| MEM |  MEM[/program|/debug &vert; /classify &vert; /free &vert; /module(name)] [/page] | Displays the amount of used and free memory in the system. |
| SCANDISK | SCANDISK [/SURFACE] [/AUTOFIX] [/CHECKONLY]  | Scans and fixes disk errors. |
| UNDELETE | UNDELETE [drive:][path][filename]   | Restores a deleted file. |
| ASSIGN | ASSIGN [drive1:=[drive2:]] | Redirects requests for drive letters to a different drive.  |
| FDISK | FDISK | Manages disk partitions. |
| BACKUP | BACKUP [source] [destination] [/S]  | Backs up files and directories. |
| RESTORE | RESTORE [source] [destination] [/S] | Restores files and directories from a backup. |
| MSCDEX | MSCDEX [/D: driver /L:drive] [/M:bufsize] [/E /S /V]   | Provides CD-ROM access. |
| SYS | SYS [drive1:][path]   | Transfers system files to a disk. |
| SHARE | SHARE [/F:(space)] [/L:(locks)] | Installs file-sharing and locking capabilities. |
| SMARTDRV | SMARTDRV [size] [/E /V] [/C] [/L:size]  | Disk caching utility. |
| SETVER | SETVER [drive:][path]filename [/B:bytes]  | Sets the MS-DOS version number for a program. |
| ASSIGN | ASSIGN [/D]  | Disables automatic drive-letter assignments. |
| FASTHELP | FASTHELP [command] [command] /?   | Provides a quick overview of MS-DOS commands. |
| FC | FC [/A] [/C] [/L] [/LBn] [/N] [/OFF[LINE]] [/T]   | Compares two files or sets of files and displays the differences between them. |
| FIND | FIND [/V] [/C] [/N] [/I] [/OFF[LINE]] "string" [[drive:][path]filename[ ...]]   | Searches for a text string in files. |
| MORE | MORE [filename]   | Display the content of a text file one screen at a time |
| ECHO | ECHO [on/off]   | This command can either show or hide the text of the commands you type. Command echoing is on by default |
| ECHO | ECHO [<message>]  | Specifies the text to display on the screen. |
| PATH | PATH [[drive:][path] [;...]]   | Displays or sets a search path for executable files. |
| SET | SET [variable=[string]]  | Sets or displays environment variables. |
| VOL | VOL [drive:]  | Displays a disk label and serial number. |
| SUBST | SUBST [drive1: [drive2:]path] | Associates a path with a drive letter. |
| EDLIN  | EDLIN [drive:][path][filename] | Edits text files. |
| DEBUG | DEBUG [drive:][path][filename]  | Starts the Debug program for testing and debugging assembly-language programs. |
| HIMEM.SYS | HIMEM.SYS [/TESTMEM:off] [/HMAMIN=amount]  | Provides upper memory block (UMB) and high memory area (HMA) support. |
| UNFORMAT | UNFORMAT [drive:][path]   | Restores a formatted disk. |
| GRAPHICS | GRAPHICS [type] [[drive:][path]filename] [/R] [/B] [/LCD][/PRINTBOX:STD &vert; /PRINTBOX:LCD]  | Enables output of graphical screen content to print |
| QBASIC | QBASIC [drive:][path]  | Starts the MS-DOS-based application for creating and running BASIC programs. |
| KEYB | KEYB [/CODEPAGE=page[,country]] [/E]  | Configures a keyboard for a specific language. |
| CHOICE | CHOICE [/C:choices] [/N] [/S] [/T:c,nn]  | Provides a prompt with a list of choices. |
| DISKCOMP | DISKCOMP [drive1:][drive2:]  | Compares the contents of two floppy disks. |
| PRINT | PRINT [/D:device] [filename] | Sends a text file to a printer. |
| SORT | SORT [drive:][path][filename]   | Sorts the contents of a text file. |
| APPEND | APPEND [[drive:]path[;...]]  | Sets or displays the search path for data files. |
| ASSOC | ASSOC [.ext[=[fileType]]]   | Associates file extension with a file type. |
| LABEL | LABEL [drive:][label]  | Creates, changes, or deletes the volume label of a disk. |
| RECOVER | RECOVER [drive:][path][filename]   | Recovers readable information from a bad or defective disk.  |
| FASTOPEN | FASTOPEN [/X] [drive:] [path] [/R]   | Speeds up the opening of files. |
| GOTO | GOTO <label>   | Directs the command interpreter to a labeled line in a batch program. |
| SHIFT | SHIFT [/n <N>]   | Shifts the position of batch parameters in a batch file. |
| JOIN | JOIN path [drive:] | Joins a drive letter and directory path. |
| SMARTDRV | SMARTDRV [size] [buffers] [doublebuffer] [/E] [/C] [/L] [/V] [/B]   | Manages and optimizes disk caching. |
| BATCH | BATCH [filename] | Executes the commands specified in a batch file. |
| CALL | CALL [drive:][path]filename [batch-parameters]  | Calls one batch program from another. |

