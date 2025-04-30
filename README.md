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

<h2>Project Walk-through</h2>

Begin by launching Active Directory Users and Computers and selecting the option to create a new user.

Fill in the user's basic details, including first name, last name, and a user logon name formatted as the first initial followed by the last name (e.g., jdoe).

Set a temporary password for the user and enable the option requiring them to change the password at next logon to enhance account security.

Finalize the user creation process by reviewing the summary screen and clicking "Finish."

After the user is created, open their profile properties and enter their job title in the Description field for easier identification and organization.

Next, proceed to create a new security group. Provide a meaningful name that reflects the department or team (e.g., "Finance Staff").

Navigate to the user's account, access the "Member Of" tab, and click "Add" to include them in the newly created group.

Search for the appropriate group name, confirm the selection, and apply the changes to officially assign the user to the group.

To verify group membership, open the group’s properties and check the “Members” tab to ensure the user appears on the list.

Repeat this process until you have created a total of 10 users and 10 corresponding groups, ensuring each user is added to a relevant group.

Transitioning to bulk user creation, start by downloading the Excel and PowerShell script files provided in your course resources.

Rename the downloaded PowerShell file from .docx to .ps1 to make it executable in PowerShell.

Open the Excel file and enter data for up to 15 users, including first names, last names, and passwords. Make sure to update the OU (Organizational Unit) field to reflect your specific environment.

Once the spreadsheet is complete, move both the Excel file and the PowerShell script into a shared directory accessible from your VM.

Inside your VM, create a new folder called “Temp” and copy both files from the shared location into this folder for easier access.

Launch PowerShell, navigate to the Temp directory using 'cd C:\Temp', and confirm the contents using the 'dir' command. Then run the script by typing '.\import' and pressing Tab to auto-complete the filename.

PowerShell will execute the script, read the Excel file, and create each user account automatically based on your input data.

To confirm successful account creation, open Active Directory Users and Computers and verify that the new users appear in the correct Organizational Unit.

<h2>Educational Purpose</h2>
This project provides hands-on experience in managing directory services using Active Directory and scripting with PowerShell. It simulates IT administrative workflows relevant to enterprise environments, reinforcing skills in automation, access control, and group policy management.

<h2>Real-World Relevance</h2>
Effective user and group management is critical for maintaining organizational security and efficiency. By leveraging Active Directory and PowerShell, IT professionals can implement structured, role-based access control and streamline onboarding processes at scale.

<h2>Reference</h2>
Microsoft (n.d.). Ownership and user-schema separation in SQL Server - SQL Server. SQL Server | Microsoft Learn.  
[https://learn.microsoft.com/en-us/sql/relational-databases/security/authentication-access/ownership-and-user-schema-separation](https://learn.microsoft.com/en-us/sql/relational-databases/security/authentication-access/ownership-and-user-schema-separation?view=sql-server-ver16)
