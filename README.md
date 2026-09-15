# dotfiles

Personal configuration files, managed as Git submodules.

## Included

- [`ghostty`](./ghostty) — Ghostty configuration.
- [`kitty-config`](./kitty-config) — Kitty configuration.
- [`nvim`](./nvim) — Neovim configuration.

Each configuration remains an independent repository with its own history and remote.

## Clone

```bash
git clone --recurse-submodules git@github.com:costynus/dotfiles.git
```

For an existing clone:

```bash
git submodule update --init --recursive
```

To update submodules later:

```bash
git submodule update --remote --recursive
```

Submodules in this repository are configured to track upstream branches (for example, `trunk`), but that setting does not automatically change the parent repository's recorded submodule commit. After updating a submodule, review the change and commit the updated submodule gitlink in this repository.
