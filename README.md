<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Item 1
- Item 2
- Item 3
- Item 4
- Item 5

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/ZgNMxPP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Created an Azure Virtual Machine Windows 10, 4 vCPUs

</p>
<br />

<p>
<img src="https://i.imgur.com/VZwuhRZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Downloaded osTicket-Installation-Files.zip and unzipped it.
</p>
<br />

<p>
<img src="https://i.imgur.com/nAERF28.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Enabled IIS in Windows WITH CGI (World Wide Web Services -> Application Development Features -> [X] CGI)
</p>
<br />

<p>
<img src="https://i.imgur.com/I5QbuD6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
From the “osTicket-Installation-Files” folder, I installed PHP Manager for IIS (PHPManagerForIIS_V1.5.0.msi)
</p>
<br />

<p>
<img src="https://i.imgur.com/0jcZPbV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
From the “osTicket-Installation-Files” folder, I installed the Rewrite Module (rewrite_amd64_en-US.msi)
</p>
<br />

<p>
<img src="https://i.imgur.com/tJ2ZwNs.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
I created the directory C:\PHP, and from the “osTicket-Installation-Files” folder, I unzipped PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip) into the “C:\PHP” folder
</p>
<br />

<p>
<img src="https://i.imgur.com/O2nRFQ7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
From the “osTicket-Installation-Files” folder, I installed VC_redist.x86.exe.
</p>
<br />

<p>
<img src="https://i.imgur.com/Ufins8y.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
From the “osTicket-Installation-Files” folder, I installed MySQL 5.5.62 (mysql-5.5.62-win32.msi)
</p>
<br />

<p>
<img src="https://i.imgur.com/zD6xK4T.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After the installation, the MySQL Server Configuration Wizard Launched, which eventually prompted me to set the security settings. I set both the username and password as "root".
</p>
<br />

<p>
<img src="https://i.imgur.com/AxvD8v7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
I then opened IIS as an Admin & Registered PHP from within IIS (PHP Manager -> C:\PHP\php-cgi.exe)
</p>
<br />

<p>
<img src="https://i.imgur.com/CT8uXtT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After that, I reloaded IIS (Opened IIS, Stopped and Started the server)
</p>
<br />

<p>
<img src="https://i.imgur.com/q8UfKyw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Installed osTicket v1.15.8. From the “osTicket-Installation-Files” folder, I unzipped “osTicket-v1.15.8.zip” and copied the “upload” folder into “c:\inetpub\wwwroot”. Within “c:\inetpub\wwwroot”, I renamed “upload” to “osTicket”
</p>
<br />

<p>
<img src="https://i.imgur.com/Sg2y300.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
I went to Sites -> Default -> osTicket on the IIS Manager. On the right, I clicked “Browse *:80 (http)” to launch the osTicket setup page.
</p>
<br />

<p>
<img src="https://i.imgur.com/OPPvufd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Went back to IIS, sites -> Default -> osTicket. Double-clicked PHP Manager. Clicked “Enable or disable an extension” and enabled: php_imap.dll & php_intl.dll
</p>
<br />

<p>
<img src="https://i.imgur.com/B9TtCak.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Renamed: ost-config.php. From: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php. To: C:\inetpub\wwwroot\osTicket\include\ost-config.php
</p>
<br />

<p>
<img src="https://i.imgur.com/MZvEBiV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Assigned Permissions for ost-config.php. Disabled inheritance -> Remove All. New Permissions -> Everyone -> All

</p>
<br />

<p>
<img src="https://i.imgur.com/2N5NEOb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Continued Setting up osTicket in the browser
</p>
<br />

<p>
<img src="https://i.imgur.com/aWJlzud.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
From the “osTicket-Installation-Files” folder, I installed HeidiSQL.
</p>
<br />

<p>
<img src="https://i.imgur.com/aZ0giQu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Opened Heidi SQL. Created a new session and entered the user and password "root". Connected to the session.
</p>
<br />

<p>
<img src="https://i.imgur.com/prd9uVw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Created a database called “osTicket”
</p>
<br />

<p>
<img src="https://i.imgur.com/t8pmS1N.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
I continued Setting up osTicket in the browser. I set up the MySQL Database as "osTicket", the MySQL Username as "root" & the MySQL Password as "root". I then clicked “Install Now!”

</p>
<br />

<p>
<img src="https://i.imgur.com/r7KX7t3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
osTicket is Installed!
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
<br />

