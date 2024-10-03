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

- Windows 10</b> 

<h2>List of Prerequisites</h2>

- IIS
- PHP Manager
- VC_redistx86
- MySQL 5.5.62
- Rewrite Module
- Heidi SQL

<h2>Installation Steps</h2>

<h2>Setting Up osTicket on Azure VM</h2>

1. Create Virtual Machine in Azure:
- Log in to Azure Portal.
- Create a new VM with Windows Server.
![image](https://github.com/user-attachments/assets/3ef6412d-12eb-4197-b368-5145b66ebf51)

- Connect to your VM using the Remote Desktop with the public IP address form the VM. (for mac user use the "windows app")
![image](https://github.com/user-attachments/assets/d5754cfa-60fa-45e3-80a9-0498054b379a)

- login with the same login credentials used to create the VM.
   
![image](https://github.com/user-attachments/assets/871155b7-1c14-4160-ab8f-5d96b6a90f9f)

2. Download the osTicket-Installation-Files.zip

- Inside your VM download the [osTicket-Installation-Files.zip](https://drive.google.com/uc?export=download&id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD)and unzip it onto your desktop. we will use the files to download osticket.
![image](https://github.com/user-attachments/assets/3b361ac4-d206-4ee9-bc24-bb7dfd7f2a20)

3. Enable ISS with CGI

- Go to the Control Panel and open the programs applet. Under programs, select "Turn Windows features on or off".
![image](https://github.com/user-attachments/assets/a1f6a130-c77b-4975-8c5d-7617ee57589c)

- enable (internet information services) World Wide Web Services -> Application Development Features -> enable (CGI)
![image](https://github.com/user-attachments/assets/33e9c604-072b-4a04-9276-8eead0f6ea34)

- Test if the changes were applied succesfully, type 127.0.0.1 on your browser and the page below should appear.
![image](https://github.com/user-attachments/assets/53698717-7b46-4a56-a0b8-a78511406fcd)

4. Download and install PHP manager from the osTicket-Installation-Files
- (PHPManagerForIIS_V1.5.0.msi)

![image](https://github.com/user-attachments/assets/92eee3dd-bac3-4db0-b58e-ff75e6caa7a4)

5. Download and Install the Rewrite Module

- (rewrite_amd64_en-US.msi) from the osTicket-Installation-Files
![image](https://github.com/user-attachments/assets/294e336b-3eb7-4d03-a561-4171b080ad47)


6. Creat a directoy in the C drive 

- Go to file explorer and creat the directory C:\PHP
![image](https://github.com/user-attachments/assets/61df1d0c-6c8a-4094-a42a-12445ed66dcd)

7. From the osTicket-Installation-Files intall(php-7.3.8-nts-Win32-VC15-x86.zip) into C:\PHP

- From osTicket-Installation-Files unzip the content into the newly created C:\PHP

![image](https://github.com/user-attachments/assets/a25b7d28-338a-4f58-be0d-f055e645b7c7)

8. Download and Install the (VC_redist.x86.exe) 

- install from the osTicket-Installation-Files
![image](https://github.com/user-attachments/assets/9a70d19f-c771-458f-a446-97f976109788)

9. Download and install MySQL 5.5.62 (mysql-5.5.62-win32.msi)
- install from the osTicket-Installation-Files

- select the following configurations;

  ->Typical setup

  ->launch configuration


  ->Standard configuration

  ![image](https://github.com/user-attachments/assets/0c20332f-c755-4b52-a890-baca66a769b0)

 - the user for this service is going to (username:root) (password:root) for my sql server
![image](https://github.com/user-attachments/assets/4ca0c95e-e6a3-4fc4-9d8d-d4c3059c281c)














