# Contributing to Lambdaforge

This is the short, org-wide version that applies to every repository under
[`lambdaf-org`](https://github.com/lambdaf-org). For the full walkthrough — ways to help, the
per-stack toolchains, and how review works — see the
[contributing guide](https://github.com/lambdaf-org/contributing). The
[Code of Conduct](./CODE_OF_CONDUCT.md) applies everywhere in the org.

Lambdaforge builds small, sharp tools people actually need. We keep the bar high and the process light.

## The workflow

1. **Fork** the repo and clone your fork.
2. **Branch** off the default branch with a short, descriptive name (`fix/empty-input-panic`).
3. **Make one focused change.** Keep the diff about a single thing; no unrelated reformatting.
4. **Run the checks** for the stack before you push:
   - **Rust** (`auspex-v1`, `clock`, `transl_cli`, `neuro` backend): `cargo build`, `cargo test`, `cargo fmt --all`, `cargo clippy --all-targets --all-features -- -D warnings`.
   - **Python** (`synthesis`): create a venv, `pip install -r requirements.txt`, and run the repo's documented entry point.
   - **Web / TypeScript** (`MoneyForge`, `GradeForge`, `neuro` frontend): `npm install`, `npm run lint`, `npm run build`.
   - **Java / Spring + Angular** (`algoleague_backend`, `algoleague_frontend`): `./mvnw -DskipTests package` for the backend; `npm install && npm run build` for the frontend.
   - **Claude Code prompt repos** (`overseer`, `saul-swissman`, `the-factory`): no build step — read the `README` and `CLAUDE.md`, run the flow in Claude Code, and describe what you saw.
5. **Commit** with [Conventional Commits](https://www.conventionalcommits.org): `type: short imperative summary` (≤ ~70 chars). Types: `feat`, `fix`, `docs`, `refactor`, `test`, `chore`, `perf`.
6. **Open a pull request** against the default branch. Say what it does, link the issue it closes, and update the README if public behavior changed.

Most repos squash on merge, so your PR title becomes the commit — which is why the title follows
Conventional Commits.

## What review looks for

- It does one thing, and the title says what.
- It builds, and the existing checks pass.
- New behavior has a test where the stack supports it.
- Changed commands or public behavior are reflected in the README.

## Security

Don't report vulnerabilities in public issues. See [SECURITY.md](./SECURITY.md).
