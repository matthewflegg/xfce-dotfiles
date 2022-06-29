# XFCE Dotfiles

## Theme
This is what my configuration looks like.

![image](https://user-images.githubusercontent.com/88111643/176428968-c412fdc6-e07f-4a4d-a8d8-468d5a7793e2.png)

This is meant for personal use but you can install it if you want. Instructions are below.

## Installation
Install the required packages from the AUR.
```bash
yay -S ulauncher
       xfce4-docklike-plugin
       xfce4-panel-profiles
       picom-ibhagwan-git
```

Copy this repository's configuration files, themes, and shared assets & settings to their respective local directories on your machine.
```bash
cd xfce-dotfiles
cp -r .config/* ~/.config/
cp -r .themes/* ~/.themes/
cp -r .local/share/* ~/.local/share/
```

You can now do the following:

- Disable compositing
- Set the window manager and application themes to `Qogir-Dark`
- Set the panel layout in `xfce4-panel-profiles`
- Set the default font to Cantarell 10
- Set the icon theme to Tela Circle Dark
- Set the wallpaper

## Recommendations
Delete all entries in `~/.themes/Qogir-Dark/xfwm4` that start with `top`, `bottom`, `left`, and `right` to disable borders.
Run:
```bash
cd `~/.themes/Qogir-Dark/xfwm4`
rm top-* bottom-* left-* right-*
```

Install `lightdm-gtk-greeter-settings` to set a theme for the display manager
  - You will need to copy your theme to `/usr/share/themes/`
  - You will need to copy your wallpaper(s) and user image(s) to `/usr/share/images/
  - You can also change the icons and top bar if you wish
