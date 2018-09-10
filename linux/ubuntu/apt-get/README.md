# manage debian repository
deb http://ftp.debian.org/debian stable main contrib non-free

# PPA Repositories
see https://launchpad.net/ubuntu/+ppas?  
## Utility to add PPA repositories in your debian machine
https://github.com/msfidelis/PPA-Repository-Debian/blob/master/add-apt-repository.sh
### PPA Usage
https://www.tecmint.com/add-remove-purge-ppa-in-ubuntu/
# apt config
/etc/apt/apt.conf 
里面可以配置代理信息

# 官方的repositories
sources.list

# 目录 /etc/apt/sources.list.d/
第三方的repositories 按文件存放

# 例子
https://code.visualstudio.com/docs/setup/linux

# 加密解密的钥
在加入repository的同时，也需要加入密钥，比如
sudo install -o root -g root -m 644 microsoft.gpg /etc/apt/trusted.gpg.d/  
来自 https://code.visualstudio.com/docs/setup/linux

# 参考链接
https://thishosting.rocks/install-java-ubuntu/

