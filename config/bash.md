Add to **/etc/profile** for all user, or **~/.bashrc** for current user:
```bash
# alias
alias l='ls -l'
alias la='ls -la'
alias lrt='ls -lrt'
alias vi='vim'
# for mac os
alias l='ls -lG'
alias la='ls -laG'
alias lrt='ls -lrtG'
alias vi='vim'

# PS1
function git-branch {
  local branch=`git symbolic-ref HEAD 2>/dev/null | cut -d"/" -f 3`
  if [ $branch ]; then printf "[%s]" $branch; fi
}
export PS1="\[\e[32m\]\u\[\e[m\]@\[\e[32m\]\h\[\e[m\]:\[\e[31m\]\w\[\e[m\]\[\e[32m\]\$(git-branch)\[\e[m\]$ "
# for machine without git
export PS1="\[\e[32m\]\u\[\e[m\]@\[\e[32m\]\h\[\e[m\]:\[\e[31m\]\w\[\e[m\]$ "

# go
alias gr='go run cmd/main.go'
```
