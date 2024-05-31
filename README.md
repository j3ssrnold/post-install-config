<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<!--
<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation] / !-->

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

Configure
- Roles
- Departments
- Teams
- Agents
- Users
- SLA
- Help Topics

<b>Links for Login:</h2>

Help Desk: http://localhost/osTicket/scp/login.php

End Users: http://localhost/osTicket/</b>

<h2>Configuration Steps</h2>

Step 1: Let’s get started! First, log in to osTicket using the username and password you set up earlier. Once you’re in, you’ll see the Admin Panel option at the top right of your home screen. Click on Admin, and you will be ready to begin post-installation configuration.

<p>
<img src="https://i.imgur.com/0IEg0Th.png" title="source: imgur.com" /></a>
</p>
<br />

Step 2: Now that you are in the admin panel you can set up roles for your agents. You will start from the Admin Panel -> Click agents -> Click Roles. In the name field type in Supreme Admin for a bit fun to assign an agent with Admistrator access.

<p>
<img src="https://i.imgur.com/tfyG1CT.png" title="source: imgur.com" /></a>
</p>
<br />

Next click on the Permissions tab and allow all permissions for Supreme Admin. Then Click Add Role.

<p>
<img src="https://i.imgur.com/GGcz2HJ.png" title="source: imgur.com" /></a>
</p>
<br />

***Note: Be sure that permissions for Tasks and Knowledgebases are selected as well.***

<p>
<img src="https://i.imgur.com/9k5PsEp.png" title="source: imgur.com" /></a>
</p>
<br />

Here you have Supreme Admin was added to the roster: 

<p>
<img src="https://i.imgur.com/thwzzqb.png" title="source: imgur.com" /></a>
</p>
<br />

Step 3: Next you can configure the Departments. Stay in the Admin Panel -> Click Agents --> Click Departments. In the name box type in System Administrators. Leave the other settings as default for now. <b>(You may want to go back later and edit the SLA in the System Administrator Department once those parameters are established.)</b>

<p>
<img src="https://images2.imgbox.com/c2/eb/gtRt5YOY_o.png" alt="image host"/></a>
</p>
<br />

At the bottom click create department.

<p>
<img src="https://i.imgur.com/2DEKqSw.png" title="source: imgur.com" /></a>
</p>
<br />

You have now established a department for System Administrator.

<p>
<img src="https://i.imgur.com/nR1lUjo.png" title="source: imgur.com" /></a>
</p>
<br />

Step 3: Next you should set up teams. This let's you group agents from different departments to troubleshoot/resolve issues with  tickets/users. Since Level I is already a default, create Level II support. Admin Panel -> Agents -> Teams -> Add New Team. Name it Level II Support -> Create Team. 

<p>
<img src="https://i.imgur.com/w94ngKZ.png" title="source: imgur.com" /></a>
</p>

<p>
<img src="https://i.imgur.com/bpf1vtS.png" title="source: imgur.com" /></a>
</p>
<br />

Step 4: Ticket Population: Allow anyone to create a ticket. Stay in Admin Panel -> Settings -> User Settings. Go down to Registration Required and be sure that the check box is unchecked. 

<p>
<img src="https://images2.imgbox.com/a8/26/fejBDhnO_o.png" alt="image host"/></a>
</p>
<br />

Step 5: Now you need to create Agents. In the top right make sure you click on Agent Panel -> Users -> Add New. Go ahead and add Jane. Fill in name, email, then username for Jane.

<p>
<img src="https://i.imgur.com/MjGxxWP.png" title="source: imgur.com" /></a>
</p>
<br />

Set Password. Uncheck Send the agent a password reset email. Enter and confirm password. Make sure both boxes are unchecked then click set.

<p>
<img src="https://i.imgur.com/SwJ2Rdz.png" title="source: imgur.com" /></a>
</p>
<br />

For Jane's access level, you should make Jane your Supreme Admin. Click Access -> Primary Department -> Support -> Supreme Admin. Extended Access -> System Adminstrators -> Supreme Admin -> Add. ***Make sure Alerts is checked.***

<p>
<img src="https://i.imgur.com/NOaX9Nm.png" title="source: imgur.com" /></a>
</p>
<br />

Add Jane to a team as well. Go to the teams Tab--> Select Level II Support--> Add ***Alerts should be checked.***--> Create.

