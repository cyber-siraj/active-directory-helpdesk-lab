# Active Directory Help Desk Lab

## Overview

This project demonstrates a simulated **Active Directory environment** built in a home lab using **Windows Server 2022** and a **Windows 10 client** inside Oracle VirtualBox.

The lab replicates common **IT Help Desk tasks** such as:

- Creating and managing users
- Managing security groups
- Password resets
- Account lockouts
- Domain authentication
- Basic Active Directory administration

Domain Name:

```
sirajlab.local
```

---

# Lab Environment

| Component | Technology |
|-----------|------------|
| Domain Controller | Windows Server 2022 |
| Client Machine | Windows 10 |
| Virtualization | Oracle VirtualBox |
| Directory Service | Active Directory Domain Services |

---

# Active Directory Structure

Organizational Units created:

- **Lab_Users**
- **Lab_Groups**
- **Lab_Computers**

Security Groups:

- **HR**
- **Sales**

Users created:

- Sara Sales
- Mike HR
- John Helpdesk

---

# Help Desk Ticket Scenarios

This lab simulates common **Tier 1 IT Help Desk tickets**.

---

## Ticket 1 — Password Reset

User reported they could not log into their account.

Steps performed:

1. Open **Active Directory Users and Computers**
2. Locate the user account
3. Right-click user → **Reset Password**
4. Enter new password
5. Enable **User must change password at next logon**

---

## Ticket 2 — Account Lockout

User account was locked after multiple failed login attempts.

Steps performed:

1. Open **Active Directory Users and Computers**
2. Open **User Properties**
3. Navigate to the **Account tab**
4. Check **Unlock account**
5. Apply changes

---

## Ticket 3 — Force Password Change

Enabled **User must change password at next logon** to enforce a password security policy.

---

## Ticket 4 — Disable User Account

Simulated a scenario where an employee leaves the organization.

Steps performed:

1. Open **Active Directory Users and Computers**
2. Locate the user account
3. Right click → **Disable Account**

---

# Domain Login Verification

The Windows client machine successfully authenticated with the domain.

Command used:

```
whoami
```

Result:

```
sirajlab\ssales
```

---

# Lab Screenshots

## Virtual Lab Environment

![Virtual Machines](screenshots/01-lab-virtual-machines.png)

---

## Active Directory Domain Created

![Domain Created](screenshots/02-domain-created-sirajlab.png)

---

## Active Directory Installation

![ADDS Installation](screenshots/03-adds-installation.png)

---

## Active Directory Structure

![AD Structure](screenshots/04-active-directory-structure.png)

---

## Users Created

![Users Created](screenshots/05-users-created.png)

---

## Groups Created

![Groups Created](screenshots/06-groups-created.png)

---

## DNS Configuration on Client

![DNS Configuration](screenshots/07-client-dns-config.png)

---

## Password Reset

![Password Reset](screenshots/07-password-reset.png)

---

## Force Password Change

![Password Change](screenshots/08-force-password-change.png)

---

## Disabled User Account

![Disabled User](screenshots/09-disabled-user.png)

---

## Domain Login Verification

![Domain Login](screenshots/11-domain-user-login.png)

---

## Account Unlock

![Account Unlock](screenshots/13-account-unlock.png)

---

# Skills Demonstrated

- Active Directory Administration
- Identity & Access Management
- Windows Server Management
- IT Help Desk Troubleshooting
- Password Reset Procedures
- Account Lockout Troubleshooting
- Group Management
- Domain Authentication
- Virtualization using VirtualBox

---

# Key Takeaway

This project demonstrates how Active Directory is used in real organizations to manage user identities, enforce security policies, and support IT help desk operations.

The lab provides hands-on experience with **common tasks performed by Tier 1 IT support and system administrators**.

---

# Author

**Siraj Mushtaq**

Cybersecurity / Cloud / IT Infrastructure Student  
Brooklyn, New York
IT Help Desk Troubleshooting
