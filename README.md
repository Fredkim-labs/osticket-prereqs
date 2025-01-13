<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket: Prerequisites and Installation</h1>
This tutorial provides a step-by-step guide for setting up the prerequisites and installing osTicket, an open-source help desk ticketing system. It details the configuration of a Windows 10 virtual machine in Azure, the installation of necessary software like IIS, PHP Manager, and MySQL, and the final setup of osTicket. The guide ensures a comprehensive installation process for users setting up osTicket in a virtualized environment.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure Virtual Machine
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> 

<h2>List of Prerequisites</h2>

- IIS
- PHP Manager
- Rewrite Module
- VC_redistx86
- MySQL 5.5.62
- Heidi SQL
  
<h2>Installation Steps</h2>

<p>
</p>
<p>
<h3>Create a Virtual Machine on Azure</h3>

![image](https://github.com/user-attachments/assets/b01d699d-3471-4e3f-92ba-bc2d62cc3ba3)
<be><br>
  
- The first step is to create a Virtual Machine (VM) on Azure.
- Create a Resource Group - osTicket
- Choose Windows 10 Pro, version 22H2.
- Make sure to set the size to either 2 or 4 vcpus and 16 GiB memory. I chose 4 vcpus for better performance.


![image](https://github.com/user-attachments/assets/756a4c35-ae2b-49c2-98b3-1e72874e57fc)
<br><br>

- Confirm that RDP (3389) is allowed in "Select inbound ports" to allow Remote Desktop access to the VM.</strong>
- Click on the last check box to confirm a Windows 10 license, then proceed to "Review + Create". A validation process will occur before being able to create.
</p>
<p>
</p>
<br />

<br>

<p>
<h3>Connect to your VM via the Remote Desktop Connection</h3>
<p>
  

![image](https://github.com/user-attachments/assets/a8c2a856-eeb3-4e6a-9086-05b568a2da31)
<br><br>

![image](https://github.com/user-attachments/assets/1b77fa69-3970-4465-86a2-dfc08230dfc3)
<br><br>

- Locate your VM's public IP address
- Open Remote Desktop Connection and paste the VM's IP address, then log in.</p>
<p>

</p>
<br />
<h3>Download and Unzip Installation files</h3>

![image](https://github.com/user-attachments/assets/63782d6c-68a2-4474-8e93-ca81daa7c7b0)
<br><br>

[Download zip file from here.](https://drive.google.com/uc?export=download&id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD)
- Unzip the files after the download is complete.

<h3>Enable IIS </h3>

![image](https://github.com/user-attachments/assets/57878805-3e92-4654-9e95-bd081b420017)
<br><br>

![image](https://github.com/user-attachments/assets/5afd9e6e-2a4d-4816-beaf-c73431a1a276)
<br><br>

<p> - Once the VM is open, we will need to install/enable IIS. Open Control Panel, Programs and click on Turn Windows features on or off</p>


<p><h2>Enable following features:</h2></p>

![image](https://github.com/user-attachments/assets/d552924d-3e54-49ac-86d1-75b71f7ac56e)
<br><br>

- Enable Internet Information Services</p>
- Expand World Wide Web Services </p>
- Expand Application Development Features
- Enable CGI
<br>
<p> Click okay and the features should be enabled.</p>
<br>
<p> <strong> NOTE: If the changes were applied successfully, type "127.0.0.1" in your browser, and this page below should appear. </strong></p>

![image](https://github.com/user-attachments/assets/d8c21692-4789-461d-bb3b-2ba2f7722b56)
<br> <br>

<h3>Install PHP Manager</h3>

![image](https://github.com/user-attachments/assets/65e3458e-2db9-48e5-914b-a3faa38bd809)
<br><br>

![image](https://github.com/user-attachments/assets/15844134-cf54-4648-93ef-ea53ee5519b8)
<br><br>

![image](https://github.com/user-attachments/assets/2efc66e8-a1e1-425c-94d2-eef8b92da586)
<br><br>

<p> Install PHP manager from the osTicket Installation Files folder.


<br>

<h3>Install the Rewrite Module</h3>

![image](https://github.com/user-attachments/assets/58b59768-0e19-4b7e-a5c3-d49ad7a34fd0)
<br><br>

![image](https://github.com/user-attachments/assets/2e3b847f-3b06-4b09-8e6b-c49e61786cee)
<br><br>

- Install the Rewrite module from the osTicket Installation Files folder


<h3>Create a new directory</h3>

![image](https://github.com/user-attachments/assets/f855ae73-c1e9-4d15-80ca-20077dd4a683)
<br><br>

<p>- Open File Explorer and create a new folder "PHP" on the C:\ directory </p>
<br>
<br>
<h3>Extract and Install PHP 7.3.8 </h3>

![image](https://github.com/user-attachments/assets/e691f85a-3056-45b7-8b55-ec4a406e1fe7)
<br><br>

- Extract the PHP zip file into C:\PHP
<br>
<h3>Install VC_redist.x86.exe </h3>

![image](https://github.com/user-attachments/assets/53af226a-985a-46d1-abbb-91de1619cd51)
<br><br>

![image](https://github.com/user-attachments/assets/2fdb9b38-4734-41b0-8cc1-ec7f93d16838)
<br><br>

<h3>Install MySQL 5.5.62 </h3>

![image](https://github.com/user-attachments/assets/8712a80f-1863-479b-a9e8-9556880ef035)

![image](https://github.com/user-attachments/assets/a93ed846-e079-4565-9616-447d23ff3db7)
<br><br>
- Select "Typical" option.

![image](https://github.com/user-attachments/assets/74f81681-d05c-44d7-8a17-4ee12dcf8f47)
<br><br>

![image](https://github.com/user-attachments/assets/a21db650-7ca0-44ea-bc00-b401738ff2d3)
<br><br>

![image](https://github.com/user-attachments/assets/ae25d1e6-db32-4794-b8b0-db822dc4585d)
<br><br>

- Launch the MySQL configuration wizard
- Choose standard configuration

![image](https://github.com/user-attachments/assets/86dfbffc-c860-4e84-8dcb-36ec5cce855e)
<br><br>
<strong>- Create username and password. Keep note of credentials. I used "root" for both to keep it simple.

![image](https://github.com/user-attachments/assets/3a9ea359-c457-4eab-844c-2ba866927119)
<br><br>

<h3>Launch IIS as an administrator</h3>

![image](https://github.com/user-attachments/assets/9ea88774-e13b-4641-874d-b08572f4ac17)
<br><br>
<p>- Search "IIS" in the Windows search bar, then right-click and select "Open as Administrator"</p>
<br>

<h3>&#9324; Register PHP Manager </h3>
<br>
- We will register PHP from within IIS. This means we are making the web server aware of the existence of the PHP on the computer.

![image](https://github.com/user-attachments/assets/9fa7b5f2-48dc-406f-b799-c8b74b39db4c)
<br><br>

![image](https://github.com/user-attachments/assets/c81b6f63-9d6a-40c0-8d93-ed34e6f994b7)
<br><br>

- Open PHP Manager
- Click on Register New PHP

![image](https://github.com/user-attachments/assets/99bbfaba-56c8-4809-be75-3229807c0e23)
<br><br>
<p><strong>- NOTE: Registration will require you to provide a path to "php-cgie.exe". Lead it to the PHP folder previously created and you will find the file "php-cgi"
</strong></p>
<br>

<h3>Restart the IIS server</h3>

![image](https://github.com/user-attachments/assets/699a640b-0a78-48e6-bc9e-232e9c6fa2dd)
<br><br>
- The restart button can be found on the right side of the window under Actions and Manage Server.</p>

<br>
<h3>Install osTicket</h3>

![image](https://github.com/user-attachments/assets/af5f0ea4-cd82-41b1-8630-46751bcc995b)
<br>

![image](https://github.com/user-attachments/assets/6be083d4-a0d5-44f6-9d8b-4dc7f4b4bef2)
<br>

![image](https://github.com/user-attachments/assets/c376a2b3-0820-4ae6-86ec-cea3edd933ad)
<br>
<p>- Extract the contents of osTicket v1.15.8 from the installation files</p>
- Copy the upload for to C:\intelpub\
- Rename "upload" folder to "osTicket"
<br>

<h3>Restart the IIS Again.</h3>
<br>
<br>
<h3>Launch osTicket </h3>
<p>Under Connections in IIS, VM-osTicket -> Sites -> Default Web Site -> osTicket</p>
<img width="623" alt="osTicket" src="https://imgur.com/bgZrJzV.png">
<p></p>
<p><strong>NOTE: Click on osTicket</strong></p>

<h3>&#9329; Select Browse *80 to launch osTicket</h3>
<p> On the right side of the window, under Actions -> Manage Folder -> Click on Browse *:80 (http) </p>
<img width="623" alt="browse80" src="https://imgur.com/yiQjEcK.png">
<br>
<br>
<p><strong>This should lead to osTicket opening in a separate Windows broswer</strong>.</p>
<br>
<br>
<img width="664" alt="osTicket browser" src="https://imgur.com/yOa0Jy8.png">
<br>
<br>
<h3>&#9330; Enable extensions</h3>
<p>Open IIS -> PHP Manager -> Select "Enable or Disable Extension". </p>
<p>Enable the following extensions:</p>
<p>[X]Enable: php_imap.dll</p>
<p>[X]Enable: php_intl.dll</p>
<p>[X]Enable: php_opcache.dll</p>
<img width="273" alt="php enable 2" src="https://imgur.com/8QO0yIO.png">
<br>
<br>
<h3>&#9331; Refresh osTicket</h3>

<p>After refreshing your web browser on osTicket, notice how more features are now available to use.</p>
<img width="608" alt="OSticket changes" src="https://imgur.com/bdJ05kP.png">
<br>
<br>

<h3>&#12881; Rename ost-config.php</h3>

<p> Under c:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php, rename "ost-sampleconfig.php" to "ost-config.php"</p>
<img width="527" alt="ostconfig rename" src="https://imgur.com/yP1YTT0.png">
<br>
<br>

<h3>&#12882; Change ost-config.php permissions</h3>

<p>Change ost-config.php permissions (right click)</p>
<p>Properties -> Security -> Advance -> Disable Inheritance</p> 
<p>Select "remove all inherited permissions" and add everyone as a principal. Select all boxes to ensure all permissions are granted. </p>
<img width="571" alt="Permissions" src="https://imgur.com/mANNCMT.png">

<h3>&#12883; Continue osTicket installation</h3>

<p> Continue through osTicket filling out only the first half of the page to this point.</p>
<img width="611" alt="osticket signup" src="https://imgur.com/m7WratO.png">
<br>
<br>
<p><strong>NOTE: The database credentials we'll fill out later.</strong> </p>
<br>

<h3>&#12884; Download and install Heidi SQL from the installation files</h3>

<p>Open Heidi SQL and create a new session. Make sure to fill in the username as root and create a password. After filling up your credentials now click open and a new session should show up.
</p>

<h3>&#12885; Create new database </h3>

<p>On the left side of the window, right click on "Unnamed" and create a new database named "osTicket".</p>
<img width="512" alt="SQL" src="https://imgur.com/AbElzBn.png">
<br>
<br>

<h3>&#12886; Finish osTicket Sign-Up</h3>

<p>Revert back to your osTicket browser and fill out the incomplete credentials.</p>
<img width="375" alt="osticket final signup" src="https://imgur.com/B2A1SMM.png">


<h3>&#12887; Finalize osTicket installation</h3>

<p>Click install and osTicket should begin to setup. </p>


<br>
<br>
<h1>Congratulations!! &#127881; you just installed osTicket</h1>
