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

 - Go back to IIS, sites -> Default -> osTicket
 - Double-click PHP Manager
 - Click “Enable or disable an extension”
 - Enable: php_imap.dll
 - Enable: php_intl.dll
 - Enable: php_opcache.dll
 - Refresh the osTicket site in your browser, observe the changes

 ![Screenshot 2025-04-16 105105](https://github.com/user-attachments/assets/6d66ad48-29e8-442b-b1b2-57ebcc4df51b)

 - Rename: ost-config.php
 - From: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php
 - To: C:\inetpub\wwwroot\osTicket\include\ost-config.php
   
![Screenshot 2025-04-16 111048](https://github.com/user-attachments/assets/9032c2ed-7938-42f2-9d5d-c4c224a3116e)

- Assign Permissions: ost-config.php
- Disable inheritance -> Remove All

![Screenshot 2025-04-16 111412](https://github.com/user-attachments/assets/4d7bc354-fee0-40f5-a7e7-fa5ed43009b9)

- New Permissions -> Everyone -> All

![Screenshot 2025-04-16 111626](https://github.com/user-attachments/assets/562bcf04-d399-49ec-8528-cc5a85bb4ee1)

- From the “osTicket-Installation-Files” folder, install HeidiSQL.
  ![Screenshot 2025-04-16 112352](https://github.com/user-attachments/assets/ff9af5c6-308c-4e6f-9e27-a615618c0e30)

- Open Heidi SQL
![Screenshot 2025-04-16 112651](https://github.com/user-attachments/assets/9b758de1-a2b0-49b6-bc81-ca24d2ac0d54)

- Create a new session, root/root
- Connect to the session
- Create a database called “osTicket”
![Screenshot 2025-04-16 112820](https://github.com/user-attachments/assets/08eafe55-f888-4d4d-9dc2-d5b1c949f722)

- Continue Setting up osTicket in the browser
- MySQL Database: osTicket
- MySQL Username: root
- MySQL Password: root
- Click “Install Now!”
- Browse to your help desk login page: http://localhost/osTicket/scp/login.php
![Screenshot 2025-04-16 125818](https://github.com/user-attachments/assets/73d2a9a3-df40-401a-8360-8835e75bb53d)







 


















