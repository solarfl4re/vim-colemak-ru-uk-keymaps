# Russian and Ukrainian VIM keymaps for Colemak users

Switching languages on the iPad itself doesn't work well when I SSH into my servers (Using Blink.sh) and am in VIM; the moment I leave insert mode I have to switch languages, which is tedious.
Vim's `keymap` seemed to be the solution, but the keymaps presume a QWERTY layout, which makes them unusable with Colemak. 

**Solution**: make my own keymaps for Russian and Ukrainian input while using Colemak. With `:set keymap=ukrainian-colemak` and `:set keymap=russian-colemak`, everything works great.
