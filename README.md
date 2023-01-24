<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Azure Virtual Machine Windows 10, 4 vCPUs
- IIS in Windows WITH CGI
- PHP Manager for IIS
- Rewrite Module
- PHP 7.3.8
- VC_redist.x86.exe
- MySQL 5.5.62
- osTicket v1.15.8
- HeidiSQL.



<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/iCfYqXM.png" height="100%" width="100%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create an Azure Virtual Machine,Name: Vm-osticket
Username: labuser (for example/whatever you chose)
Password: osTicketPassword1! (for example/whatever you chose)
open Vm-osticket in Remot Desdtop RDP.
Install / Enable IIS in Windows WITH CGI
World Wide Web Services -> Application Development Features -> [X] CGI
as shown above.
</p>
<br />

<p>
<img src="https://i.imgur.com/n4byQoF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
download and install PHP Manager for IIS (PHPManagerForIIS_V1.5.0.msi)
download and install the Rewrite Module (rewrite_amd64_en-US.msi)
Create the directory C:\PHP
download PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip) and unzip the contents into C:\PHP
download and install VC_redist.x86.exe.
download and install MySQL 5.5.62 (mysql-5.5.62-win32.msi)
Typical Setup ->
Launch Configuration Wizard (after install) ->
Standard Configuration ->
Password1
as shown above
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
