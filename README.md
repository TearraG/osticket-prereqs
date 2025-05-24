# osticket-prereqs
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

- Create a Microsoft Azure Virtual Machine Windows 10, 4 vCPUs
- Log Into Virtual Machine With Remote Desktop
- Download and Unzip osTicket Zip Files Onto Desktop
- Install VC Redistributable Files, MySQL 5.5.62, 
- Open IIS as Admin and Register PHP

<h2>Installation Steps</h2>

<p>

![practice resize](https://github.com/user-attachments/assets/c09f3b28-7d8a-44c6-abdb-3db65c960bc9)

First, I created a virtual machine (VM) in Microsoft Azure and named it "osTicket". I used OS Windows 10, 4 vCPUs and made sure to create a username and password for this VM. I set the VM to RDP 3389 so that I can use it to access the Windows machine remotely from my laptop. 



![osticket photo 2](https://github.com/user-attachments/assets/05e3095c-6772-4742-a742-d2c95bdf53ec)

Next, I downloaded the Windows App in the Apple Store. Once installed, I clicked the upper right corner and clicked, "Add A PC". I went back to Miscosoft Azure and copied the public IP address of the "osTicket" VM and pasted it into the IP address bar on the Windows App. Once the PC was added, I double clicked it and I used the same username and password I used to set up the VM and logged into virtual Windows PC. 



![osticket photo 3](https://github.com/user-attachments/assets/95c704a9-46e9-4446-b83f-309320a0b303)


After logging into the VM, I downloaded osTicket Installation Zip Files and unzipped them onto my Windows desktop. I then went to the Windows Control Panel and clicked on "Uninstall a Program" under the Programs tab. Next, I clicked on "Turn Windows Features On or Off". Then I made sure that the following boxes were checked: Internet Explorer 11, Internet Information Services (IIS), World Wide Web Services, Application Development Features, and CGI.


![osticket photo 4](https://github.com/user-attachments/assets/ace53965-226b-41ff-ae76-a10baaaeae71)



Next, I double clicked the osTicket folder on Desktop then installed PHP Manager, which is the background web server osTicket uses to run. I then installed the Rewrite Module within the folder. After that, I created an Active Directory on the C: drive of the computer named PHP. Next, I extracted the PHP language files into the PHP folder on the C: drive. Then, I installed the VC Redist File. Next, I installed the MySQL 5.5.62 file, which is the database that OsTicket uses to store it's data including user accounts, ticketing information, etc. 


![osTicket photo 5](https://github.com/user-attachments/assets/0b1739d7-b74b-4a70-821b-46aedc972c88)



Once this was done, I ran IIS as an admin and registered PHP within it. Next, I copied the "upload" folder from the "OS Ticket Files" zip files, pasted it into the wwwroot folder and renamed it osTicket. I reloaded the IIS, clicked on "sites", then "default", then "osTicket". On the right hand side of the ISS, I then clicked "Browse :80". The OsTicket site loaded on the screen. Next, I enabled the required extensions. I went back to the osTicket "include" folder and renamed the "ost-sampleconfig.php" file to "ost-config.php". After that, I assigned permissions to the "ost-config.php", disabling inheritence, and setting new permissions to "Everyone".  



![osTicket photo 6](https://github.com/user-attachments/assets/c96a01f4-6346-45f0-a0bd-85234e8484b3)


Lastly, once that was done, I finished setting up osTicket in the browser by installing "HeidiSQL" Database from the osTicket installation files and created a new session with the username "root" and password "root". Then, I was able to finish the osTicket browser set up by inputting the Database name "osTicket" and the same username "root" and password "root." I clicked "install" and was finished.




</p>
<br />
