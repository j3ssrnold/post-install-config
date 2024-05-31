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

Step 1: This is what the osTicket home screen should look like. You will want to use the helpdesk link and username and password you established in the previous tutorial to login. For the next few subsequent steps, you will want to be in Admin Panel. To get there you need to go to the top right of the screen and click Admin Panel to start post-installation configuration.

<p>
<img src="https://i.imgur.com/0IEg0Th.png" title="source: imgur.com" /></a>
</p>
<br />

Step 2: You will want to assign roles for your agents. Login to helpdesk with the username and password you created. In order to have a role that has access to everything, you will start from the Admin Panel -> Click agents -> Click Roles. Type in Supreme admin for fun to assign an admistrator to ticketing system. In the name field type "Supreme Admin".

<p>
<img src="https://i.imgur.com/tfyG1CT.png" title="source: imgur.com" /></a>
</p>
<br />

Next click on the Permissions tab and allow all permissions for Supreme Admin. Then Click Add Role.

***Note: Be sure that permissions for Tasks and Knowledgebases are selected as well.***

<p>
<img src="https://i.imgur.com/GGcz2HJ.png" title="source: imgur.com" /></a>
</p>
<br />

Here you can see where Supreme Admin was added to the roster: 

<p>
<img src="https://i.imgur.com/nR1lUjo.png" title="source: imgur.com" /></a>
</p>
<br />

Do not forget the next two tabs select all boxes and save changes.

<p>
<img src="https://images2.imgbox.com/d0/80/3zg7aWhP_o.png" alt="image host"/></a>

<img src="https://images2.imgbox.com/b1/97/izy6hZ0G_o.png" alt="image host"/></a> 
</p>
<br />

<p>
Step 2: Now let's configure the departments in the ticketing system. Make sure you are still in the Admin Panel -> Click Agents --> Click Departments. In the name box type in System Administrators. Leave the other settings as default. <b>(You may want to go back later and edit the SLA in the System Administrator Department once those parameters are established.)</b> At the bottom click create department. <b> REMINDER FOR FORMAT. GET SCREENSHOT WITH CREATE BUTTON AND DEPARTMENT LIST</b>**
</p>
<p>
<img src="https://images2.imgbox.com/c2/eb/gtRt5YOY_o.png" alt="image host"/></a>
</p>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
Step 3: After the previous step, You should configue teams to allow you to pull agents from different departments to handle specific issues/users via help topic or ticket filter. This allows you to create different levels of support. Let's create Level II support since Level I is already established. Again it's Admin Panel -> Agents -> Teams -> Add New Team. Name it Level II Support -> Create Team. <b>**FORMAT REMINDER INSERT TEAM LIST</b>
<p>
<img src="https://images2.imgbox.com/f6/34/TASnjgMN_o.png" alt="imgbox"/></a>
</p>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
Step 4: Allow anyone to create a ticket. Admin Panel -> Settings -> User Settings. Go down to Registration Required and be sure that the check box is unchecked. 
</p>
<p>
<img src="https://images2.imgbox.com/a8/26/fejBDhnO_o.png" alt="image host"/></a>
</p>
<br />

<p>
Step 5: Now you need to create Agents. In the top right make sure you are on Agent Panel -> Users -> Add New. Let's add Jane. Fill in name, email then set username for Jane.
</p>

<p>
<img src="https://images2.imgbox.com/53/ab/fgQu95B6_o.png" alt="imgbox"/></a>
</p>

<b>**Formatting Reminder -> screenshot of password settings and Agent List screenshot.</b> Don't make Jane reset user password at initial login.

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
Go ahead and make Jane your Supreme Admin. Click Access -> Primary Department -> Support -> Supreme Admin. Then Extended Access -> System Adminstrators -> Supreme Admin -> Make sure Alerts is checked -> Create Role.
<p>
<img src="https://images2.imgbox.com/5f/7b/nCEbgEMe_o.png" alt="imgbox"/></a>
</p>
<b>**Formatting reminder: screenshot of list</b>
</p>
<br />

<p>
Let's make a regular agent profile. Again make sure you're in Agent Panel -> Users -> Add New. Let's add Marshall Arnold, a new hire. Again we won't make Marshall reset user password at initial login. Access will be view only. 
</p>

<p>
<img src="https://images2.imgbox.com/1b/12/qTp0iznX_o.png" alt="imgbox"/></a>

<b>
Formatting Reminder: Insert Screenshot of Password Settings.  
</b>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  
<img src="https://images2.imgbox.com/9b/a7/XH3hqiYn_o.png" alt="imgbox"/></a> 
</p>
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
