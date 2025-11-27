# Release Checklist

An expanded checklist for releases, built upon the [Release & Deployment Guide](./octoacme-release-and-deployment.md). Use this checklist during release windows to ensure consistent, safe deployments.

---

## Pre-Release Requirements

**Owner: Release Manager or PM**

- [ ] All acceptance criteria met and PRs merged to release branch
- [ ] Passing CI, including tests and security scans
- [ ] Release notes drafted and reviewed
- [ ] Rollback/mitigation plan documented and communicated
- [ ] Smoke test plan prepared and assigned
- [ ] Stakeholder sign-off obtained (if required)

---

## Deployment Checklist

**Owner: Release Manager**

### Before Deployment
- [ ] Deployment window scheduled and communicated to team
- [ ] Backup or snapshot created (if applicable)
- [ ] On-call/support team notified of pending release

### Staging Deployment
- [ ] Deploy to staging environment
- [ ] Run smoke tests on staging
- [ ] Verify key functionality and integrations
- [ ] Review logs and monitoring for errors

### Production Deployment
- [ ] Deploy to production (use automated pipeline when available)
- [ ] Run post-deploy smoke tests
- [ ] Verify key user flows are working
- [ ] Monitor dashboards for errors, latency, and anomalies

---

## Rollback Steps

If deployment fails or causes critical issues:

1. **Trigger incident response** — Notify on-call and relevant stakeholders
2. **Assess severity** — Determine if rollback is necessary
3. **Execute rollback** — Revert to last known-good release
4. **Communicate status** — Update stakeholders and support team
5. **Triage root cause** — Capture action items for post-incident review

---

## Communications

### Pre-Release
- [ ] Notify stakeholders of release timing and scope
- [ ] Brief support/customer success team on new features and known issues

### Post-Release
- [ ] Announce release completion to stakeholders
- [ ] Publish release notes (internal and/or external as appropriate)
- [ ] Notify support team that release is live

---

## Stakeholder Notification Matrix

Who should be informed for different release types:

| Stakeholder Group     | Patch | Minor | Major |
|-----------------------|:-----:|:-----:|:-----:|
| Engineering Team      | ✓     | ✓     | ✓     |
| Product Manager       | ✓     | ✓     | ✓     |
| Support/Customer Success | ✓  | ✓     | ✓     |
| Stakeholders/Leadership |      | ✓     | ✓     |
| External Users/Customers |     |       | ✓     |
| Marketing/Comms       |       |       | ✓     |

---

## Post-Release Verification Timeline

| Timeframe       | Verification Activity                              |
|-----------------|---------------------------------------------------|
| Immediately     | Smoke tests pass, no critical errors in logs      |
| 15 minutes      | Key metrics stable, no spike in errors            |
| 1 hour          | User-facing functionality verified, no escalations|
| 24 hours        | Broader monitoring review, collect initial feedback|
| 1 week          | Full release retrospective (for major releases)   |

---

## Quick Reference

- **Pre-release requirements**: See [Release & Deployment Guide](./octoacme-release-and-deployment.md#pre-release-requirements)
- **Rollback playbook**: See [Release & Deployment Guide](./octoacme-release-and-deployment.md#rollback--incident-playbook)
- **Release notes template**: See [Release & Deployment Guide](./octoacme-release-and-deployment.md#release-notes-template)
