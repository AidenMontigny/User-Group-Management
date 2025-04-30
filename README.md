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
The first step is to create a new user. Once you've clicked on "New," you'll need to fill <br/> out the basic information for the user, including their first name, last name,  and user <br/> logon name. <br/><br/>
  <img src="Screenshot 2025-04-30 155151.png" height="80%" width="80%" alt="Creating New User Step 1"/>
  <br/>
<p align="left">
 After clicking 'New,' enter the user's basic information, including first name, last name,<br/> and a logon name formatted as the first initial followed by the last name. <br/><br/>
  <img src="Screenshot 2025-04-30 155200.png" height="80%" width="80%" alt="Password Setup"/>
  <br/>
<p align="left">
Next, create a logon password for the user. Be sure to select the option "User must change <br/>password at next logon" to allow the user to create their own password upon their first login. <br/><br/>
  <img src="Screenshot 2025-04-30 155206.png" height="80%" width="80%" alt="Finish User Creation"/>
  <br/>
<p align="left">
After completing the password setup, you'll be taken to the final page for creating the user.<br/> Simply click "Finish" to finalize the process, and the new user <br/> will be created. <br/><br/>
  <img src="Screenshot 2025-04-30 155212.png" height="80%" width="80%" alt="Job Description Entry"/>
  <br/>
<p align="left">
  Once the user is created, double-click on their name to open their profile. In the window <br/>that appears, enter the user’s job title in the "Description" field. <br/><br/>
  <img src="Screenshot 2025-04-30 155242.png" height="80%" width="80%" alt="Group Creation"/>
  <br/>
  <p align="left">
After assigning the user a job title, the next step is to create a corresponding group to add<br/> them to. <br/><br/>
  <img src="Screenshot 2025-04-30 155348.png" height="80%" width="80%" alt="User Group Assignment Tab"/>
  <br/>
<p align="left">
After clicking on 'Group,' a window will appear allowing you to create and name the new group. <br/><br/>
  <img src="Screenshot 2025-04-30 155354.png" height="80%" width="80%" alt="Add to Group"/>
  <br/>
  <p align="left">
Next, select the user (e.g., Caleb Mill) and navigate to the 'Member Of' tab. "<br/><br/>
  <img src="Screenshot 2025-04-30 155400.png" height="80%" width="80%" alt="Group Assignment Confirmation"/>
  <br/>
  
<p align="left">
Next, click on 'Add' and search for the designated group, 'Finance Staff,' to include the user. <br/><br/>
  <img src="Screenshot 2025-04-30 155410.png" height="80%" width="80%" alt="Verify Group Members"/>
  <br/>
<p align="left">
After clicking 'OK,' the user will be successfully added to the selected group. <br/><br/>
  <img src="Screenshot 2025-04-30 155428.png" height="80%" width="80%" alt="Repeat for 10 Users and Groups"/>
  <br/>
<p align="left">
To confirm the user was added, double-click the group and navigate to the 'Members' tab to <br/> view all current group members. <br/><br/>
  <img src="Screenshot 2025-04-30 155434.png" height="80%" width="80%" alt="Download Resources"/>
  <br/>
<p align="left">
Repeat this process until you have created 10 groups, each with a unique user assigned. <br/><br/>
  <img src="Screenshot 2025-04-30 155440.png" height="80%" width="80%" alt="Rename Script File"/>
  <br/>
<p align="left">
Download the 'PowerShell Script' and change its file extension from '.Docx' to '.PS1' to <br/> enable it to open and run properly on your VM. <br/><br/>
  <img src="Screenshot 2025-04-30 155449.png" height="80%" width="80%" alt="Excel User Entry"/>
  <br/>
<p align="left">
Next, open the 'Excel' file and add up to 15 users. For each user, enter their 'First Name,'<br/>  'Last Name,' and a 'Password.' Finally, update the Organizational Unit (OU) to  <br/>reflect your specific OU. <br/><br/>
  <img src="Screenshot 2025-04-30 155457.png" height="80%" width="80%" alt="Move Files to Shared Folder"/>
  <br/>
<p align="left">
Once completed, upload both files to your shared folder and open them on your VM. <br/><br/>
   <img src="Screenshot 2025-04-30 155504.png" height="80%" width="80%" alt="User Import Success"/>
  <br/>
<p align="left">
Open PowerShell and enter the following commands: 'cd c:\Temp,' 'Dir,' and '.\import' <br/> (press Tab to autocomplete the script path). <br/><br/>
  <!-- No screenshot for this step -->
<p align="left">
Once you execute the commands, PowerShell will automatically process them. You can then open the <br/> 'Users' file, where you will see the newly created users listed. <br/><br/>
  <img src="Screenshot 2025-04-30 155510.png" height="80%" width="80%" alt="User Verification"/>
  <br/>

<h2>Educational Purpose</h2>
This project provides hands-on experience in managing directory services using Active Directory and scripting with PowerShell. It simulates IT administrative workflows relevant to enterprise environments, reinforcing skills in automation, access control, and group policy management.

<h2>Real-World Relevance</h2>
Effective user and group management is critical for maintaining organizational security and efficiency. By leveraging Active Directory and PowerShell, IT professionals can implement structured, role-based access control and streamline onboarding processes at scale.
