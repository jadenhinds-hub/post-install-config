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

<table>
  <tr>
    <td>
     
   <img width="1440" alt="Screenshot 2025-06-04 at 12 59 32 PM" src="https://github.com/user-attachments/assets/9d77077a-b156-4570-945d-3799865e53c9" />

<p>- This is the staff control panel, used by admins and help desk agents. They see tickets come in here and can do several other things in this system. .</p>


<table>
  <tr>
    <td>
      <img width="1440" alt="Screenshot 2025-06-04 at 12 54 56 PM" src="https://github.com/user-attachments/assets/aaeeb7ca-6a6b-46af-82ad-0691d42725a8" />

  
  </tr>
</table>
<p>- This is the end users page. Here they can submit tickets.</p>


<h3>Section 2: Roles</h3>

<table>
  <tr>
    <td>
      <img width="1440" alt="Screenshot 2025-06-04 at 11 53 13 AM" src="https://github.com/user-attachments/assets/3ecfb9b2-5abc-4307-97c0-6457dd60600f" />
<img width="1440" alt="Screenshot 2025-06-04 at 11 53 53 AM" src="https://github.com/user-attachments/assets/9eb2f13b-927c-45f1-9e7b-e8ffbd9e6f47" />

  
  </tr>
</table>
<p>- Configure a new role within the Admin Panel. (Remember, "Agent Panel" will display in the top-right of your screen while in the Admin Panel.)</p> 
<p>- Within Admin Panel, go to  Agents, then Roles. From there, you'll press add new role.</p> 
<p>- Title the new role "Supreme Admin" and click the Permissions tab.</p>
<p>- To make the Supreme Admin have all the permissions, go to tickets, tasks, and knowledgebase and select all boxes. .</p>
<img width="1440" alt="Screenshot 2025-06-04 at 11 53 53 AM" src="https://github.com/user-attachments/assets/7fa917ac-edaf-4207-8cd6-0261113b23e0" />

<br/>



<p>- Next, we'll add a new Department.</p>

<h3>Section 3: Departments</h3>

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

<h3>Section 6: Service Level Agreements (SLA)</h3>

<p>
<img width="750" alt="PI29" src="https://github.com/user-attachments/assets/a7b03923-b42d-4cc0-bcbb-b07a5c0a23e4" />
</p>

<p>- The purpose of the SLA Plan is to provide a length of time in which the help desk Administrator expects tickets to be closed.</p>
<p>- From Agent Panel, click Manage -> SLA -> + Add New SLA Plan.</p>
<br/>

<p>
<img width="750" alt="PI30" src="https://github.com/user-attachments/assets/88a03023-8a2e-4ccb-ac6b-b05cd4e11d9c" />
</p>

<p>- Name: "Sev-A" | Grace Period: 1 hour | Schedule: 24/7</p>
<p>- Click Add Plan.</p>
<br/>

<p>
<img width="750" alt="PI31" src="https://github.com/user-attachments/assets/4e4c2490-7452-4493-90ff-00fbeb4e47a2" />
</p>

<p>- Name: "Sev-B" | Grace Period: 4 hours | Schedule: 24/7</p>
<p>- Click Add Plan.</p>
<br/>

<p>
<img width="750" alt="PI32" src="https://github.com/user-attachments/assets/bda12229-512b-42be-9b98-dffceb4b7062" />
</p>

<p>- Name: "Sev-C" | Grace Period: 8 hours | Schedule: Monday - Friday, 8am - 5pm with Holidays. (Normal business hours)</p>
<p>- Click Add Plan.</p>
<br/>

<p>
<img width="750" alt=<img width="975" alt="PI33" src="https://github.com/user-attachments/assets/49b09cf1-5465-4fa0-9b5d-5ce2eb5996c6" />
</p>

<p>- The SLA Plans have been successfully added. We will use these when creating and working tickets in the next project.</p>
<p>- You can learn more about Service Level Agreements within osTicket by clicking the link in the Post-Install Configuration Objectives above.<p/>
<br/>

<h3>Section 7: Help Topics</h3>

<p>
<img width="750" alt="PI34" src="https://github.com/user-attachments/assets/6194a8bb-0051-46e3-b109-f50b3938e254" />
</p>

<p>- For the final section of this project, we will add some Help Topics.</p>
<p>- From Agent Panel, click Manage -> Help Topics -> + Add New Help Topic. <p/>
<br/>

<table>
  <tr>
    <td>
      <img width="1000" alt="PI35" src="https://github.com/user-attachments/assets/9df07a0d-2cbd-4ee1-9886-aff4c4f42304" />
    </td>
    <td>
      <img width="1000" alt="PI36" src="https://github.com/user-attachments/assets/51bc7442-76e0-47ae-9f11-ad9da82ea9e8" />
    </td>
  </tr>
</table>
<p>- Under Help Topic Information, Topic: Buisness Critical Outage | Parent Topic: Report a Problem. See Figure 35</p>
<p>- Click Add Topic.  </p>
<p>- Under Help Topic Information, Topic: Personal Computer Issues | Parent Topic: Report a Problem. See Figure 36</p>
<p>- Click Add Topic.</p>
<br/>

<table>
  <tr>
    <td>
      <img width="1000" alt="PI37" src="https://github.com/user-attachments/assets/8e46c387-782d-4c93-8634-8deb4f3e0eb9" />
    </td>
    <td>
      <img width="1000" alt="PI38" src="https://github.com/user-attachments/assets/44622da8-fd2a-4d81-8677-18cfec813ff6" />
    </td>
  </tr>
</table>
<p>- Under Help Topic Information, Topic: Equipment Request | Parent Topic: General Inquiry. See Figure 37</p>
<p>- Click Add Topic. </p>
<p>- Under Help Topic Information, Topic: Password Reset | Parent Topic: Report a Problem. See Figure 38</p>
<p>- Click Add Topic. </p>
<br/>

<table>
  <tr>
    <td>
      <img width="1000" alt="PI39" src="https://github.com/user-attachments/assets/2c81095c-4f59-4c35-8056-8e19460a5c69" />
    </td>
    <td>
      <img width="1000" alt="PI40" src="https://github.com/user-attachments/assets/77f141a2-0575-4ece-9140-e571d166cd1b" />
    </td>
  </tr>
</table>
<p>- Under Help Topic Information, Topic: Other | Parent Topic: General Inquiry. See Figure 39</p>
<p>- Click Add Topic.  </p>
<p>- Look at all those Topics!. If you noticed, osTicket already had some deafult Help Topics preloaded for us but adding new ones gave us a chance to learn more about the process.</p>
<p>- You can learn more about Help Topics within osTicket by clicking the link in the Post-Install Configuration Objectives above.<p/>
<br/>

<h2>Conclusion</h2>

<p>This concludes our project. We have successfully completed the post-install configurations for osTicket. We will put our settings to the test in the next lab when we create and work tickets as a User, Agent, and Admin. Don't forget to Stop (turn off) the VMs in Azure. As always, Thank You for your time and viewing this Project. We'll see you on the next one! 😎      
</p>
<br />

























