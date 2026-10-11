# Day 3 — Slow Laptop Investigation

**Learning area:** Windows performance troubleshooting  
**German terminology:** Leistung, Datenträgerauslastung, Arbeitsspeicher

## 1. Problem Statement

Investigate a reported slow-laptop problem and identify which system resources may contribute to poor performance.

## 2. Observations

| Item | Actual observation |
|---|---|
| Overall disk usage | Low |
| Top process observed | Chrome |
| Disk activity | Fluctuating |
| Slow-performance condition | Not observed during the check |

## 3. Investigation Steps

1. Open Task Manager using `Ctrl + Shift + Esc`.
2. Inspect CPU, memory, and disk usage.
3. Identify the processes using the most system resources.
4. Observe Chrome's resource usage.
5. Check for Windows Update or other background activity if relevant.
6. Compare readings if the slowdown occurs again.

## 4. Findings

Disk usage was low during the observation, so sustained high disk utilization was not evident at that time.

Chrome appeared as the top process, but this alone does not prove that it caused the reported issue.

Disk activity fluctuated. More information is needed to determine whether these changes are normal or related to a performance problem.

The slow-performance condition was not observed during the check, so the root cause remains unconfirmed.

## 5. Troubleshooting Decision

Do not apply a fix without sufficient evidence.

If the issue occurs again, record CPU, memory, and disk readings while the laptop is slow. Compare these with readings when the laptop is operating normally.

## 6. Verification

**Result:** Initial investigation completed. Root cause not confirmed; no fix verified.

## 7. German IT Vocabulary

| German | English |
|---|---|
| Leistung | Performance |
| Datenträgerauslastung | Disk utilization |
| Arbeitsspeicher | RAM / memory |
| Prozess | Process |
| Hintergrundprozess | Background process |
| Auslastung | Utilization |
| Ursache | Cause |
| Fehlerbehebung | Troubleshooting |

## 8. What I Learned

- System readings must be interpreted in context.
- The top process is not necessarily the cause of a problem.
- A reported issue may not occur during an investigation.
- Findings and unresolved questions should be documented honestly.

## 9. Next Learning Goal

Continue practising Windows performance checks and learn to interpret CPU, memory, and disk activity together.
