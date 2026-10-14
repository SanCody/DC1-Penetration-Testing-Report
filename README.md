# DC-1 Penetration Testing Report

A vulnerability assessment and penetration test of the **DC-1** machine from VulnHub, completed as part of the CPT V4 practical assessment at RedTeam Hacker Academy.

## Overview
DC-1 is a deliberately vulnerable Linux machine running Drupal 7. This report documents the full attack path, from discovery to root access, with evidence and remediation guidance.

## Key Findings
| ID | Finding | Severity |
|----|---------|----------|
| PT-01 | Unauthenticated RCE in Drupal (Drupalgeddon2, CVE-2018-7600) | Critical |
| PT-02 | Sensitive configuration file exposure | High |
| PT-03 | Database credential disclosure | High |
| PT-04 | Privilege escalation via SUID misconfiguration | Critical |
| PT-05 | Weak authentication and password storage | Medium |
| PT-06 | Sensitive information disclosure | Medium |
| PT-07 | Unnecessary service exposure | Low |

## Methodology
Host discovery → service enumeration → vulnerability analysis → exploitation → post-exploitation and privilege escalation, following PTES.

## Tools Used
Netdiscover, Nmap, Metasploit Framework, MySQL client

## Report
- [DC1_VAPT_Report.pdf](./DC1_VAPT_Report.pdf)

## Disclaimer
This work was performed on an intentionally vulnerable machine in an isolated lab environment, for educational purposes only. Do not attempt these techniques against systems you do not own or have explicit permission to test.
