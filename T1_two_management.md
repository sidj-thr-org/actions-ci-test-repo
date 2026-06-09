# T1: Two Management Approvals

**Expected result: PASS**

Both approvers are in `qvac-mgmt` (Management). The `pending-approvals` check requires `codeowners >= 1` AND `total >= 2`. Here codeowners=2, total=2 — threshold met.

## Approvers

| Account | Team | Role |
|---------|------|------|
| sidj-ubq | qvac-mgmt | Management |
| siddharthjaincodes | qvac-mgmt | Management |

## Team structure (octoops)

```json
{
  "org": "sidj-thr-org",
  "teams": [
    { "name": "qvac-mgmt", "privacy": "closed", "members": [
        { "username": "sidj-ubq", "role": "member" },
        { "username": "siddharthjaincodes", "role": "member" }
    ]},
    { "name": "qvac-internal-merge", "privacy": "closed", "members": [] },
    { "name": "qvac-internal-dev",   "privacy": "closed", "members": [] }
  ]
}
```
