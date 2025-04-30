<h1>User and Group Management</h1>

<h2>Description</h2>
This project demonstrates the process of managing users and groups in a Windows Server environment using both GUI tools (Active Directory Users and Computers) and automated scripts via PowerShell. It includes manual user creation, group assignment, and bulk importing of users from an Excel spreadsheet. These tasks reflect real-world IT administrative practices in managing organizational access control.

<br/>

<h2>Languages and Utilities Used</h2>

- <b>Windows Server (Active Directory)</b>  
- <b>PowerShell</b>  
- <b>Microsoft Excel</b>

<h2>Environments Used</h2>

- <b>Windows 10 / Windows Server VM</b>  
- <b>Hyper-V or compatible Virtualization Platform</b>


<h2>Project Walk-through:</h2>

<p align="left">
Created a new user in Active Directory by entering the required details including first name, last name, and a logon name following the "First Initial + Last Name" format.<br/><br/>
  <img src="Screenshot 2025-04-30 155151.png" height="80%" width="80%" alt="Creating New User Step 1"/>
  <br/>
<p align="left">
Assigned a temporary password and selected the option to require the user to change it at next login, ensuring secure credential setup.<br/><br/>
  <img src="Screenshot 2025-04-30 155200.png" height="80%" width="80%" alt="Password Setup"/>
  <br/>
<p align="left">
Completed the new user creation process by reviewing and confirming the summary before clicking "Finish."<br/><br/>
  <img src="Screenshot 2025-04-30 155206.png" height="80%" width="80%" alt="Finish User Creation"/>
  <br/>
<p align="left">
Opened the newly created user's properties and entered their job title in the description field for role identification.<br/><br/>
  <img src="Screenshot 2025-04-30 155212.png" height="80%" width="80%" alt="Job Description Entry"/>
  <br/>
<p align="left">
Initiated group creation to associate users with job-based access controls by assigning them to security groups.<br/><br/>
  <img src="Screenshot 2025-04-30 155242.png" height="80%" width="80%" alt="Group Creation"/>
  <br/>
<p align="left">
Selected an existing user and navigated to the "Member Of" tab to begin the group assignment process.<br/><br/>
  <img src="Screenshot 2025-04-30 155348.png" height="80%" width="80%" alt="User Group Assignment Tab"/>
  <br/>
<p align="left">
Clicked the "Add" button to search for and assign the user to the appropriate group (e.g., "Finance Staff").<br/><br/>
  <img src="Screenshot 2025-04-30 155354.png" height="80%" width="80%" alt="Add to Group"/>
  <br/>
<p align="left">
Confirmed that the group was added successfully and finalized the process by clicking "OK."<br/><br/>
  <img src="Screenshot 2025-04-30 155400.png" height="80%" width="80%" alt="Group Assignment Confirmation"/>
  <br/>
<p align="left">
Opened the group properties and checked the "Members" tab to verify the user is listed, confirming successful assignment.<br/><br/>
  <img src="Screenshot 2025-04-30 155410.png" height="80%" width="80%" alt="Verify Group Members"/>
  <br/>
<p align="left">
Repeated the previous steps until 10 users and 10 corresponding groups were created and linked appropriately.<br/><br/>
  <img src="Screenshot 2025-04-30 155428.png" height="80%" width="80%" alt="Repeat for 10 Users and Groups"/>
  <br/>
<p align="left">
Downloaded the Excel spreadsheet and PowerShell script from the course resources to prepare for bulk user creation.<br/><br/>
  <img src="Screenshot 2025-04-30 155434.png" height="80%" width="80%" alt="Download Resources"/>
  <br/>
<p align="left">
Renamed the PowerShell script from a .docx to a .ps1 file format, enabling it to be executed in PowerShell.<br/><br/>
  <img src="Screenshot 2025-04-30 155440.png" height="80%" width="80%" alt="Rename Script File"/>
  <br/>
<p align="left">
Populated the Excel spreadsheet with up to 15 users, including their first and last names, passwords, and specific OU path.<br/><br/>
  <img src="Screenshot 2025-04-30 155449.png" height="80%" width="80%" alt="Excel User Entry"/>
  <br/>
<p align="left">
Copied both the Excel file and PowerShell script to the shared folder accessible from the virtual machine.<br/><br/>
  <img src="Screenshot 2025-04-30 155457.png" height="80%" width="80%" alt="Move Files to Shared Folder"/>
  <br/>
<p align="left">
Created a folder named "Temp" on the VM and moved both files into this folder for execution.<br/><br/>
  <!-- No screenshot for this step -->
<p align="left">
Opened PowerShell and ran the following commands to execute the import script:<br/>
<code>cd C:\Temp</code><br/>
<code>dir</code><br/>
<code>.\import (press TAB to auto-complete)</code><br/><br/>
  <!-- No screenshot for this step -->
<p align="left">
Confirmed that the users listed in the Excel sheet were successfully created in Active Directory after running the script.<br/><br/>
  <img src="Screenshot 2025-04-30 155504.png" height="80%" width="80%" alt="User Import Success"/>
  <br/>
<p align="left">
Verified the newly added users within the Active Directory Users and Computers interface to ensure accuracy.<br/><br/>
  <img src="Screenshot 2025-04-30 155510.png" height="80%" width="80%" alt="User Verification"/>
  <br/>



<h2>Educational Purpose</h2>
This project provides hands-on experience in managing directory services using Active Directory and scripting with PowerShell. It simulates IT administrative workflows relevant to enterprise environments, reinforcing skills in automation, access control, and group policy management.

<h2>Real-World Relevance</h2>
Effective user and group management is critical for maintaining organizational security and efficiency. By leveraging Active Directory and PowerShell, IT professionals can implement structured, role-based access control and streamline onboarding processes at scale.

<h2>Reference</h2>
Microsoft (n.d.). Ownership and user-schema separation in SQL Server - SQL Server. SQL Server | Microsoft Learn.  
[https://learn.microsoft.com/en-us/sql/relational-databases/security/authentication-access/ownership-and-user-schema-separation](https://learn.microsoft.com/en-us/sql/relational-databases/security/authentication-access/ownership-and-user-schema-separation?view=sql-server-ver16)
