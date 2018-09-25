# Python2和Python3安装在同一个系统
 * 当python2和python3安装在同一个系统的时候.不要将python3链接到python上去。这样会和系统安装命令冲突，如apt-get install
 * Python2的library使用pip命令安装
 * Python3的library使用pip3命令安装
 * 最好使用virtualenv安装，参考Tensorflow的安装文档

# Jupyter安装
  * 使用jupyter notebook --generate-config命令生成配置文件
  * 修改配置文件
  
  c.NotebookApp.allow_origin = '*' #allow all origins  
  c.NotebookApp.ip = '0.0.0.0' # listen on all IPs  
参考：https://stackoverflow.com/questions/42848130/why-i-cant-access-remote-jupyter-notebook-server
