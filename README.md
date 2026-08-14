# Surxe-dev

This is the sandboxed development account for [Surxe](https://github.com/Surxe).

It exists for one reason: to keep AI-assisted tooling behind a hard privilege
boundary. On my Debian workstation, Claude Code runs as a separate, unprivileged
PC user with its own GitHub identity (this one), so automation never has access
to my primary account's credentials or my home directory.

## How the boundary works

- **Separate PC user:** the automation user is its own Linux account with no sudo and no write access into my primary user's files.
- **Separate GitHub account:** commits made by tooling are authored here, as Surxe-dev, and stay clearly distinct from my own work on [Surxe](https://github.com/Surxe).
- **Copy, never symlink:** the `install.sh` in [my-system](https://github.com/Surxe/my-system) deploys shared config by *copying* it into each user's home. Nothing this account touches can write back across the boundary into my primary user's files.

## What runs here

Development work on the same projects Surxe maintains (datamined game databases,
wikis, and personal Linux tooling), just committed from the sandboxed side of the
line. If you're looking for the projects themselves, the person behind them, and
how to get in touch, start at [Surxe](https://github.com/Surxe).

## Reach me

- Discord: **@Surxe**

---

![Discord](https://img.shields.io/badge/Discord-%40Surxe-5865F2?style=flat&logo=discord&logoColor=white)
![Public repos](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/users/Surxe-dev&query=$.public_repos&label=public%20repos&style=flat&logo=github&logoColor=white&color=2ea043)
![PRs merged](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.github.com%2Fsearch%2Fissues%3Fq%3Dtype%3Apr%2Bauthor%3ASurxe-dev%2Bis%3Amerged&query=$.total_count&label=PRs%20merged&style=flat&logo=git&logoColor=white&color=f05032)
![PRs merged since 2026](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.github.com%2Fsearch%2Fissues%3Fq%3Dtype%3Apr%2Bauthor%3ASurxe-dev%2Bis%3Amerged%2Bmerged%3A%253E%253D2026-01-01&query=$.total_count&label=PRs%20merged%20since%202026&style=flat&logo=git&logoColor=white&color=8957e5)
