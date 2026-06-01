# Branch Strategy

## Objective

Provide a controlled software delivery process using GitHub branch governance.

---

## Branch Structure

main
│
stage
│
develop
│
├── feature/*
├── bugfix/*
└── hotfix/*

---

## Branch Purposes

### main

Production-ready code only.

Rules:

- Pull Request required
- Minimum 1 approval
- Force push blocked
- Direct commit blocked

---

### stage

Pre-production testing branch.

Used for:

- QA validation
- UAT testing
- Release verification

Rules:

- Pull Request required
- QA approval required

---

### develop

Integration branch.

Used for:

- Combining completed features
- Internal testing

Rules:

- Developers merge approved feature branches

---

### feature/*

Examples:

feature/login-page

feature/payment-module

Purpose:

- New feature development

Flow:

feature/* → develop

---

### bugfix/*

Examples:

bugfix/payment-calculation

bugfix/profile-validation

Purpose:

- Non-production defect fixes

Flow:

bugfix/* → develop

---

### hotfix/*

Examples:

hotfix/login-outage

hotfix/payment-failure

Purpose:

- Critical production fixes

Flow:

hotfix/* → main

---

## Release Flow

Feature Development

feature/* → develop

QA Validation

develop → stage

Production Release

stage → main

Emergency Release

hotfix/* → main

---

## Benefits

- Controlled releases
- Audit trail
- Safer deployments
- Reduced production risk
- Better code reviews
