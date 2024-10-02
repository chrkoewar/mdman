# glow

markdown pager and browser

## documentation
- [github](https://github.com/charmbracelet/glamour)
- [themes](https://github.com/charmbracelet/glamour/blob/master/styles/gallery/README.md)

## keys
- `e`       edit .md file
- `enter`   view rendered .md file

## arguments
- `-w 60`               wrap at 60 chars
- `-s dark|light`       style theme
- `-s mystyle.json`     custom style

## cmd
- `Read from file`      glow README.md
- `Read from stdin`     echo "[Glow](https://github.com/charmbracelet/glow)" | glow -
- `README from GitHub`  glow github.com/charmbracelet/glow
- `Fetch from HTTP`     glow https://host.tld/file.md
