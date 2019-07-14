# asyncomplete-tsuquyomi.vim

[Tsuquyomi](https://github.com/Quramy/tsuquyomi) completion source for [asyncomplete.vim](https://github.com/prabirshrestha/asyncomplete.vim)

## Install

```vim
Plug 'prabirshrestha/asyncomplete.vim'
Plug 'ishitaku5522/asyncomplete-tsuquyomi.vim'
```

## Register asyncomplete-tsuquyomi.vim

```vim
au User asyncomplete_setup call asyncomplete#register_source(asyncomplete#sources#tsuquyomi#get_source_options({
      \ 'name': 'tsuquyomi',
      \ 'whitelist': ['javascript','typescript'],
      \ 'completor': function('asyncomplete#sources#tsuquyomi#completor')
      \  }))
```
