**Standard Operating Procedure**

**SOP-101: Change Control**

|                     |            |                  |            |
|---------------------|------------|------------------|------------|
| **Document ID:**    | SOP-101    | **Version:**     | 1.0        |
| **Effective Date:** | YYYY-MM-DD | **Review Date:** | YYYY-MM-DD |

1\. Purpose

This procedure establishes the process for managing changes to the
XRD-based diagnostic system, ensuring all modifications are reviewed,
approved, tested, and documented in compliance with FDA 21 CFR Part 11
and Part 820 requirements.

2\. Scope

This SOP applies to all changes affecting: software code, documentation,
system configuration, database schema, infrastructure, and laboratory
procedures.

3\. Change Control Workflow

**Step 1: Initiate Change Request**

- Create Change Request in GitHub Issue using FORM-001 template

- Document business justification and impact assessment

- Assign to Development Lead for technical review

**Step 2: Technical Review & Approval**

- Development Lead reviews technical feasibility

- QA Lead reviews quality and compliance impact

- Quality Manager provides final approval

**Step 3: Implementation**

- Developer creates feature branch from main

- Implements changes following coding standards

- All commits must reference Change Request number

- Creates Pull Request when ready for review

**Step 4: Code Review**

- Minimum 2 approvers required (not including author)

- At least 1 approver must be Dev Lead or QA Lead

- CI/CD tests must pass before merge allowed

- All review comments must be resolved

**Step 5: Merge & Deploy**

- Dev Lead or SRE Lead merges to main branch

- Automated tests run on main branch

- Quality Manager approves production deployment

- SRE Lead executes deployment

**Step 6: Verification & Closure**

- QA Lead verifies change in production

- Update Change Request with deployment details

- Close Change Request with sign-off

4\. Critical Requirements

- **NO direct commits to main/production branches**

- **Branch protection MUST be enabled on main**

- **All changes MUST have traceability to Change Request**

- **Quality Manager approval required for prod deployment**
