# AWS Cloud Security Lab

> Cloud security work in AWS: IAM least privilege, an EC2 honeynet, and Python automation that audits S3 for misconfigurations.

![Category](https://img.shields.io/badge/Category-Cloud%20Security-blue) ![Tools](https://img.shields.io/badge/Tools-AWS%20%7C%20Python%20%7C%20boto3-informational)

## Overview
| | |
|---|---|
| **Objective** | Secure an AWS environment and automate detection of risky configurations |
| **Tools** | AWS IAM, EC2, S3, Python (boto3) |
| **Skills shown** | Cloud IAM, least privilege, honeypot deployment, security automation |

> ✏️ **Fill in:** replace the bracketed notes below with your exact steps and results.

---

## Part 1: IAM and Least Privilege
- Created a dedicated admin user instead of using the root account; MFA enabled on root.
- [Policies attached and the reasoning for each]

## Part 2: EC2 Honeynet
- Deployed an EC2 instance as a honeypot with SSH key authentication.
- [Security group rules, how long it ran, number of login attempts, top source countries]

## Part 3: S3 Misconfiguration Scanner (Python + boto3)
- Script lists all buckets and flags public access, missing encryption, and disabled versioning.
- Code: [`scanner.py`](./scanner.py)

## Results
[Key numbers and findings]

## Security Notes
- **No credentials are stored in this repo.** Keys are loaded from the local AWS CLI profile or environment variables.
- Account IDs, IP addresses, and ARNs are redacted from screenshots.

## Key Takeaways
- Misconfiguration, not exotic exploits, is the top cause of cloud breaches.
- Automating checks makes security repeatable.
