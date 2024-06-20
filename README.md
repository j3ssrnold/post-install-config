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

<h3>Step 1: To begin log in to osTicket using the username and password you set up in the previous tutorial.</h3> 

-  Notice the Admin Panel option at the top right of your home screen. Click on Adminand you will be ready to begin post-installation configuration.

    <p>
    <img src="https://i.imgur.com/0IEg0Th.png" title="source: imgur.com" /></a>
    </p>
<br />

<h3>Step 2: Configure Agent Roles.</h3>

-  Admin Panel --> Click agents --> Click Roles.
    -  In the name field type in Supreme Admin for a bit fun to assign an agent with Administrator access.

    <p>
    <img src="https://i.imgur.com/tfyG1CT.png" title="source: imgur.com" /></a>
    </p>
<br />

- Next click on the Permissions tab and allow all permissions for Supreme Admin. Then Click Add Role.

    <p>
    <img src="https://i.imgur.com/GGcz2HJ.png" title="source: imgur.com" /></a>
    </p>
<br />

  >[!Note]
  >Be sure that permissions for Tasks and Knowledgebases are selected as well.

-  Save Changes

      <p>
      <img src="https://i.imgur.com/9k5PsEp.png" title="source: imgur.com" /></a>
      </p>
<br />

- Your Supreme Admin is now added to the roster. It should look like this below: 

    <p>
    <img src="https://i.imgur.com/thwzzqb.png" title="source: imgur.com" /></a>
    </p>
<br />

<h3>Step 3: Configure Departments.</h3> 

-  Stay in the Admin Panel --> Click Agents --> Click Departments.
    -  In the name box type in System Administrators --> Leave the other settings as default for now. 

    <p>
    <img src="https://images2.imgbox.com/c2/eb/gtRt5YOY_o.png" alt="image host"/></a>
    </p>

>[!TIP]
>You may want to go back later and edit the SLA in the System Admin Departmnet once those parameters are established.
<br />

-  At the bottom click create department.

    <p>
    <img src="https://i.imgur.com/2DEKqSw.png" title="source: imgur.com" /></a>
    </p>
<br />

-  You have now established a department for System Administrator.

    <p>
    <img src="https://i.imgur.com/nR1lUjo.png" title="source: imgur.com" /></a>
    </p>
<br />

<h3>Step 4: Configure teams.</h3> 

-  This let's you group agents from different departments to troubleshoot/resolve issues with tickets/users. Since Level I is already a default, create Level II support.
    -  Admin Panel -> Agents -> Teams -> Add New Team. Name it Level II Support -> Create Team.</b>

    <p>
    <img src="https://i.imgur.com/w94ngKZ.png" title="source: imgur.com" /></a>
    </p>
<br />

-  You can now view Level II Support in Teams.

    <p>
    <img src="https://i.imgur.com/bpf1vtS.png" title="source: imgur.com" /></a>
    </p>
<br />

<h3>Step 5: Ticket Population: Allow anyone to create a ticket.</h3> 

-  Stay in Admin Panel -> Settings -> User Settings. Go down to Registration Required and be sure that the check box is unchecked.</b>

    <p>
    <img src="https://images2.imgbox.com/a8/26/fejBDhnO_o.png" alt="image host"/></a>
    </p>

>[!IMPORTANT]
>Make sure to complete this step. If not, you will not be allowed to log in as a guest; making you register the "users" you create in a few steps
<br />


<h3>Step 6: Now you need to create Agents, Jane and Marhsall.</h3> 

-  At the top right make sure you click on Agent Panel --> Users --> Add New. --> Fill in name, email, then username for Jane.</b>

    <p>
    <img src="https://i.imgur.com/MjGxxWP.png" title="source: imgur.com" /></a>
    </p>
<br />

-  Set Password. Uncheck Send the agent a password reset email. Enter and confirm password. Make sure both boxes are unchecked then click set.

    <p>
    <img src="https://i.imgur.com/SwJ2Rdz.png" title="source: imgur.com" /></a>
    </p>
<br />

- For Jane's access level, you should make Jane your Supreme Admin. Click Access -> Primary Department -> Support -> Supreme Admin. Extended Access -> System Adminstrators -> Supreme Admin -> Add. ***Make sure Alerts box is checked.***

<p>
<img src="https://i.imgur.com/NOaX9Nm.png" title="source: imgur.com" /></a>
</p>
<br />

- Add Jane to a team as well. Go to the teams Tab--> Select Level II Support--> Add ***Alerts should be checked.***--> Create.

<p>
<img src="https://i.imgur.com/hRWp4i3.png" title="source: imgur.com" /></a>
</p>
<br />

- Jane is now added to the Agent Roster. 

<p>
<img src="https://i.imgur.com/9pjXsnZ.png" title="source: imgur.com" /></a>
</p>
<br />


