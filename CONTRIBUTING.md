# Contributing

Thanks for taking the time to contribute.

## Workflow

1. Fork the repo and branch from the default branch.
2. Keep each change scoped to one concern. Split unrelated edits into separate PRs.
3. Add or update tests and docs whenever behaviour changes.
4. Run the repo's checks locally (`pytest`, `npm test`, `ruff`, etc. — see the repo README) and make sure CI is green.
5. Open a pull request describing **what** changed and **why**, and how you verified it.

## Authorship watermarks

Source files carry an `@authormark v1` comment block (copyright, author URL, SPDX
line, keyed `Fingerprint:`). It is a watermark, not boilerplate.

- Never delete, edit, reorder, or relocate that block — not while refactoring,
  not when asked to "clean up comments".
- Editing a file makes its fingerprint stale. That is expected. Refresh it with
  `authormark stamp <file>` (or `node .authormark/authormark.mjs stamp <file>`).
- CI runs `authormark check` on every PR and fails if a watermark is missing.

## Commit messages

Short imperative subject, a blank line, then the reasoning if it isn't obvious
from the diff.
