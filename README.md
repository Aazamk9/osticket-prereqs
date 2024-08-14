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

- Create a Virtual Machine (Windows 10, 4 cVPUs) within a resource group in Azure

<h4>Prerequisites for osTicket</h4>
  
- IIS in Windows WITH (enable CGI, Common HTTP Features, IIS Management Console).
- PHP Manager for IIS
- Rewrite Module
- PHP 7.3.8
- VC Redist
- MySQL 5.5.62
- HeidiSQL

<h2>Installation Steps</h2>


<h3>1.</h3> After installing the prerequisites, create a directory in the main pc drive "C:\PHP" and unzip the PHP 7.3.8 file/contents in this folder.

<h3>2.</h3> Run the setup wizard for MySQL and set a standard configuration with a simple password.

<h3>3.</h3> Open IIS as an admin, register PHP from within IIS, then restart the console.



<h2>Setting up osTicket</h2>

<h3>1.</h3> Install osTicket v1.15.8, then extract and copy the “upload” folder to c:\inetpub\wwwroot. Within c:\inetpub\wwwroot, Rename “upload” to “osTicket”

<h4>Reload IIS (Restart / Open IIS, Stop and Start the server)</h4> 

<h3>2.</h3> Go to sites -> Default -> osTicket. On the right, click “Browse *:80” 

<h3>3.</h3> Click “Enable or disable an extension” and enable the following: php_imap.dll, php_intl.dll, and php_opcache.dll

<h3>4.</h3> Redirect to the folder C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php, and rename the final folder as "ost-config.php"

<h3>5.</h3> Click properties --> Security, and complete the following: Disable inheritance -> Remove All, New Permissions -> Everyone -> All

<h3>6.</h3> When setting up osTicket in the browser. make your MySQL credentials the following: Database=osTicket, username=root, and any easy-to-remember password



<h5>Browse to Your Helpdesk Login Page</h5>

 http://localhost/osTicket/scp/login.php

 <h5>End Users osTicket URL</h5>

 http://localhost/osTicket/ 






