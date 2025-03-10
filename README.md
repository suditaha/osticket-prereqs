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
<img src="https://i.imgur.com/AxvD8v7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Opened IIS as an Admin & Registered PHP from within IIS (PHP Manager -> C:\PHP\php-cgi.exe)
</p>
<br />

<p>
<img src="https://i.imgur.com/CT8uXtT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Reloaded IIS (Opened IIS, Stopped and Started the server)
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

