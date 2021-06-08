# Installation

## Linux

### X11

Copy `share/xkb/symbols/mle` into `/usr/share/X11/xkb/symbols` and restart X.
To select the layout, use `setxkbmap -layout mle -variant layman` (or `-variant
dvorak` if you prefer).

If you use `ibus` to manage input methods, additionally copy
`share/ibus/component/simple.mle.xml` into `/usr/share/ibus` and restart
`ibus`.

### Virtual console

Copy the desired keymap from `share/kbd/keymaps` into
`/usr/local/share/kbd/keymaps` and run `sudo loadkeys
/usr/local/share/kbd/keymaps/layman-mle.map` (replacing `layman-mle.map` with
`dvorak-mle.map` if you prefer).

To make this change persistent, add the following line to `/etc/vconsole.conf`:

```
KEYMAP=/usr/local/share/kbd/keymaps/layman-mle.map
```

## macOS

Copy `Library/Keyboard Layouts/mle_Layman.keylayout` into `/Library/Keyboard
Layouts` (for global installation) or `~/Library/Keyboard Layouts` (to install
just for the current user)
