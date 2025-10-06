# TryHackMe — Firewall Lab: Block HTTP (port 80)

**Date:** 2025-10  
**Source:** TryHackMe (Firewall practical)  
**Objective:** Configure a firewall to block malicious HTTP traffic (port 80) from a hostile source to a web server in a controlled lab environment.

---

## Short summary
This lab simulates a small network where malicious packets (marked in red in the lab UI) attempt to reach a web server on port **80** (HTTP). The task was to deploy the provided static site, identify the malicious source, and configure the firewall so that traffic on port 80 from that source no longer reaches the web server (203.0.110.1). All steps were performed within the TryHackMe lab environment.

---

## Steps performed
1. Deployed the static site in the lab environment and opened the traffic capture/console.  
2. Inspected the packet view and identified malicious packets (red) targeting the web server at **203.0.110.1** on port **80**.  
3. Implemented a firewall rule to block the malicious source on port 80 (lab-only).  
4. Verified the firewall by re-checking the traffic; malicious packets were successfully blocked (see `screenshots/firewall-blocked-traffic-redacted.png`).  
5. Documented findings and recommended follow-ups (logging, alerting, and persistent blocking mechanisms).

---

## Key learning points
- Firewalls control network access by filtering traffic by IP, protocol and port.  
- Targeted rules (block single source IP on a specific port) reduce collateral impact compared to broad rules.  
- Verification is essential: always confirm that legitimate traffic is still allowed and malicious traffic is dropped.  
- Logging and alerting of blocked traffic are crucial for visibility and follow-up investigations.

---

## Skills practised
- Basic firewall configuration and rule testing  
- Network troubleshooting and verification (observing blocked vs allowed packets)  
- Safe lab documentation and redaction for public sharing

---

## Files included
- `commands-sanitised.sh` — optional example commands (lab-only; replace lab IPs where appropriate).  
- `screenshots/firewall-blocked-traffic-redacted.png` — redacted screenshot showing blocked malicious traffic.

**Note:** All activity was performed in a TryHackMe lab environment. Any IPs or sensitive values used for demonstration are either reserved/test addresses or redacted. Do NOT run these commands against real-world targets without explicit permission.
