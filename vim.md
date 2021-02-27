Add to **/etc/vim/vimrc** and **/etc/vim/vimrc.tiny** and **~/.vimrc**:
```
syntax on
set number
set t_Co=256
set tabstop=4
set softtabstop=4
set shiftwidth=4
set hlsearch
set incsearch
set nowrapscan
set ignorecase smartcase
set shortmess=atI
set autoindent
set cindent
set list
set listchars=tab:>-,trail:-
set cursorline
set nocompatible
set backspace=indent,eol,start
```



For root user, the configuration may not work. It's because it only apply to vim but not vi.
Need to add this to **~/.bashrc** and reopen terminal:
```
alias vi='vim'
```
