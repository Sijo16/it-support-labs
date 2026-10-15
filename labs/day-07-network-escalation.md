# Day 7 — Network Troubleshooting and Escalation

## Objective

Review basic network troubleshooting, interpret test results, and document an incident for escalation to an administrator.

## Scenario

A user reports that websites cannot be opened in Google Chrome or Microsoft Edge. Both browsers display the error:

"This site can't be reached."

Other applications appear to work normally.

## Troubleshooting Performed

### 1. IP Configuration

**Command:**

```cmd
ipconfig
```

**Observations:**
- Wi-Fi was connected.
- A private IPv4 address was present.
- A default gateway was listed.

**Finding:** The laptop had a basic IPv4 configuration.

### 2. Default Gateway Connectivity

**Test:** Ping the configured default gateway.

**Result:** Replies received.

**Finding:** The gateway responded to ICMP echo requests during testing.

### 3. External IP Connectivity

**Command:**

```cmd
ping 8.8.8.8
```

**Result:** Replies received.

**Finding:** The external IP address was reachable by ICMP during testing.

### 4. DNS Resolution

**Command:**

```cmd
nslookup google.com
```

**Result:** IP address(es) were returned, and a DNS server was shown.

**Finding:** DNS resolution succeeded for `google.com` during testing.

### 5. Browser and Proxy Investigation

**Observations:**
- Google Chrome and Microsoft Edge both failed to open websites.
- Both browsers displayed "This site can't be reached."
- Proxy settings were enabled.
- Whether the proxy configuration was required by the organisation had not been confirmed.

**Finding:** A browser-specific issue was less likely because both browsers were affected. Proxy configuration, firewall restrictions, or other HTTPS connectivity problems remained possible causes.

## Incident Assessment

The gateway ping, external IP ping, and DNS lookup succeeded. These results demonstrated basic IP connectivity and successful DNS resolution for the tested domain.

However, the tests did not confirm that all web traffic, including HTTPS, was working correctly.

**Root cause:** Unconfirmed.

No proxy or firewall settings were changed during the investigation.

## Escalation Note

**Incident ID:** INC-007

**Issue:** Unable to access websites using Chrome or Microsoft Edge.

**Actions completed:**
- Checked IP configuration.
- Tested default gateway connectivity.
- Tested external IP connectivity.
- Checked DNS resolution.
- Identified that proxy settings were enabled.

**Escalation reason:** Further investigation may require administrator access or verification of organisational network policies.

**Requested action:** Verify the approved proxy configuration and investigate relevant firewall policies and HTTPS connectivity.

**Status:** Escalated — awaiting administrator investigation.

## Skills Practised

- Windows Command Prompt
- IPv4 configuration
- Default gateway troubleshooting
- ICMP connectivity testing
- DNS name resolution
- Browser troubleshooting
- Proxy and firewall awareness
- Evidence-based incident escalation
- Helpdesk ticket documentation

## German IT Vocabulary

| German | English |
|---|---|
| die Netzwerkverbindung | Network connection |
| die Fehlermeldung | Error message |
| der Proxyserver | Proxy server |
| die Firewall-Regel | Firewall rule |
| die Fehlerbehebung | Troubleshooting |
| die Eskalation | Escalation |
| der Administrator | Administrator |
| die Ursache | Cause |
| nicht bestätigt | Unconfirmed |
| das Ticket weiterleiten | Forward the ticket |

## Key Learning

Successful basic network tests do not prove that every network service is working. A first-line technician should collect evidence, avoid unauthorised configuration changes, document findings accurately, and escalate when required.

**Lab status:** Review and simulated troubleshooting completed. Root cause not confirmed.
