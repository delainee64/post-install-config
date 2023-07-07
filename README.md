# post-install-config

<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Create an Admin User account, Organizational Unit, and New Employee to the Domain Admins Security Group. 
- Join the Client to the DC
- Set up Remote Desktop for users/non-administrative users.
- Create a Bunch of Users

<h2>Configuration Steps</h2>

<p>
<img src="https://github.com/delainee64/post-install-config/assets/114307952/7fa54e56-f2a9-4ca4-825f-6fa7fda7c3f0" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
First, log in to http://localhost/osTicket/scp/login.php using your credentials.
</p>

<p>
<img src="https://github.com/delainee64/post-install-config/assets/114307952/d00657d8-c7f2-41a1-9c25-79a37b87dcbe" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once you are logged in to your account, select the "Admin Panel".
</p>

<p>
<img src="https://github.com/delainee64/post-install-config/assets/114307952/069f56f1-e778-4068-8b01-2f13a6774177" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Select "Agents" --> "Roles" --> "Add New Role".
</p>

<p>
<img src="https://github.com/delainee64/post-install-config/assets/114307952/6719c135-c705-4951-8328-b7a2bb3cca17" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Under "Definitions" give your role a name, I chose "Supreme Admin". Then click over to "Permissions" and check all of the boxes. Check all of the boxes for "Tasks" and "Knowledgebase" as well.
</p>

<p>
<img src="https://github.com/delainee64/post-install-config/assets/114307952/f74409d1-1ba7-4edf-9726-cda3498f4a18" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Select "Departments" and "Add New Department".
</p>

<p>
<img src="https://github.com/delainee64/post-install-config/assets/114307952/77d33e5b-efa8-4bdb-81d8-f1409a5d9e0c" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Give your department a name. I chose, "System Administrators". Then scroll to the bottle and "Create Department".
</p>

<p>
<img src="https://github.com/delainee64/post-install-config/assets/114307952/ec968cf7-a2b7-4178-8639-386302f2e68d" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Select "Teams" and "Add New Team".
</p>

<p>
<img src="https://i.imgur.com/jsNIo6X.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
Choose a name and click on "Members" and select yourself. Click "Create Team".
</p>

<p>
<img src="https://github.com/delainee64/post-install-config/assets/114307952/83d54688-9be8-4a51-99e9-d89b6972fbb3" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Select "Agents" and "Add New Agent".
</p>

<p>
<img src="https://i.imgur.com/5N1rl2N.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Enter their name, email address, username, and create a password for them. Then select "Access" and place them in the "System Administrators" and "Supreme Admin" departments. Then select "Teams" and add them to the "Level II Support" team.
</p>

<p>
<img src="https://github.com/delainee64/post-install-config/assets/114307952/0a823a56-6271-43c1-b635-591ba49a094a" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Repeat the following step to create another new user, I named my new user "John Doe". Place him in the "Support" and "View Only" departments and extend his access to "Support".
</p>

<p>
<img src="https://github.com/delainee64/post-install-config/assets/114307952/69ca73da-1576-4a00-9efa-e83b9076805e" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next, select "Agent Panel" --> "Users" --> "Add User".
</p>

<p>
<img src="https://github.com/delainee64/post-install-config/assets/114307952/d87c6b5b-450c-405c-aa52-2d4d26481199" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Give your new user a name and email address. Repeat this process one more time to add another user.
</p>

<p>
<img src="https://github.com/delainee64/post-install-config/assets/114307952/5bc682ff-42b0-4917-91d3-fc450fe0e078" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go back to "Admin Panel" --> "Manage" --> "SLA" --> "Add New SLA Plan".
</p>

<p>
<img src="https://github.com/delainee64/post-install-config/assets/114307952/e118026d-1e0e-4974-8150-570ea5f852d2" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Give your SLA a name, a grace period, and a schedule. Create two more SLA plans. One called "SEV-B" with a grace period of 4 hours on a 24/7 schedule. Lastly, create another SLA plan named "SEV-C" with a grace period of 8 hours on a Monday - Friday Schedule.
</p>

<p>
<img src="https://github.com/delainee64/post-install-config/assets/114307952/cb602440-d9d5-46e6-9fda-895ceb17901e" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Select "Help Topics" --> "Add New Help Topic."
</p>

<p>
<img src="https://github.com/delainee64/post-install-config/assets/114307952/2951d98c-3d18-422c-ab24-dc9d7f1427f2" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Finally, give your help topic a name and make sure it is set to "Top Level Topic". Create three more help topics with the names "Personal Computer Issues", "Equipment Request" and "Password Reset".
</p>
