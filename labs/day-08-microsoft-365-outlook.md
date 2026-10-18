# Day 8 — Microsoft 365 Fundamentals and Outlook Troubleshooting

## 1. Learning Objectives

By completing this lab, I learned how to:

- Understand Microsoft 365 user accounts, licences, and permissions.
- Distinguish application-specific issues from general account-access issues.
- Follow a structured troubleshooting process.
- Gather evidence before attempting a fix.
- Recognize when administrator assistance is required.
- Document findings in a professional IT support ticket.

## 2. Microsoft 365 Fundamentals

### User Account
A user account identifies an employee and enables authentication to organizational services.

### Licence
A Microsoft 365 licence determines which services and features a user is entitled to use. Actual access can also depend on service configuration and provisioning.

### Permissions
Permissions determine which resources and actions a user is authorized to access.

**Important:** Successful sign-in does not guarantee access to every Microsoft 365 application or feature.

## 3. Simulated Incident — INC-008

**Issue:** Outlook desktop repeatedly requests sign-in.

**User:** Sijo  — new employee.

**Reported symptoms:**
- Microsoft Teams works normally.
- Outlook on the web opens and displays emails.
- Outlook desktop repeatedly displays the sign-in window.
- The same prompt returns after the employee enters her credentials.
- No error code is reported.
- Outlook worked the previous day.

**User impact:** The employee cannot use desktop Outlook, although web-based email remains accessible.

**Initial hypothesis:** The issue may be specific to Outlook desktop authentication or configuration.

**Note:** This is a working hypothesis, not a confirmed root cause.

## 4. Troubleshooting Procedure

### Step 1 — Clarify the symptom
Ask whether Outlook fails to open, repeatedly requests sign-in, or opens but cannot access the mailbox.

Record the exact behavior and any displayed error.

### Step 2 — Compare application access
Confirm whether Microsoft Teams and Outlook on the web work.

**Finding:** Both services work, making a general account-access problem less likely.

### Step 3 — Restart Outlook
Ask the employee to close Outlook normally, save any work, and reopen the application.

**Finding:** The repeated sign-in prompt persists.

### Step 4 — Check Office account and activation
Where accessible, inspect the account information and product activation status in an Office application, such as Word.

**Finding:** The correct company account is displayed, and Office reports Product Activated.

**Limitation:** Office activation does not prove that Outlook authentication is working correctly.

### Step 5 — Check the connected work account
Inspect Windows Settings → Accounts → Access work or school.

**Finding:** The company work account is connected.

**Limitation:** A connected work account does not prove that every application authentication process is functioning correctly.

### Step 6 — Consult the approved troubleshooting procedure
Review the organization's knowledge base for Outlook authentication issues. Gather the diagnostic evidence requested by the procedure.

Do not delete credentials, modify registry settings, disconnect the work account, reset the account, or change licences without appropriate authorization.

### Step 7 — Escalate when necessary
If the problem remains unresolved or requires elevated access, escalate to the appropriate administrator or support team.

Include the symptoms, checks performed, results, user impact, and outstanding questions.

## 5. Troubleshooting Findings

| Check | Result |
|---|---|
| Microsoft Teams | Working |
| Outlook on the web | Working |
| Outlook restart | Issue persists |
| Office account | Correct company account displayed |
| Office activation | Product Activated |
| Windows work account | Connected |
| Outlook desktop sign-in | Repeated prompt |
| Root cause | Not confirmed |

## 6. Professional Ticket Note

**Incident:** INC-008

**Summary:** Outlook desktop repeatedly requests sign-in.

**Investigation:** Confirmed that Teams and Outlook on the web work normally. Restarting Outlook did not resolve the issue. Word displays the correct company account and reports Product Activated. The company work account is connected in Windows Settings.

**Findings:** The problem appears limited to Outlook desktop. No error code has been reported. The root cause remains unconfirmed.

**Next action:** Consult the approved Outlook authentication troubleshooting procedure and gather additional diagnostic evidence. Escalate if further investigation requires administrator privileges.

**Status:** Open — further investigation required.

## 7. German IT Support Vocabulary

| German | English |
|---|---|
| das Benutzerkonto | User account |
| die Lizenzzuweisung | Licence assignment |
| die Berechtigung | Permission |
| die Anmeldung | Sign-in |
| die Authentifizierung | Authentication |
| die Fehlermeldung | Error message |
| die Anwendung | Application |
| das Postfach | Mailbox |
| die Fehlerbehebung | Troubleshooting |
| die Eskalation | Escalation |
| die Ursache | Cause |
| die Untersuchung | Investigation |

### Useful workplace phrases

- **Können Sie sich bei Outlook anmelden?** — Can you sign in to Outlook?
- **Welche Fehlermeldung wird angezeigt?** — What error message is displayed?
- **Outlook im Web funktioniert, aber die Desktop-Anwendung nicht.** — Outlook on the web works, but the desktop application does not.
- **Ich prüfe das Problem und dokumentiere die Ergebnisse.** — I will investigate the issue and document the findings.
- **Ich leite das Ticket an das zuständige Support-Team weiter.** — I will forward the ticket to the appropriate support team.

## 8. Key Lessons

1. Identify the exact symptom before choosing a fix.
2. Use evidence to narrow down possible causes.
3. Distinguish a working hypothesis from a confirmed root cause.
4. Follow approved troubleshooting procedures.
5. Never make unauthorized changes to company-managed systems.
6. Escalate with useful diagnostic evidence rather than simply forwarding the complaint.

## 9. Lab Status

- [x] Microsoft 365 account, licence, and permission fundamentals reviewed.
- [x] Simulated Outlook incident investigated.
- [x] Findings documented.
- [x] Escalation criteria identified.
- [x] German IT support vocabulary practised.

**Lab type:** Simulated troubleshooting exercise.

**Outcome:** Troubleshooting workflow practised; root cause not confirmed.
