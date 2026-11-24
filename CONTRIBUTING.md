# Contributing

Each repository's `AGENTS.md` holds its working rules, for people and for agents alike. Read it first.

## Pull requests

- A pull request does not need an issue. If you have a change, open the pull request.
- Keep one topic per pull request.
- Checks decide whether it merges. Nobody approves pull requests by hand, so a red check is the thing to fix.
- Changes to check scripts are welcome. They take effect at the next release, when a new check image is built and adopted, and only if the new image still catches every seeded fault the current one catches.

## Issues

There are two kinds.

- **Task**: something the maintainer has decided should happen.
- **Break**: something an evaluation run found getting through the containment, with its run record.

Agents open Break issues only, and only from an evaluation run. An agent-opened issue with no linked pull request and no reply closes automatically.

## Security problems

Do not open an issue. Follow the security policy.

## Licence

Contributions are dual licensed under MIT or Apache-2.0, as each repository's README describes.
