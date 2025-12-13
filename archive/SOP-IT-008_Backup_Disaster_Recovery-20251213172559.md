**Standard Operating Procedure**

**SOP-IT-008: Backup & Disaster Recovery**

|                     |            |                  |            |
|---------------------|------------|------------------|------------|
| **Document ID:**    | SOP-IT-008 | **Version:**     | 1.0        |
| **Effective Date:** | YYYY-MM-DD | **Review Date:** | YYYY-MM-DD |

1\. Purpose

This SOP establishes backup procedures and disaster recovery protocols
to ensure business continuity and data protection for FDA-regulated
systems.

2\. Scope

This SOP applies to all critical IT systems, databases, and data storage
containing GxP-relevant information.

3\. Backup Strategy

**Database Backups:**

- Full backup: Daily at 2 AM UTC

- Incremental backup: Every 6 hours

- Retention: 30 days recent, 7 years compliance data

**Code & Documentation:**

- GitHub: Automatic replication to secondary region

- SharePoint: Microsoft 365 built-in redundancy

**Configuration & Infrastructure:**

- Infrastructure as Code (IaC) in GitHub

- AWS snapshot policy: Daily with 30-day retention

4\. Disaster Recovery

**Recovery Time Objective (RTO):**

- Critical systems: 4 hours

- Non-critical systems: 24 hours

**Recovery Point Objective (RPO):**

- Database: 6 hours (incremental backup interval)

- Code: Near-zero (GitHub replication)

5\. Testing Requirements

- **Restore test: Monthly**

- **Full DR drill: Annually**

- Results documented and reviewed by Quality Manager

6\. Approvals

This document requires electronic signature approval via DocuSign (21
CFR Part 11 compliant).

|                            |          |                      |
|----------------------------|----------|----------------------|
| **Role**                   | **Name** | **Signature & Date** |
| Author                     | \[Name\] | \[DocuSign\]         |
| Reviewer (QA Lead)         | \[Name\] | \[DocuSign\]         |
| Approver (Quality Manager) | \[Name\] | \[DocuSign\]         |
