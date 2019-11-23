# Russian and Ukrainian VIM keymaps for Colemak users

Switching languages on the iPad itself doesn't work well when I SSH into my servers (Using Blink.sh) and am in VIM; the moment I leave insert mode I have to switch languages, which is tedious.

Vim's [`keymap`](https://vimhelp.org/options.txt.html#%27keymap%27) seemed to be the solution, but the keymaps presume a QWERTY layout, which makes them unusable with Colemak. 

**Solution**: make my own keymaps for Russian and Ukrainian input while using Colemak. With `:set keymap=ukrainian-colemak` and `:set keymap=russian-colemak`, everything works great.

## Install
[`mbyte-keymap` help page:](https://vimhelp.org/mbyte.txt.html#mbyte-keymap)
>The value of the 'keymap' option specifies a keymap file to use.  The name of
>this file is one of these two:
>
>        keymap/{keymap}_{encoding}.vim
>        keymap/{keymap}.vim
> [...]
>
>'runtimepath' is used to find these files.  To see an overview of all
>available keymap files, use this: 
>        :echo globpath(&rtp, "keymap/*.vim")

I use neovim and put them in `~/.config/nvim/keymap/`.
