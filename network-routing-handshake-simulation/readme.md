# TryHackMe — TCP Routing & Multi-Handshake Lab

**Date:** 2025-10-07  
**Source:** TryHackMe (TCP routing / handshake simulation)  
**Objective:** Use the network simulator to send a TCP packet from `computer1` to `computer3`, observe the routing and handshake sequence, and reconstruct the resulting flag.

---

## Short summary
This short lab demonstrates how TCP packets traverse a simulated network and how multiple handshake exchanges can occur during routing and retries. The simulator breaks down every hop and action taken by a packet as it moves from point A to B. In this exercise, I sent a TCP packet from **computer1** to **computer3** and observed five handshake attempts before the final successful exchange revealed the lab flag.

---

## Steps performed
1. Deployed the provided static site and opened the network simulator in the TryHackMe lab UI.  
2. Initiated a TCP packet from `computer1` destined for `computer3`.  
3. Monitored the simulator as it displayed each hop and the handshake attempts — counted **five** handshake attempts/rounds during the process.  
4. Observed the final successful TCP handshake and recorded the flag (redacted for public sharing as `<FLAG_REDACTED>`).  
5. Captured and saved a redacted screenshot showing the handshake sequence and routing steps (`screenshots/tcp-routing-handshakes-redacted.png`).

---

## Key learning points
- How TCP establishes a connection across multiple hops and how retransmissions/extra handshakes can occur if packets are delayed or lost.  
- The importance of understanding routing and intermediate devices when troubleshooting connectivity issues.  
- How simulators can visualise per-hop behaviour and help debug network flows without needing access to physical equipment.

---

## Skills practised
- TCP handshake & retransmission observation  
- Basic packet routing comprehension and hop-by-hop analysis  
- Documentation and safe redaction of lab artifacts

---

## Files included
- `screenshots/tcp-routing-handshakes-redacted.png` — redacted screenshot showing the simulator output.  

**Note:** The flag and any sensitive or identifying values are redacted (`<FLAG_REDACTED>`). All work was performed in a TryHackMe lab environment only.
