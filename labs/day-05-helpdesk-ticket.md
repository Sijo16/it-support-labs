# Day 5 — Helpdesk Ticket Documentation

**Ticket ID:** INC-005  
**Category:** Windows Application Support  
**Status:** Open — Investigation Pending  
**German terminology:** Störung, Fehlerbehebung, Eskalation

## 1. Issue Description (Problembeschreibung)

The user reports that one application takes longer to open than other applications.

## 2. Initial System Observations

| Resource | Reading |
|---|---:|
| Disk utilization | 8% |
| CPU utilization | 15% |
| Memory utilization | 55% |

The administrator resolved the initial disk-utilization issue. The remaining application performance problem has not been resolved.

## 3. Investigation and Analysis

Since other applications open normally, the next investigation should focus on the affected application.

Possible checks include:

- Inspect Task Manager for the application's process.
- Check whether the process remains after the application window is closed.
- Record any error messages.
- Determine whether the delay occurs every time the application starts.
- Gather further evidence before selecting a corrective action.

These checks are planned; their results have not yet been confirmed.

## 4. Access and Escalation

The current user account has standard-user permissions.

Any action requiring administrator privileges must be performed by an authorized administrator. Escalation is appropriate if such access is needed.

## 5. Current Outcome

- Initial disk-utilization issue: Resolved by the administrator.
- Remaining application issue: Under investigation.
- Root cause: Not confirmed.
- Application-specific fix: Not verified.
- Ticket status: Open.

## 6. What I Learned

- Narrow the investigation when only one application is affected.
- Distinguish planned diagnostic steps from completed checks.
- Document observed facts rather than assumptions.
- Respect access permissions and escalate when necessary.
- Verify the result before closing a ticket.

## 7. German IT Vocabulary

| German | English |
|---|---|
| Störung | Incident / fault |
| Anwendung | Application |
| Fehlerbehebung | Troubleshooting |
| Eskalation | Escalation |
| Administratorrechte | Administrator privileges |
| Ursache | Cause |
| Bearbeitungsstatus | Ticket status |
| Gelöst | Resolved |
| In Bearbeitung | In progress |
| Überprüfung | Verification |
