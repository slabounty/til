# Copy Filename to Clipboard

To copy the filename of the current window to the clipboard, use:

```
:let @" = expand("%")
```

It might be worth considering moving this to a mapping.

```
:nmap <Leader>cp :let @+ = expand("%")<cr>
```
