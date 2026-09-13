# dotfiles

Мои персональные конфигурации, собранные в одном репозитории с помощью Git submodules.

## Состав

- [`kitty-config`](./kitty-config) — конфигурация терминала Kitty.
- [`nvim`](./nvim) — конфигурация Neovim.

Каждая конфигурация остаётся самостоятельным репозиторием со своей историей и удалённым репозиторием.

## Клонирование

Клонируйте репозиторий вместе со всеми submodules:

```bash
git clone --recurse-submodules git@github.com:costynus/dotfiles.git
```

Если репозиторий уже был клонирован без submodules, инициализируйте их так:

```bash
git submodule update --init --recursive
```

## Обновление конфигураций

Сначала обновите нужный submodule, затем зафиксируйте новую ссылку в `dotfiles`:

```bash
cd kitty-config
git pull origin trunk

cd ..
git add kitty-config
git commit -m "Update kitty-config submodule"
git push
```

Для `nvim` принцип такой же.