<b>Now create a support profile. You should add Marshall Arnold, a help desk professional. Stay in Admin Panel --> Agents --> Add new agent. Fill in name, email, and username for Marshall.</b>

<p>
<img src="https://i.imgur.com/5a9sf7B.png" title="source: imgur.com" /></a>
</p>
<br />

- Set Password. Uncheck Send the agent a password reset email. Enter and confirm password. Make sure both boxes are unchecked then click set.

<p>
<img src="https://i.imgur.com/1UOe157.png" title="source: imgur.com" /></a>
</p>
<br />

- For Marhsall's access level: Click Access -> Primary Department -> Support -> ***Extended Access not View Only. If you leave his access at view only, Marshall will not be able to close tickets on his own.*** 

<p>
<img src="https://i.imgur.com/GdmJSGF.png" title="source: imgur.com" /></a>
</p>
<br />

- You have now created Marshall's Agent Account.

<p>
<img src="https://i.imgur.com/5a9sf7B.png" title="source: imgur.com" /></a>
</p>
<br />


<b>Step 6: Next you need to create End Users. Use Karen and Chad as two examples. Go to Agent Panel -> Users -> Add New. For the purposes of this tutorial we will just fill out name and email. Click Add user.</b>

- Account Details should look like this: 

<p>
<img src="https://i.imgur.com/wYdRzxV.png" title="source: imgur.com" /></a>
</p>
<br />

- Karen is added in the user list.

<p>
<img src="https://i.imgur.com/ElznjgS.png" title="source: imgur.com" /></a>
</p>
<br />

<b>Time to add Chad. Again, Agent panel -> Users -> Add New. Just add the name and email for Chad.</b>

- Account Details should look like this:

<p>
<img src="https://i.imgur.com/8kOQdP6.png" title="source: imgur.com" /></a>   
</p>  
<br />

- Chad is in the user list now:

<p>
<img src="https://i.imgur.com/El3Cbwk.png" title="source: imgur.com" /></a>
</p>
<br />

<b>Step 7: Next you need to set up the SLA levels in the system. This will give our agents a way to prioritze ticekts in the system. For the purposes of this tutorial, you will need to set SLAs at Sev-A, B, and C. Revert to Admin Panel (top right) -> Manage -> SLA.</b>

- For Sev-A: 1 hour/24-7. In Name Box -> Sev-A. In Grace Period -> 1. From the Schedule drop down menu -> select 24/7.

<p>
<img src="https://i.imgur.com/lje1ZuW.png" title="source: imgur.com" /></a>
</p>
<br />

- For Sev-B: 4 hours/24-7. In Name Box -> Sev-B. In Grace Period -> 4. From the Schedule drop down menu -> select 24/7.

<p>
<img src="https://i.imgur.com/88j7ZIs.png" title="source: imgur.com" /></a>
</p>
<br />

- For Sev-C: 8hours/M-F 8a-5p, with holidays In Name Box -> Sev-C. In Grace Period -> 8. From the Schedule drop down menu -> select M-F/8a-5p, with holidays.

<p>
<img src="https://i.imgur.com/E15QudZ.png" title="source: imgur.com" /></a> 
</p>
<br />

- Now your SLAs are in the Directory:

<p>
<img src="https://i.imgur.com/96BTUYj.png" title="source: imgur.com" /></a>
</p>
<br />

<b>Step 8: For your last step, you need to configure Help Topics. You should add four common categories: Business Critical Outage, Personal Computer Issues, Equipment Request, and Password Reset. Again confirm you are in Admin Panel -> Manage -> Help Topics.</b>

- First, add Business Critical Outage. Fill in the name, <b>**then Add/Create Topic.**</b>

<p>
<img src="https://i.imgur.com/oXHKev1.png" title="source: imgur.com" /></a>
</p>
<br />

- Second, add Personal Computer Issues. Fill in the name, <b>**then Add/Create Topic.**</b>

<p>
<img src="https://i.imgur.com/uxZgY96.png" title="source: imgur.com" /></a>
</p>
<br />

- Third, add Equipment Reset.  Fill in the name, <b>**then Add/Create Topic.**</b>

<p>
<img src="https://i.imgur.com/9nzdNOC.png" title="source: imgur.com" /></a>
</p>
<br />

- Last, add Password reset. Fill in the name, <b>**then Add/Create Topic.**</b>

<p>
<img src="https://i.imgur.com/mZ8bX6M.png" title="source: imgur.com" /></a>
</p>
<br />

- Your Help Topics are now populated.

<p>
<img src="https://i.imgur.com/rjF6cEd.png" title="source: imgur.com" /></a>
</p>
<br />

<b>Congrats! You have completed the intial Post-Installation Configuration.</b>
