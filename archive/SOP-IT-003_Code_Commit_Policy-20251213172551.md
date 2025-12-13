**Standard Operating Procedure**

**SOP-IT-003: Code & Commit Policy**

|                     |            |                  |            |
|---------------------|------------|------------------|------------|
| **Document ID:**    | SOP-IT-003 | **Version:**     | 1.0        |
| **Effective Date:** | YYYY-MM-DD | **Review Date:** | YYYY-MM-DD |

1\. Purpose

This SOP establishes coding standards, commit practices, and Pull
Request workflow to ensure code quality, traceability, and FDA
compliance.

2\. Scope

This SOP applies to all software development activities using GitHub for
version control and code review.

3\. Commit Message Format

**Required Format:**

\[CR-YYYY-XXXX\] Short description (max 72 chars)

Extended body:

What: What changed Why: Business justification How: Implementation
details Tested: Verification method

3.1 Good Example

\[CR-2024-0042\] Fix XRD calibration drift What: Updated wavelength
calibration coefficients Why: Lab found 0.5nm drift after 100 scans How:
Linear correction based on reference peaks Tested: Verified on 50
historical scans, all within spec

3.2 Bad Example

fixed bug ← No CR number, no details, no value

4\. Commit Requirements

- **ALWAYS reference Change Request number \[CR-YYYY-XXXX\]**

- **GPG sign all commits (git commit -S)**

- **NO direct commits to main branch**

- Atomic commits (one logical change per commit)

- Test code before committing

5\. Pull Request Process

**5.1 Creating Pull Request:**

- Use PR template (includes CR number, description, testing)

- Link to Change Request in description

- Assign minimum 2 reviewers (not including yourself)

**5.2 Review Requirements:**

- **Minimum 2 approvals required**

- **At least 1 must be Dev Lead or QA Lead**

- **Author CANNOT approve their own PR**

- All CI/CD tests must pass

- All review comments resolved

**5.3 Code Review Checklist:**

- Functionality: Does code work as intended?

- Quality: Is code readable and maintainable?

- Testing: Are tests adequate and passing?

- Compliance: Commits GPG-signed, CR referenced?

**5.4 Merge Process:**

- **Only Dev Lead or SRE Lead can merge**

- Use 'Squash and merge' strategy

- Delete feature branch after merge

- Update Change Request status

6\. Approvals

This document requires electronic signature approval via DocuSign (21
CFR Part 11 compliant).

|                            |          |                      |
|----------------------------|----------|----------------------|
| **Role**                   | **Name** | **Signature & Date** |
| Author                     | \[Name\] | \[DocuSign\]         |
| Reviewer (QA Lead)         | \[Name\] | \[DocuSign\]         |
| Approver (Quality Manager) | \[Name\] | \[DocuSign\]         |
