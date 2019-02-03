# References
[Spring Boot Reference Guide](https://spring.io/projects/spring-boot#learn)  

# Spring Boot 项目是一个Maven或者Gradle项目
声明式依赖

# 简化Spring项目的开发
## 简化了pom.xml的声明
通过starters的声明
## 通过一些规则，简化了Spring Annotation
  * root package的子 package下声明的组件会被收集到

##  @EnableAutoConfiguration 
根据jar的依赖自动配置Spring配置文件
   
## @ComponentScan
If you structure your code as suggested above (locating your application class in a root package), you can add @ComponentScan without any arguments. All of your application components (@Component, @Service, @Repository, @Controller etc.) are automatically registered as Spring Beans.

## @Configuration
allow to register extra beans in the context or import additional configuration classes

## @SpringBootApplication
The @SpringBootApplication annotation is equivalent to using @Configuration, @EnableAutoConfiguration, and @ComponentScan with their default attributes

# 打包/发布方式
所有的程序发布到一个Jar里面， 区别与普通的web程序打包成war文件
# 工具支持

# Spring Boot CLI

# Developer Tools
## 开发中的服务器自动重启

## Remote Applications
远程的方式运行程序







