# Day 2 — Basic Network and Windows Troubleshooting

**Learning area:** Network connectivity and Windows diagnostics  
**German terminology:** Netzwerkverbindung, Netzwerkadapter, Geräte-Manager

## 1. Objective

Learn how to inspect network connectivity and check basic Windows system information before attempting a fix.

## 2. Practical Checks Performed

| Check | Observation |
|---|---|
| Wi-Fi connectivity | Wi-Fi worked normally |
| Wireless adapter | Qualcomm Wireless Adapter |
| Device Manager status | Device reported: "This device is working properly" |
| Windows Update | Restart required |
| System inspection | Settings, Task Manager, Device Manager, and installed applications inspected |

## 3. Investigation Process

1. Check whether Wi-Fi is connected.
2. Open Device Manager (*Geräte-Manager*).
3. Expand Network adapters (*Netzwerkadapter*).
4. Inspect the wireless adapter's status.
5. Check Windows Update for pending updates or a restart.
6. Review relevant system information before changing settings.

## 4. Findings and Analysis

The Wi-Fi connection was working normally during the check, and Windows reported no problem with the wireless adapter.

A pending restart for Windows Update was also observed. This does not establish that the update caused a network issue.

No network fault was confirmed during these checks.

## 5. Additional Network Commands to Learn

These commands can be used in future labs:

- `ipconfig` — inspect IP configuration.
- `ping` — test basic reachability.
- `ipconfig /all` — inspect IP address, DHCP, DNS, and gateway details.
- `nslookup` — investigate DNS name resolution.

**Note:** These commands are planned for further practice;

## 6. German IT Vocabulary

| German | English |
|---|---|
| Netzwerk | Network |
| Netzwerkadapter | Network adapter |
| WLAN-Verbindung | Wi-Fi connection |
| Geräte-Manager | Device Manager |
| IP-Adresse | IP address |
| Standardgateway | Default gateway |
| DNS-Auflösung | DNS resolution |
| Neustart erforderlich | Restart required |

## 7. Next Learning Goal

Practise checking IP configuration and distinguishing a Wi-Fi connection issue from an IP addressing or DNS problem.
