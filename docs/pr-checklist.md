# Pull Request Checklist

A checklist for contributors to complete before requesting review. Copy this into your PR description and check off each item.

---

## Before Requesting Review

- [ ] **Issue linked**: PR description includes a link to the related issue (e.g., `Closes #123`)
- [ ] **Acceptance criteria present**: Acceptance criteria from the issue are listed in the PR description
- [ ] **Tests added/updated**: New or modified functionality has corresponding tests
- [ ] **CI passing**: All automated checks (tests, linting, security scans) pass
- [ ] **Changelog/release notes**: If applicable, changelog or release notes have been updated
- [ ] **Reviewer requested**: At least one reviewer has been assigned
- [ ] **Small, atomic changes**: PR is focused and ideally ≤400 lines changed
- [ ] **Documentation updated**: If behavior changes, relevant docs are updated

---

## PR Description Template

Copy and paste the template below into your pull request description:

```markdown
## Summary
<!-- Brief description of the changes -->

## Related Issue
<!-- Link to the issue this PR addresses -->
Closes #

## Changes Made
<!-- List the key changes in this PR -->
- 

## Acceptance Criteria
<!-- Copy acceptance criteria from the issue -->
- [ ] 

## Testing
<!-- Describe how you tested these changes -->
- 

## Checklist
- [ ] Issue linked
- [ ] Acceptance criteria present
- [ ] Tests added/updated
- [ ] CI passing
- [ ] Changelog/release notes updated (if applicable)
- [ ] Reviewer requested
- [ ] Small, atomic changes
- [ ] Documentation updated (if behavior changes)
```

---

## Tips for Effective PRs

- **Keep PRs small**: Smaller PRs are easier to review and less risky to merge
- **Write clear descriptions**: Help reviewers understand the context and purpose
- **Respond to feedback promptly**: Keep the review cycle moving
- **Self-review first**: Review your own changes before requesting review from others
