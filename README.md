|                                                     𝐆𝐫𝐮𝐯𝐛𝐨𝐱                                                     |                                                 𝐆𝐫𝐮𝐯𝐛𝐨𝐱 𝐌𝐚𝐭𝐞𝐫𝐢𝐚𝐥                                                  |
| :-------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------: |
| ![origin](https://user-images.githubusercontent.com/37491630/61659102-426d5e80-acb6-11e9-8e61-057d2c5668ff.png) | ![material](https://user-images.githubusercontent.com/37491630/61659107-44cfb880-acb6-11e9-8875-89799072a4a2.png) |

Gruvbox Material is based on Gruvbox, but with a very different color palette, almost all foreground colors are adjusted.

Although the palette is different, I will try to keep the extended highlight groups consistent with [gruvbox-community/gruvbox](https://github.com/gruvbox-community/gruvbox).

# Installation

## Via Plugin Manager

Take [vim-plug](https://github.com/junegunn/vim-plug) for example:

```vim
Plug 'sainnhe/gruvbox-material'
```

For better syntax highlighting support, please install [sheerun/vim-polyglot](https://github.com/sheerun/vim-polyglot).

## Manually

1. Clone this repository.
2. Copy `/path/to/gruvbox-material/colors/*` to `~/.vim/colors/`
3. To install [airline](https://github.com/vim-airline/vim-airline) theme, copy `/path/to/gruvbox-material/autoload/airline/themes/gruvbox_material.vim` to `~/.vim/autoload/airline/themes/gruvbox_material.vim`
4. To install [lightline](https://github.com/itchyny/lightline.vim) theme, copy `/path/to/gruvbox-material/autoload/lightline/colorscheme/gruvbox_material.vim` to `~/.vim/autoload/lightline/colorscheme/gruvbox_material.vim`

## AUR

There is a package available for Arch Linux users in AUR: [gruvbox-material-git](https://aur.archlinux.org/packages/gruvbox-material-git/)

# Usage

## Vim

Put this in your vimrc:

```vim
colorscheme gruvbox-material

" for soft background
colorscheme gruvbox-material-soft

" for hard background
colorscheme gruvbox-material-hard
```

If you want to apply this color scheme temporarily, run this command in vim(**this may cause color broken**):

```vim
:colorscheme gruvbox-material
```

## Airline

To enable [airline](https://github.com/vim-airline/vim-airline) color scheme, put this in your vimrc:

```vim
let g:airline_theme = 'gruvbox_material'
```

To apply it without reloading:

```vim
:AirlineTheme gruvbox_material
```

## Lightline

To enable [lightline](https://github.com/itchyny/lightline.vim) color scheme, put this in your vimrc:

```vim
let g:lightline = {}
let g:lightline.colorscheme = 'gruvbox_material'

" or this line
let g:lightline = {'colorscheme' : 'gruvbox_material'}
```

To apply it without reloading:

```vim
:let g:lightline.colorscheme = 'gruvbox_material'
:call lightline#init()
:call lightline#colorscheme()
```

# Customization

- By default, italic is enabled. To disable italic, add `let g:gruvbox_material_kill_italic=1` to your vimrc.
- By default, bold is partly enabled. To completely enable bold, add `let g:gruvbox_material_enable_bold=1` to your vimrc.

# Contribution

This color scheme is generated by [lifepillar/vim-colortemplate](https://github.com/lifepillar/vim-colortemplate). To hack it, install this plugin and edit `templates/*.colortemplate`, then rebuild the color schemes and execute `templates/util.sh`.

As mentioned above, I will try to keep the extended highlight groups consistent with [gruvbox-community/gruvbox](https://github.com/gruvbox-community/gruvbox). However, I may not be able to update in time. If so, you can open an issue to remind me or open a PR.

# Related Projects

- [Alacritty](https://gist.github.com/kamek-pf/2eae4f570061a97788a8a9ca4c893797)
- [Tilix](https://gist.github.com/sainnhe/5c44ffcd2465198ced6d80ac57b38b34)

# License

[MIT](./LICENSE) && [Anti-996](./Anti-996-LICENSE)
