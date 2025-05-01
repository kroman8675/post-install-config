<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Computer)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (22H2)

<h2>Configuration Objectives</h2>

- Step 1: Configure Roles, Departments, and Teams
- Step 2: Allow ticket creation
- Step 3: Configure Agents and Users
- Step 4: Configure SLA's and Help Topics

<h2>Configuration Steps</h2>
- Step 1: Configure Roles, Departments, and Teams
<img width="912" alt="Screenshot 2025-05-01 at 3 04 51 PM" src="https://github.com/user-attachments/assets/b71ae1b5-799f-4ad0-be8a-6c94c0688ef4" />
Get logged in at this link: http://localhost/osTicket/scp/login.php , and go into the admin panel if not already which is at the top right of the site.

<img width="912" alt="Screenshot 2025-05-01 at 3 04 51 PM" src="https://github.com/user-attachments/assets/3f114afa-bd9e-4e9d-a96d-33078382a6d5" />
Then click Agents and then Roles. Select Add New Roles, type Admin, and click on the Permissions tab. In the permissions tab select all the permissions under Tickets, Tasks and Knowledgable. After that click Add Role.

<img width="1182" alt="Screenshot 2025-05-01 at 3 16 44 PM" src="https://github.com/user-attachments/assets/035324db-bbe9-4567-b64c-5ad3d13c1ad2" />
Click on Agents then Departments. Click Add New Department

<img width="871" alt="Screenshot 2025-05-01 at 3 26 33 PM" src="https://github.com/user-attachments/assets/05ba494b-65a1-4ffc-8f5b-9ed9cde8320b" />
For the Parent leave it as Top Level Department. I named the Department SysAdmins and select Private for the Type, then click Create Dept.







<br />
