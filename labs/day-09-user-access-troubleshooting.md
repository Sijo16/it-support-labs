# Day 9 — Microsoft 365 User Access Troubleshooting

## 1. Learning Objectives

- Understand authentication and authorization.
- Troubleshoot access-denied errors.
- Perform basic user-access checks.
- Document incidents professionally.
- Escalate permission issues safely.

## 2. Key Concepts

### Authentication (Authentifizierung)

Authentication verifies the identity of a user.

**Question:** Who are you?

Examples:
- Entering a username and password.
- Completing Multi-Factor Authentication (MFA).
- Signing in to a company Microsoft 365 account.

### Authorization (Autorisierung)

Authorization determines which resources a signed-in user is allowed to access.

**Question:** What are you allowed to access?

Examples:
- Opening a shared company folder.
- Accessing department-specific documents.
- Viewing files according to assigned permissions.

**Key difference:** A user can sign in successfully but still be denied access to a particular resource.

## 3. Troubleshooting Scenario — INC-009

**Employee:** Markus Weber  
**Department:** Finance  
**Issue:** Access denied when opening a shared Finance folder.

### Reported Symptoms

- Markus can sign in to his company account.
- Microsoft Teams works.
- Other shared Finance folders are accessible.
- One specific folder cannot be opened.
- The folder was shared through a link provided by his manager.
- The error message is: `Access denied`.
- A colleague can access the same folder.
- The first-line technician does not have administrator privileges.

### Initial Assessment

Authentication appears to be working because Markus can sign in.

The issue may relate to folder permissions, link configuration, or another resource-specific access restriction.

The root cause is not confirmed.

## 4. Troubleshooting Steps

### Step 1 — Clarify the Problem

Ask the user:
- Which exact folder cannot be opened?
- What is the full error message?
- When did the issue begin?
- Can the user access other shared folders?
- How is the folder being opened?

### Step 2 — Verify the Account and Resource

- Confirm that the correct company account is being used.
- Check that the provided link points to the intended folder.
- Record the folder path or resource name.
- Confirm whether the issue affects one resource or several.

### Step 3 — Compare Access Carefully

- Confirm whether an authorized colleague can open the same folder.
- Do not assume both employees have identical permissions.
- Avoid accessing the resource using another employee's account.
- Do not change permissions without authorization.

### Step 4 — Document and Escalate

If the problem requires administrator access:
- Record the symptoms and checks completed.
- Include the exact error message and affected resource.
- Request an access-permission review.
- Ask the administrator to verify the user's required access against approved access requirements.

**Important:** Never grant full access without a valid business need and proper authorization.

## 5. Helpdesk Ticket — INC-009

**Ticket ID:** INC-009  
**Employee:** Markus Weber  
**Department:** Finance  
**Category:** Access / Permissions  
**Status:** Escalated to Administrator

### Issue Description

The user cannot access a specific shared Finance folder through a link provided by his manager. The displayed error message is "Access denied."

### Troubleshooting Performed

- Confirmed that the user can sign in to the company account.
- Confirmed that other shared Finance folders are accessible.
- Verified that the correct company account and folder link are being used.
- Confirmed that a colleague can access the same folder.

### Action Taken

Escalated to the administrator for a review of the user's access permissions against the approved access requirements for the folder.

### Root Cause

Not yet confirmed. Awaiting administrator investigation.

## 6. Common Mistakes to Avoid

- Resetting a password when authentication is already working, without evidence that credentials are the problem.
- Assuming the manager forgot to grant permission.
- Granting excessive permissions to solve an access issue.
- Making unauthorized changes to access controls.
- Escalating without collecting useful evidence.
- Marking a suspected cause as the confirmed root cause.

## 7. German IT Support Vocabulary

| German term | English meaning |
|---|---|
| die Authentifizierung | Authentication |
| die Autorisierung | Authorization |
| die Berechtigung | Permission |
| die Zugriffsrechte | Access rights |
| die Zugriffsverweigerung | Access denied |
| der freigegebene Ordner | Shared folder |
| die Fehlermeldung | Error message |
| die Berechtigungsprüfung | Permission review |
| die Eskalation | Escalation |
| der Administrator | Administrator |
| der Benutzer | User |
| die Fehlerbehebung | Troubleshooting |

## 8. Key Takeaways

- Successful sign-in does not guarantee access to every resource.
- Investigate the scope of the issue before selecting a solution.
- Collect evidence before escalating.
- Follow least-privilege principles.
- Do not change permissions without proper authorization.
- Keep the root cause marked as unconfirmed until evidence establishes it.

## 9. Practical Reflection

**Question:** Why should an IT Support technician request a permission review instead of immediately granting full access?

**Answer:** A permission review verifies the access required for the user's role. Granting unnecessary access can expose confidential information and violate security policies.

---


**Next lesson:** Day 10 — Active Directory and Microsoft Entra ID Fundamentals
