<p align="center">
  <img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

# osTicket - Post-Install Configuration
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.

## Environments and Technologies Used

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

## Operating Systems Used

- Windows 10 (21H2)

## Post-Install Configuration Objectives

- Configure Roles
- Configure Teams and Departments
- Configure Agents
- Configure SLA
- Create Help Topics

## Configuration Steps

### 1. Configure Roles

<p>
  <img src="https://i.imgur.com/ufs9DZo.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
To configure roles, go to: Admin Panel > Agents > Roles. Add a new role, name it, and enable all ticket permissions.

---

### 2. Configure Teams and Departments

<p>
  <img src="https://i.imgur.com/2CTnRRu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
- Go to Admin Panel > Agents > Departments, name the department, and select a manager. Click Create Dept.
- Next, go to Admin Panel > Agents > Teams. Select Add team, name it "Level II Support", and add members by clicking on the Members tab.
- Go to Admin Panel > Settings > User Settings to make sure the Registration Required box is not checked.

---

### 3. Configure Agents

<p>
  <img src="https://i.imgur.com/OIsYUDw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
- Go to Admin Panel > Agents and click Add New Agent.
- Enter the agent's name and email, then click the Set Password button.
  - Deselect the Send the agent a password reset box.
  - Create a password and deselect the Require password change box, then click Set.
- Click the Access tab and select System Administrators.
- Also select the department you created earlier.
- Under Extended Access, select the department you created and add the Support department.
- In the Teams tab, select the team you created.
- Click Create.
- To add another agent with limited permissions, go to Agent Panel > Users and click Add User.
- Create a name, email, and password, then click Add User.

---

### 4. Configure SLA (Service Level Agreements)

<p>
  <img src="https://i.imgur.com/rVfrerR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
- Go to Admin Panel > Manage > SLA and click Add New SLA Plan.
- Set these SLA times:
  - Sev-A: 1 hour (24/7)
  - Sev-B: 4 hours (24/7)
  - Sev-C: 8 hours (Monday - Friday)

---

### 5. Create Help Topics

<p>
  <img src="https://i.imgur.com/sY9NZGT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
- Go to Admin Panel > Manage > Help Topics and click Add Help Topic.
  - Title the first one "Business Critical Outage".
  - The second: "Personal Computer Issues".
  - The third: "Equipment Request".
  - Lastly: "Password Reset".
- Log into the user portal at: [http://localhost/osTicket/](http://localhost/osTicket/).
- Use a user account to create tickets.
