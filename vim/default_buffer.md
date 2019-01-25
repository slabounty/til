# Default Buffer Name

The default buffer name is `"`, so given a file 

```
hello |world
this is a test
```
where the cursor is on the `|`, doing a 

```
ywjo # open a line below the last one
Ctrl-r"Esc
```

will add a new line with the word `world`.
