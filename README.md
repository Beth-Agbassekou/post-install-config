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

- Setup a Supreme Admin Role
- Setup a Team
- Create Users and Agents
- Create SLAs
- Create Help Topics

<h2>Configuration Steps</h2>

<p>
<img width="1440" alt="Screenshot 2023-11-26 at 3 35 08 PM" src="https://github.com/Beth-Agbassekou/post-install-config/assets/148320585/0d3d4067-21e1-4d72-b773-9a900eecd83d">
<img width="1440" alt="Screenshot 2023-11-26 at 3 35 51 PM" src="https://github.com/Beth-Agbassekou/post-install-config/assets/148320585/62a54328-5564-45ae-8108-d41fc334726d">

<img width="1440" alt="Screenshot 2023-11-26 at 3 35 08 PM" src="https://github.com/Beth-Agbassekou/post-install-config/assets/148320585/0d3d4067-21e1-4d72-b773-9a900eecd83d">
<img width="1440" alt="Screenshot 2023-11-26 at 3 35 51 PM" src="https://github.com/Beth-Agbassekou/post-install-config/assets/148320585/62a54328-5564-45ae-8108-d41fc334726d">
<img width="1440" alt="Screenshot 2023-11-26 at 3 39 04 PM" src="https://github.com/Beth-Agbassekou/post-install-config/assets/148320585/65b40721-b596-4dbe-b82e-dc159a964208">
<img width="1440" alt="Screenshot 2023-11-26 at 3 39 12 PM" src="https://github.com/Beth-Agbassekou/post-install-config/assets/148320585/14a377bf-2d73-49bc-b67d-41efd126591d">
<img width="1440" alt="Screenshot 2023-11-26 at 3 39 19 PM" src="https://github.com/Beth-Agbassekou/post-install-config/assets/148320585/176f2299-21dc-48e3-a0f9-e806fbda3f11">
<img width="1440" alt="Screenshot 2023-11-26 at 3 42 28 PM" src="https://github.com/Beth-Agbassekou/post-install-config/assets/148320585/97d99942-d02d-4472-9f58-fc5279ef73df">
</p>
<p>
The first thing I did was set up a role called Supreme Admin, to practice setting permissions. When creating the role of Supreme Admin I wanted to allow all permissions to test how roles work. I allowed all permissions, to see how roles work, especially with elevated permission. I also added a new department called System Administrators and gave that group System Administrator privileges. 
</p>
<br />
<img width="1440" alt="Screenshot 2023-11-26 at 3 43 07 PM" src="https://github.com/Beth-Agbassekou/post-install-config/assets/148320585/a7127adb-c00f-4d6e-aa5d-1390c3b193ec">
<img width="1440" alt="Screenshot 2023-11-26 at 3 44 57 PM" src="https://github.com/Beth-Agbassekou/post-install-config/assets/148320585/3afef593-a355-41f3-8664-72ab8d3177d9">
<img width="1440" alt="Screenshot 2023-11-26 at 3 50 45 PM" src="https://github.com/Beth-Agbassekou/post-install-config/assets/148320585/44e31ea9-d8f7-4d0e-be40-b86ae3bd3d1f">
<img width="1440" alt="Screenshot 2023-11-26 at 3 51 36 PM" src="https://github.com/Beth-Agbassekou/post-install-config/assets/148320585/2e7a884a-b403-436e-bbef-0ffdada444d9">
<img width="1440" alt="Screenshot 2023-11-26 at 3 52 16 PM" src="https://github.com/Beth-Agbassekou/post-install-config/assets/148320585/d72666d2-9bf0-4c4a-a53c-320f2f37d950">
<img width="1440" alt="Screenshot 2023-11-26 at 3 56 01 PM" src="https://github.com/Beth-Agbassekou/post-install-config/assets/148320585/ebf75591-4b77-46b6-aa36-0c4c2dac22fb">
<img width="1440" alt="Screenshot 2023-11-26 at 3 59 25 PM" src="https://github.com/Beth-Agbassekou/post-install-config/assets/148320585/b9a2fc4e-02b5-4556-80a0-32a798a4eded">
<p>
  <p>
 I created a new team of Level I Support and Level II Support. Then, I created agents and users to create tickets. Level I support has entry-level permissions and can escalate privileges. Then Level II support is in between Level I support and System Admin. So they have some more privileges, but no admin permissions. 
  </p>
  <img width="1440" alt="Screenshot 2023-11-26 at 4 00 15 PM" src="https://github.com/Beth-Agbassekou/post-install-config/assets/148320585/94da6174-9072-41e7-8d95-8912fad13c5e">
<img width="1440" alt="Screenshot 2023-11-26 at 4 01 42 PM" src="https://github.com/Beth-Agbassekou/post-install-config/assets/148320585/1e8b1517-ba49-47ed-8eba-ed22ec21293f">
<img width="1440" alt="Screenshot 2023-11-26 at 4 04 48 PM" src="https://github.com/Beth-Agbassekou/post-install-config/assets/148320585/50e10303-23ee-4d82-a417-f0f63b97a33f">
</p>

<p>
In this portion, I created Service Level Agreements. I created three Service Level Agreements: SEV-A, SEV-B, and SEV-C, respectively. SEV-A is an SLA I created to contact the client every hour on a 24-hour scale until this is solved. SEV-A is for an extreme business critical emergency. SEV-B is an SLA that requires employees to contact the client every 4-hours on a 24-hour scale until this is resolved. This is for a moderate business crisis. SEV-C is an SLA that was created to address minor issues including Level I IT Support issues. SEV-C works by contacting the customer every 8 hours on a normal business schedule including holidays. I also created Help Topics. The Help Topics I created were Password Reset, Personal Computer Issues, Equipment Reset, and Business Critical Outage.
</p>
<br /># post-install-config
