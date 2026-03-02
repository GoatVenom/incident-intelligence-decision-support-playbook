# Threat Actor Profile: Financially Motivated Initial Access Brokers (IABs)

## Overview
This profile assesses financially motivated cybercriminal actors commonly referred to as Initial Access Brokers (IABs). These actors specialize in obtaining unauthorized access to enterprise environments and monetizing that access through resale to ransomware affiliates, fraud groups, or other criminal operators. IAB activity represents a critical early-stage risk factor for ransomware deployment, data exfiltration, and downstream financial loss.

## Motivations and Objectives
- Monetize compromised credentials and remote access
- Enable ransomware, extortion, and fraud operations
- Rapid exploitation of weak authentication controls
- Low dwell time prior to resale or handoff

## Observed Tools, Techniques, and Methods
Commonly observed tradecraft includes:
- Credential harvesting via phishing or commodity malware
- Credential reuse against VPNs, cloud services, and remote access portals
- Abuse of valid accounts for persistence
- Basic reconnaissance to validate access value prior to resale

These techniques emphasize speed and scalability over stealth.

## MITRE ATT&CK Mapping (High-Level)

| Tactic | Technique |
|------|----------|
| Initial Access | Valid Accounts (T1078) |
| Credential Access | Phishing (T1566) |
| Persistence | Account Manipulation (T1098) |
| Discovery | Account Discovery (T1087) |

## Targeting Patterns
- Large enterprises with distributed authentication environments
- Organizations with high-value user or privileged accounts
- Industries with strong monetization potential, including financial services and retail

## Relevance to Incident Scenario
Observed indicators in the incident scenario align with known IAB tradecraft, increasing the likelihood that detected activity represents pre-ransomware or pre-fraud access staging rather than isolated opportunistic behavior.

## Intelligence Assessment
Early identification of IAB activity enables containment actions that significantly reduce escalation risk. Failure to disrupt access at this stage increases the probability of ransomware deployment or account takeover within days.
