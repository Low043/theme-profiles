## Tools
- [waybar](https://github.com/Alexays/Waybar)
- [rofi](https://github.com/davatorium/rofi)
- [rofi-themes](https://github.com/adi1090x/rofi/tree/master): Type-1 Style-5
- [nwg-look](https://github.com/nwg-piotr/nwg-look)
- [nemo](https://github.com/linuxmint/nemo)
- [mpvpaper](https://github.com/GhostNaN/mpvpaper)
- [ssdm-themes](https://github.com/Keyitdev/sddm-astronaut-theme): custom based on sakura
- [oh my zsh](https://github.com/ohmyzsh/ohmyzsh?tab=readme-ov-file)

## Download Links
- [Download Themes](https://github.com/daniruiz/flat-remix-gtk)
- [Download Icons](https://github.com/daniruiz/flat-remix)

## Setup Commands
- enable home crossing: `chmod o+x ~`
- enable profile read: `chmod -R 755 ~/theme-profiles`
- link waybar: `ln -s ~/theme-profiles/waybar ~/.config/waybar`
- set rofi theme on hyprland.conf: `$menu = ~/.config/rofi/launchers/type-1/launcher.sh`
- link nwg themes: `ln -s ~/theme-profiles/themes ~/.themes`
- link nwg icons: `ln -s ~/theme-profiles/icons ~/.icons`
- set nemo as default on hyprland.conf: `$fileManager = nemo`
- link mpvpaper: `ln -s ~/theme-profiles/wallpapers/<WALLPAPER> ~/theme-profiles/wallpapers/default`
- link sddm config: `sudo ln -s ~/theme-profiles/sddm/default /usr/share/sddm/themes/sddm-astronaut-theme/Themes/custom`
- link sddm backgrounds: `sudo ln -s ~/theme-profiles/wallpapers /usr/share/sddm/themes/sddm-astronaut-theme/Backgrounds`
- set sddm metadata.desktop ConfigFile: `Themes/custom`
- link kitty configs: `ln -s ~/theme-profiles/kitty.conf ~/.config/kitty/kitty.conf`
- link zsh configs: `ln -s ~/theme-profiles/zsh ~/.zshrc`

## Hyprland Binds
```bash
bind = $mainMod, T, exec, $terminal
bind = $mainMod, C, killactive
bind = $mainMod, M, exit,
bind = $mainMod, E, exec, $fileManager
bind = $mainMod, F, togglefloating,
bind = $mainMod, R, exec, $menu
bind = $mainMod, W, exec, killall waybar; waybar
bind = $mainMod, Q, exec, killall waybar
```

## Hyprland Exec-onces
Obs: HDMI-A-1 is my monitor type, check yours with `hyprctl monitors`
Obs2: wallpapers/default setted in mpvpaper link command
```bash
exec-once = mpvpaper -o "loop-file=inf no-audio hwdec=vaapi" HDMI-A-1 ~/theme-profiles/wallpapers/default
exec-once = waybar
```

### Green Cat
- Wallpaper: [Cat in the swamp](https://moewalls.com/animal/cat-in-the-swamp-live-wallpaper)
- Theme: Green Dark
- Icons: Green Dark

### Death & Life
- Wallpaper: [Death and life 2](https://moewalls.com/abstract/death-and-life-2-live-wallpaper)
- Theme: Grey Dark
- Icons: Grey Dark