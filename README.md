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

<h2>Project Walk-through (Step-by-Step):</h2>

<p align="left"><b>Step 1:</b> Open Active Directory Users and Computers to begin user creation.<br/><br/>
  <img src="screenshot1.png" width="80%" alt="Step 1 Screenshot"/>
</p>

<p align="left"><b>Step 2:</b> Click “New User” and begin entering the user’s first name, last name, and username.<br/><br/>
  <img src="screenshot2.png" width="80%" alt="Step 2 Screenshot"/>
</p>

<p align="left"><b>Step 3:</b> Create and confirm a temporary password, and require the user to change it at next logon.<br/><br/>
  <img src="screenshot3.png" width="80%" alt="Step 3 Screenshot"/>
</p>

<p align="left"><b>Step 4:</b> Complete user creation by clicking “Finish”.<br/><br/>
  <img src="screenshot4.png" width="80%" alt="Step 4 Screenshot"/>
</p>

<p align="left"><b>Step 5:</b> Open the user's properties and add their job title to the Description field.<br/><br/>
  <img src="screenshot5.png" width="80%" alt="Step 5 Screenshot"/>
</p>

<p align="left"><b>Step 6:</b> Begin creating a new group that the user will belong to.<br/><br/>
  <img src="screenshot6.png" width="80%" alt="Step 6 Screenshot"/>
</p>

<p align="left"><b>Step 7:</b> Assign a name to the group (e.g., Finance Staff).<br/><br/>
  <img src="screenshot7.png" width="80%" alt="Step 7 Screenshot"/>
</p>

<p align="left"><b>Step 8:</b> Navigate to the user’s “Member Of” tab.<br/><br/>
  <img src="screenshot8.png" width="80%" alt="Step 8 Screenshot"/>
</p>

<p align="left"><b>Step 9:</b> Add the user to the group you created.<br/><br/>
  <img src="screenshot9.png" width="80%" alt="Step 9 Screenshot"/>
</p>

<p align="left"><b>Step 10:</b> Confirm group membership through the group’s “Members” tab.<br/><br/>
  <img src="screenshot10.png" width="80%" alt="Step 10 Screenshot"/>
</p>

<p align="left"><b>Step 11:</b> Repeat the process to create 10 users and 10 groups.<br/><br/>
  <img src="screenshot11.png" width="80%" alt="Step 11 Screenshot"/>
</p>

<p align="left"><b>Step 12:</b> Download the Excel and PowerShell scripts from the resources provided.<br/><br/>
  <img src="screenshot12.png" width="80%" alt="Step 12 Screenshot"/>
</p>

<p align="left"><b>Step 13:</b> Modify the PowerShell file extension from `.docx` to `.ps1`.<br/><br/>
  <img src="screenshot13.png" width="80%" alt="Step 13 Screenshot"/>
</p>

<p align="left"><b>Step 14:</b> Fill out the Excel spreadsheet with at least 15 users (first name, last name, password, OU).<br/><br/>
  <img src="screenshot14.png" width="80%" alt="Step 14 Screenshot"/>
</p>

<p align="left"><b>Step 15:</b> Move both the Excel file and PowerShell script into a shared folder, then into a Temp folder on your VM.<br/><br/>
  <img src="screenshot15.png" width="80%" alt="Step 15 Screenshot"/>
</p>

<p align="left"><b>Step 16:</b> Open PowerShell, navigate to the Temp directory, and run the import script.<br/><br/>
  <img src="screenshot16.png" width="80%" alt="Step 16 Screenshot"/>
</p>

<p align="left"><b>Step 17:</b> Confirm that the script has successfully created the users in Active Directory.<br/><br/>
  <img src="screenshot17.png" width="80%" alt="Step 17 Screenshot"/>
</p>

<p align="left"><b>Step 18:</b> Review the user list in ADUC to verify the bulk import was successful.<br/><br/>
  <img src="screenshot18.png" width="80%" alt="Step 18 Screenshot"/>
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
