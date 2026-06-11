# Security Policy

## Reporting a vulnerability

Please don't open a public issue for a security problem — that tells everyone how to exploit it
before it's fixed.

Instead, report it privately one of two ways:

- **GitHub** (preferred): on the affected repository, open **Security → Report a vulnerability**
  (private vulnerability reporting), or
- **Direct**: message [@191-iota](https://github.com/191-iota) on GitHub and ask for a private
  channel.

Tell us what you found, how to reproduce it, and what an attacker could do with it. We'll confirm
we received it, work on a fix, and credit you when it ships unless you'd rather stay anonymous.

## Scope

These are small, mostly local-first tools. Several (`overseer`, `saul-swissman`, `the-factory`,
`auspex-v1`) run on your own machine and send nothing off it; the most useful reports there are
about data leaving the machine when it shouldn't, or untrusted input reaching a model or a shell.
For the hosted apps (`algoleague_*`), auth, isolation of submitted code, and data exposure are the
areas we care most about.

## Supported versions

We patch the latest version on the default branch. There are no long-term support branches.
