<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop (now Windows App)
- Internet Information Services (IIS)
- osTicket

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)
- macOS Sequoia

<h2>Post-Install Configuration Objectives</h2>

- 1: Admin/ Analyst Login Page vs End Users Pages
- 2: Roles
- 3: Departments
- 4: Teams
- 5: Agents
- 6: Users
- 7: SLA
- 8: Help Topics

  <h2>Configuration Steps</h2>

<h3>Section 1: Admin/ Analyst Login Page vs End Users Pages</h3>
<br />
<table>
  <tr>
    <td>
     
   <img width="1440" alt="Screenshot 2025-06-04 at 12 59 32 PM" src="https://github.com/user-attachments/assets/9d77077a-b156-4570-945d-3799865e53c9" />
<br />
<p>- This is the staff control panel, used by admins and help desk agents. They see tickets come in here and can do several other things in this system. .</p>


<table>
  <tr>
    <td>
      <img width="1440" alt="Screenshot 2025-06-04 at 12 54 56 PM" src="https://github.com/user-attachments/assets/aaeeb7ca-6a6b-46af-82ad-0691d42725a8" />

  <br />
  </tr>
</table>
<p>- This is the end users page. Here they can submit tickets.</p>

<br />
<h3>Section 2: Roles</h3>
<br />
<table>
  <tr>
    <td>
      <img width="1440" alt="Screenshot 2025-06-04 at 11 53 13 AM" src="https://github.com/user-attachments/assets/3ecfb9b2-5abc-4307-97c0-6457dd60600f" />
<img width="1440" alt="Screenshot 2025-06-04 at 11 53 53 AM" src="https://github.com/user-attachments/assets/9eb2f13b-927c-45f1-9e7b-e8ffbd9e6f47" />

  <br />
  </tr>
</table>
<p>- Configure a new role within the Admin Panel. (Remember, "Agent Panel" will display in the top-right of your screen while in the Admin Panel.)</p> 
<p>- Within Admin Panel, go to  Agents, then Roles. From there, you'll press add new role.</p> 
<p>- Title the new role "Supreme Admin" and click the Permissions tab.</p>
<p>- To make the Supreme Admin have all the permissions, go to tickets, tasks, and knowledgebase and select all boxes. .</p>
<br />
<img width="1440" alt="Screenshot 2025-06-04 at 11 53 53 AM" src="https://github.com/user-attachments/assets/7fa917ac-edaf-4207-8cd6-0261113b23e0" />

<br/>



<p>- Next, we'll add a new Department.</p>
<br />
<h3>Section 3: Departments</h3>
<br />
<table>
  <tr>
    <td>
<img width="1440" alt="Screenshot 2025-06-04 at 11 55 36 AM" src="https://github.com/user-attachments/assets/7ded4896-7e3c-4c7d-af2e-82722ec9e43b" />

  
   
  </tr>
</table>
<p>- Within Admin Panel, click Agents -> Departments -> + Add New Department.</p>
<p>- Under Settings, leave Parent as "Top-Level Department" and name the department "SysAdmins".</p>

<p>

</p>

<p>- The SysAdmins Department has been successfully added. </p>
<br />

<h3>Section 4: Teams</h3>

<table>
 <img width="1440" alt="Screenshot 2025-06-04 at 11 56 39 AM" src="https://github.com/user-attachments/assets/5831a7b6-17ae-45d7-b79f-0902162ff06c" />

</table>
<p>- Now, we'll add a new Team. Within Admin Panel, click Agents -> Teams -> + Add New Team.</p>
<p>- Name the Team "Online Banking". </p>
<p>- We'll will add members when we add Agents later. Click Create Team.</p>
<p>- You can learn more about Teams within osTicket by clicking the link in the Post-Install Configuration Objectives above.</p>



<p>- Next, we'll change a setting that will allow somone to create a ticket without having to register an account. The end user will be able to create thier own ticket. </p>
<p>- From Admin Panel, click Agents -> Settings -> Users. </p>
<p>- Under Authentication Settings, uncheck the box next to "Require registration and login to create tickets". Click Save Changes.</p>
<br />
<img width="1440" alt="Screenshot 2025-06-04 at 11 58 04 AM" src="https://github.com/user-attachments/assets/3d6b5c98-066c-41e9-b53b-4904d4c3a51b" />


<h3>Section 5: Agents </h3>

<img width="1440" alt="Screenshot 2025-06-04 at 12 01 28 PM" src="https://github.com/user-attachments/assets/8f1d8124-f951-416f-8453-8430bdf8960d" />
<img width="1440" alt="Screenshot 2025-06-04 at 12 01 34 PM" src="https://github.com/user-attachments/assets/31e58cdf-4540-4671-be8e-dd08e77cf08d" />



