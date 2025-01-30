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

- Enable Internet Information Services
- Install Web Platform Installer
- Install Visual C++ Redistributal
- Intsall MySQL/Setup Username and Password
- Configure Permission and install osTicket

<h2>Installation Steps</h2>


![image](https://github.com/user-attachments/assets/9d7a109e-620c-4357-9012-e78d04e3ef1c)

<p>

</p>
<p>To enable IIS you open the Control Panel then go to Programs and within that on the left you clicked Turns Windows Features. Then you check the Internet Information Services box then click the expand box. Next you click the World Wide Web Services. Within that you click Application Development and then you click CGI.
</p>
<br />


![image](https://github.com/user-attachments/assets/1354c14a-179c-41c7-b01f-562fed08aa17)



<p>

</p>
<p>
First you go into osTicket Installation file to install PHP Manager then from within the same folder you are going to install Rewrite Module. Next you go to File Explorer then go to the C drive and create a folder called PHP. Then from the "osTicket-installation-files" you unzip the PHP into the C\PHP folder.
</p>
<br />


![image](https://github.com/user-attachments/assets/1822de46-ffde-4ff1-95ab-9b8ae685a343)

<p>

</p>
<p>
From the "osTicket-Installation-Files" folder install VC_redist.x86.
</p>
<br />


![image](https://github.com/user-attachments/assets/1c9cf2eb-da6b-44c9-b622-864b6d53a394)


![image](https://github.com/user-attachments/assets/be354b7d-e14f-49e3-bd9f-e65e2b36bb81)

<p>

</p>
<p>
From the "osTicket-Installation-Files" folder you install MySQL 5.5.62. Then you choose Typical Setup then install. Next you Launch Configuration Wizard then you choose Standard Configuration. For the selected Modify Security Settings for the Username and Password type in "root" then click Next.
</p>
<br />


![image](https://github.com/user-attachments/assets/08d69d08-8a02-42c4-9fb4-a4e69435cd99)

![image](https://github.com/user-attachments/assets/9a8aecd4-940b-4bec-bb8e-d2be39769326)

![image](https://github.com/user-attachments/assets/b4e1f33d-10e8-49db-a3d0-9bf10bed0430)

![image](https://github.com/user-attachments/assets/d788fb2b-dbe1-412f-aade-3f7e7ea98a79)

![image](https://github.com/user-attachments/assets/55bff808-1b1b-4e89-8d9c-4bbbc24959ac)

![image](https://github.com/user-attachments/assets/198db738-c08c-4cc1-aa4f-44b1e3a3b2a6)

<p>

</p>
<p>
Open IIS as an Admin. Then you open and register PHP from within the IIS. Next you reload IIS. Next to install osTicket, From the "osTicket-Installation-Files" folder unzip “osTicket-v1.15.8.zip” and copy the “upload” folder into “c:\inetpub\wwwroot” and rename folder "upload" to "osTicket". Reload IIS and then go "site" "default site" then "osTicket". Go to PHP Manager then click “Enable or Disable an Extension” then Enable: php_imap.dll Enable: php_intl.dll Enable: php_opcache.dll. then refresh osTicket in browser. 
In C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php change sampleconfig.php to ost-config.php. To assign permission got to ost-config.php then to Disable Inheritance then click Remove All Then New Permission then go to Everybody and click All
</p>
<br />

