# TryHackMe — Topology Flaws

**Date:** 2025-09  
**Source:** TryHackMe (Topology Flaws lab)  
**Objective:** Explore common network topologies and their single-point-of-failure flaws (Ring, Bus, Star) through interactive simulations.

## Short summary
This lab demonstrates how faults affect different network topologies:
- **Ring topology:** breaking the ring stops packet flow around the loop.  
- **Bus topology:** a single backbone cable carries traffic both ways — heavy load and cable faults cause major issues.  
- **Star topology:** every device relies on a central switch; if the switch fails, the whole network is down.

## Steps I performed
1. Observed normal packet flow in each topology using the lab UI.  
2. **Cut the cable** in the Ring topology and verified packets no longer circulated (`ring-cut-redacted.png`).  
3. Observed Bus topology behaviour under fault conditions (noted throughput limits).  
4. **Disabled the central switch** in the Star topology and verified network failure (`star-failure-redacted.png`).  
5. Documented lessons and remediation ideas (redundancy, alternate paths, resilient switching).

## Skills practised
- Network topology fundamentals (Ring, Bus, Star)  
- Understanding single points of failure and basic network resilience concepts  
- Observational lab documentation and safe redaction for public sharing

## Files included
- `commands-sanitised.sh` — example/sanitised commands (illustrative).  
- `screenshots/` — redacted images showing experiments.

**Note:** All sensitive or identifying lab values are redacted for public posting.
