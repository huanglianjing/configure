Add to **/etc/vim/vimrc** for all user, or **~/.vimrc** for current user:

```
syntax on
set number
set nocompatible
set showcmd
set t_Co=256
set tabstop=4
set softtabstop=4
set shiftwidth=4
set cursorline
set showmatch
set hlsearch
set incsearch
set ignorecase
set nowrapscan
set noswapfile
set autochdir
set list
set listchars=tab:>-,trail:-
set shortmess=atI
set backspace=indent,eol,start
if &diff
    colors blue
endif
```



For root user, the configuration may not work. It's because it only apply to vim but not vi.
Need to add this to **~/.bashrc** and reopen terminal:

```bash
alias vi='vim'
```

