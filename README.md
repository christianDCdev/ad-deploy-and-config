<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Active Directory Deployment and Configuration</h1>
Welcome back!  In this project we will be building upon the Active Directory environment created in the previous project.
<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>Prerequisites</h2>

-  Please complete <a href="https://github.com/christianDCdev/ad-deploy-and-config">Setup for Active Directory Infrastructure</a> before beginning this project

<h2>Objectives</h2>

- Install Active Directory
- Create a Domain Admin user
- 

<h2>Configuration Steps</h2>

<h3>&#9312; Install Active Directory</h3>
<p>

- Connect to your DC-1 VM via Remote Desktop
- Open Server Manager Application
- Click "Add Roles and Features"
- Click "Next" until you reach "Server Roles"
- Select "Active Directory Domain Services" and click "Add Features"
<img src="https://i.imgur.com/GiPCO9P.png" height="80%" width="80%" alt="AD Domain services"/>

- Click "Next" until you reach "Confirmation"
- Check box that says "Restart the destination server automatically if required"
- Click "Install" to complete installation
  
</p>

<h3>&#9313; Promote DC-1 to a Domain Controller</h3>

<p>

- Within the Server Manager Dashboard, click on the flag at top right and click "Promote this server to a domain controller"
<img src="https://i.imgur.com/dXntZsV.png" height="80%" width="80%" alt="domain controller promotion"/>

- Select "Add a new forest" option
- Set "Root domain name:" to "mydomain.com"
<img src="https://i.imgur.com/OtjZXv7.png" height="80%" width="80%" alt="domain controller promotion"/>

- Under "DNS options", uncheck "Create DNS delegation"
- Complete forest installation and your VM should automatically restart once installation is finished
- Log back into DC-1 VM as a domain user by typing "mydomain.com\(your username)" as your username (Example: mydomain.com\labuser)

</p>
<br />
<h3>&#9314; Create Client VM</h3>

<p>

-
  
</p>
<br />

<h3>&#9315; Set Domain Controller's Private IP Address to "Static"</h3>

<p>

- 
  
</p>
<br />

<h3>&#9316; Connect to the Domain Controller with Remote Desktop</h3>

<p>

- 
  
</p>
<br />

<h3>&#9317; Disable Firewalls in the Domain Controller</h3>

<p>

- 
  
</p>
<br />

<h3>&#9318; Connect Client VM to Domain Controller VM</h3>

<p>

- 
  
</p>
<br />

<h3>&#9319; Connect to Client VM with Remote Desktop</h3>

<p>

- 
  
</p>
<br />

<h3>&#9320; Ensure Connectivity Between Domain Controller and Client</h3>

<p>

- 
  
</p>

<h2>Conclusion</h2>

<p>
If you're reading this, then hopefully you have succesfully completed every step of this project.  This project has built the foundation for the following Active Directory projects.  Now that our Domain Controller and Client are connected and configured, we can dig deeper into more advanced implementations and configurations of Active Directory.

- If you would like to continue to the next step in this series of Active Directory projects, please click <a href="https://github.com/christianDCdev/ad-deploy-and-config">here</a>

</p>
