# .github

Organization-wide defaults for `vac-dev-team`.

| Path | What it does |
|---|---|
| `profile/README.md` | The organization's public profile |
| `SECURITY.md` | Default security policy for every repository |
| `CONTRIBUTING.md` | Default contribution guide |
| `.github/ISSUE_TEMPLATE/` | The two issue forms, Task and Break |
| `.github/pull_request_template.md` | Default pull request template |
| `.github/workflows/check.yml` | The check that judges pull requests in product repositories |

## Who can change this repository

The owner and the maintainer App. Builder agents have no access.

## How a change to `check.yml` takes effect

It does not take effect on merge. The organization ruleset "protected main" requires this workflow at one pinned commit. A newer version judges nothing until the owner moves that pin, once per release.