<p>
<img src="https://i.imgur.com/hRWp4i3.png" title="source: imgur.com" /></a>
</p>
<br />

Jane is now added to the Agent Roster. 

<p>
<img src="https://i.imgur.com/9pjXsnZ.png" title="source: imgur.com" /></a>
</p>
<br />


Now for a support profile. You shoukd add Marshall Arnold, a help desk professional. Stay in Admin Panel --> Agents --> Add new agent. Fill in name, email, and username for Marshall.

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

Set Password. Uncheck Send the agent a password reset email. Enter and confirm password. Make sure both boxes are unchecked then click set.

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

For Marhsall's access level, . Click Access -> Primary Department -> Support -> ***Extended Access not View Only.*** If you leave his access at view only, Marshall will not be able to close tickets on his own. 

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

Set Password. Uncheck Send the agent a password reset email. Enter and confirm password. Make sure both boxes are unchecked then click set.

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

You have now created Marshall's Agent Account.

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
<b>Step 6:</b> Now that you have Admins and Agents set up, you need to create End Users. Let's use Karen and Chad as two examples. Make sure you are in Agent Panel -> Users -> Add New. For the purposes of this tutorial we will just fill out name and email. Then Click Add user. 
</p>

<p>
<img src="https://images2.imgbox.com/60/7b/HXMJJd1I_o.png" alt="imgbox"/></a>
</p>

<p>
<b>**Formatting Reminder** Add image of user list after creating. </b>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

Time to add Chad. Again, Agent panel -> Users -> Add New. Just add the name and email for Chad.

<p>
<img src="https://images2.imgbox.com/df/09/uMcCsTBI_o.png" alt="imgbox"/></a>   
</p>  
<b>**Formatting Reminder** Add user list again to be sure everyone was added correctly.</b>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
<b>Step 7:</b> Now it's time to set up the SLA levels in our system. This will give our agents a way to prioritze ticekts in the system. For the purposes of this tutorial, you will need to set SLAs at Sev-A, B, and C. Revert to Admin Panel (top right) -> Manage -> SLA.

For Sev-A: 1 hour/24-7. In Name Box -> Sev-A. In Grace Period -> 1. From the Schedule drop down menu -> select 24/7.
</p>

<p>
<img src="https://images2.imgbox.com/b4/03/3tEuXxrD_o.png" alt="imgbox"/></a>
</p>

For Sev-B: 4 hours/24-7. In Name Box -> Sev-B. In Grace Period -> 4. From the Schedule drop down menu -> select 24/7.

<p>
<img src="https://images2.imgbox.com/15/59/SyedcK9t_o.png" alt="imgbox"/></a>
</p>

For Sev-C: 8hours/M-F 8a-5p, with holidays In Name Box -> Sev-C. In Grace Period -> 8. From the Schedule drop down menu -> select M-F/8a-5p, with holidays.

<p>
<img src="https://images2.imgbox.com/da/98/oh8kqh9i_o.png" alt="imgbox"/></a> 
</p>
<br />

<p>
<b>Step 8:</b> For your last step, you need to configure Help Topics. We will add four common categories: Business Critical Outage, Personal Computer Issues, Equipment Request, and Password Reset. Again confirm you are in Admin Panel -> Manage -> Help Topics. 

First, add Business Critical Outage. Fill in the name, <b>**then Add/Create Topic.**</b>

<p>
<img src="https://images2.imgbox.com/0f/4d/fv5HGNj7_o.png" alt="imgbox"/></a>
</p>

Second, add Personal Computer Issues. Fill in the name, <b>**then Add/Create Topic.**</b>

<p>
<img src="https://images2.imgbox.com/4c/28/uwmZonmZ_o.png" alt="imgbox"/></a>
</p>

Third, add Equipment Reset.  Fill in the name, <b>**then Add/Create Topic.**</b>

<p>
<img src="https://images2.imgbox.com/5f/5f/aK59IotF_o.png" alt="imgbox"/></a>
</p>

Last, add Password reset. Fill in the name, <b>**then Add/Create Topic.**</b>

<p>
<img src="https://images2.imgbox.com/a0/cf/wCT1R9tD_o.png" alt="imgbox"/></a>
</p>

<b>**Formatting reminder. Add image of list of created help topics.</b>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

Congrats! You have configured the ticketing system for both agents and users.
