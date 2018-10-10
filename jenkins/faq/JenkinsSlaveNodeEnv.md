# description
连接方式， SSH. 在Slave Node上面运行Shell的时候， 脚本访问不了Slave系统里面的Path，或者其他环境变量

# Solution 1
通过SSH自动加载配置文件里面的变量
  * /etc/ssh/sshd_config 添加 PermitUserEnvironment=yes
  * 将key, value加入到~/.ssh/environment

https://support.cloudbees.com/hc/en-us/articles/229724088-How-to-set-up-a-Jenkins-agent-to-have-the-same-path-as-the-user-when-connected-via-Remote-Desktop-

# Solution 2
加一句脚本 source .profile

# Solution 3
将环境变量加入到Jenkins Node的配置里面
