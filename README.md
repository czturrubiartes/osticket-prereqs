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

- Create Virtual Machine in Azure
- Create a Resource Group
- Install / Enable IIS in Windows WITH
CGI and Common HTTP Features
- download and install PHP Manager for IIS
- download and install the Rewrite Module
- Download PHP 7.3.8
- download and install VC_redist.x86.exe.
- download and install MySQL 5.5.62

<h2>Installation Steps</h2>

<p>
<img src="https://cdn.shopify.com/s/files/1/0285/1815/4285/files/D0Fyf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Reload IIS (Open IIS, Stop and Start the server),Install osTicket v1.15.8, after downloading osTicket Download osTicket from the Installation Files Folder and
Extract and copy “upload” folder to c:\inetpub\wwwroot Within c:\inetpub\wwwroot, Rename “upload” to “osTicket”. after completeing that reload IIS and Go to sites -> Default -> osTicket. and Enable or disable an extension”
Enable: php_imap.dll
Enable: php_intl.dll
Enable: php_opcache.dll
Refresh the osTicket site in your browse, observe the changes. Your screen after these steps should look like the following image.


</p>
<br />

<p>
<img src="https://www.liveagent.com/app/uploads/2023/02/osticket-interface.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now from the installation files, download and instal Heidi SQL. Open HeidiSQL, Create new session, connect to the session, create a database called "osTicket"
Continue Setting up osticket in the browser. Go to MySQL Database, MySQL Username, MySQL Password, and Lastly finish installing.
</p>
<br />

<p>
<img src="https://installatron.com/images/remote/ss5_osticket.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Congratulations, hopefully it is installed with no errors!  
Browse to your help desk login page: http://localhost/osTicket/scp/login.php

End Users osTicket URL:
http://localhost/osTicket/ 

Clean up
Delete: C:\inetpub\wwwroot\osTicket\setup
Set Permissions to “Read” only: C:\inetpub\wwwroot\osTicket\include\ost-config.php


</p>
<br />
