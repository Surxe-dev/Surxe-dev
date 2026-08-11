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

![Surxe-dev's GitHub stats](https://github-readme-stats.vercel.app/api?username=Surxe-dev&show_icons=true&hide_border=true)
