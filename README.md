# AD-Creating-Users
This shows how administrator and normal user accounts are made in the Active Directory

# osTicket-Post-Installation-Configuration
This is the list of all Virtual Machines and software that must be setup, downloaded and installed, for the osTicket system to work.

<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles
- Configure Departments
- Configure Teams
- Allow anyone to create tickets
- Configure Agents (workers)
- Configure Users (customers)
- Configure SLA
- Configure Help Topics

<h2>Configuration Steps</h2>


<h3>Configure Roles</h3>
Create a "Supreme Admin" Role, in the Admin Panel
Admin Panel -> Agents -> Roles
<p>

<h3>Configure Departments</h3>
Create a "System Administrators" Department
Admin Panel -> Agents -> Departments

<h3>Configure Teams</h3>
Create "Level I Support" and "Level II" Support Teams
Admin Panel -> Agents -> Teams

<h3>Allow anyone to create Tickets</h3>
Admin Panel -> Settings -> User Settings
Require registration and login to create tickets

<h3>Configure Agents (Workers)</h3>
Create two agents (Jane and John)
Admin Panel -> Agents -> Add New

<h3>Configure Users (Customers)</h3>
Create two Users (Karen and Ken)
Agent Panel -> Users -> Add New

<h3>Configure SLA</h3>
Create three different SLA's with different priority settings
    Sev-A (1 hour, 24/7)
    Sev-B (4 hours, 24/7)
    Sev-C (8 hours, business hours)

<h3>Configure Help Topics</h3>
Create four different help topics
    Business Critical Outage
    Personal Computer Issues
    Equipment Request
    Password Reset
Admin Panel -> Manage -> Help Topics


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

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />
