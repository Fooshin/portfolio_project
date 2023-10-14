# Vulnerability Assessment Report <br/> 1st January 2023

## System Description
The server hardware consists of a powerful CPU processor and 128GB of memory. It runs on the latest version of Linux operating system and hosts a MySQL database management system. It is configured with a stable network connection using IPv4 addresses and interacts  with other servers on the network. Security measures include SSL/TLS encrypted connections.
## Scope
The scope of this vulnerability assessment relates to the current access controls of the system. The assessment will cover a period of three months, from June 2023 to August 2023. NIST SP 800-30 Rev. 1 is used to guide the risk analysis of the information system.
## Purpose
This database is valuable to the business because it contains information regarding the guarded data of customers and other business related assets. To not have this data secured and protected or even available leaves the company vulnerable to theft, leaks, and loss of business. If this server were to be compromised, it would stop operations and could in some scenarios bring the company out of compliance with security standards liable to legal action and monetary damages.

## Risk Assessment
| Threat Source | Threat Event| Likelihood | Severity | Risk |
| :----:        |    :----:   |   :----:   |:----:    | :----:| 
| Competitor    | Obtain sensitive information via exfiltration | 1 | 3 | 3 |
| Hacker | Attack and bring down server or ransom data | 3 | 3 | 9|
| Disgruntled Employee | Leaves company and maintains access | 2 | 3 | 6 |

## Approach
The larger the company grows, and the more money and opportunity the company has; its assets will be targeted. It only takes one person to notice these vulnerabilities and proactive measures should be taken to reduce these risks and threats. As the business grows, to not have these vulnerabilities patched or remediated will inevitably cause damage to the company.
## Remediation Strategy
First, with minimal affect to business operations take down the server from public access. Set up controls and properly configure to harden the server from vulnerable access. Next, add layers of implementation of authentication, authorization, and auditing mechanisms to ensure that only authorized users access the database server. These may include enforcing stronger passwords, role-based access controls, and multi-factor authentication to limit user privileges. Add encryption of data in motion using TLS instead of SSL. Upgrading and auditing firewalls and IDPs to detect suspicious behavior, as well as monitoring and incident response strategies would be recommended.