# osTicket-prereqs
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://youtu.be/LOzmM5ZjKi0?si=dGXg9uRfSszDLDtK)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Working Computer
- Internet Access 
- Azure Account
- RDP

<h2>Installation Steps</h2>

-Create an Azure Virtual Machine Windows 10, 4 vCPUs
- Name: osticket-vm
- Username: labuser
- Password: osTicketPassword1!
- Log into the VM with Remote Desktop
- download, https://drive.google.com/uc?export=download&id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD
- once downloaded, right click zipped file and extract all onto desktop
- We will use the files in this folder to install osTicket and some of the dependencies
- Go to control panel
- In programs and features click "Turn on windows features on or off"
- Next Go to IIS(internet information services)
- Then to World Wide Web Services and to Application Development Features
- Finally click CGI and hit ok/install



![Screenshot 2025-04-15 185146](https://github.com/user-attachments/assets/950026a5-aa75-46eb-a098-99b924b0f793)

<h2> Installing Files </h2>

![Screenshot 2025-04-15 190634](https://github.com/user-attachments/assets/52be80e6-2d0c-4e19-bde0-2cc4fe210082)

- From the “osTicket-Installation-Files” folder, install PHP Manager for IIS (PHPManagerForIIS_V1.5.0.msi)
- From the “osTicket-Installation-Files” folder install the Rewrite Module (rewrite_amd64_en-US.msi)
- From the “osTicket-Installation-Files” folder, install VC_redist.x86.exe.
-Side bar just accept and hit okay for all the following software.

<h2>Create the directory C:\PHP</h2>

 unzip the file php-7.3.8-nts-Win32-VC15-x86.zip and extract all into the PHP file in the C:drive

![Screenshot 2025-04-15 190314](https://github.com/user-attachments/assets/753a2764-990c-4958-b1e8-79eb4ef7b879)

- From the “osTicket-Installation-Files” folder, install MySQL 5.5.62 (mysql-5.5.62-win32.msi)
- Typical Setup ->
- Launch Configuration Wizard (after install)
- Standard Configuration
- Username: root
- Password: root
- Next Open IIS as an Admin
- Register PHP from within IIS (PHP Manager -> C:\PHP\php-cgi.exe)
- Reload IIS (Open IIS, Stop and Start the server)

  ![Screenshot 2025-04-16 104953](https://github.com/user-attachments/assets/cb621686-0764-44ab-9df9-92327f7fe8a8)


![Screenshot 2025-04-16 103141](https://github.com/user-attachments/assets/5cfac91a-d486-4e03-9ff3-ae0851ecd2f7)

- Install osTicket v1.15.8
- From the “osTicket-Installation-Files” folder, unzip “osTicket-v1.15.8.zip” and copy the “upload” folder into “c:\inetpub\wwwroot”
- Within “c:\inetpub\wwwroot”, Rename “upload” to “osTicket”

![Screenshot 2025-04-16 103959](https://github.com/user-attachments/assets/c0b02bee-c1b5-47ce-9ce9-999a28acb634)

- Reload IIS (Open IIS, Stop and Start the server)
- Go to sites -> Default -> osTicket
- On the right, click “Browse *:80”

 ![Screenshot 2025-04-16 104716](https://github.com/user-attachments/assets/36ec457e-5b2a-4a37-91f2-ec7ed780b037)
 


 


















</p>
<br />

<p>
<img />
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
