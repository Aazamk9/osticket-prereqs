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

- Create a Virtual Machine (Windows 10, 4 cVPUs) within a resource group in Azure

<h4>Install The Following</h4>
  
- IIS in Windows WITH (then enable CGI, Common HTTP Features and IIS Management Console).
- PHP Manager for IIS
- Rewrite Module
- PHP 7.3.8
- VC Redist
- MySQL 5.5.62

<h2>Installation Steps</h2>


<h3>1.</h3> After installing the prerequisites, create a directory in the main pc drive "C:\PHP" and unzip the PHP 7.3.8 file/contents in this folder.

<h3>2.</h3> Run the setup wizard for MySQL and set a standard configuration with a simple password.

<h3>3.</h3> Open IIS as an admin, register PHP from within IIS, then restart the console.

