<p align="center">
<img src="https://i.imgur.com/pqTjnLb.png" alt="osTicket logo"/>
</p>

## Day 5 – Backup and Continuity

As construction delays pushed us back to Chicago temporarily, I needed to ensure the current system setup could be restored once we return to Arlington Heights.

I created a snapshot of the Domain Controller VM, capturing the system’s current state, ensuring seamless recovery of user data, policies, and configurations when we’re back in Arlington. (Got guidance from ChatGPT on proper snapshot usage and backup strategies.)

### 🧪 Lab Tasks

#### 1. Create a Snapshot of the Domain Controller VM:

Use Azure portal to create a snapshot of the Domain Controller VM. Ensure that the snapshot captures the current state of the system, including user data, policies, and configurations.

Verify that the snapshot is stored correctly in the Azure storage account.

#### 2. Verify Backup Integrity:

Ensure the snapshot includes all necessary Active Directory components, such as the SYSVOL folder, Group Policy objects, and user data.

Perform a test restore operation on a non-production environment to confirm that the backup works as expected.

#### 3. Document Snapshot Information:

Record the snapshot creation date, the state of the system, and any relevant details (e.g., VM size, resource usage at the time of snapshot).

Store this information in a secure location for future reference and disaster recovery planning.

#### 4. Create a Backup Strategy for Active Directory:

Develop a backup strategy that includes periodic snapshots of the Domain Controller VM, ensuring minimal data loss and quick recovery in case of failure.

Identify and implement best practices for securing backups and ensuring they are available for restoration when needed.

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
