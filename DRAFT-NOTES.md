# Notes on these drafts (delete this file before publishing)

None of this has been run. The repository it belongs to does not exist yet.

## Fill in before use

- `check.yml`: replace `REPLACE_WITH_THE_PUBLISHED_CHECK_DIGEST` with the digest that `container.yml`'s manifest job prints after the first publish.
- `break.yml` and `task.yml` use `type: Break` and `type: Task`. Create those two issue types in the organization first (setup guide, Stage 10), or the forms will not apply a type.
- Neither form sets `projects:`. Add `projects: ["vac-dev-team/<number>"]` once the roadmap project exists and you know its number. The person opening the issue needs write access to that project.

## Limits to know about

- `check.yml` currently runs the pull request's own `scripts/check.sh`, because the check scripts are not baked into the image yet. A pull request cannot change this workflow, but it can still change that script. The "pinned judge" property arrives when the checks move into `vac` and ship inside the image.
- `check.yml` is untested as a container job. The image sets `CARGO_HOME`, `RUSTUP_HOME` and `PATH` itself, and marks every directory as safe for git, which is what a container job needs; that has not been confirmed on a runner.
- Whether a ruleset-required workflow runs on pull requests from forks is not stated in GitHub's documentation.
- The `upload` field in `break.yml` and issue forms in general are labelled public preview by GitHub.
- Issue forms may not constrain issues created through the API. The reporter App should fill the same fields.
- `blank_issues_enabled: false` still shows a blank-issue option to people with write access.
- The stale-issue workflow and `dependabot.yml` from the setup guide belong in the product repository, not here, and are not drafted.

## Not included

- A LICENSE file. GitHub does not support an organization-wide default licence; each repository keeps its own.
- A code of conduct. Add one if you want it; I did not pick one for you.
