# morvane-labwc-theme

The MorvaneOS look for labwc: the `MorvaneOS-Dark` window theme with rounded corners,
and the Twilight wallpaper. The active window has a Pastel Pink border as well as a
brighter title, so it isn't told apart by colour alone.

Installs `/etc/xdg/labwc/rc.xml` (choosing the theme) and `/etc/xdg/labwc/autostart`
(the wallpaper), which labwc reads when you don't have your own in
`~/.config/labwc`. labwc's built-in defaults, key bindings included, apply to
everything `rc.xml` doesn't set. If you make your own `~/.config/labwc/rc.xml`,
copy the `<theme>` part across to keep the look.

The window theme is the Openbox-format one in
[morvane-gtk-theme](https://github.com/MorvaneOS/morvane-gtk-theme)
(`/usr/share/themes/MorvaneOS-Dark/openbox-3/themerc`); terminal colours (alacritty)
come from [morvane-wm-theme](https://github.com/MorvaneOS/morvane-wm-theme). The
MorvaneOS installer installs this package with labwc.

## Changing it

Edit `tools/build.py`, then:

```
python tools/build.py
```

Needs only Python. Commit the output, bump `pkgver`, build and publish.

## License

LGPL-2.1-or-later.
