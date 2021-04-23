Add to **/etc/profile** for all user, or **~/.bashrc** for current user:
```bash
alias l='ls -l'
#alias l='ls -lG' # for mac os
alias la='ls -la'
#alias la='ls -laG' # for mac os
alias vi='vim'

function git-branch {
  local branch=`git symbolic-ref HEAD 2>/dev/null | cut -d"/" -f 3`
  if [ $branch ]; then printf "[%s]" $branch; fi
}
export PS1="\[\e[32m\]\u\[\e[m\]@\[\e[32m\]\h\[\e[m\]:\[\e[31m\]\w\[\e[m\]\[\e[32m\]\$(git-branch)\[\e[m\]$ "
```
