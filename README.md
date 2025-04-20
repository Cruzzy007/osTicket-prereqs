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

<h2>Create the directory C:\PHP</h2>
- unzip the file php-7.3.8-nts-Win32-VC15-x86.zip and extract all into the PHP file in the C:drive

![Screenshot 2025-04-15 190314](https://github.com/user-attachments/assets/753a2764-990c-4958-b1e8-79eb4ef7b879)




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
