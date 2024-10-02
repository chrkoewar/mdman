# stow

manage dotfiles as a linkfarm

## documentation
[offical documentation](https://www.gnu.org/software/stow/manual/stow.html)

## parameters

- `--vn`            simulate / dry-run
- `--dir`           -d source / stow dir
- `--target`        -t link / target dir
- `--ignore`        -i ignore list
- `--delete`        -d delete symlinks

## config

~/.stowrc lists ignored files

## example
```
stow --dir ~/.dotfiles --target ~ public
```
