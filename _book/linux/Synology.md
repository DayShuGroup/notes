### 群晖Synology 开启ssh 登录

1. 在控制面板中开启 ssh 登录
2. 通过有管理员权限的用户登录
3. 通过输入 sudo -i , 然后输入当前用户密码, 进入 root
4. 输入如下命令可以修改root 用户的密码 synouser --setpw root 123456 (123456为密码)
5. 如果通过ssh登录不进去, 需要去开启
6. 进入文件 vi /etc/ssh/sshd_config 搜索文件 “PermitRootLogin” 更改为 yes, 或者 打开注释(如果是注释掉的话)
7. 重启 ssh 服务, 在此群晖中没有找到合适的命令, 可以通过网页中的控制面板禁用,启用服务生效.

