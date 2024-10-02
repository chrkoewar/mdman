# neomutt

E-Mail Client

## documentation
- [mutt manual](http://mutt.org/doc/manual/)
- [cheat sheet](https://github.com/JoshuaEstes/CheatSheets/blob/master/mutt.md)

## keys
- `o`           fetch mail
- `e`           edit email attachment
- `Q`           query abook
- `a`           add sender to abook
- `i1`          goto mailboxe 1
- `D`           delete-message
- `U`           undelete-message
- `$/S`         sync-mailbox
- `space`       markieren
- `%`           toggle sichern
- `.`           mailbox-list   mailboen mit neuen nachrichten
- `@`           display-address
- `B`           sidebar-toggle-visible
- `Mt`          trash  move to trash
- `Mi`          inbox
- `Ma`          archive
- `R`           group-reply
- `T`           tag-pattern
- `W`           clear-flag
- `Y`           edit-label
- `b`           bouce-message
- `f`           forward-message
- `c`           andere mailbox
- `gi/j/t/s`    goto inbox etc
- `m`           mail
- `r`           reply
- `x`           menu verlassen
- `|`           pipe-entry
- `^L`          refresh
- `!`           shell-escape
- `N`           mark unread :: toggle-new
- `O`           mark read :: mark-as-old
- `Ctrl-Shift-O"(` <sidebar-open>)
- `[shift][t]` tag-pattern
- `[t]`     tag-message
- `Q	query` abook
- `&` link to thread
- `\#` split thread
- `@` view full adress
- `a` create alias
- `b` bounce
- `f` forward
- `r` reply
- `m` compose mail
- `g` reply to all
- `c` open folder
- `D` delete
- `U` undelete
- `F` important
- `N` toggle read/unread
- `t` tag
- `shift` t tag pattern
- `esc` t tag thread
- `w` set status
- `W` clear status

## commands
```
:enter-command
compose-to-sender
delete-pattern
fetch-mail
imap-fetch-all
- `read-thred` faden als gelesen
sort-mailbox
sort-reverse
toggle-read
```

## command line
```
... send mail from cli
mutt -a file -s "Subject of Mail" -a file -- test@example.com < bodyTextFile
mw -Y           sync all accoutns
mw -cron        check regularily
```


