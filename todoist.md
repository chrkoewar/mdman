# todoist

ToDo List Manager

## commands
```
Todoist add 'test' -N 'projectname' -p <1-4>
linkks: markdown syntax or https:// (link description)
https://github.com/sachaos/todoist

todoist q 'newtask #project'
todoist close <tab> <tab> <tab> #multiple
@label +coworker

 content 
todoist -c 'neuer content' 23452352
 priority
todoist -p 2 23452352
 project
todoist modify -P <Tab> <Tab>
 open in browser
todoist show -o

todoist modify --date 'every Monday,Wednesday,Friday 07:00' ${task_id}  
USAGE:
   todoist modify [command options] <Item ID>

OPTIONS:
   --content value, -c value       content
   --priority value, -p value      priority (1-4) (default: 4)
   --label-names value, -L value   label names (separated by ,)
   --project-id value, -P value    project id (default: 0)
   --project-name value, -N value  project name
   --date value, -d value          date string (today, 2020/04/02, 2020/03/21 18:00)

install todoist from github https://github.com/sachaos/todoist/blob/master/README.md

todoist q/a > inbox
todoist MODIFY
todoist show only main task

maybe:
https://blog.doist.com/todoist-filters/
https://www.leightonprice.com/todoist/filters.html

todoist referenz: https://github.com/sachaos/todoist

todoist list --filter '(overdue | today) & p1'
filtering (today | overdue) & #Work
reference: https://todoist.com/help/articles/introduction-to-filters
assigned to: 
subtask
p1 / p2 priority
Culture Academy/Einkäufe

todoist >> inbox / privat / ca .. diss

Auswahl mit zsh
peco und .zhrc file .... 
<C-x> t t: select task with peco
<C-x> t p: select project with peco
<C-x> t l: select labels with peco
<C-x> t c: select task and close with peco
<C-x> t d: select date
<C-x> t o: select task, and open it with browser when has url
```

## todoist web

- `?` Hilfe
- `E` Erledigen
- `STRG+E` Bearbeiten
- `C` Kommentieren
- `T` Datum
- `V` Projekt
- `Y` Priorität
- `+` Person
- `STRG+K` MEnu
- `/`   Suche
- `Q` hinzufügen
- `GI` Inbox
- `GT` heute
- `GP` Projekt
- `GU` demnächst
- `GA` Aktivität
- `P1` Priorität

