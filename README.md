# Molokai Color Scheme for Vim

This is a fork of [fatih/molokai](https://github.com/fatih/molokai) to better adjust the theme to fit
what is used by [bat](https://github.com/sharkdp/bat) tool.


## Installation

Use a plugin manager, i.e:

* [vim-plug](https://github.com/junegunn/vim-plug)
  * `Plug 'mbodock/molokai'`


or copy the file on your .vim/colors folder.

## Settings

If you prefer the scheme to match the original monokai background color, put this in your .vimrc file: 
```
let g:molokai_original = 1
```

There is also an alternative scheme under development for color terminals which
attempts to bring the 256 color version as close as possible to the the default
(dark) GUI version. To access, add this to your .vimrc:
```
let g:rehash256 = 1
```

## Vim-go

This theme was specifically adapted comparing the bat output for Go files.

To better fit this output you should also configure your vim-go to highlight
more items like functions, methods, operators, etc.

The best settings so far for this is:

```vim
let g:go_highlight_build_constraints = 1
let g:go_highlight_extra_types = 1
let g:go_highlight_fields = 1
let g:go_highlight_function_calls = 0
let g:go_highlight_function_parameters = 1
let g:go_highlight_functions = 1
let g:go_highlight_operators = 1
let g:go_highlight_types = 1
```

## Original Description

Molokai is a Vim port of the monokai theme for TextMate originally created by
Wimer Hazenberg. 

256-Color terminals are also supported, though there are some differences with
the Gui version. Only the dark gray background style is supported on terminal
vim at this time.
