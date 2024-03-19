<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles
- Configure Departments
- Configure Teams
- Configure Agents (workers)
- Configure Users (customers)
- Configure SLA
- Configure Help Topics

<h2>Configuration Steps</h2>

![Screenshot 2024-03-13 at 9 41 43 AM](https://github.com/ory-it/post-install-config/assets/67742620/36cdfcf1-d22f-4a29-92c3-32c3354cf249)
<h3>Configure Roles</h3>

a. Admin Panel -> Agents -> Roles <br/>
b. Supreme Admin
<p>
  To create an administrator role in osTicket, first log into the Admin Panel, then navigate to the Agents section where you'll find options for roles and permissions. Here, you can create a new role by selecting "Add New Role" or a similar option, naming it (e.g., "Administrator"), and setting the desired permissions that typically include full access to the system's features like viewing and responding to tickets, managing users, and configuring settings. After saving the role, assign it to individual staff members by editing their profiles to ensure they have the appropriate level of access.
</p>
<br/>


![Screenshot 2024-03-13 at 9 46 21 AM](https://github.com/ory-it/post-install-config/assets/67742620/24976789-63bf-403b-a877-05315aeb100c)
<h3>Configure Departments</h3>

a. Admin Panel -> Agents -> Departments <br/>
b. System Administrators
<p>
  Creating a department role involves accessing the Admin Panel with administrator credentials and navigating to the "Departments" section, where you can manage department-specific settings. Here, you'll find the option to either modify an existing department or create a new one, which involves specifying the department's name, its manager, and the role's permissions related to ticket handling, such as ticket assignment, response capabilities, and access to department-specific data. It's important to carefully configure these permissions to ensure that agents within the department have the appropriate level of access and capabilities for efficient ticket management. After setting up the department and its roles, assign agents to ensure they're equipped with the necessary permissions to fulfill their responsibilities, and conduct a review or a test run to confirm that the configuration aligns with your operational requirements.
</p>
<br/>


![Screenshot 2024-03-13 at 9 47 52 AM](https://github.com/ory-it/post-install-config/assets/67742620/79fa6cc2-23af-4bac-8d34-8c31c5d793fb)
<h3>Configure Teams</h3>

a. Admin Panel -> Agents -> Teams
  - Level I Support
  - Level II Support
<p>
 To configure Level 1 and Level 2 support teams in osTicket, start by logging into the Admin Panel with sufficient privileges and navigate to the "Teams" section, depending on how you wish to structure your support tiers. For a team-based approach, create two teams named "Level 1 Support" and "Level 2 Support," and define their roles and permissions accordingly—Level 1 Support might have permissions for initial ticket response and basic troubleshooting, while Level 2 Support is granted additional permissions for handling more complex issues that require advanced technical knowledge. Assign staff members to these teams based on their skills and expertise. It's crucial to define the escalation rules or triggers within osTicket's system to automate the process where possible, ensuring smooth and effective ticket escalation from Level 1 to Level 2 support.
</p>
<br/>


![Screenshot 2024-03-13 at 9 50 09 AM](https://github.com/ory-it/post-install-config/assets/67742620/7c303624-3704-484a-8ab1-0e5b04d1986a)
<h3>Allow anyone to create tickets</h3>

a. Admin Panel -> Settings -> User Settings <br/>
b. Registration Required: Require registration and login to create tickets 
<p>
 To enable anyone to create tickets in osTicket, ensuring that your support platform is accessible to all users, including non-registered individuals, you'll need to adjust the system's ticket submission settings. Log in to the Admin Panel with administrative rights and navigate to the "Settings" section, where you'll find options related to ticket submission. Look for settings labeled "User Settings". Enable the option that allows tickets to be created by non-registered or guest users. This adjustment removes the requirement for users to create an account before submitting a ticket, thereby broadening access to your support services. After making these changes, save your settings and consider conducting a test to verify that external users can successfully submit tickets without needing to log in or register, ensuring your support system is truly open to all.
</p>
<br/>


![Screenshot 2024-03-13 at 9 55 45 AM](https://github.com/ory-it/post-install-config/assets/67742620/71fba146-e148-4b5a-a284-b33c2e50a64f)
<h3>Configure Agents (workers)</h3>

a. Admin Panel -> Agents -> Add New
  - Jane
  - John
<p>
  To create agents "Jane Doe" and "John Doe" in osTicket, you'll need to access the Admin Panel with administrator privileges and head to the "Agents". In this area, look for an option to "Add New". Click on this to start the agent creation process, where you'll be prompted to enter details such as the agent's full name, email address, and assigned department or team. For "Jane Doe" and "John Doe," fill in their respective names in the designated fields, along with unique email addresses for each to ensure they can receive notifications and communicate within the system. Additionally, set their roles and permissions according to their responsibilities within your support team, and assign them to the appropriate departments or teams if your support structure requires it. After filling in all necessary information and configuring their accounts, save your changes to finalize the creation of the agents.
</p>
<br/>


![Screenshot 2024-03-13 at 9 59 48 AM](https://github.com/ory-it/post-install-config/assets/67742620/c2c5d475-8b40-4f16-8b1d-dedf174a810f)
<h3>Configure Users (customers)</h3>

a. Agent Panel -> Users -> Add New
  - Rick Snachez
  - Morty Smith
<p>
  To create users "Rick Snachez" and "Morty Smith" in osTicket, typically intended for individuals who will be submitting tickets or need access to the client side of the system, you'll start by logging into the osTicket Agent Panel with appropriate administrative rights. Once logged in, navigate to the section dedicated to managing users or clients, often labeled as "Users". Within this section, find the option to "Add New", which will lead you to a form where you can input user details. For creating "Karen" and "Ken," enter their full names, email addresses, and any other required information such as phone numbers or user roles. After completing the details for each user, save your changes to create their profiles in the system. This process allows Karen and Ken to start submitting tickets to your support team and engage with your support services.
</p>
<br/>


![Screenshot 2024-03-13 at 10 02 06 AM](https://github.com/ory-it/post-install-config/assets/67742620/5fc805e2-cc54-415b-b097-792ef8eea349)
<h3>Configure SLA</h3>

a. Admin Panel -> Manage -> SLA
  - Sev-A (1 hour, 24/7)
  - Sev-B (4 hours, 24/7)
  - Sev-C (8 hours, business hours)
<p>
  To configure a Service Level Agreement (SLA) in osTicket, ensuring timely responses and resolutions for tickets, begin by logging into the Admin Panel with administrative credentials. Navigate to the "SLA Plans" section, where you can manage existing SLAs or create new ones. To set up a new SLA, click on an option like "Add New SLA" or "Create SLA Plan," which will prompt you to define specific parameters such as the SLA name, the duration within which a ticket must be addressed (e.g., response and resolution times), and the conditions under which this SLA will be applied (such as ticket priority or department). You may also specify the working hours if your SLA needs to account for business hours only. After filling in these details, save the SLA plan. The final step involves assigning this SLA to relevant tickets, which can be done automatically based on the conditions you've set or manually by agents when creating or updating tickets. Properly configured SLAs help ensure that your team meets expected service standards and provides timely support to users.
</p>
<br/>


![Screenshot 2024-03-13 at 10 04 13 AM](https://github.com/ory-it/post-install-config/assets/67742620/1362254b-c2e0-479d-8f45-e6d4ec933da3)
<h3>Configure Help Topics</h3>

a. Admin Panel -> Manage -> Help Topics
  - Business Critical Outage
  - Personal Computer Issues
  - Equipment Request
  - Password Reset
<p>
  In osTicket, configuring Help Topics involves defining specific categories or issues that users can select when submitting a ticket, which helps streamline the support process by directing tickets to the appropriate department or staff member. To set this up, log into the Admin Panel with administrative rights and navigate to the "Manage" section, where you'll find an option for "Help Topics." Here, you can either edit existing topics or create new ones by clicking on "Add New". When creating a new Help Topic, you'll be prompted to enter details such as the topic name (for example, "Business Critical Outage" or "Personal Computer Issues"), the department it should be routed to, the SLA plan associated with it, and any custom form fields that should be presented to the user when selecting this topic. Additionally, you can configure auto-response settings and other behaviors specific to each topic. After setting up your Help Topics, remember to save your changes. This configuration not only aids users in categorizing their issues accurately but also allows your support team to prioritize and respond to tickets more efficiently.
</p>
<br/>

