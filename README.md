# [suacantstop] / Nebula Pulse Dotfiles

Конфигурация NixOS + Home Manager, подготовленная как конкурсный райс-проект с единой авторской темой **Nebula Pulse**.

## Концепт

Nebula Pulse - это холодная космическая база с яркими акцентами:

- База: глубокий индиго и графитовые тона.
- Акценты: электрический синий, неон-циан, фиолет.
- Сигнальные цвета: персиковый (warning) и розовый (danger).

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


## Установка

- Абсолютно чистая Nix os
- Юзернейм: `nixos` **(рекомендованно)**
- Базовое понимание флейков Nix

```bash
# Install git
> sudo nano /etc/nixos/configuration.nix

# Add to systemPackages: git
> sudo nixos-rebuild switch

# Clone this repository
> mkdir Pictures
> git clone https://github.com/suacantstop/Nebula-Pulse-Dotfiles.git
> cd Nebula-Pulse-Dotfiles/nixos

# Copy configuration files
> sudo rm -rf /etc/nixos/configuration.nix
> sudo cp -a home/ img/ modules/ configuration.nix flake.lock flake.nix /etc/nixos

# Rebuild
> sudo nixos-rebuild switch --flake /etc/nixos#nixos

# Reboot your system
> reboot
```


