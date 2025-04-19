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
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="iponfig">5 IPCONFIG: display the IP configuration</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ping">6 PING: check latency and connectivity</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="netstat">7 NETSTAT: display network connections</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="netuse">8 NET USE: create or delete Windows user accounts</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="netuse2">9 NET USE: create a network drive</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="sfc">10 SFC: check and repair system files</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="shutdown">11 SHUTDOWN: shutting down your PC with CMD</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="systeminfo">12 SYSTEMINFO: display system information</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="tasklist">13 TASKLIST: list the processes</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="taskkill">14 TASKKILL: kill a process</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="tracert">15 TRACERT: do a traceroute</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="xcopy">16 XCOPY: copy files in command prompt</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

