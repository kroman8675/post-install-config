<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Computer)
- Remote Desktop

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

<img width="1023" alt="Screenshot 2025-05-01 at 6 48 15 PM" src="https://github.com/user-attachments/assets/df8a8075-a9e8-4004-aa60-e2b3e0dd2397" />

Click the Agent Panel at the top right of the screen. Select the Users tab and Click Add User. I have put in a fake email address and for the Full Name I put Adam Baker, Click Add useer.

- Step 3: Configure SLA's and Help Topics

<img width="955" alt="Screenshot 2025-05-01 at 6 51 50 PM" src="https://github.com/user-attachments/assets/d71a8af5-9b34-4ebb-b7d5-66c9f65d819d" />

Go back into the Admin Panel and click Manage then SLA. Click Add a New SLA Plan.

<img width="960" alt="Screenshot 2025-05-01 at 7 00 57 PM" src="https://github.com/user-attachments/assets/13fbc12b-5925-40b8-9520-c39f5116c2ba" />

For the name I put Major, set the Grace Period to 1 hour, and the schedule to 24/7. Click Add Plan.

<img width="959" alt="Screenshot 2025-05-01 at 7 09 59 PM" src="https://github.com/user-attachments/assets/c1a87c8b-eddc-4f3a-85ef-bf9141b461a9" />

Click Add a New SLA Plan.I put Modereate as the name, set the Grace Period to 4 hours, and the schedule to 24/7. Click Add Plan.

<img width="957" alt="Screenshot 2025-05-01 at 7 12 26 PM" src="https://github.com/user-attachments/assets/d55d1c2d-6c81-4c7c-bd26-74b0dfba2e77" />

Click Add a New SLA Plan. For the name I put Minor, set the Grace Period to 8 hours, and the schedule to Monday - Friday 8am - 5pm with U.S. Holidays.

<img width="955" alt="Screenshot 2025-05-01 at 7 17 50 PM" src="https://github.com/user-attachments/assets/1cac9158-1749-45eb-8816-46254adadd43" />

Select Help Topics and click Add a New Help Topic. For the topic put Business Outage and the Parent Topic as Report a Problem. Click Add Topic.

<img width="957" alt="Screenshot 2025-05-01 at 7 21 29 PM" src="https://github.com/user-attachments/assets/cec9d869-93e8-482d-83d4-573f1d9875ce" />

Select Help Topics and click Add a New Help Topic. Put PC Issues as the Topic and the Parent Topic as Report a Problem. Click Add Topic.

<img width="956" alt="Screenshot 2025-05-01 at 7 23 18 PM" src="https://github.com/user-attachments/assets/07f8eacd-1e3e-44c7-b4e4-68998c6733c1" />

Click Help Topics and select Add a New Help Topic. Put Equipment Request as the Topic and the Parent Topic as General Inquiry. Click Add Topic.

<img width="957" alt="Screenshot 2025-05-01 at 7 25 09 PM" src="https://github.com/user-attachments/assets/afb45ced-334c-4810-9010-ca42639bc6c9" />

Select Help Topics and click Add a New Help Topic. Put Password Reset as the Topic and the Parent Topic as Report a Problem / Access Issue. Click Add Topic.

<img width="958" alt="Screenshot 2025-05-01 at 7 36 15 PM" src="https://github.com/user-attachments/assets/4dc0b44c-f07c-4c80-ab72-f35e95c120fe" />

Click Help Topics and select Add a New Help Topic. Put Other as the Topic and the Parent Topic as General Inquiry. Click Add Topic.








 

<br />
