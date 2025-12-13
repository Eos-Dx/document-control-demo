**Standard Operating Procedure**

**SOP-106: Document Control**

|                     |            |                  |            |
|---------------------|------------|------------------|------------|
| **Document ID:**    | SOP-106    | **Version:**     | 1.0        |
| **Effective Date:** | YYYY-MM-DD | **Review Date:** | YYYY-MM-DD |

1\. Purpose

This procedure defines the Document Lifecycle using GitHub, Confluence,
and SharePoint to ensure FDA compliance (21 CFR Part 11 and Part 820).

2\. Three-System Approach

**GitHub (Version Control & Audit Trail):**

- All SOPs authored in Markdown format

- Immutable commit history with cryptographic signatures

- Pull Request workflow for document review

**Confluence (Collaboration & Workflows):**

- Auto-published from GitHub for team access

- Workflow management and review process

- DHF/DMR structure and organization

**SharePoint (Final Regulatory Records):**

- Signed and approved PDFs only

- Immutable archival with 7+ year retention

- 21 CFR Part 11 compliant e-signatures via DocuSign

3\. Document Lifecycle

- Step 1: Draft in GitHub feature branch

- Step 2: Create Pull Request for review

- Step 3: Quality Manager approval → merge to main

- Step 4: Auto-publish to Confluence

- Step 5: Generate PDF and sign via DocuSign

- Step 6: Archive signed PDF to SharePoint

4\. Critical Controls

- **Branch protection on main branch (no direct commits)**

- **Minimum 2 reviewers for document Pull Requests**

- **Quality Manager must approve before merge**

- **Only signed PDFs stored in SharePoint**

- **SharePoint records are immutable after signing**
