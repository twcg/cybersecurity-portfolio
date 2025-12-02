# Enterprise Linux Security Hardening & Automation

## Overview
A production-ready framework for automated security hardening, compliance validation, and continuous monitoring of Linux servers, implementing CIS benchmarks and NIST 800-53 controls.

## Key Results
- **Reduced Critical Vulnerabilities by 85%** (OpenVAS scans)
- **Increased Hardening Index from 58 to 82** (Lynis audit)
- **Fully Automated Remediation** via Ansible (5-minute deployment)

## Project Structure
- `src/ansible/` - All hardening playbooks and roles
- `src/monitoring/` - Dashboard design & detection rules
- `docs/` - Detailed project documentation
- `evidence/` - Scan reports and execution proof

## Quick Start
1. Clone repo: `git clone [your-repo-url]`
2. Review hardening playbooks: `cd src/ansible/`
3. See validation evidence: `open evidence/scans/`

## Documentation
Full walkthrough available in the [docs/](docs/) directory.