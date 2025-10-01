# TryHackMe — TCP/IP: Three-Way Handshake (Reassembly Lab)

**Date:** 2025-09  
**Source:** TryHackMe (TCP/IP — Three-Way Handshake lab)  
**Objective:** Reassemble a simulated TCP conversation to understand the TCP three-way handshake and normal connection termination (FIN/ACK).

---

## Short summary
This lab walks through the TCP three-way handshake and the connection closing sequence. Using the static lab packet conversation, I reconstructed the order of TCP messages (SYN, SYN-ACK, ACK) and observed the FIN/ACK sequence used to tear down a connection. This exercise reinforces how TCP establishes and closes reliable connections and how packet sequencing matters for session state.

---

## Steps I performed
1. Opened the static conversation in the lab UI and inspected each message entry.  
2. Identified the SYN (client → server) initiating the handshake.  
3. Located the SYN/ACK (server → client) response.  
4. Confirmed the final ACK (client → server) to complete the three-way handshake.  
5. Observed the connection termination sequence (FIN, FIN/ACK, ACK) and noted state transitions.  
6. Reassembled the conversation in order and recorded the resulting “flag” (redacted here as `<FLAG_REDACTED>`).

---

## Key learning points
- **SYN, SYN-ACK, ACK** is the 3-step process that establishes a TCP connection.  
- The **FIN / FIN-ACK / ACK** sequence gracefully closes TCP connections.  
- Correct packet ordering and state tracking are essential for troubleshooting and forensics.  
- Understanding handshake/teardown behavior is foundational for network troubleshooting and intrusion analysis.

---

## Skills practised
- TCP fundamentals and packet sequencing  
- Basic packet inspection and session reassembly logic  
- Lab documentation and redaction best practice

---

## Files included
- `commands-sanitised.sh` — illustrative commands (no real targets or credentials).  
- `screenshots/handshake-reassembly-redacted.png` — screenshot showing reassembled handshake (redacted).  
- `screenshots/connection-close-redacted.png` — screenshot showing FIN/ACK teardown (redacted).

**Note:** The actual lab flag and any sensitive details have been redacted for public posting (`<FLAG_REDACTED>`). This work was completed in a TryHackMe lab environment only.
