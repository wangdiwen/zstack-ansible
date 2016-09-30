# 使用说明

- 你的操作系统需要是Linux/Unix
- zstack-ansible通过命令行执行，所以需要你的操作系统已经安装了ansible工具
> ansible install
> sudo pip install ansible

- 设置你的服务器地址
> 修改ansible.cfg

- 执行剧本
在playbooks下面有2个剧本

zk_config_sshd.yml：配置安装服务器的sshd端口，允许root访问，设置自定义root密码可以修改ssh_root_pwd变量，根据剧本注释进行操作. 如果你的安装服务器之前没有开启root密码和远程登陆，可以执行该剧本!

zk_deploy_single.yml: 自动部署zstack到安装服务器，可以自定义剧本中的vars下面的各个变量，zstack_开头的变量请不要改动.


> $ ansible-playbook -vv playbooks/zk_config_sshd.yml -c paramiko --extra-vars 'host=zk-server ansible_port=<ssh-old-port>'

> $ ansible-playbook -vv playbooks/zk_deploy_single.yml -c paramiko  --extra-vars 'host=zk-server ansible_port=<ssh-port>'


# 部署信息
```
剧本执行过程中，会进行一次重启服务器，需要耐心等待.
部署结束后，安装服务器上的zstack信息如下：
zstack UI面板：http://xxx:5000
image的文件列表：http://xxx/image

如果采用默认zstack_开头的变量配置，
http路径为：/var/www/html/http_root
nfs路径为： /var/www/html/nfs_root
backup存储路径为：/backup_root
```
