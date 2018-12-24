# 环境搭建
## 安装本地Jenkins
### 需要安装的Jenkins插件
Job DSL	

## 开发工具

### Blue Ocean Editor
用来开发流程，挺好的
### Command-line Pipeline Linter
语法检查，仅仅是语法检查，不识别step真实存在
### "Replay" Pipeline Runs with Modifications
直接在Jenkins上修改代码，做测试。提高开发速度。

### IDE Integrations

#### VS Code
集成了Command-line Pipeline Linter， 检查语法而已。
https://marketplace.visualstudio.com/items?itemName=janjoerke.jenkins-pipeline-linter-connector

### Pipeline Unit Testing Framework

### 参考文档
[Pipeline Development Tools](https://jenkins.io/doc/book/pipeline/development/)  

### 开发工具与Jenkins的集成

## Git Repositories

## 参考文档

[Tutorial Using the Jenkins Job DSL](https://github.com/jenkinsci/job-dsl-plugin/wiki/Tutorial---Using-the-Jenkins-Job-DSL)  

# 一些心得
## Jenkinsfile里面调用groovy代码
### 前提
首先在Jenkins配置里面加到Global Pipeline Libraries里面

### Global Pipeline Libraries
   * global variables也就是vars目录下的代码中，可以调用src目录下面的代码，通过import

### 在Jenkinsfile里面调用Global Library里面的class和global variables
   可行

### 在Jenkinsfile里面调用当前repository里面的class
通过load方法， 并且有两种调用方法，具体参考 [load file](https://github.com/jenkinsci/pipeline-examples/tree/master/pipeline-examples/load-from-file)
```
 def externalMethod = load("externalMethod.groovy")
 externalMethod.lookAtThis("Steve")
 def externalCall = load("externalCall.groovy")
    externalCall("Steve")
```
# 一些问题
## 为什么要在global pipeline library里面加上Jenkinsfile文件

