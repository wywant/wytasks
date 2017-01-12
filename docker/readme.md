准备工作
1. Ubuntu默认情况下，没有安装SSH Server,运行 apt-get install openssh-server
2. 允许root 远程ssh,修改/etc/ssh/sshd_config，注意不是/etc/ssh/ssh_config
设置PermitRootLogin yes，注释掉其他PermitRootLogin xxxx
http://askubuntu.com/questions/469143/how-to-enable-ssh-root-access-on-ubuntu-14-04



安装文档
https://docs.docker.com/engine/installation/linux/ubuntulinux/
如果在局域网里面，需要参考后半部分DNS服务器的设置

Image不能pull问题
有些image可以用docker search命令查找到，但是不能用docker pull 命令pull。原因是它们不是真正的image,需要在后面加上tag,如docker pull ansible/ansible:ubuntu1604。具体的tag可以到网页版的搜索结果中查看。 
