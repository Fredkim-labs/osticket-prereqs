<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Installation</h1>
This will outline the installation process of the open-source help desk ticketing system osTicket.<br />

<h2>Technologies and Programs Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Prerequisites and Installation of osTicket</h2>

- Create a resource group to connect to the Microsft Azure Virtual
- Create a Virtal Machine using Microsft Azure.
- Install and Enable IIS
- Install PHP Manager
- Install IIS URL Rewrite Module
- Install VC_redist.x86.exe
- Install MySQL Server
- Set up IIS for PHP
- Install osTicket and Enable Needed Extensions
- Install HeidiSQL, Setup and Create a database

<h2>Installation Steps</h2>

![image](https://github.com/user-attachments/assets/31942d6b-20f5-4057-9b44-f66dbc55ad3f)
<p>
Open the Control Panel and Click Programs Icon.
</p>
<p>
 ______________________________________________________________________________________________________________________________
</p>

![image](https://github.com/user-attachments/assets/95927234-9016-45df-8830-4dfc3085650d)
<p>
Click Turn Windows on or off
</p>
<p>
 ______________________________________________________________________________________________________________
</p>

![image](https://github.com/user-attachments/assets/598dabe8-32ee-4df0-ad8c-8cf8d1dd05be)
<p>
Check the box for Internet Information Services (IIS)
</p>
<p>
Expand IIS and Expand WorldWide Web Services, than Application Development Features
</p>
<p>
Check the box for CGI and Click Ok
</p>
<p>
 ________________________________________________________________________________________________________________________________________________________
</p>
 
![image](https://github.com/user-attachments/assets/bc40140c-329f-435f-aa4c-4327dadf6c8b)
<p>
 Install PHP Manager 
</p>
<p>
 ________________________________________________________________________________________________________________________________________________________
</p>

![image](https://github.com/user-attachments/assets/65bf05b2-2aba-4369-91e6-d2d4cbfb0fe2)
<p>
  Install IIS URL Rewrite Module
</p>
<p>
 ________________________________________________________________________________________________________________________________________________________
</p>

![image](https://github.com/user-attachments/assets/20ea6756-8a07-4488-ae88-22b8b1fec5dd)
<p>
  Install VC_redist.x86.exe
</p>
<p>
 ________________________________________________________________________________________________________________________________________________________
</p>

![image](https://github.com/user-attachments/assets/d2803a59-0d04-4581-98ba-2016e8288028)
![image](https://github.com/user-attachments/assets/35bb07a3-1665-40b6-8f00-20ed6131d017)
<p>
  Install MySQL Server
</p>
<p>
  After installation completed. Click box to launch MySQL Configuration Wizard and click finish
</p>
<p>
 ________________________________________________________________________________________________________________________________________________________
</p>

![image](https://github.com/user-attachments/assets/d7076ca1-1697-4de4-a3f8-b743da75869c)
![image](https://github.com/user-attachments/assets/e7ccde61-1170-4e88-ae29-1139612d26ed)
<p>
  Start the MySQL server Wizard
</p>
<p>
  Create a password for the server
</p>
<p>
 ________________________________________________________________________________________________________________________________________________________
</p>

![image](https://github.com/user-attachments/assets/642e3593-b6a0-40ef-b072-771cb1d29fce)
![image](https://github.com/user-attachments/assets/babffab8-108e-49d3-b8c2-25ca59b1c158)
![image](https://github.com/user-attachments/assets/968812e5-ba57-4af8-8bee-2519e724d4aa)
<p>
 Open IIS as Admin
</p>
<p>
 Open PHP Manager and Register New PHP and restart server
</p>
<p>
 ________________________________________________________________________________________________________________________________________________________
</p>

<p>
 Install osTicket
</p>
<p>
 ________________________________________________________________________________________________________________________________________________________
</p>

![image](https://github.com/user-attachments/assets/2c4d26b4-dbbc-4e06-a76a-b9c2c5335795)
![image](https://github.com/user-attachments/assets/775c3516-a5a8-4a7c-875b-fe91fecf36d1)
<p>
 Install and Launch Heidi SQL 
</p>
<p>
 ________________________________________________________________________________________________________________________________________________________
</p>

![image](https://github.com/user-attachments/assets/e6fd16b7-57fa-42e2-a3c8-380dc00497f3)
![image](https://github.com/user-attachments/assets/84587cdf-70a0-410b-9d33-bb0cba9314a3)
<p>
 Use Password from MySQL server
</p>
<p>
 ________________________________________________________________________________________________________________________________________________________
</p>

![image](https://github.com/user-attachments/assets/8be94c2a-0fc1-4fe5-9edd-1b643635b827)
![image](https://github.com/user-attachments/assets/3a359aa1-64f9-40df-857d-13030fbb7d5d)
![image](https://github.com/user-attachments/assets/8ebc3199-99aa-4e70-8c4b-e8686c2b7cca)
<p>
 Create a new database
</p>
<p>
 ________________________________________________________________________________________________________________________________________________________
</p>

![image](https://github.com/user-attachments/assets/51676ed8-4f5d-4b71-a2bc-13e108cd2c22)
![image](https://github.com/user-attachments/assets/10b9d3e6-b349-41a1-a731-918fa144e015)
<p>
 Fill out form and Fill in the proper database.
</p>
<p>
 Fill out database username and password
</p>
<p>
 ________________________________________________________________________________________________________________________________________________________
</p>

![image](https://github.com/user-attachments/assets/6eb27778-cc2c-422b-b130-cd699f1a8aa9)
![image](https://github.com/user-attachments/assets/e853013b-e033-472b-9ef9-246af32aa3a4)
<p>
 If osTicket is properly installed, http://localhost/osTicket/scp/login.php and http://localhost/osTicket/ will be accessable
</p>
<p>
 ________________________________________________________________________________________________________________________________________________________
</p>
<br />
