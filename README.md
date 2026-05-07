# 🔐 Active Directory to Okta Integration Lab

## 📌 Project Overview

This project demonstrates how to integrate an on-premises Active Directory (AD) environment with Okta using the Okta AD Agent.

The goal of this lab is to simulate a real-world enterprise identity environment where users and groups are managed in Active Directory and synchronized to Okta for centralized identity and access management.

This project showcases skills in:
- Identity Lifecycle Management
- Directory Integration (AD → Okta)
- User and Group Provisioning
- SSO Readiness Architecture

---

## 🏗️ Architecture Diagram

![image alt](https://github.com/prosper87ab/prosper87ab/blob/main/ADtoOktaDiagram.png))

### 🔍 Architecture Explanation

- Active Directory is the source of truth for user identities
- Okta acts as the Identity Provider (IdP)
- Okta AD Agent securely connects AD to Okta
- Users and groups are synchronized from AD into Okta
- Authentication can be delegated to AD

---

## 🛠️ Technologies Used

- Windows Server (Active Directory Domain Services)
- Okta Developer Tenant
- Okta Active Directory Agent
- PowerShell (optional for automation)
- VirtualBox / VMware (for lab environment)

---

## ⚙️ Lab Setup Steps

### 1️⃣ Active Directory Setup

- Installed Active Directory Domain Services (AD DS)
- Promoted server to Domain Controller
- Created domain: `iamlab.local`

📸 Screenshot:
![AD Users](images/02-ad-users-created.png)

---

### 2️⃣ Created Users in Active Directory

- Created multiple test users:
  - John Doe
  - Jane Smith
  - IAM Admin User

📸 Screenshot:
![AD Users](images/02-ad-users-created.png)

---

### 3️⃣ Created AD Security Groups

- Created groups:
  - IT_Admins
  - HR_Team
  - Finance_Team

📸 Screenshot:
![AD Groups](images/03-ad-groups-created.png)

---

### 4️⃣ Installed Okta AD Agent

- Downloaded Okta AD Agent
- Installed on domain-joined server
- Authenticated agent with Okta tenant
- Linked AD domain to Okta

📸 Screenshot:
![AD Agent](images/04-okta-ad-agent-installed.png)

---

### 5️⃣ Configured Directory Integration in Okta

- Navigated to:
  - Directory → Directory Integrations
- Verified AD connection status
- Enabled provisioning and import settings

📸 Screenshot:
![Directory Integration](images/05-okta-directory-integration.png)

---

### 6️⃣ Imported Users from AD to Okta

- Ran import from AD
- Verified users appear in Okta directory

📸 Screenshot:
![Users Imported](images/06-users-imported-okta.png)

---

### 7️⃣ Imported Groups from AD to Okta

- Synced AD groups into Okta
- Verified group memberships

📸 Screenshot:
![Groups Imported](images/07-groups-imported-okta.png)

---

### 8️⃣ Configured Import & Matching Rules

- Set username format (e.g., email)
- Enabled automatic confirmation
- Configured attribute mappings

📸 Screenshot:
![Import Settings](images/08-import-settings.png)

---

### 9️⃣ Assigned Users to Applications

- Assigned users/groups to applications in Okta
- Demonstrated role-based access

📸 Screenshot:
![User Assignment](images/09-user-assignment.png)

---

### 🔟 Tested Authentication Flow

- Verified login via Okta
- Confirmed AD credentials work (Delegated Authentication)

📸 Screenshot:
![Login Test](images/10-login-test.png)

---

## 🔐 Key IAM Concepts Demonstrated

- Identity Source of Truth (Active Directory)
- Identity Federation (Okta as IdP)
- Just-In-Time Provisioning (Optional)
- Role-Based Access Control (RBAC)
- Directory Synchronization
- Delegated Authentication

---

## 🚀 Key Outcomes

- Successfully integrated AD with Okta
- Synced users and groups from AD to Okta
- Demonstrated centralized identity management
- Validated authentication and access workflows

---

## 📈 Resume Bullet Points (ATS Optimized)

- Integrated on-premises Active Directory with Okta using Okta AD Agent, enabling centralized identity management
- Configured user and group synchronization from AD to Okta, supporting lifecycle management and RBAC
- Implemented directory integration and provisioning workflows in Okta, improving access control efficiency
- Performed user import, attribute mapping, and authentication testing in a hybrid identity environment
- Simulated enterprise IAM architecture with AD as source of truth and Okta as Identity Provider (IdP)

---

## 🧠 What I Learned

- How enterprise IAM systems integrate with legacy directories
- How Okta handles directory synchronization and authentication
- Real-world troubleshooting for identity sync issues
- Importance of identity lifecycle and governance

---

## 🔄 Future Improvements

- Add SAML-based application integration
- Implement MFA policies in Okta
- Automate user provisioning with PowerShell
- Add lifecycle workflows (joiner/mover/leaver)

---

## 📬 Contact

Feel free to connect with me on LinkedIn or reach out for collaboration!
