# kitty

Terminal Emulator

## documentation
- [kitty.conf documentation](https://sw.kovidgoyal.net/kitty/conf/)
- [kitten hints](https://www.mankier.com/1/kitten-hints)
- [config example](https://gist.github.com/fwfurtado/e7e40cf8b07cff18c6d7bd1649676abf)

## keys
- `ctrl a`          launch menu
- `[km] ⮠`      switch to tab
- `ctrl shift`      [km] | leader
- `[km] r`          reload config
- `[km] ⮠`          new window
- `[km] w`          close window
- `[km] f5`         load_config_file
- `ctrl l`          clear screen

### hints / progs
- `[km] f`          hints ...
- `f`               copy
- `l`               copy line
- `w`               w3m
- `e`               vim [via openvim]
- `q`               qutebrowser
- `d`               axel
- `y`               dlyt
- `a`               dlyt
- `m`               mpv
- `b`               mpvb
- `[km] e`          vim [inline]

### copy
- `[km] y>v`        edit hint new vim instance
- `[km] y>e`        edit hint in main vim
- `[km] y>y`        yank hint
- `[km] y>c`        yank line
- `[km] y>w`        yank word

### history
- `ctrl ⎵`          show_scrollback [vim]
- `[km] ⎵`          show_scrollback_pager
- `[km] s`          open last cmd output in vim 

### windows
- `[km] alt n`      new_window
- `[km] j`          next_window
- `[km] k`          previous_window
- `[km] z`          start_resizing_window

### tabs 
- `[km] n`          new_tab
- `[km] x`          close_tab
- `[km] ⇾`          next_tab
- `[km] ⇓`          move_tab_forward
- `ctrl ⭾`          next_tab
- `[km] end`        goto_tab 1
- `[km] 2`          goto_tab 2
- `[km] d`          detach_window
- `[km] o`          close_other_tabs_in_os_window¶ 

### appearance
- `ctrl minus`      change_font_size all -1.0
- `ctrl plus`       change_font_size all  1.0
- `[km] 0`          set_background_opacity  0.1
- `[km] 9`          set_background_opacity -0.1

## themes
```
choose via "kitten themes" or alias "kitty-themes"
user themes are stored in $CONFIG_DIR/kitty/themes
```
- `inferno`         dark, matching red
- `xaos`            dark, based on Mona Lisa

## keybinding example
```
map `[km] o` pass_selection_to_program firefox     ... pass screen selection to prog
kitty @ focus-tab -m index:1    ... focus first tab from cmd line
kitty @ detach-tab -m index:1   ... break tab out to another window   
```
