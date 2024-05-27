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

<p>
Step 1: You will want to assign roles for your agents. Login to helpdesk with the username and password you created. In order to have a role that has access to everything, you will start from the Admin Panel -> Click agents -> Click Roles. Type in Supreme admin for fun to assign an admistrator to ticketing system. In the name field type "Supreme Admin".
</p>
<p>
<img src="https://images2.imgbox.com/50/d6/U77PNESp_o.png" alt="imgbox"/></a>
</p>
<br />

<p>
Next click on the Permissions tab and allow all permissions for Supreme Admin. Then Click Add Role.
</p>

<p>
<img src="https://images2.imgbox.com/47/35/8NffhlO6_o.png" alt="imgbox"/></a>

<img src="https://images2.imgbox.com/28/45/xgY6hHBg_o.png" alt="image host"/></a>
</p>

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
<br />

<p>
Step 3: After the previous step, You should configue teams to allow you to pull agents from different departments to handle specific issues/users via help topic or ticket filter. This allows you to create different levels of support. Let's create Level II support since Level I is already established. Again it's Admin Panel -> Agents -> Teams -> Add New Team. Name it Level II Support -> Create Team. <b>**FORMAT REMINDER INSERT TEAM LIST</b>
<p>
<img src="https://images2.imgbox.com/f6/34/TASnjgMN_o.png" alt="imgbox"/></a>
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
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
