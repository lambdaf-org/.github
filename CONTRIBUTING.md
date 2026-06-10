# Contributing to Lambdaforge

Thanks for considering a contribution. This file applies to every repository in the
[`lambdaf-org`](https://github.com/lambdaf-org) organization. For the longer walkthrough, dev setup per
stack, and conventions, read the [**contributor guide**](https://github.com/lambdaf-org/contributing).

Lambdaforge builds small, sharp tools that people actually use. We keep the bar high and the process light.

## Ways to help

- **Report a bug.** Open an issue with steps to reproduce, what you expected, and what happened.
- **Propose a feature.** Open an issue describing the problem first, then the idea. Small, focused proposals land fastest.
- **Send a fix or feature.** Pick up an open issue (comment so we know you are on it) and open a pull request.
- **Improve docs.** READMEs, examples, and the contributor guide are fair game and always welcome.

## Quick workflow

1. Fork the repo and create a branch off the default branch: `git checkout -b fix/short-description`.
2. Make your change. Keep the diff focused on one thing.
3. Run the project's checks locally (build, tests, linter, formatter). See the repo README and the [contributor guide](https://github.com/lambdaf-org/contributing) for the exact commands per stack.
4. Commit with a clear message. We use [Conventional Commits](https://www.conventionalcommits.org): `feat:`, `fix:`, `docs:`, `refactor:`, `test:`, `chore:`.
5. Open a pull request against the default branch and fill in the template. Link the issue it closes.

## What we look for in a PR

- It does one thing, and the title says what.
- It builds, and existing checks pass.
- New behavior has a test where the stack supports it.
- Public behavior or commands that changed are reflected in the README.
- No unrelated reformatting that buries the real change.

## Ground rules

- Be civil. Our [Code of Conduct](./CODE_OF_CONDUCT.md) applies everywhere in the org.
- Found a security issue? Do not open a public issue. Follow [SECURITY.md](./SECURITY.md).
- By contributing, you agree your work is licensed under the same license as the repository you contribute to.

Not sure where to start? Open an issue and ask. We are happy to point you at something.
