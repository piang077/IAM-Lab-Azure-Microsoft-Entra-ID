# IAM-Lab-Azure-Microsoft-Entra-ID
# Overview

This lab demonstrates cloud-based Identity and Access Management (IAM) using Microsoft Entra ID. The goal is to configure, test, and secure user identities and access controls in a modern enterprise environment. All tasks follow best practices for account management, authentication, and access security.

**The lab focuses on**

- Creating and managing users and groups

- Implementing password policies and MFA

- Enabling Self-Service Password Reset (SSPR)

- Configuring Conditional Access policies

- Testing access scenarios and auditing activity

The lab was conducted in a cloud trial environment, providing hands-on experience with modern IAM features without the need for on-premises infrastructure. Prior hands-on experience with Active Directory provided foundational knowledge of user and group management, which was applied in this cloud-based IAM lab.

**Lab Tasks**

**1. User Management**

- Task 1: Create a New User

  - Logged into Microsoft Entra Admin Center

  - Created a new internal user account

  - Set username, display name, and user details

  - Enabled account and set usage location

  - Logged in as the new user to confirm access and MFA setup
- **[Screenshots](https://github.com/piang077/IAM-Lab-Azure-Microsoft-Entra-ID/tree/main/Lab1)**


- Task 2: Assign License

  - Opened Microsoft 365 Admin Center

  - Selected available license (Power Automate Free)

  - Assigned license to the created user

- Task 3: Invite External User

  - Invited a guest/external user using email

  - Sent invitation message

  - Added external collaborator to tenant

- Task 4: Assign Roles

  - Assigned Azure role to internal user

  - Used role-based access control (RBAC)

- Task 5: Bulk Import Users

  - Downloaded CSV template

  - Edited user details in file

  - Uploaded CSV for bulk user creation

---


**2. Group Management**
### Create Microsoft 365 Group

* Created group **Project23**
* Added description and assigned membership type
* Added internal user as member

### Create Security Group (Dynamic Membership)

* Created **Guest Users** security group
* Configured dynamic rule:

  * `userType = Guest`
* Automatically populated guest users

### Add Users to Groups

* Added external user to Project23 group
* Practised adding membership:

  * From group settings
  * From user profile

### Assign Group Owners

* Added group owner for Project23
* Verified ownership permissions

### Assign License to Group

* Assigned Microsoft 365 license to group
* Applied licenses automatically to all group members

---



**3. Multi-Factor Authentication (MFA)**

- Enabled MFA for selected users

- Tested MFA login flow

- Documented challenges and outcomes

**4. Self-Service Password Reset (SSPR)**

- Enabled SSPR for all users

- Tested reset workflow and email/phone verification

- Ensured secure configuration

**5. Conditional Access**

- Created policies to enforce MFA based on location, device, or group

- Tested policy impact on different users

- Documented any exceptions or issues

**6. Auditing and Access Testing**

- Reviewed sign-in logs for suspicious activity

- Checked policy compliance for users and groups

- Documented results and recommended improvements

# Outcome

- Applied hands-on cloud IAM skills relevant to modern enterprise security

- Demonstrated user management, policy configuration, and secure access practices

- Produced well-documented methodology and screenshots suitable for professional review
