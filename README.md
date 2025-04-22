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

- Microsoft Azure account
- Remote Desktop
- Virtual Machines
- osticket installation
- SQL

![image](https://github.com/user-attachments/assets/a8fb22d1-c105-49be-a837-e957c3a5839a)![image](https://github.com/user-attachments/assets/6b538348-eb9e-4d0a-a99b-df71f0006aa4)
![image](https://github.com/user-attachments/assets/e9abb06c-f2b3-441d-8d23-ea5173fce02f)![image](https://github.com/user-attachments/assets/9e95eb6f-b232-46f3-97fa-48103c0ee5b2)

1. Set Up the Azure VM

VM Name: osticket-vm

Username: labuser

Password: osTicketPassword1!

Size: 4 vCPUs running Windows 10 Pro

2. Log in to the VM

Use Remote Desktop and the login info above to get into the VM.

3. Get the VM Ready for osTicket

Download osTicket files: Grab the osTicket-Installation-Files.zip, unzip it, and drop it into a new folder on the desktop called osTicket-Installation-Files.

4.Turn on IIS with CGI Support

Go to Control Panel > Programs and Features > Turn Windows Features On/Off

Enable IIS and under World Wide Web Services > Application Development Features, make sure CGI is checked.

5. Install What osTicket Needs

PHP Manager for IIS: Run PHPManagerForIIS_V1.5.0.msi from the folder.

URL Rewrite Module: Run rewrite_amd64_en-US.msi from the same folder.

PHP:

Create a folder at C:\PHP

Unzip php-7.3.8-nts-Win32-VC15-x86.zip into that folder

VC Redistributable: Install VC_redist.x86.exe

MySQL 5.5.62: Install mysql-5.5.62-win32.msi using the Typical Setup option

Set up MySQL with:

Username: root

Password: root

6.Done!

At this point, the VM should be all set with IIS, PHP, and MySQL—ready for the osTicket installation.

