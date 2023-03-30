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

- Item 1
- Item 2
- Item 3
- Item 4
- Item 5

<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/PC6to0L.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
</p>
<p>
We finally have our osTicket set up! The very first step in the post-instalation process is to configure roles. Roles are the permissions granted to Agents per Department that they have access to. Each Role has a set of permissions that can be checked/unchecked for agents given that Role in association with a Department they have access to. An unlimited number of roles can be created and assigned to Agents with access to various departments. For the purposes of this demonstration, I am going to be setting up a role called "Supreme Admin" which will allow us to do anything within osTicket. It will allow us to create tickets, assign tickets, and so on. So lets start. The first thing we have to do is go into the Admin Panel from our osTicket main page. 
</p>
<br />

<p>
<img src="https://i.imgur.com/g6mK6uU.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/prlJaCQ.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
</p>
<p>
From here we want to go to the "Agents" tab and click on "Roles". From here We can create a new role and that is exactly what we are going to do by clicking "Add New Role". In my example I named it "Supreme Admin". The next order of business will be setting permissions and we can do that by clicking "Permissions"  and checking off everything we see in the Tickets, Tasts, and Knowledgebase tabs. Lastly, we want to make sure that we click "Add Role" on the bottom and proceed. 
</p>
<br />

<p>
<img src="https://i.imgur.com/dVCGYlE.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now we have to set up our "Departments". Since tickets are routed through Departments in the help desk, there are many settings that can be set for each Department. So for example, the networking department would handle any tickets relating to any network issue. Each department could potentially even have its own SLA (Service Level Agreement). The SLA outlines the expected amount of time (in hours) that a ticket is expected to be closed once opened. If the ticket is not closed in the allotted amount of time, it will then be Overdue. We can begin by going back to our Agent Panel and clicking the "Agents" tab on the top right. From there we can click "Departments". Just like with creating an admin in the previous step, we can go ahead and click "Add New Department". If we look at the image above we can see the screen that will allow us to configure all our department settings. I named mine "System-Administrator" and left everything else blank. YOu can always come back and edit any changes you want so just go ahead and click "Create Dept" on the bottom.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
