# Day 10 – Active Directory & Microsoft Entra ID Fundamentals

## Learning Objectives

- Understand Active Directory Domain Services (AD DS).
- Identify users, computers, groups, domains, and domain controllers.
- Understand Microsoft Entra ID and cloud identity management.
- Differentiate authentication and authorization.
- Troubleshoot basic account and access issues.
- Understand L1 support responsibilities and escalation.

## 1. Active Directory Domain Services (AD DS)

Active Directory Domain Services is a Microsoft directory service used in on-premises Windows domain environments.

It helps organizations centrally manage:

- User accounts
- Computer accounts
- Security groups
- Authentication
- Access to organizational resources

### Important Terms

| Term | Meaning |
|---|---|
| User Account | An account used by an employee to sign in |
| Computer Account | An account representing a computer in a domain |
| Security Group | A group used to manage access permissions |
| Domain | A logical environment for centrally managing users and computers |
| Domain Controller | A server that manages domain authentication and directory services |

## 2. Security Groups and Permissions

Security groups simplify access management.

Example:

A company has a security group named `Finance-Staff`.

Employees who require access to Finance resources may be added to this group according to an approved access request.

However, group membership alone does not automatically grant access. The relevant resource permissions must also be configured for that group.

**Important:** L1 technicians should never grant access without authorization.

## 3. Microsoft Entra ID

Microsoft Entra ID is Microsoft's cloud-based identity and access management service.

It helps organizations manage access to:

- Microsoft 365
- Microsoft Azure
- Cloud applications
- Other supported organizational services

Important features include:

- Multi-Factor Authentication (MFA)
- Conditional Access
- Cloud identity management
- Single Sign-On (SSO)

Some organizations synchronize identities between on-premises Active Directory and Microsoft Entra ID. They are related services, but they are not the same.

## 4. AD DS vs Microsoft Entra ID

| Feature | Active Directory (AD DS) | Microsoft Entra ID |
|---|---|---|
| Environment | On-premises | Cloud-based |
| Identity | Domain accounts | Cloud identities |
| Common use | Windows domain resources | Microsoft 365 and cloud applications |
| Authentication | Kerberos and NTLM | Modern cloud authentication |
| Management | Domain controllers | Cloud administration |

## 5. Common Account Statuses

| Status | Meaning | L1 Action |
|---|---|---|
| Enabled | Account is enabled | Investigate the reported issue |
| Disabled | Account sign-in is blocked | Verify authorization and escalate |
| Locked | Account has been locked, often after repeated failed attempts | Follow approved unlock procedure or escalate |
| Password Expired | Password has reached its expiry date | Follow the approved password-reset process |

A locked account may result from repeated incorrect password attempts, including attempts from another device using an outdated saved password.

## 6. Practical Helpdesk Scenarios

### Scenario 1 – INC-010: Finance Folder Access

**User:** Anna Müller  
**Department:** Finance  
**Issue:** Cannot access the Finance network folder.

**Findings:**
- User can sign in successfully.
- Other employees can access the folder.
- User's account is enabled.
- Group membership and folder permissions have not yet been verified.
- An approved access request confirms that Anna requires access.
- Anna is not a member of the Finance-Staff security group.
- L1 does not have permission to modify group membership.

**L1 Action:**

Document the findings and escalate to an authorized administrator.

**Suggested escalation note:**

"Please review Anna's group membership and update it according to the approved access request."

**Learning:** Authentication can work successfully while authorization to a particular resource is missing.

### Scenario 2 – INC-011: Windows Account Locked

**User:** Markus Weber  
**Department:** Finance  
**Issue:** Unable to sign in to the company Windows computer.

**Findings:**
- Sign-in worked the previous day.
- User attempted to enter the password several times.
- Windows displays an account-locked message.

**Correct L1 troubleshooting approach:**

1. Record the exact error message.
2. Confirm when the issue started.
3. Ask about recent sign-in attempts.
4. Check account status through an approved procedure, if authorized.
5. Escalate to an authorized administrator if account administration is outside L1 permissions.

**Important Security Rules:**
- Never ask users to share their passwords.
- Never make unauthorized account changes.
- Never grant unnecessary administrative privileges.
- Always document troubleshooting and escalation.

## 7. German IT Support Vocabulary

| English | German |
|---|---|
| Active Directory | Active Directory |
| Domain Controller | Domänencontroller |
| User Account | Benutzerkonto |
| Security Group | Sicherheitsgruppe |
| Group Membership | Gruppenmitgliedschaft |
| Locked Account | Gesperrtes Konto |
| Disabled Account | Deaktiviertes Konto |
| Password | Kennwort |
| Identity Management | Identitätsverwaltung |
| User Sign-in | Benutzeranmeldung |
| Access Rights | Zugriffsrechte |
| Permission Review | Berechtigungsprüfung |

## 8. Key Takeaways

- Active Directory manages identities and resources in on-premises Windows domains.
- Microsoft Entra ID manages cloud identities and access.
- Security groups help administrators manage resource access.
- Authentication and authorization are different.
- Account lockouts require investigation, not guesswork.
- L1 technicians must follow approved procedures and escalate tasks requiring additional privileges.

## Training Disclaimer

The incidents in this document are simulated helpdesk training exercises. They demonstrate troubleshooting knowledge and do not represent actual production support experience.
