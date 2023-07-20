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

- Create Organizational Units
- Create an Administrator
- Join the Client VM to the domain
- Setup the Client's Remote Desktop for non-administrative users
- Create normal users and log into the Client VM with one of them.

<h2>Creating your Active Directory with Admin and normal users.</h2>
<h3>Creating Organizatonal Units and an Administrator</h3>
 - In Active Directory Users and Computers, create two organizational units with the names "_EMPLOYEES" and "_ADMINS

 <img src="https://i.imgur.com/uUyrwB5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

 - Within the _ADMINS folder, create a new employee named "Jane Doe" with the username "jane_admin".
<img src="https://i.imgur.com/STn9O7o.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 - Add Jane Doe to the Domain Admins security group
 <img src="https://i.imgur.com/uVpakVF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  - Log out of the Remote Desktop connection to DC-1 and log back in as “mydomain.com\jane_admin”. Continue to use "jane_admin" from now on.
 
<p></p>

<h3>Joining the Client VM to your domain</h3>
 - From the Azure Portal, set Client-1's DNS settings to DC-1's Private IP address.
<p>Restart Client-1 from the Azure Portal
<img src="https://i.imgur.com/5HlwKQD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/AFmhkzH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 - Login to Client-1 as the original local administrator and join it to the domain
<p>Note:The remote desktop will restart</p>
<img src="https://i.imgur.com/VgtQfE1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 - Login to the Domain Controller and verity Client-1 shows up in Active Directory Users and Computers inside the "Computers" container on the root of the domain.
<img src="https://i.imgur.com/QADRVXj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<p></p>
<h3>Setting up the Client's Remote Desktop for non-administrative users</h3>
 - Login to Client-1 as my.domain.com/jane_admin and allow "domain users" access to remote desktop.
<img src="https://i.imgur.com/Wx6mi3i.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

 - With this being done, you can now log into Client-1 as a normal non-administrative user.

<p></p>
<h3>Creating a number of non-administrative users</h3>
 - Login to DC-1 as jane_admin
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 - Open PowerShell_ise as an administrator
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 - Create a new file and paste the contents of this [script](https://github.com/joshmadakor1/AD_PS/blob/master/Generate-Names-Create-Users.ps1) into it
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 - Run the script and observe the accounts being created
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 - Open the Active Directory Users and Computers and observe the accounts in their respective Organizational Unit
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />
