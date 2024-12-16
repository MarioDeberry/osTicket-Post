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
  - To configure roles, go to: Admin Panel > Agents > Roles. Add a new role, name it, and enable all ticket permissions.

<p>
  <img src="https://imgur.com/mF2ommb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

---

### 2. Configure Teams and Departments
  - Go to Admin Panel > Agents > Departments, name the department, and select a manager. Click Create Dept.
  - Next, go to Admin Panel > Agents > Teams. Select Add team, name it "Level II Support", and add members by clicking on the Members tab.
  - Go to Admin Panel > Settings > User Settings to make sure the Registration Required box is not checked.

<p>
  <img src="https://imgur.com/YKWwYBv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

---

### 3. Configure Agents
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
<p>
  <img src="https://imgur.com/aYLW8l1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>


---

### 4. Configure SLA (Service Level Agreements)
- Go to Admin Panel > Manage > SLA and click Add New SLA Plan.
- Set these SLA times:
  - Sev-A: 1 hour (24/7)
  - Sev-B: 4 hours (24/7)
  - Sev-C: 8 hours (Monday - Friday)
<p>
  <img src=https://imgur.com/mjhPg3C.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

---

### 5. Create Help Topics
- Go to Admin Panel > Manage > Help Topics and click Add Help Topic.
  - Title the first one "Business Critical Outage".
  - The second: "Personal Computer Issues".
  - The third: "Equipment Request".
  - Lastly: "Password Reset".
- Log into the user portal at: [http://localhost/osTicket/](http://localhost/osTicket/).
- Use a user account to create tickets.
<p>
  <img src="https://imgur.com/YeZXILV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

