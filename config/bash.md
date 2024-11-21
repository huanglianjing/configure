应用到当前用户：添加配置到 ~/.bashrc

应用到所有用户：添加配置到 /etc/profile



常用命令别名

```bash
alias l='ls -l'
alias la='ls -la'
alias lrt='ls -lrt'

# mac os
alias l='ls -lG'
alias la='ls -laG'
alias lrt='ls -lrtG'
alias vi='vim'
```



命令提示符

```bash
export PS1="\[\e[32m\]\u\[\e[m\]@\[\e[32m\]\h\[\e[m\]:\[\e[31m\]\w\[\e[m\]$ "

# 如果安装了git可以显示分支名称
function git-branch {
  local branch=`git symbolic-ref HEAD 2>/dev/null | cut -d"/" -f 3`
  if [ $branch ]; then printf "[%s]" $branch; fi
}
export PS1="\[\e[32m\]\u\[\e[m\]@\[\e[32m\]\h\[\e[m\]:\[\e[31m\]\w\[\e[m\]\[\e[32m\]\$(git-branch)\[\e[m\]$ "
```



Go

```bash
alias gr='go run cmd/main.go'
```