<p>- Time to add some Agents. From Admin Panel, click -> Agents -> Agents -> + Add New Agent. </p>
<p>- Under Account, name the Agent "Jane Doe". Enter an email (I did jane@lognpacific.com).  </p>
<p>- Username: jane_doe </p>
<p>- Click Set Password. </p>

<p>- Do the same thing and add John Doe. I used the email john@lognpacific.com. </p>


<h3>Section 6: Users </h3>
<img width="1440" alt="Screenshot 2025-06-04 at 12 04 47 PM" src="https://github.com/user-attachments/assets/6d263665-6aa7-464d-99bd-ac10d0882026" />

<p>- Now, we need to add a User. Click Agent Panel at the top-right of the screen.</p>
<p>- From Agent Panel, click Users -> + Add User.  </p>
<p>- Enter email address: karen@lonpacific.com (Fake Email).</p>
<p>- Name the User "Karen" and click Add User. </p>
<br/>


<p>- Karen has been added as a User.</p>
<p>- We'll have Karen creating tickets for our Agents in the next project. </p>
<p>- Set a password. Uncheck "Require password change at next login". Click Update. Do the same steps to add Ken.  </p>

<br/>

<h3>Section 7: Service Level Agreements (SLA)</h3>

<p>
<img width="1440" alt="Screenshot 2025-06-04 at 12 05 10 PM" src="https://github.com/user-attachments/assets/df143a41-6954-4a0e-8761-cd3b11c04bc8" />

</p>

<p>- The purpose of the SLA Plan is to provide a length of time in which the help desk Administrator expects tickets to be closed.</p>
<p>- From Agent Panel, click Manage -> SLA -> + Add New SLA Plan.</p>
<br/>



<p>- Name: "Sev-A" | Grace Period: 1 hour | Schedule: 24/7</p>
<p>- Click Add Plan.</p>
<br/>

<p>
  <img width="1440" alt="Screenshot 2025-06-04 at 12 06 30 PM" src="https://github.com/user-attachments/assets/ab6f1699-fa70-4f9f-b9cf-cddc8964317a" />

</p>

<p>- Name: "Sev-B" | Grace Period: 4 hours | Schedule: 24/7</p>
<p>- Click Add Plan.</p>
<br/>



<p>- Name: "Sev-C" | Grace Period: 8 hours | Schedule: Monday - Friday, 8am - 5pm with Holidays. (Normal business hours)</p>
<p>- Click Add Plan.</p>
<br/>



<p>- The SLA Plans have been successfully added. We will use these when creating and working tickets in the next project.</p>

<br/>
<img width="1440" alt="Screenshot 2025-06-04 at 12 07 33 PM" src="https://github.com/user-attachments/assets/e4cda515-689a-4e8a-b9dc-d79a6d91bb93" />


<h3>Section 8: Help Topics</h3>

  <img width="1440" alt="Screenshot 2025-06-04 at 12 09 52 PM" src="https://github.com/user-attachments/assets/50bde65e-d761-4898-990c-55736cd63fa0" />



<p>- For the final section of this project, we will add some Help Topics.</p>
<p>- From Agent Panel, click Manage -> Help Topics -> + Add New Help Topic. <p/>
<br/>

<table>
  
</table>
<p>- Under Help Topic Information, Topic: Buisness Critical Outage | Parent Topic: Report a Problem. See Figure 35</p>
<p>- Click Add Topic.  </p>
<p>- Under Help Topic Information, Topic: Personal Computer Issues | Parent Topic: Report a Problem. See Figure 36</p>
<img width="1440" alt="Screenshot 2025-06-04 at 12 08 36 PM" src="https://github.com/user-attachments/assets/d05cc889-1702-443c-8bdd-59bbe934c9fc" />

<p>- Click Add Topic.</p>


<br/>

<table>

</table>
<p>- Under Help Topic Information, Topic: Equipment Request | Parent Topic: General Inquiry. See Figure 37</p>
<p>- Click Add Topic. </p>
<p>- Under Help Topic Information, Topic: Password Reset | Parent Topic: Report a Problem. See Figure 38</p>
<p>- Click Add Topic. </p>
<br/>



<p>- Under Help Topic Information, Topic: Other | Parent Topic: General Inquiry. See Figure 39</p>
<p>- Click Add Topic.  </p>
<p>- We have now created 5 different topics. 

<h2>Conclusion</h2>

<p>This concludes our project. We have successfully completed the post-install configurations for osTicket. We will put our settings to the test in the next lab when we create and work tickets as a User, Agent, and Admin.
</p>
<br />

























