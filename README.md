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

<p>

After logging into the VM, I downloaded osTicket Installation Zip Files and unzipped them onto my Windows desktop. I then went to the Windows Control Panel and clicked on "Uninstall a Program" under the Programs tab. Next, I clicked on "Turn Windows Features On or Off". Then I made sure that the following boxes were checked: Internet Explorer 11, Internet Information Services (IIS), World Wide Web Services, Application Development Features, and CGI.


</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>




</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>




</p>
<br />
