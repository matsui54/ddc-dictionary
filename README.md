# ddc-dictionary
ddc source for dictionary

## Required

### denops.vim
https://github.com/vim-denops/denops.vim

### ddc.vim
https://github.com/Shougo/ddc.vim

## Configuration examples

```vim
" you neeed to set 'dictionary' option
setlocal dictionary+=/usr/share/dict/words

call ddc#custom#patch_global('sources', ['dictionary'])
call ddc#custom#patch_global('sourceOptions', {
      \ '_': {'matchers': ['matcher_head']},
      \ 'dictionary': {'mark': 'D'},
      \ })
```

## Original version
https://github.com/deoplete-plugins/deoplete-dictionary
