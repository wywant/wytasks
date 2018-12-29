# 关于plugin的两个概念
  * A plugin
  * One instance of a plugin 

# Jenkins中插件的两种形式
  * 插件可以继承自[hudson.Plugin](https://javadoc.jenkins.io/hudson/Plugin.html)
  * 或者扩展点[hudson.Extension](https://javadoc.jenkins.io/hudson/Extension.html)

# 插件的地址
根据Jenkins架构文档， 对象都是和URL绑定的。
插件的URL是${rootURL}/plugin/foo/，这里的foo是插件的名字foo.jpi

## src/main/webapp下的文件
所有src/main/webapp目录下的文件，在${rootURL}/plugin/foo/都可以，文档说包括jelly文件

## system configuration page config.jelly
Plugin有一个可选的config.jelly文件，If present, it will become a part of the system configuration page (http://server/hudson/configure)  
当然也可以通过Descriptors,  正如javadoc里面说的， this is convenient for exposing/maintaining configuration that doesn't fit any Descriptors.



