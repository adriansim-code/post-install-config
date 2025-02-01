<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation](https://youtu.be/19WpzGui8vw?si=3o16AAeoSqoUwib9)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles for grouping permissions.
- Set up Departments to define ticket visibility.
- Add Agents and Users to the system.
- Configure SLA policies.
- Define Help Topics for ticket categorization.

<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/otM8fiQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Navigate to Admin Panel → Agents → Roles. Here, you can create custom roles and define specific permissions for agents based on their responsibilities. The Supreme Admin role has full access to all osTicket features and settings, ensuring comprehensive control over the system. To manage ticket visibility and categorize support responsibilities, configure departments by navigating to Admin Panel → Agents → Departments. Departments help separate different support areas, such as Help Desk, SysAdmins, and Networking, ensuring tickets are routed to the appropriate teams.
</p>
<br />

<p>
<img src="https://i.imgur.com/o5OJkdL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To configure agents, navigate to Admin Panel → Agents → Add New. Here, you can add support workers like Jane (assigned to the SysAdmins department) and John (assigned to the Support department). Configuring agents properly ensures that tickets are assigned to the correct personnel for resolution.
</p>
<br />

<p>
<img src="https://i.imgur.com/VscpPZo.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To configure users (customers), navigate to Agent Panel → Users → Add New. Users, such as Karen and Ken, represent the end users who will be submitting support tickets. Properly setting up users allows for seamless ticket submission and tracking.
</p>
<br />

<p>
<img src="https://i.imgur.com/qmikrGi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In this section, you’ll define different severity levels, starting with Sev-A. For Sev-A, set the Grace Period to 1 hour and choose the Schedule as 24/7. This means the response time will be within 1 hour, no matter the time of day. Next, configure Sev-B with a Grace Period of 4 hours and the same Schedule of 24/7, which means that response time will be within 4 hours, again 24/7. Lastly, for Sev-C, set the Grace Period to 8 hours, but this time select Business Hours for the schedule. This indicates that Sev-C issues will have up to 8 hours to be addressed, but only during standard business hours.
</p>
<br />

<p>
<img src="https://i.imgur.com/8KQOJtX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After setting up the SLA, you will configure the Help Topics for when users create tickets. Again, head to the Admin Panel, then go to Manage, and select Help Topics. Here, you’ll add the different categories that users can select when creating a ticket. The available help topics are:
  Business Critical Outage - For issues that impact business operations significantly.
  Personal Computer Issues - For any personal computer-related problems.
  Equipment Request - If users need to request new equipment.
  Password Reset - For assistance with account access or password recovery.
  Other - For any issue that doesn’t fall into the categories above.
</p>
<br />
