<p align="center">
<img src="https://i.imgur.com/pqTjnLb.png" alt="osTicket logo"/>
</p>

## Day 5 – Backup and Continuity

As construction delays pushed us back to Chicago temporarily, I needed to ensure the current system setup could be restored once we return to Arlington Heights.

I created a snapshot of the Domain Controller VM, capturing the system’s current state, ensuring seamless recovery of user data, policies, and configurations when we’re back in Arlington. (Got guidance from ChatGPT on proper snapshot usage and backup strategies.)

### 🧪 Lab Tasks

#### 1. Create a Snapshot of the Domain Controller VM:
I used the Azure portal to create a snapshot of the Domain Controller virtual machine. I made sure the snapshot captured the current system state, including all user data, group policies, and configurations. After creating the snapshot, I double-checked that it was successfully stored in the Azure storage account, ensuring it would be available for future restoration if needed.

<p align="center">
<img src="https://i.imgur.com/1k6Cndm.png" alt="osTicket logo"/>
</p>

***

<p align="center">
<img src="https://i.imgur.com/BIEWRLD.png" alt="osTicket logo"/>
</p>

***

#### 2. Verify Backup Integrity:
Next, I verified that the snapshot included all critical Active Directory components like the SYSVOL folder, Group Policy objects, and user data. To ensure the backup's reliability, I conducted a test restore operation in a non-production environment, confirming the snapshot worked as expected and all necessary services and data were intact.

<p align="center">
<img src="https://i.imgur.com/tRETr37.png" alt="osTicket logo"/>
</p>

***

#### 3. Document Snapshot Information:
I recorded the snapshot’s creation date, the system’s state at the time, and technical details such as the VM size and current resource usage. I stored this documentation securely so it can be quickly accessed during disaster recovery scenarios or future audits.

<p align="center">
<img src="https://i.imgur.com/Yb6iUfh.png" alt="osTicket logo"/>
</p>

***

#### 4. Create a Backup Strategy for Active Directory:
To strengthen our AD backup approach, I developed a strategy that includes taking regular snapshots of the Domain Controller VM. This plan is designed to reduce the risk of data loss and support fast recovery in the event of a failure. I also researched and applied best practices for securing our backups and making sure they’re always available when restoration is required.

<p align="center">
<img src="https://i.imgur.com/Lymrqgw.png" alt="osTicket logo"/>
</p>

***

### 🖥️ Technology Stack
#### Azure Active Directory

#### Azure Virtual Machines (VMs)

#### Snapshot and Backup Tools

#### PowerShell (for backup scripting)

### 🎯 Goals Accomplished
#### ✅ Created a Snapshot of the Domain Controller VM

#### ✅ Verified Backup Integrity through Test Restoration

#### ✅ Developed a Backup Strategy for Active Directory

#### ✅ Documented Snapshot Details for Future Reference

#### ✅ Planned and Prepared a Disaster Recovery Strategy

### ✅ Conclusion – Jose’s Role in a Real-World Scenario
This five-day Active Directory lab wasn’t just a technical checklist—it became a dynamic case study for what real IT professionals face: provisioning new infrastructure, managing users, securing sensitive data, and preparing for disaster recovery.

I used this lab to solidify my Azure and AD skills, build a deployment story I could confidently walk through in an interview, and sharpen my troubleshooting instincts. Tools like ChatGPT were essential in helping me think through real-world context, confirm steps, and make this more than just a lab—it became a professional simulation.
