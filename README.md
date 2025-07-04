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

![image](https://github.com/user-attachments/assets/8bb10b05-1e9f-4c22-a33c-7237de8426ee)


Click the link and log in: http://localhost/osTicket/scp/login.php, and go into the Admin Panel.

<img width="955" alt="Screenshot 2025-06-28 at 7 17 27 PM" src="https://github.com/user-attachments/assets/6099e1d7-a580-4f91-acf1-c81f4ac0de24" />


Then click the Agents tab, then Roles and select Add New Roles.

<img width="956" alt="Screenshot 2025-06-28 at 7 23 48 PM" src="https://github.com/user-attachments/assets/2b9f050a-aeaa-4c80-8f1e-3075948ea494" />


Type Admin for the name and then click on the Permissions tab. In the permissions tab select all the permissions under Tickets, Tasks, and Knowledgable. After that click Add Role.

<img width="1182" alt="Screenshot 2025-05-01 at 3 16 44 PM" src="https://github.com/user-attachments/assets/035324db-bbe9-4567-b64c-5ad3d13c1ad2" />

In the Agents tab click Departments. Then click Add New Department

<img width="871" alt="Screenshot 2025-05-01 at 3 26 33 PM" src="https://github.com/user-attachments/assets/05ba494b-65a1-4ffc-8f5b-9ed9cde8320b" />

For the Parent leave it as Top Level Department. I named the Department SysAdmins and select Private for the Type, then click Create Dept.

<img width="955" alt="Screenshot 2025-05-01 at 5 20 16 PM" src="https://github.com/user-attachments/assets/b3bf5ccb-ab68-435c-b00b-eb6668fe0a62" />

In the Agents tab click Teams, select Add New Team. I put Online Education for the team name, and select Create Team.


- Step 2: Configure Agents and Users

<img width="958" alt="Screenshot 2025-06-28 at 7 30 25 PM" src="https://github.com/user-attachments/assets/58ea5679-0342-4531-bbea-c0d7ac7282be" />

In the Admin panel click the Agents tab and Agent then select Add New Agent. 

<img width="951" alt="Screenshot 2025-06-28 at 7 33 12 PM" src="https://github.com/user-attachments/assets/e0ef9630-e103-4d98-a503-705ea6fb4f28" />

For the name I put James Smith, a fake email, and the username James. 

<img width="964" alt="Screenshot 2025-06-28 at 7 36 04 PM" src="https://github.com/user-attachments/assets/d3d07371-35e7-4310-895a-6bfe54c8c877" />


Click Set Password next to the Username and uncheck the Send the agent a password reset email, I put in a password for James to use. Uncheck Require Password Change at next Logon, click Set.

<img width="962" alt="Screenshot 2025-05-01 at 6 19 51 PM" src="https://github.com/user-attachments/assets/4c3e3b32-a4e0-43b0-b438-72f198ac8e9f" />

Click the Access tab and Select Department, choose SysAdmins. For Select Role choose Admin. All permissions should be selected. 

<img width="957" alt="Screenshot 2025-06-28 at 7 41 22 PM" src="https://github.com/user-attachments/assets/433e4f15-5c68-478d-962f-0e469624bf3b" />

Select the Teams tab and click Select Team and choose the Online Education Team, click Add then Create.


<img width="956" alt="Screenshot 2025-06-28 at 7 45 02 PM" src="https://github.com/user-attachments/assets/63a74d84-4030-4c31-8292-4763f8f45956" />


I'm now going to create another Agent. Click Add New Agent. For the name I put Joan Miller, a fake email, and the username Joan. 


<img width="960" alt="Screenshot 2025-06-28 at 7 47 46 PM" src="https://github.com/user-attachments/assets/bf6b4b71-1362-4d8a-8196-235f52b663e7" />


Click Set Password and uncheck the Send the agent a password reset email, I put in a password for Joan to use. Again make sure Require Password Change at next Logon is unchecked, click Set. 


<img width="970" alt="Screenshot 2025-06-28 at 7 50 26 PM" src="https://github.com/user-attachments/assets/0bb247f7-2f64-466c-855f-b9d81b12c8cc" />


Click the Access tab and for Select Department, choose Support. For Select Role choose Expanded Access. 


<img width="1440" alt="Screenshot 2025-06-28 at 7 53 33 PM" src="https://github.com/user-attachments/assets/b7214dcb-34b0-492e-80e5-f714ce38c26a" />

Click Permissions and for Users make sure that Delete is unchecked and do the same for Organization. Make Joan part of the Online Education Team aswell, click Create.


<img width="960" alt="Screenshot 2025-06-28 at 7 57 54 PM" src="https://github.com/user-attachments/assets/df3f1af9-f27e-4043-8ae2-56f58acdc7d5" />


Now let's create a user. To get started click the Agent Panel.


<img width="1423" alt="Screenshot 2025-06-28 at 8 00 31 PM" src="https://github.com/user-attachments/assets/5cbc719f-5869-4829-b3b0-ce8fd18bb378" />


Select the Users tab and Click Add User. I put in a fake email address and for the Full Name I put Adam Baker, Click Add user.

- Step 3: Configure SLA's and Help Topics

<img width="955" alt="Screenshot 2025-05-01 at 6 51 50 PM" src="https://github.com/user-attachments/assets/d71a8af5-9b34-4ebb-b7d5-66c9f65d819d" />

Go back into the Admin Panel and click the Manage tab then SLA. Click Add a New SLA Plan.

<img width="960" alt="Screenshot 2025-05-01 at 7 00 57 PM" src="https://github.com/user-attachments/assets/13fbc12b-5925-40b8-9520-c39f5116c2ba" />

For the name I put Major, set the Grace Period to 1 hour, and the schedule to 24/7. Click Add Plan.

<img width="959" alt="Screenshot 2025-05-01 at 7 09 59 PM" src="https://github.com/user-attachments/assets/c1a87c8b-eddc-4f3a-85ef-bf9141b461a9" />

Click Add a New SLA Plan. Set the name to Modereate, set the Grace Period to 4 hours, and the schedule to 24/7. Click Add Plan.

<img width="957" alt="Screenshot 2025-05-01 at 7 12 26 PM" src="https://github.com/user-attachments/assets/d55d1c2d-6c81-4c7c-bd26-74b0dfba2e77" />

Click Add a New SLA Plan. For the name I put Minor, set the Grace Period to 8 hours, and the schedule to Monday - Friday 8am - 5pm with U.S. Holidays. Click Add Plan.

<img width="955" alt="Screenshot 2025-05-01 at 7 17 50 PM" src="https://github.com/user-attachments/assets/1cac9158-1749-45eb-8816-46254adadd43" />

Now select the Help Topics tab and click Add a New Help Topic. For the topic I put Business Outage and the Parent Topic as Report a Problem. Click Add Topic.

<img width="957" alt="Screenshot 2025-05-01 at 7 21 29 PM" src="https://github.com/user-attachments/assets/cec9d869-93e8-482d-83d4-573f1d9875ce" />

Select the Help Topics tab and click Add a New Help Topic. Put PC Issues as the Topic and the Parent Topic as Report a Problem. Click Add Topic.

<img width="956" alt="Screenshot 2025-05-01 at 7 23 18 PM" src="https://github.com/user-attachments/assets/07f8eacd-1e3e-44c7-b4e4-68998c6733c1" />

Click Help Topics tab and select Add a New Help Topic. Put Equipment Request as the Topic and the Parent Topic as General Inquiry. Click Add Topic.

<img width="957" alt="Screenshot 2025-05-01 at 7 25 09 PM" src="https://github.com/user-attachments/assets/afb45ced-334c-4810-9010-ca42639bc6c9" />

Select Help Topics tab and click Add a New Help Topic. Put Password Reset as the Topic and the Parent Topic as Report a Problem / Access Issue. Click Add Topic.

<img width="958" alt="Screenshot 2025-05-01 at 7 36 15 PM" src="https://github.com/user-attachments/assets/4dc0b44c-f07c-4c80-ab72-f35e95c120fe" />

Click the Help Topics and select Add a New Help Topic. This will be out last Help Topic, put Other as the Topic and the Parent Topic as General Inquiry. Click Add Topic. Our ticketing System is now configured!









 

<br />
