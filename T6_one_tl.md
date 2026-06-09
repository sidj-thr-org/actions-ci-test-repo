# T6: One Team Lead Only

**Expected result: FAIL**

Only `sidj-ubq` (Team Lead) approves. `siddharthjaincodes` is placed in `qvac-internal-dev` for write access but does not approve. codeowners=1 but total=1 — fails the `total >= 2` condition.

## Approvers

| Account | Team | Role | Approves? |
|---------|------|------|-----------|
| sidj-ubq | qvac-internal-merge | Team Lead | Yes |
| siddharthjaincodes | qvac-internal-dev | Member | No |

## Team structure (octoops)

```json
{
  "org": "sidj-thr-org",
  "teams": [
    { "name": "qvac-mgmt", "privacy": "closed", "members": [] },
    { "name": "qvac-internal-merge", "privacy": "closed", "members": [
        { "username": "sidj-ubq", "role": "member" }
    ]},
    { "name": "qvac-internal-dev", "privacy": "closed", "members": [
        { "username": "siddharthjaincodes", "role": "member" }
    ]}
  ]
}
```
