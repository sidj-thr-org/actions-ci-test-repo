# actions-ci-test-repo

Test repository for [`@sidj-thr/actions-ci`](https://www.npmjs.com/package/@sidj-thr/actions-ci).

## What this repo tests

| Trigger | Expected behaviour |
|---------|-------------------|
| PR opened | Posts a `## Review Status` comment immediately |
| PR labeled `verified` | Re-evaluates and updates the comment |
| PR synchronized (new commit pushed) | Re-evaluates and updates the comment |
| Issue comment `pending_reviews` on a PR | Manually re-triggers the check |

## Workflows

### `pending-approvals.yml`

Runs `npx @sidj-thr/actions-ci pending-approvals` on every relevant PR event.

- Exits `0` (green) when the PR has enough approvals
- Exits `1` (red) when approvals are still pending — the job is non-blocking (`continue-on-error` can be added if needed)

## Required secrets & variables

Configure these in **Settings → Secrets and variables → Actions** of this repo.

### Secrets

| Name | Description |
|------|-------------|
| `CI_TOKEN` | GitHub token with `pull-requests: write` and `issues: write` |
| `APP_ID` | GitHub App ID used for team membership resolution |
| `APP_PRIVATE_KEY` | GitHub App private key (PEM) |

### Variables

| Name | Description | Default |
|------|-------------|---------|
| `MAINTAINERS_TEAM` | GitHub team slug for Management | *(required)* |
| `TEAM_LEADS_TEAM` | GitHub team slug for Team Leads | *(required)* |
| `MIN_APPROVALS` | Minimum total approvals required | `2` |

## How to run a manual test

1. Open a PR in this repo
2. Comment `pending_reviews` on the PR — the workflow will trigger and post/update the review status comment
3. Add approvals from the relevant teams and watch the comment update

## Package version

To pin to a specific version instead of `latest`, change the workflow step to:

```yaml
run: npx @sidj-thr/actions-ci@0.1.0 pending-approvals ...
```
TC2 test commit
retrigger Wed Jul  1 17:19:46 IST 2026
