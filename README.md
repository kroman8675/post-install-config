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
- Step 2: Configure Agents and Users
- Step 3: Configure SLA's and Help Topics

<h2>Configuration Steps</h2>
- Step 1: Configure Roles, Departments, and Teams
<img width="912" alt="Screenshot 2025-05-01 at 3 04 51 PM" src="https://github.com/user-attachments/assets/b71ae1b5-799f-4ad0-be8a-6c94c0688ef4" />
 Get logged in at this link: http://localhost/osTicket/scp/login.php , and go into the admin panel if not already which is at the top right of the site.

<img width="912" alt="Screenshot 2025-05-01 at 3 04 51 PM" src="https://github.com/user-attachments/assets/3f114afa-bd9e-4e9d-a96d-33078382a6d5" />
 Then click Agents and then Roles. Select Add New Roles, type Admin, and click on the Permissions tab. In the permissions tab select all the permissions under Tickets, Tasks and Knowledgable. After that click Add Role.

<img width="1182" alt="Screenshot 2025-05-01 at 3 16 44 PM" src="https://github.com/user-attachments/assets/035324db-bbe9-4567-b64c-5ad3d13c1ad2" />
 In the Agents tab click Departments. Click Add New Department

<img width="871" alt="Screenshot 2025-05-01 at 3 26 33 PM" src="https://github.com/user-attachments/assets/05ba494b-65a1-4ffc-8f5b-9ed9cde8320b" />
 For the Parent leave it as Top Level Department. I named the Department SysAdmins and select Private for the Type, then click Create Dept.

<img width="955" alt="Screenshot 2025-05-01 at 5 20 16 PM" src="https://github.com/user-attachments/assets/b3bf5ccb-ab68-435c-b00b-eb6668fe0a62" />
 In the Agents tab cick Teams, select Add New Team. I put Online Education as the team name, and select Create Team.


- Step 2: Configure Agents and Users

<img width="963" alt="Screenshot 2025-05-01 at 6 13 06 PM" src="https://github.com/user-attachments/assets/ef014e25-bf6e-4d71-97ec-e53e8524847f" />
 Click the Agents tab in the Admin panel and then Add New Agent. For the name I put James Smith, a fake email, and the username James. Click Set Password and uncheck the Send the agent a password reset email, I put in a password for James to use. Uncheck Require Password Change at next Logon, click Set.

<img width="962" alt="Screenshot 2025-05-01 at 6 19 51 PM" src="https://github.com/user-attachments/assets/4c3e3b32-a4e0-43b0-b438-72f198ac8e9f" />
 Click Access and Select Department, choose SysAdmins. For Select Role choose Admin. The permissions can stay the same, all permission should be selected. For the Teams I made James part of the Online Education Team, click Create.

<img width="953" alt="Screenshot 2025-05-01 at 6 35 44 PM" src="https://github.com/user-attachments/assets/ddd9419f-58e6-4229-8326-ed78f9d79618" />
 Click Add New Agent. For the name I put Joan Miller, a fake email, and the username Joan. Click Set Password and uncheck the Send the agent a password reset email, I put in a password for Joan to use. Again make sure Require Password Change at next Logon is unchecked, click Set. Click Access and Select Department, choose Support. For Select Role choose Expanded Access. Click Permissions and for users make sure that Delete is unchecked and do the same for Organizations. Make Joan part of the Online Education Team aswell, click Create.





 

<br />
