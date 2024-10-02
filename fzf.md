# fzf

## documentation
[examples](https://thevaluable.dev/practical-guide-fzf-example/)

## arguments
- `--no-multi`
- `--exact`
- `--wrap`
- `--wrap-sign=>`
- `--ansi`
- `--layout=reverse-list`
- `--margin=0%,0%,0%,0%`
- `--height=50%`
- `--info=hidden`
- `--prompt=`
- `--pointer=▶`
- `--border=double` 
- `--header-lines=1`
- `--preview`
- `--color=dark,fg:blue`

## color items
- `fg:blue`             foreground
- `fg+:cyan`            foreground alt
- `preview-fg:white`    preview foregroudn
- `bg+:black`           background
- `query:blue`          user query string
- `hl:blue`             highlight
- `hl+:red`             highlight alt
- `border:red`          border

## match patterns
- `btrkt`	fuzzy-match	Items that match sbtrkt
- `'wild`	exact-match (quoted)	Items that include wild
- `^music`	prefix-exact-match	Items that start with music
- `.mp3$`	suffix-exact-match	Items that end with .mp3
- `!fire`	inverse-exact-match	Items that do not include fire
- `!^music`	inverse-prefix-exact-match	Items that do not start with music
- `!.mp3$`	inverse-suffix-exact-match	Items that do not end with .mp3

