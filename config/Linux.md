设置某用户免密码使用 sudo 命令

```bash
chmod +w /etc/sudoers

# 在 /etc/sudoers 中添加以下行：
# <user> ALL=(ALL) NOPASSWD:ALL

chmod -w /etc/sudoers
```

