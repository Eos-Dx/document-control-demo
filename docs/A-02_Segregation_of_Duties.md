**APPENDIX A-02**

**Segregation of Duties (SoD)**

|                     |            |                  |            |
|---------------------|------------|------------------|------------|
| **Document ID:**    | A-02       | **Version:**     | 1.0        |
| **Effective Date:** | YYYY-MM-DD | **Review Date:** | YYYY-MM-DD |

1\. Purpose

This appendix defines the Segregation of Duties (SoD) matrix to ensure
that no single individual has control over all phases of a critical
process. This reduces the risk of errors, fraud, and non-compliance with
FDA regulations (21 CFR Part 11 and Part 820).

2\. Scope

This SoD matrix applies to all software development, quality management,
and laboratory operations processes within the organization.

3\. Key Principles

- **No single person can initiate AND approve a change**

- **Development and Quality Assurance must be independent**

- **Code review requires at least 2 approvers (not including author)**

- **Production deployment requires Quality Manager approval**

- **Document approval requires segregation between author and approver**

4\. Segregation of Duties Matrix

The following table defines which roles can perform which actions. ✓ =
Allowed, ✗ = Prohibited

| **Action**                         | **Dev Lead** | **Developer** | **QA Lead** | **Quality Mgr** | **SRE Lead** | **Product Owner** |
|------------------------------------|--------------|---------------|-------------|-----------------|--------------|-------------------|
| Create Change Request              | ✓            | ✓             | ✓           | ✗               | ✓            | ✓                 |
| Approve Change Request             | ✓            | ✗             | ✓           | **✓**           | ✗            | ✗                 |
| Write Code                         | ✓            | ✓             | ✗           | ✗               | ✓            | ✗                 |
| Approve Pull Request (Code Review) | ✓            | ✓\*           | ✓           | ✗               | ✓            | ✗                 |
| Merge to Main Branch               | ✓            | ✗             | ✗           | ✗               | ✓            | ✗                 |
| Deploy to Production               | ✗            | ✗             | ✗           | **✓**           | ✓            | ✗                 |
| Approve SOP Document               | ✗            | ✗             | ✓           | **✓**           | ✗            | ✗                 |
| Execute Lab IQ/OQ/PQ               | ✗            | ✗             | ✓           | ✗               | ✓            | ✗                 |
| Approve Lab Results                | ✗            | ✗             | **✓**       | ✓               | ✗            | ✗                 |

*\* Developer can approve Pull Request only if they are NOT the author*

5\. Critical Requirements

- **Minimum 2 approvers required for all Pull Requests**

- **Quality Manager must approve all production deployments**

- **No developer can approve their own Pull Request**

- **Branch protection must be enforced on main/production branches**

- **All changes must go through Pull Request process (no direct commits
  to main)**

6\. Approvals

This document requires electronic signature approval via DocuSign (21
CFR Part 11 compliant).

|                            |          |                      |
|----------------------------|----------|----------------------|
| **Role**                   | **Name** | **Signature & Date** |
| Author                     | \[Name\] | \[DocuSign Field\]   |
| Reviewer (QA Lead)         | \[Name\] | \[DocuSign Field\]   |
| Approver (Quality Manager) | \[Name\] | \[DocuSign Field\]   |
