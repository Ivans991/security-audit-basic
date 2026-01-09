# Security Analysis Report

## 1. Objective
The objective of this analysis is to review the exposed network services of the evaluated system and identify potential security risks based on the results obtained during the reconnaissance phase.

---

## 2. Scope
- Target: Localhost (personal system)
- Operating System: Windows 11
- Type of analysis: Basic network service exposure analysis
- Tools used: Nmap

---

## 3. Scan Summary
The Nmap scan identified the following network behavior:
- The host was reachable and responsive.
- Most TCP ports were closed or filtered.
- A limited number of services associated with the Windows operating system were detected.

---

## 4. Identified Services

| Port | State | Service | Description |
|-----|------|--------|------------|
| 135 | Open | msrpc | Microsoft Remote Procedure Call service |
| 137 | Filtered | netbios-ns | NetBIOS Name Service |
| 445 | Open | microsoft-ds | SMB file sharing service |

---

## 5. Risk Analysis
The detected services are common in Windows environments, especially within local networks. However, services such as SMB and RPC are frequently targeted in cyberattacks when exposed beyond trusted networks.

No evidence of active exploitation was identified during this analysis.

---

## 6. Recommendations
- Restrict access to SMB and RPC services using firewall rules.
- Avoid exposing internal services to public networks.
- Maintain the system updated with the latest security patches.
- Periodically review open ports and active services.

---

## 7. Conclusion
The system shows a limited attack surface with standard Windows services active. While no critical vulnerabilities were identified, proper configuration and access control are essential to reduce potential risks.
