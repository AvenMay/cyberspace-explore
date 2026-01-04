# GUI

## Web Dashboard

- cockpit
- cPanel

## X11 

```X11-Client -> X11 Server -> WindowManager -> Compositor```

- **X11-Client**: xterm, firefox, gedit, vlc, GTK/Qt
- **X11-Server**: Xorg, Xvfb, XWayland
- **WindowsManager**: Metacity, Kwin, OpenBox, Fluxbox, i3, bspwm
- **Compositor**: Compton/Picom, KWin, Mutter, xcompmgr

## Wayland

```
Wayland-Client -> Wayland-Server[server/wm/compositor]
```

- **Wayland-Client**: GTK/Wayland, QtWayland, wlroots
- **Wayland-Server(WindowsManager+Compositor)**: Weston, Hyprland, Sway, Niri
- **Linux-Distribution**: Omarchy, BluefinLinux


## Desktop-Environment

- GNOME
- KDE
- Xfce

## GUI Development