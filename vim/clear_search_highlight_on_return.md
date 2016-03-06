# Undo Search Highlighting

I like having search highlight on in vim, but after I've found what I
want, it's distracting so I put this in my .vimrc

```
" Clears search highlighting by just hitting a return. The <BS> clears the
" command line. From Zdenek Sekera [zdenek.sekera@cern.ch] on the vim list.
nnoremap <CR> :noh<CR>/<BS>
```
