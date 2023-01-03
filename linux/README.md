# Custom xkb symbols

- Copy the file `xkb/symbols/mysymbols` to `/usr/share/X11/xkb/symbols`
- Apply the file `xkb.patch` to `/usr/share/X11/xkb/` like this:

```
cd /usr/share/X11/xkb/
patch -p2 < PATH-TO/xkb.patch
```

- To activate in Gnome, perform the following command:

```
gsettings set org.gnome.desktop.input-sources xkb-options "['mysymbols:ctrl_alt_win_menu']"
```
