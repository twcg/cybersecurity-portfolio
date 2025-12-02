# 🔒 Enterprise Security Automation Portfolio

## 🚀 Transforming Manual Security into Automated Compliance

**Professional cybersecurity automation framework implementing CIS-hardened infrastructure through Ansible, reducing deployment time from 45 minutes to 45 seconds while ensuring audit-ready compliance.**

---

## 📊 Portfolio Highlights

| Metric | Achievement |
|--------|-------------|
| **Deployment Time** | 95% faster (45min → 45sec) |
| **Critical Vulnerabilities** | 0 in hardened SSH |
| **NIST 800-53 Compliance** | 5/5 controls automated |
| **Audit-Ready** |
| **Lynis Hardening Index** | 58 | 82 | **↑ 24 points** |
| **CIS Compliance** | 71% of SSH controls implemented |
| **Automation Coverage** | 100% of security configurations |
---

## 🛠️ Featured Projects

### 🔧 Automated Linux Security Hardening
**Infrastructure-as-Code security implementation**
- **Technologies**: Ansible, SSH, CIS Benchmarks
- **Results**: Eliminated critical SSH vulnerabilities, enforced key-based authentication
- **Evidence**: [View Implementation](02-automated-implementation/ansible/)

### 🔍 Vulnerability Management Pipeline  
**Continuous security monitoring & remediation**
- **Technologies**: Greenbone, Automated Scanning, Risk Assessment
- **Results**: Identified and remediated cryptographic weaknesses in SSH configuration
- **Evidence**: [View Case Study](02-automated-implementation/assets/security-scans/vulnerability-remediation.md)

- ### 📋 Compliance-as-Code Framework
**Audit-ready security controls**
- **Standards**: CIS Ubuntu Linux 24.04 LTS, NIST 800-53 alignment
- **Coverage**: 5/5 NIST controls + 5/7 CIS controls implemented and automated
- **Evidence**: [View Compliance Reports](03-compliance-reports/)

---

## 🛡️ Security Compliance Dashboard

### SSH Service Hardening (CIS Section 5.2)
| Control | CIS Benchmark | Status | Evidence |
|---------|---------------|--------|----------|
| Disable root SSH login | 5.2.8 | ✅ **Implemented** | [View Code](https://github.com/twcg/cybersecurity-portfolio/blob/cybersecurity-portfolio/02-automated-implementation/ansible/roles/ssh-hardening/templates/sshd_config.j2#L8) |
| Disable password authentication | 5.2.3 | ✅ **Implemented** | [View Code](https://github.com/twcg/cybersecurity-portfolio/blob/cybersecurity-portfolio/02-automated-implementation/ansible/roles/ssh-hardening/templates/sshd_config.j2#L9) |
| Configure SSH Protocol | 5.2.2 | ✅ **Implemented** | [View Code](https://github.com/twcg/cybersecurity-portfolio/blob/cybersecurity-portfolio/02-automated-implementation/ansible/roles/ssh-hardening/templates/sshd_config.j2#L5) |
| Set MaxAuthTries | 5.2.5 | ✅ **Implemented** | [View Code](https://github.com/twcg/cybersecurity-portfolio/blob/cybersecurity-portfolio/02-automated-implementation/ansible/roles/ssh-hardening/templates/sshd_config.j2#L6) |
| Configure ClientAlive intervals | 5.2.12 | ✅ **Implemented** | [View Code](https://github.com/twcg/cybersecurity-portfolio/blob/cybersecurity-portfolio/02-automated-implementation/ansible/roles/ssh-hardening/templates/sshd_config.j2#L7) |
| Firewall configuration | 3.5.1.1 | 🟡 **Planned** | Target: Q4 2025 |
| Auditd implementation | 4.1.1.1 | 🟡 **Planned** | Target: Q4 2025 |

**Progress: ██████████ 71%** (5/7 controls implemented)

### NIST 800-53 Controls (Automated)
| Control | Name | Status | Evidence |
|---------|------|--------|----------|
| AC-2 | Account Management | ✅ **Automated** | [View Mapping](03-compliance-reports/) |
| AC-3 | Access Enforcement | ✅ **Automated** | [View Mapping](03-compliance-reports/) |
| CM-6 | Configuration Settings | ✅ **Automated** | [View Mapping](03-compliance-reports/) |
| IA-2 | Identification & Authentication | ✅ **Automated** | [View Mapping](03-compliance-reports/) |
| SC-28 | Protection of Information at Rest | ✅ **Automated** | [View Mapping](03-compliance-reports/) |

**NIST Progress: ██████████ 100%** (5/5 controls automated)


---

## 🎯 Business Impact

### Operational Efficiency
- **95% Time Reduction**: Server hardening accelerated from 45 minutes to 45 seconds
- **Zero Configuration Drift**: Version-controlled automation ensures consistency
- **Reduced MTTR**: Security incidents can be remediated through automated re-deployment

### Risk Management  
- **Critical Risk Elimination**: 0 critical vulnerabilities in hardened SSH service
- **Compliance Assurance**: CIS benchmark compliance with audit trail
- **Scalable Security**: Framework supports enterprise multi-environment deployment

---

## 🔬 Technical Evidence

### Implementation Proof
- [Ansible Automation Code](02-automated-implementation/ansible/)
- [SSH Hardening Configuration](02-automated-implementation/ansible/roles/ssh-hardening/templates/sshd_config.j2)
- [Playbook Execution Evidence](02-automated-implementation/assets/automation-evidence/execution-evidence/successful_playbook_run.png)

### Security Validation
- [Vulnerability Management Case Study](02-automated-implementation/assets/security-scans/vulnerability-remediation.md)
- [Greenbone Scan Results](02-automated-implementation/assets/security-scans/security-scan-post-ansible/04-rescan-results/)
- [Compliance Verification](02-automated-implementation/assets/security-scans/security-scan-post-ansible/04-rescan-results/results-after-patchpng.png)

---
## 📄 Compliance Evidence

### Automated Validation
- [NIST 800-53 Compliance Reports](03-compliance-reports/assets/)
- [Compliance Automation Framework](03-compliance-reports/)
- [Control Implementation Evidence](03-compliance-reports/README.md)

### Technical Implementation
- [Ansible Automation Code](02-automated-implementation/ansible/)
- [SSH Hardening Configuration](02-automated-implementation/ansible/roles/ssh-hardening/templates/sshd_config.j2)
- [Vulnerability Management Case Study](02-automated-implementation/assets/security-scans/vulnerability-remediation.md)
  
## 🚀 Quick Start

```bash
# Deploy security hardening
git clone https://github.com/twcg/cybersecurity-portfolio.git
cd cybersecurity-portfolio/02-automated-implementation/ansible
ansible-playbook -i inventories/production.ini hardening-playbook.yml
