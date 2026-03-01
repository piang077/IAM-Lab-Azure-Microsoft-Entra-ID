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

### Create New User
- Created a new internal user account in Microsoft Entra Admin Center
- Configured username, display name, and profile properties
- Enabled account and configured usage location
- Verified login and completed MFA setup

### Assign License
- Accessed Microsoft 365 Admin Center
- Assigned **Microsoft Power Automate Free** license to user

### Invite External User
- Invited guest user via email
- Added external collaborator to tenant
- Sent onboarding message

### Assign Roles (RBAC)
- Assigned directory roles to user
- Practised role assignment using:
  - User profile method
  - Roles & Admins section
- Configured eligible and active role assignments

### Bulk Import Users
- Downloaded bulk user CSV template
- Edited user details
- Uploaded CSV file for bulk account creation
- Verified successful user provisioning

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
## 3. Password Protection & Smart Lockout

### View & Configure Lock Settings
- Opened Microsoft Entra Admin Center and navigated to **Authentication methods → Password protection**
- Reviewed current **lockout threshold** and **duration** values

### Configure Custom Smart Lockout
- Set **Lockout threshold**: 5 failed login attempts
- Set **Lockout duration**: 30 seconds
- Enabled **custom banned password list**

### Add Banned Passwords
- Added the following to the banned list:
  - Contoso
  - London
  - Widget

### Enforce Policy
- Set **Mode** to **Enforced**
- Saved configuration

---
## 4. Self-Service Password Reset (SSPR)
### Enable SSPR for Specific Group
- Opened Microsoft Entra Admin Center and navigated to **Protection → Password reset**
- Set **Self-service password enabled** to **Selected**
- Added **Project23** group to enable SSPR for its members
- Saved configuration

---

### Configure Authentication Methods
- Selected **Authentication methods** within Password reset
- Set **Number of methods required** to **1**
- Enabled methods for users:  
  - Email  
  - Mobile phone  
  - Mobile app code  
- Saved changes

---

### Configure Registration Settings
- Selected **Registration** within Password reset
- Set **Require users to register when signing in** to **Yes**
- Set **Number of days before users are asked to re-confirm** to **90**
- Saved changes

---

### Configure Reset Notifications
- Selected **Notifications** within Password reset
- Left **Notify users on password reset** as **Yes**  
- Set **Notify all admins when other admins reset their password** to **Yes**
- Saved changes

---



# Outcome

- Applied hands-on cloud IAM skills relevant to modern enterprise security

- Demonstrated user management, policy configuration, and secure access practices

- Produced well-documented methodology and screenshots suitable for professional review
