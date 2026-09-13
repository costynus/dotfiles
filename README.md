# dotfiles

Personal configuration files, managed as Git submodules.

## Included

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

## Update a submodule

```bash
cd kitty-config
git pull origin trunk

cd ..
git add kitty-config
git commit -m "Update kitty-config submodule"
git push
```

Use the same process for `nvim`.
