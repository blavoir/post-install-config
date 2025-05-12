<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation](https://youtu.be/eNeOdn5xqpE)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (22H2)

<h2>Post-Install Configuration Objectives</h2>

- Creating Roles
- Creating Departments
- Creating Teams
- Creating Agents
- Adding SLAs and Help Topics

<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/pRTcLk3.gif" height="80%" width="80%" alt="Role Creation"/>
</p>
<p>
In osTicket, roles are used to define what staff members (agents) can do within the staff panel. Log in if you haven't already, nagivate to the admin panel. <b>Then nagivate to agents section tab then, to roles. Create a new role, define it a name and select the permissions you want the role to have.</b> You can create as many roles as you need related to your use case. In this example, I will be creating a "Supreme Admin" with all the permissions. 
</p>
<br />

<p>
<img src="https://i.imgur.com/K1WaldW.gif" height="80%" width="80%" alt="Department Creation"/>
</p>
<p>
Departments are used to organize tickets based on the subject matter or the type of support needed. <b>Under the same tab, next to roles go to departments. Click "Add New Department", add a name, change its parameters if needed and add people that correspond with it. </b> In this example, I will be creating a "SysAdmins" department. You can also create sub-departments of another one via the Parent option.
</p>
<br />

<p>
<img src="https://i.imgur.com/t8bWqRC.gif" height="80%" width="80%" alt="Team Creation"/>
</p>
<p>
Teams are used to group staff members together so they can work collaborate on tickets across departments. <b>Now head over to Teams. Click "Add New Team", give a name and add any members if necessary.</b> Teams also have the option to assign a individual as a "Team Lead" and their status as being active or disabled. In this example, I will be creating a "Online Banking" team.
</p>
<br />

<p>
<img src="https://i.imgur.com/kZgu2ts.gif" height="80%" width="80%" alt="Allow registration"/>
</p>
<p>
Head over to the settings tab, then to users. Ensure that anyone can create tickets by <b>unchecking "Require registration aand login to create tickets" </b> for this example as we will be later illustrating example tickets. You may not do this for your organization.
</p>
<br />

<p>
<img src="https://i.imgur.com/tt00JeI.gif" height="80%" width="80%" alt="Agent Creation"/>
</p>
<p>
Agents also represented as staff members are the people who manage and respond to tickets in the system. <b>Go back to agents and then the sub heading agents. Create a new agent, everything that is bold (name, email address and username) are required to be filled, and head over to Access and add them to a department with a role.</b> You also have the option to add specific permissions to the specific agent as well as add them to teams. 
</p>
<br />

<p>
<img src="https://i.imgur.com/6Mp9t6N.png" height="80%" width="80%" alt="Example: Agents"/>
</p>
<p>
In this example, I have created "Jane Doe" and "John Man" as agents. <b>Jane</b> is assigned to the SysAdmins department and is part of the online banking team while <b>John</b> is assigned to the support department. Feel free to add as many agents as you need.
</p>
<br />


<p>
<img src="https://i.imgur.com/YokIKdL.gif" height="80%" width="80%" alt="SLAs"/>
</p>
<p>
SLAs (Service Level Agreement) is a set of rules that define how quickly support staff should respond to and resolve tickets. <b>Head over to Manage, under Manage go to SLA. Create a SLA plan and add a number (in hours) of the grace period that you want.</b> You can also create as many SLAs as per your organization policies as well as changing the schedules related to them. In this example, I have created 3 SLAs (Sev-A, Sev-B, Sev-C) with Sev-A being the most critical (1 hour grace period) to Sev-C being the least with (8 hour grace period done with business hours). 
</p>
<br />



<p>
<img src="https://i.imgur.com/puetAVi.gif" height="80%" width="80%" alt="Help Topics"/>
</p>
<p>
Help Topics are used to categorize new tickets based on what the customer needs help with. They act as guided labels. <b>Head over to Help Topics under the same tab Manage. Click "Add New Help Topic", Add a name and then create it.</b> You also have the option to have new tickets be set automatically with predefined settings as well as adding forms to them. You can also link help topics within parent topics. In this example, I have created a category Report a Problem and several help topics such as Business Critical Outage, Personal Computer Issues and Equipment Request.  
</p>
<p>There's a lot of tinkering that can be done with osTicket and I encourage to dive more into as osTicket is packed with many features. I've shown the some relevant settings that a organziation may be interested in setting up.</p>
<br />

[Ticket Examples](https://github.com/blavoir/ticket-lifecycle)
