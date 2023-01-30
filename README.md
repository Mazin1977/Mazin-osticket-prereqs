<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com/watch?v=K7T_JjvEamg)

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
<img src="https://i.imgur.com/pn8rGd9.png" height="100%" width="100%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create an Azure Virtual Machine,Name: Vm-osticket,
Username: labuser (for example/whatever you chose),
Password: osTicketPassword1! (for example/whatever you chose),
Open Vm-osticket in Remot Desdtop RDP.
Install / Enable IIS in Windows WITH CGI,
World Wide Web Services -> Application Development Features -> [X] CGI,
as shown above.
</p>
<br />

<p>
<img src="https://i.imgur.com/8xVdH9T.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download and install PHP Manager for IIS (PHPManagerForIIS_V1.5.0.msi),
Download and install the Rewrite Module (rewrite_amd64_en-US.msi) as shown above.

</p>
<br />
<p>
<img src="https://i.imgur.com/FT6hoJn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create the directory C:\PHP,
Download PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip) and unzip the contents into C:\PHP,
Download and install VC_redist.x86.exe. as shown above.
</p>
<br />
<p>
<img src="https://i.imgur.com/JXyYx38.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Download and install MySQL 5.5.62 (mysql-5.5.62-win32.msi),
Typical Setup ->,
Launch Configuration Wizard (after install) ->,
Standard Configuration ->,
Password1,
as shown above,
Open IIS as an Admin.
Register PHP from within IIS as shown above.
Reload IIS (Open IIS, Stop and Start the server)
</p>
<br />
<p>
<img src="https://i.imgur.com/O0X2RrM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Install osTicket v1.15.8,
Download osTicket from the Installation Files Folder,
Extract and copy “upload” folder to c:\inetpub\wwwroot,
Within c:\inetpub\wwwroot, Rename “upload” to “osTicket”,
Reload IIS (Open IIS, Stop and Start the server),
Go to sites -> Default -> osTicket,
On the right, click “Browse *:80”
Note as shown above that some extensions are not enabled
Go back to IIS, sites -> Default -> osTicket,
Double-click PHP Manager,
Click “Enable or disable an extension”,
Enable: php_imap.dll,
Enable: php_intl.dll,
Enable: php_opcache.dll,
Refresh the osTicket site in your browse, observe the changes,
Rename: ost-config.php,
From: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php,
To: C:\inetpub\wwwroot\osTicket\include\ost-config.php,
Assign Permissions: ost-config.php,
Disable inheritance -> Remove All,
New Permissions -> Everyone -> All,
Continue Setting up osTicket in the browser (click Continue),
Name Helpdesk,
Default email (receives email from customers),
download and install HeidiSQL.
Open Heidi SQL,
Create a new session, root/Password1,
Connect to the session,
Create a database called “osTicket”,
Continue Setting up osticket in the browser,
MySQL Database: osTicket,
MySQL Username: root,
MySQL Password: Password1,
Click “Install Now!”..
Congratulations, hopefully it is installed with no errors!

</p>
