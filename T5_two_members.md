# T5: Two Members (No Codeowner)

**Expected result: FAIL**

Both approvers are only in `qvac-internal-dev` (Member). Members are not codeowners. codeowners=0, total=2 — fails the `codeowners >= 1` condition.

## Approvers

| Account | Team | Role |
|---------|------|------|
| sidj-ubq | qvac-internal-dev | Member |
| siddharthjaincodes | qvac-internal-dev | Member |

## Team structure (octoops)

```json
{
  "org": "sidj-thr-org",
  "teams": [
    { "name": "qvac-mgmt", "privacy": "closed", "members": [] },
    { "name": "qvac-internal-merge", "privacy": "closed", "members": [] },
    { "name": "qvac-internal-dev", "privacy": "closed", "members": [
        { "username": "sidj-ubq", "role": "member" },
        { "username": "siddharthjaincodes", "role": "member" }
    ]}
  ]
}
```
