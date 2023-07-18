# Active Directory: Creating Administrators and Users
This walkthrou shows how administrator and normal user accounts are made in the Active Directory, after the Active Directory has been installed



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)
- Windows Server 22

<h2>Active Directory Creation Objectives</h2>

- Creat Organizational Units
- Create an Administrator
- Join the Client VM to the domain
- Setup the Client's Remote Desktop for non-administrative users
- Create normal users and log into the Client VM with one of them.

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
