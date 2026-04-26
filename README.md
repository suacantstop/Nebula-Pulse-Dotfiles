# Nebula Pulse Dotfiles

Конфигурация NixOS + Home Manager, подготовленная как конкурсный рэйсинг-проект с единой авторской темой **Nebula Pulse**.

## Концепт

Nebula Pulse - это холодная космическая база с яркими акцентами:

- База: глубокий индиго и графитовые тона.
- Акценты: электрический синий, неон-циан, фиолет.
- Сигнальные цвета: персиковый (warning) и розовый (danger).

Готовые схемы типа Nord/Everforest не использованы как основа палитры.

## Палитра

Основные цвета заданы в [home/programs/palette.nix](/etc/nixos/home/programs/palette.nix):

- `#0f111a` - base background
- `#161925` - elevated background
- `#20263a` - selection background
- `#2a3352` - border / hover background
- `#d9e0ff` - primary foreground
- `#a9b4d0` - secondary foreground
- `#78a6ff` - primary accent
- `#57d6ff` - secondary accent
- `#c792ff` - tertiary accent
- `#ffb86c` - warning
- `#7be0a3` - success
- `#ff6d96` - danger

## Что настроено

Полностью переработаны все модули в `home/programs`:

- Hyprland, Waybar, Foot, Fuzzel, Kitty, Alacritty
- Fish, Fastfetch
- GTK/Qt theme layer
- NVF (Neovim), Firefox, Git, Rofi

Тема сквозная: шрифты, цвета, иконки, терминалы, панель, лаунчер, WM и редактор.

## Скриншоты

Папка со скриншотами: [home/contest/screenshots](/etc/nixos/home/contest/screenshots)

![Wallpaper base](contest/screenshots/01-wallpaper-base.jpg)
![Workspace preview](contest/screenshots/02-workspace-preview.jpg)
![Terminal preview](contest/screenshots/03-terminal-preview.png)

## Приложенные файлы

- [palette.json](contest/attachments/palette.json)
- [contest-checklist.md](contest/attachments/contest-checklist.md)
- [capture-showcase.sh](contest/scripts/capture-showcase.sh)

## Применение

```bash
sudo nixos-rebuild switch --flake /etc/nixos#nixos
```

## Нюанс по скриншотам

В репозиторий добавлены превью-изображения для структуры submission.
Актуальные скриншоты рабочего стола можно снять скриптом:

```bash
bash /etc/nixos/home/contest/scripts/capture-showcase.sh
```
