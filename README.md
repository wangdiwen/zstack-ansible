# zstack-ansible
```
zstack-ansible is a ZStack automation deployment project based on Ansible.
zstack-ansible provides a alternative solution except ZStack All-in-one bash script.
```

# OS Support

|OS|type|
| --- |---|
| Debian 8.x | support |
| Ubuntu     | not yet |
| CentOS     | not yet |
| Fedora     | not yet |

> zstack-ansible just support Debian 8.x at present.

# Zstack version
#### zstack-ansible based on zstack 1.6.2 version.

# Usage
参考项目文件 usage.md

# Welcome contribution
> 由于ZStack官方的安装部署脚本已经完美支持Centos 7.2+，而对于其他常用的开源系统，比如Debian，并没有太多支持，zstack-ansible项目将会先从我本人所用的Debian系统进行ZStack的整合和移植工作. 其他操作系统诸如 Centos/Fedora/Ubuntu 将会陆续进行开放出来.

> 如果你对zstack-ansible感兴趣，欢迎提交PR，也可以与我联系，共同成长！

# Why zstack-ansible

1. ZStack官方仅提供All-in-one脚本部署，没有采用其他运维自动化工具的支持，诸如：ansible/Puppet etc.
2. ZStack打包好的一键部署方案，固然很好，但是其包装的过于厉害，导致很多有兴趣了解其软件架构的同学，无法知道ZStack到底用到了哪些开源软件，然后如何通过ZStack核心代码进行整合关联. 而zstack-ansible将会把ZStack用到的开源软件一一展示出来，让研究学习的同学能够清楚知道，哪些是开源组件，哪些是Zstack官方开发的代码和模块.


# What is ZStack
> ZStack is open source IaaS(infrastructure as a service) software aiming to automate datacenters, managing resources of compute, storage, and networking all by APIs. Users can setup ZStack environments in a download-and-run manner, spending 5 minutes building a POC environment all on a single Linux machine, or 30 minutes building a multi-node production environment that can scale to hundreds of thousands of physical servers.

# Help links
- ZStack english site: http://zstack.org/
- ZStack chinese site: http://zstack.org.cn/
- Zstack github  site: https://github.com/zstackorg/zstack
- ZStack issues  site: https://github.com/zstackorg/zstack/issues


# Contact me
```
小鱼人
QQ: 785644342
Wechat: steven_diwen
Email: wangdiwen1@corp.netease.com
```
