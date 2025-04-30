<h1>User and Group Management</h1>

<h2>Description</h2>
This project demonstrates the process of managing users and groups within a Windows Server environment using both GUI tools (Active Directory Users and Computers) and automated PowerShell scripting. It is designed as a hands-on educational assignment to teach key concepts in IT system administration, including user creation, group assignment, OU configuration, and scripting automation.

The project begins with the manual creation of users and groups via the ADUC interface, followed by bulk user creation using an Excel file and a PowerShell script. It emphasizes structured organizational unit (OU) usage and proper permission assignment through group schemas. These concepts reflect real-world practices in corporate IT environments for secure and scalable identity management.


<h2>Languages and Utilities Used</h2>

- <b>Windows Server (Active Directory)</b>  
- <b>PowerShell</b>  
- <b>Microsoft Excel</b>

<h2>Environments Used</h2>

- <b>Windows 10 / Windows Server VM (Virtual Machine)</b>  
- <b>Hyper-V or other Virtualization Software</b>

<h2>Project Walk-through:</h2>

<p align="left">
<b>Step 1:</b> Create a New User in Active Directory.<br/>
- Fill out required fields: First Name, Last Name, and User Logon Name (First Initial + Last Name).<br/>
- Assign a temporary password and enable "User must change password at next logon".<br/>
- Click "Finish" to complete the user creation.<br/><br/>
</p>

<p align="left">
<b>Step 2:</b> Edit User Properties.<br/>
- Open the user’s properties.<br/>
- In the “Description” field, input their job title (e.g., "Finance Specialist").<br/><br/>
</p>

<p align="left">
<b>Step 3:</b> Create and Assign a Group.<br/>
- Navigate to the Groups section and create a new group (e.g., “Finance Staff”).<br/>
- Go to the user’s “Member Of” tab and add them to the appropriate group.<br/>
- Verify group membership via the group’s “Members” tab.<br/><br/>
</p>

<p align="left">
<b>Step 4:</b> Repeat the process for 10 unique users and 10 groups.<br/><br/>
</p>

<h3>Automated User Creation with PowerShell:</h3>

<p align="left">
<b>Step 5:</b> Bulk Import Users via PowerShell Script.<br/>
- Convert the provided PowerShell script from <code>.docx</code> to <code>.ps1</code>.<br/>
- Update the accompanying Excel sheet with up to 15 users, specifying First Name, Last Name, Password, and OU.<br/>
- Copy both files into a shared folder, then into a "Temp" folder on the VM.<br/><br/>
</p>

<p align="left">
<b>Step 6:</b> Run the PowerShell Script.<br/>
- Open PowerShell and run the following commands:<br/>
  <code>cd C:\Temp</code><br/>
  <code>dir</code><br/>
  <code>.\import-users.ps1</code> (use Tab to autocomplete)<br/>
- Users will be created in Active Directory according to the Excel data.<br/><br/>
</p>

<h2>Educational Purpose</h2>

This project reinforces the importance of:
- Centralized user and group management
- Role-based access control
- The efficiency of automation in system administration
- Understanding user/group schema implementation in enterprise IT settings

<h2>Real-World Relevance</h2>

User and group schemas are foundational in any corporate IT infrastructure. They enable secure, scalable access management and simplify administrative tasks by assigning permissions based on group roles. Tools like Active Directory and PowerShell are widely used in industry, making this project directly applicable to real-world scenarios.

<h2>Reference</h2>

Microsoft (n.d.). Ownership and user-schema separation in SQL Server - SQL Server. SQL Server | Microsoft Learn.  
[https://learn.microsoft.com/en-us/sql/relational-databases/security/authentication-access/ownership-and-user-schema-separation](https://learn.microsoft.com/en-us/sql/relational-databases/security/authentication-access/ownership-and-user-schema-separation?view=sql-server-ver16)
