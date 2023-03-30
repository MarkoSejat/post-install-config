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
<img src="https://i.imgur.com/CrJTeQd.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now we have to set up our "Departments". Since tickets are routed through Departments in the help desk, there are many settings that can be set for each Department. So for example, the networking department would handle any tickets relating to any network issue. Each department could potentially even have its own SLA (Service Level Agreement). The SLA outlines the expected amount of time (in hours) that a ticket is expected to be closed once opened. If the ticket is not closed in the allotted amount of time, it will then be Overdue. We can begin by going back to our Agent Panel and clicking the "Agents" tab on the top right. From there we can click "Departments". Just like with creating an admin in the previous step, we can go ahead and click "Add New Department". If we look at the image above we can see the screen that will allow us to configure all our department settings. I named mine "System-Administrator" and left everything else blank. YOu can always come back and edit any changes you want so just go ahead and click "Create Dept" on the bottom. We should be able to see our newly created "System Administrator" department appear with 0 agents assigned to it. 
</p>
<br />

<p>
<img src="https://i.imgur.com/jvU44VB.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/PTxiWam.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
</p>
<p>
We will now be setting up "Teams". Teams allow you to pull Agents from different Departments and organize them to handle a specific issue or user via a Help Topic or Ticket Filter. Having Agents from different Departments assigned to a Team will supersede the parameters of the Agents’ Department rules. For example, you can create a Help Topic associated with a particular product you produce, and assign it to a Team of specialist Agents from different Departments. So again, going back to our admin panel we can go to Agents > Teams > Add New Team. For this lab I created a team called "Level II Support" and added myself under the "members" Tab. Click "Create Team" and thats it. 
</p>
<br />

<p>
<img src="https://i.imgur.com/GePDo8w.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now that we have our roles, departments, and teams set up we need to allow users the ability to create tickets. We are now going to set it up so that anonymous users who arent in the system can go ahead and create tickets. We can do this by going to Admin Panel > Settings > Users > Settings > and make sure that "Require registration and login to create tickets" is unchecked.  
</p>
<br />

<p>
<img src="https://i.imgur.com/MJQj6gn.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next we will be setting up our "Agents". Agents are basically the help-desk employee workers who are actually going through all the tickets and so on. Agents are given access to the help desk with the intent to respond and resolve the tickets. When adding an Agent to the help desk, they will need to be assigned to a Primary Department and given a Primary Role for the Tickets/Tasks routed to that department. Agents can be given Extended Access to additional departments of the help desk as well as assigned different Roles to those departments; this can be configured in the Access tab of the Agent’s Profile. We can start off by going to our Admin Panel > Agents > Add New Agent. I will create a few different ones for demonstration purposes. 
</p>
<br />

<p>
<img src="https://i.imgur.com/wToLGIF.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/AZl1oIG.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/ZX1mAob.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
</p>
<p>
After we set the password we can adjust different configurations under each tab. I placed Jane Doe in the Systems-Administrator Department and Level II Support under teams. 
</p>
<br />

<p>
<img src="https://i.imgur.com/U8Lo8mt.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/ZaMOVHi.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
</p>
<p>
I am now going to create yet another user named John Doe following the same steps as before. This time I will be giving John Doe "view only" ability under "Access" and placing him in "Support" under Primary Department.
</p>
<br />

<p>
<img src="https://i.imgur.com/yNrmYKG.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
</p>
<p>
Since we cannot have a ticketing system without any actual users, we will have to create our own for the purpose of this lab. Users can now create an account and log-in to create a ticket or check a ticket’s status. As always with osTicket, users or ticket creators are associated with their email address as the unique identifier of each user. The User Directory, located on the Agent Panel, allows agents to search tickets by user as well as create Organizations to associate the user to. Agents can be configured as internal Account Managers for tickets created by users of an Organization. Users are the ticket owners of the tickets in the help desk. When a ticket is created in the help desk, the user is associated with their email address in the User Directory of the help desk. Users can be added or deleted from the User Directory of the help desk at any time. Please note, if the user is deleted the tickets of the user must also be deleted.
</p>
<br />

<p>
<img src="https://i.imgur.com/vLYqSnV.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/1Fek9lj.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
</p>
<p>
We will start off by creating a new user named "Karen". We can do this by going to the agent panel as opposed to the admin panel that we have used until now. From there we can click on "Users" and then "Add User".  If you look at the photos above you can see that I created a generic email address as Karen@osticket.com and just named the user "Karen Karen".
</p>
<br />

<p>
<img src="https://i.imgur.com/y7ot74F.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
</p>
<p>
I will now create a second user just like I did with Karen but this time I will name the user "Ken Ken". 
</p>
<br />

<p>
<img src="https://i.imgur.com/WrPICgX.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
</p>
<p>
Our next order of business is configuring our SLAs which we talked about before when setting up departments. If you dont remember, SLA Plans or Service Level Agreements, are unlimited in osTicket. The purpose of the SLA Plan is to provide a length of time in which the help desk Administrator expects tickets to be closed. SLA Plans can be created by going to the Admin Panel > Manage > SLA Plans. Click on the top right of the table to “Add New SLA Plan”.  
</p>
<br />

<p>
<img src="https://i.imgur.com/1IIBQbP.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/hEHOqFD.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
</p>
<p>
We will create three SLA plans. Sev-A (1 hour, 24/7), Sev-B (4 hours, 24/7), Sev-C (8 hours, business hours). We can do this by clicking "Add New SLA Plan".

</p>
<br />

<p>
<img src="https://i.imgur.com/SlwEL6I.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
</p>
<p>
The last step in this section will be configuring the Help Topics. Help Topics will help streamline your end-user’s help desk experience to ensure proper assignment and prompt response to the ticket. Create as many Help Topics as needed and can even nest Help Topics within each other for further breakdown (For example, Human Resources and Human Resources/Payroll.) Help Topics will determine what Department the ticket is routed to which will determine which Agents have access to the ticket. The Help Topic also can determine other configurations of the ticket, such as the ticket’s SLA (or Service Level Agreement) and priority of a ticket, i.e. Emergency to Low. There are two places where the Help Topic must be selected on New Tickets; the client portal and new tickets created internally by staff. When Users select the Help Topic, they are not aware of the configurations in place for that Help Topic. 
</p>
<br />


<p>
<img src="https://i.imgur.com/8ZymBju.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
</p>
<p>
We can go to Admin Panel > Manage > Help Topics > Add New Help Topic. 
</p>
<br />

<p>
<img src="https://i.imgur.com/TcqiuCX.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
</p>
<p>
We will create the following help topics:
<br>
Business Critical Outage
<br>
Personal Computer Issues
<br>
Equipment Request
<br>
Password Reset
<br>
Once we have our Help Topics created we can complete this section of the project. I will demonstrate everything that we have done up to this point in the next project! Thank you.
</p>
<br />
