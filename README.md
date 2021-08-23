# vim-hybrid

Dark colorscheme for Vim.
This is a fork of [wong/vim-hybrid](https://github.com/w0ng/vim-hybrid).

## Differences

I have modified a few highlight groups to my taste. Mainly related to the tab
and status lines.

## Requirements

- gVim 7.3+ on Linux, Mac and Windows.
- Vim 7.3+ on Linux and Mac, using a terminal that supports 256 colors.

## Installation

1.  Copy `colors/hybrid.vim` to:

	```
	.vim/colors/hybrid.vim
	```

	or alternatively, use a plugin manger.

2.  Add to `.vimrc`:

	```vim
	syntax on
	set background=dark
	colorscheme hybrid
	```

## Define custom terminal colors (recommended)

Due to the limited 256 palette, colors in Vim and gVim will still be slightly
different.

In order to have Vim use the same colors as gVim (the way this color scheme is
intended) define the basic 16 colors in your terminal.

1.  Add the default palette to `.Xresources` or terminal emulator:

	```bash
	! Set terminal colors to use the palette from Hybrid theme.
	*background: #1D1F21
	*foreground: #C5C8C6
	! black
	*color0: #282A2E
	*color8: #373B41
	! red
	*color1: #A54242
	*color9: #CC6666
	! green
	*color2: #8C9440
	*color10: #B5BD68
	! yellow
	*color3: #DE935F
	*color11: #F0C674
	! blue
	*color4: #5F819D
	*color12: #81A2BE
	! magenta
	*color5: #85678F
	*color13: #B294BB
	! cyan
	*color6: #5E8D87
	*color14: #8ABEB7
	! white
	*color7: #707880
	*color15: #C5C8C6
	```

2.  Add to `.vimrc`:

	```vim
	let g:hybrid_custom_term_colors = 1
	colorscheme hybrid
	```
