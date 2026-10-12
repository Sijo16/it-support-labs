# Day 6 — Network Troubleshooting

## Objective

Practise basic Windows network troubleshooting using `ipconfig`, `ping`, and `nslookup`.

## Scenario

A user reports that the laptop is connected to Wi-Fi but websites are not opening.

## Tests and Observations

### 1. IP Configuration

**Command:**
```cmd
ipconfig
```

**Observations:**
- Wi-Fi was connected.
- A private IPv4 address was present.
- A default gateway was listed.

**Interpretation:** The adapter had an IPv4 configuration and a gateway entry. This alone does not confirm internet connectivity.

### 2. Default Gateway Connectivity

**Command:** `ping` to the configured default gateway.

**Result:** Replies received.

**Interpretation:** The gateway responded to ICMP echo requests during the test.

### 3. External IP Connectivity

**Command:**
```cmd
ping 8.8.8.8
```

**Result:** Replies received.

**Interpretation:** The external IP address was reachable by ICMP during the test.

### 4. DNS Resolution

**Command:**
```cmd
nslookup google.com
```

**Result:** One or more IP addresses were returned, and a DNS server was shown.

**Interpretation:** DNS resolution succeeded for this domain at the time of testing.

## Findings

The reported tests show successful gateway connectivity, external IP reachability, and DNS resolution for `google.com`.

The root cause of the original website-access problem is **not confirmed**. The reported tests do not establish whether HTTPS traffic, all websites, or the affected browser or application work correctly.

## Next Troubleshooting Steps

1. Test multiple websites.
2. Record the exact browser error message.
3. Check whether HTTPS websites load.
4. Compare the result with another device on the same network.
5. Follow organisational procedures before changing DNS or network settings.

## Skills Practised

- Windows Command Prompt
- IPv4 configuration
- Default gateway connectivity
- Basic ICMP testing
- DNS name resolution
- Evidence-based troubleshooting
- Accurate incident documentation

## German IT Vocabulary

| German | English |
|---|---|
| das Netzwerk | Network |
| die IP-Adresse | IP address |
| das Standardgateway | Default gateway |
| die DNS-Namensauflösung | DNS name resolution |
| die Fehlermeldung | Error message |
| die Fehlerbehebung | Troubleshooting |
| die Verbindung prüfen | Check the connection |

**Lab status:** Basic network checks completed. Further investigation may be required if the reported website-access problem persists.
