Add to **/etc/profile** for all user, or **~/.bashrc** for current user:
```
alias l='ls -l'
#alias l='ls -lG' # for mac os
alias la='ls -la'
#alias la='ls -laG' # for mac os
alias vi='vim'
export PS1='\[\e[1;32m\]\u\[\e[m\]@\[\e[1;32m\]\H\[\e[m\]:\[\e[44m\]\w\[\e[m\]$ '
```
