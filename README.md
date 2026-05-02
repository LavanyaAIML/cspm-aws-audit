# ☁️ Cloud Security Posture Management (CSPM) — AWS Audit

**Tools:** AWS, Prowler, IAM, S3, EC2, CIS Benchmark, NIST CSF  
**Type:** Blue Team | Cloud Security | Compliance Audit  
**Status:** Completed — 2026

---

## 📌 Project Overview

This project is a hands-on cloud security audit of an AWS environment using **Prowler**, an open-source CSPM tool. The goal was to identify misconfigurations, benchmark the environment against **CIS AWS Foundations**, and produce a structured remediation roadmap aligned with the **NIST Cybersecurity Framework (CSF)**.

---

## 🔍 What I Did

- Deployed and configured **Prowler v3** against a personal AWS test environment
- Scanned **IAM, S3, and EC2** services for security misconfigurations
- Identified **25+ CIS Benchmark violations** including overly permissive IAM policies, public S3 buckets, and unencrypted EBS volumes
- Mapped each finding to **NIST CSF functions** (Identify, Protect, Detect, Respond, Recover)
- Documented step-by-step remediation for each critical finding
- Estimated **~60% reduction in cloud risk exposure** after applying recommended fixes

---

## 🚨 Key Findings (Sample)

| # | Service | Finding | Severity | CIS Control |
|---|---------|---------|----------|-------------|
| 1 | IAM | Root account has active access keys | Critical | 1.4 |
| 2 | IAM | MFA not enabled for all IAM users | High | 1.10 |
| 3 | S3 | Public read access enabled on bucket | High | 2.1.1 |
| 4 | EC2 | Security group allows 0.0.0.0/0 inbound SSH | High | 5.2 |
| 5 | IAM | Overly permissive inline policy (AdministratorAccess) | Critical | 1.16 |

> Full findings report available in `/findings/prowler_report.html`

---

## 🛠️ Remediation Approach

Each finding was remediated or documented with:
- **Root cause** — why the misconfiguration exists
- **Fix steps** — CLI commands or console steps to resolve
- **NIST CSF mapping** — which function and category it addresses
- **CIS Benchmark reference** — specific control number

---

## 📚 Skills Demonstrated

- Cloud security posture assessment
- IAM hardening and least-privilege principles
- CIS Benchmark evaluation
- NIST CSF compliance documentation
- AWS CLI and security tooling (Prowler)

---

## 🔗 References

- [Prowler GitHub](https://github.com/prowler-cloud/prowler)
- [CIS AWS Foundations Benchmark](https://www.cisecurity.org/benchmark/amazon_web_services)
- [NIST Cybersecurity Framework](https://www.nist.gov/cyberframework)
