# ag

> The Silver Searcher. Like ack, but faster.

- Find files containing "foo", and print the line matches in context:

`ag {{foo}}`

- Find files containing "foo" in a specific directory:

`ag {{foo}} {{path/to/directory}}`

- Find files containing "foo", but only list the filenames:

`ag -l {{foo}}`

- Find files containing "FOO" case-insensitively, and print only the match, rather than the whole line:

`ag -i -o {{FOO}}`

- Find "foo" in files with a name matching "bar":

`ag {{foo}} -G {{bar}}`

- Find files whose contents match a regular expression:

`ag '{{^ba(r|z)$}}'`

- Find files with a name matching "foo":

`ag -g {{foo}}`

- Search for files with extensions matching ".js":

`ag {{foo}} -G '\.js'`

- Search up to NUM directories deep:

`ag {{foo}} --depth=1`

- Ignore directories whose names match this pattern:

`ag {{foo}} --ignore=node_modules`

- Ignore files whose extensions match this pattern:

`ag {{foo}} --ignore='*json'`