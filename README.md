# VPS-cesu
服务器测速脚本，自用，暂时没有一键


# AWS切换root登录教程

echo root:123456 |sudo chpasswd root

sudo sed -i 's/^#\?PermitRootLogin.*/PermitRootLogin yes/g' /etc/ssh/sshd_config

sudo sed -i 's/^#\?PasswordAuthentication.*/PasswordAuthentication yes/g' /etc/ssh/sshd_config

sudo reboot

其中在输入命令时echo root:123456的123456需要切换为自己的密码
在sudo reboot重启之后就可以使用root登录了
