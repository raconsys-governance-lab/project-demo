# Pull Request Policy

## Purpose

Ensure all code changes are reviewed, traceable, and approved before merging.

---

## General Rules

- Direct commits to protected branches are prohibited.
- All changes must be submitted through Pull Requests.
- Every Pull Request must contain a meaningful title and description.
- Pull Requests should be linked to a work item, issue, or task.

---

## Pull Request Template

### Summary

Describe the purpose of this change.

### Changes

List major changes included.

### Testing

Describe validation performed.

### Risk Assessment

Low / Medium / High

### Rollback Plan

Describe rollback steps if required.

---

## Approval Requirements

### Develop Branch

Minimum Requirements:

- Developer self-review
- Optional peer review

Merge Flow:

feature/* → develop

---

### Stage Branch

Minimum Requirements:

- 1 approval required
- QA validation completed

Merge Flow:

develop → stage

---

### Main Branch

Minimum Requirements:

- 1 approval required
- Release validation completed
- Production approval granted

Merge Flow:

stage → main

---

## Review Checklist

Reviewers should verify:

- Code quality
- Security considerations
- Naming standards
- Error handling
- Documentation updates
- No unnecessary files included

---

## Merge Strategy

Allowed:

- Squash Merge
- Rebase Merge

Avoid:

- Large unreviewed merge commits

---

## Emergency Hotfix Process

For critical production issues:

hotfix/* → main

Requirements:

- Immediate review
- Production approval
- Post-release validation

---

## Governance Compliance

Pull Requests violating this policy may be rejected.

Maintained By:
Raconsys Governance Team
