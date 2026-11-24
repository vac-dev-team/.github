# Security policy

## Reporting a vulnerability

Report it privately. On the repository's **Security** tab, choose **Report a vulnerability**. That opens a private report only the maintainers can see.

Please do not open a public issue or pull request for a vulnerability.

A useful report says:

- which repository and commit you tested;
- what you ran, including the policy file if one was involved;
- what you expected the containment to stop, and what got through;
- the run record or logs, with any secrets removed.

## What counts

This project contains programs. A way for a contained program to do something its policy does not grant is a vulnerability here. Examples: reaching a host outside the policy, reading a credential, escaping the sandbox, regaining authority after it was removed, or forging an operator reset.

## Known limits

These are documented limits, not vulnerabilities. Reports that improve on them are still welcome.

- A program that already holds root in the shared kernel is not contained.
- What a program does with access the policy granted is limited only by the budgets. An allowed host is allowed.
- A credential that lives inside the sandbox cannot be taken back.
- The model server runs outside the sandbox.
- Linux itself is tested, not proved.

## Supported versions

The project is a research prototype with no supported releases yet. Reports against the default branch are the most useful.
