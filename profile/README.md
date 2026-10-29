# Colors

Coding agents made Terraform and Ansible obsolete. Colors keeps the
conventions that worked — desired state in `colors.yml`, toolchain in `.envrc`,
secrets in `.envrc.private`, distribution through Agent Skills — and builds
packages as direct programs that drive the cloud providers' own CLIs.

**Website:** [www.getcolors.ai](https://www.getcolors.ai) ·
**Announcement:** [Rebooting getcolors.ai](https://www.getcolors.ai/blog/getcolors-reboot) ·
**Discord:** [join](https://discord.gg/3aQzzrrdFj)

## The foundation: three colours

| SDK | Language | |
|---|---|---|
| [green](https://github.com/getcolors/green) | Clojure / Babashka | canonical |
| [red](https://github.com/getcolors/red) | TypeScript / Bun | |
| [blue](https://github.com/getcolors/blue) | Python / uv | |

Each implements the same workflow model: a graph of steps that take and return
one map of options, wired statically and routed dynamically. Anyone can build a
package on a colour.

## Packages

[PocketDeploy](https://github.com/pocketcontext/pocketdeploy) is a starter
package built on Blue to run [PocketContext](https://www.pocketcontext.com/):
compute on OCI, DigitalOcean, Google Cloud and Hetzner, a SQLite ledger of
resources and operations, and encrypted recovery through VaultContext.
Packages can build on it in turn:

- [rybbit](https://github.com/getcolors/rybbit) — single-node Rybbit analytics on Hetzner
- [walter](https://github.com/getcolors/walter) — Google Cloud or OCI development machines
- [alice](https://github.com/getcolors/alice) — ephemeral Transmission server on DigitalOcean
- [dotfiles](https://github.com/getcolors/dotfiles) — Ubuntu or macOS home configuration (on Green)

## Skills

- [skills](https://github.com/getcolors/skills) — Agent Skills, including `create-context-skill`

Earlier OpenTofu/Ansible packages and deployments are archived and read-only.
