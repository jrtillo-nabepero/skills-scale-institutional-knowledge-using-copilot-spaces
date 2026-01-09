# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- Release notes drafted (coordinated with Technical Writer)
- Rollback / mitigation plan documented
- Smoke tests prepared
- QA Lead provides signoff on test execution and quality
- DevOps Engineer confirms deployment pipeline readiness and infrastructure capacity
- Customer Success/Support Lead briefed on customer impact and support readiness

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support
- [ ] DevOps Engineer monitors system health and performance post-deployment
- [ ] Customer Success/Support Lead confirms support team readiness and customer communication

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call
  - DevOps Engineer executes rollback to last known-good release if necessary
  - Triage root cause and capture action items
  - Customer Success/Support Lead coordinates customer communication and manages escalations

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
