# T3: Two Team Leads

**Expected result: PASS**

Both approvers are in `qvac-internal-merge` (Team Lead). Team Leads count as codeowners. codeowners=2, total=2 — threshold met.

## Approvers

| Account | Team | Role |
|---------|------|------|
| sidj-ubq | qvac-internal-merge | Team Lead |
| siddharthjaincodes | qvac-internal-merge | Team Lead |

## Team structure (octoops)

```json
{
  "org": "sidj-thr-org",
  "teams": [
    { "name": "qvac-mgmt", "privacy": "closed", "members": [] },
    { "name": "qvac-internal-merge", "privacy": "closed", "members": [
        { "username": "sidj-ubq", "role": "member" },
        { "username": "siddharthjaincodes", "role": "member" }
    ]},
    { "name": "qvac-internal-dev", "privacy": "closed", "members": [] }
  ]
}
```
