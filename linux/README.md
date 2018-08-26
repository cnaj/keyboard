# Custom xkb symbols

- Copy the file `xkb/symbols/mysymbols` to `/usr/share/X11/xkb/symbols`
- Add the following line to `/usr/share/X11/xkb/rules/evdev` under the `! option = symbols` section:

```
mysymbols:ctrl_alt_win_menu  =  +mysymbols(ctrl_alt_win_menu)
```
