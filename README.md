# Active Directory Help Desk Lab

## Overview
This project demonstrates a simulated Active Directory environment built in a home lab using Windows Server and a Windows client machine in VirtualBox. The lab simulates real IT help desk tasks such as user management, password resets, account lockouts, and domain authentication.

Domain Name: sirajlab.local

---

## Lab Environment

Domain Controller: Windows Server 2022  
Client Machine: Windows 10  
Virtualization: Oracle VirtualBox  

---

## Active Directory Structure

Organizational Units created:

- Lab_Users
- Lab_Groups
- Lab_Computers

Security Groups:

- HR
- Sales

Users created:

- Sara Sales
- Mike HR
- John Helpdesk

---

## Help Desk Ticket Scenarios

### Ticket 1 — Password Reset

User reported they could not log into their account.

Steps performed:

1. Open Active Directory Users and Computers
2. Locate the user account
3. Right-click user → Reset Password
4. Enter new password
5. Enable **User must change password at next logon**

---

### Ticket 2 — Account Lockout / Unlock

User account was locked after multiple failed login attempts.

Steps performed:

1. Open Active Directory Users and Computers
2. Open the user properties
3. Navigate to the **Account** tab
4. Check **Unlock account**
5. Apply changes

---

### Ticket 3 — Force Password Change

Enabled **User must change password at next logon** to enforce security policy.

---

### Ticket 4 — Disable User Account

Disabled a user account to simulate an employee leaving the organization.

---

## Domain Login Verification

Client machine successfully authenticated to the domain.

Command used:

```
whoami
```

Result:

```
sirajlab\ssales
```

---

## Skills Demonstrated

Active Directory Administration  
User Account Management  
Password Reset Procedures  
Account Lockout Troubleshooting  
Group Management  
Domain Authentication  
IT Help Desk Troubleshooting
