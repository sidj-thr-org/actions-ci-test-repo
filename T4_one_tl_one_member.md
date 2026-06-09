# T4: One Team Lead + One Member

**Expected result: PASS**

`sidj-ubq` is a Team Lead in `qvac-internal-merge`; `siddharthjaincodes` is a Member in `qvac-internal-dev`. codeowners=1 (Team Lead counts), total=2 — both conditions met.

## Approvers

| Account | Team | Role |
|---------|------|------|
| sidj-ubq | qvac-internal-merge | Team Lead |
| siddharthjaincodes | qvac-internal-dev | Member |

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
