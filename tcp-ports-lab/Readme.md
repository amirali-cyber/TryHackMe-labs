# TryHackMe — Ports (Practical: connect to port 1234)

**Date:** 2025-10  
**Source:** TryHackMe (Ports practical)  
**Objective:** Understand TCP/UDP ports and practise making a simple client connection to a listening service (lab-only) to retrieve a flag.

---

## Short summary
This lab demonstrates how network services listen on ports (0–65535) and how clients connect to a specific port to exchange data. The practical task required connecting to an endpoint on port **1234** to receive a lab flag. The exercise reinforced how ports map services to application behaviour and the difference between well-known, registered, and ephemeral ports.

---

## What I did (steps performed)
1. Read the lab notes about port ranges and common ports (0–1023 = well-known/common ports; 1024–49151 = registered; 49152–65535 = dynamic/ephemeral).  
2. From the TryHackMe lab environment, connected to the provided endpoint on port **1234** (lab environment only). Example client used: `nc` (netcat) — `nc <LAB_IP> 1234`.  
3. The service responded with a flag; I recorded the flag value but redacted it for public posting (`<FLAG_REDACTED>`).  
4. Took a redacted screenshot showing the successful connection and the returned message (`screenshots/port-1234-connection-redacted.png`).  
5. Noted key learning points and safety practices.

---

## Key learning points
- Ports allow multiple services to run on the same IP by separating traffic by number.  
- Well-known ports (0–1023) are typically reserved for system or core services (HTTP:80, HTTPS:443, SSH:22).  
- Tools like `nc` (netcat), `telnet`, and `ncat` can be used to interact with simple TCP services for testing and learning.  
- Always perform active probing from authorised lab environments — do **not** connect to public IPs/ports without permission.

---

## Skills practised
- Understanding port ranges and service-port mapping  
- Basic client connections to TCP services (netcat/telnet)  
- Safe lab documentation and redaction

---

## Files included
- `commands-sanitised.sh` — illustrative commands for lab use only.  
- `screenshots/port-1234-connection-redacted.png` — redacted screenshot showing the successful connection.

**Note:** The lab flag and any sensitive details are redacted (`<FLAG_REDACTED>`). All activity was performed inside a TryHackMe lab environment only.
