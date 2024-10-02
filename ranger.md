## ranger

### documentation
- [wiki](https://github.com/ranger/ranger/wiki)
- [mapping keys](https://github.com/ranger/ranger/wiki/Keybindings)
- [linemodes](https://github.com/ranger/ranger/wiki/Custom-linemodes)
- [keybindigs](https://gist.github.com/heroheman/aba73e47443340c35526755ef79647eb)

### references
- `%D` other pane current directory
- `%S` other pane selected file
- `%f` the highlighted file
- `%d` the path of the current directory
- `%s` the selected files in the current directory
- `%t` all tagged files in the current directory
- `%c` the full paths of the currently copied/cut files
- `%p` the full paths of selected files

### keys
- `m`       mark > letter
- `'`       goto marker
- `t`       tag
- `"?`      tag with letter
- `cw`      <bulk>rename
- `C-p`     repeat command
- `f`       filter as you type	> execute
- `Mf`      filename
- `Mi`      fileinfo
- `Mm`     mtime
- `Mp`      permissions
- `Ms`      sizemtime
- `Mt`      metatitle
- `uma`     delete marker a
- `@`       shell %s
- `zh`      toggle hidden files
- `~`       viewmode >> next tab
- `cn`      tab new
- `cw`      tab open
- `=`       chmod
- `a`       rename_append
- `yy`      copy
- `gh`      home
- `gn`      tab new
- `gc`      tab close
- `space`   mark
- `f5`      copy
- `f6`      cut 
- `/`       search
- `dd`      cut
- `yy`      copy
- `pp`      paste
- `!`       shell command
- `:`       ranger command
- `S`       terminal in curr dir
- `f`       scout  .... datei filter
- `pl`      creating softlinks
- `phl`         create hardlinks
- `o`       sort
- `v`       select all
- `!`       shell
- `:`       command
- `@`       command with arg
- `S`       shell in dir
- `.`       filter  f/d/m c ... clear
- `alt+1/2` new tab
- `~`       dual pane view
- `yd`      copy directory name only
- `yn`      copy file name only
- `yp`      copy full path

### commands
-`:bulkrename`
- `:flat 1/2/3`     list subdirs and files in current list
- `:compress`	    compress selection to archive
- `bulkrename` 
- `delete` 
- `chmod` 
- `edit` 
- `filter` 
- `find` 
- `search` 
- `grep` 
- `mark` 
- `mark_tag` 
- `mkdir` 
- `rename` 
- `touch` 
- `unmark` 
- `unmark_tag` 


### config
```
rifle.conf	mime types especially for ranger
hide specific files in plugins/plugin_file_filter.py
```

### cmd
ranger --list-tagged-files='*'		consolen ausgabe alle getaggten dateien


