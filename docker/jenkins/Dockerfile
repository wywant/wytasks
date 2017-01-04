#this is docker file for jboss server
#build command
#docker build -t wanhua/jboss/v8 .
FROM ubuntu:15.10
MAINTAINER wanhua liu <wanhua.liu01@sap.com>
ENV http_proxy http://proxy:8080
ENV https_proxy http://proxy:8080
ENV no_proxy 127.0.0.1,localhost
ENV JAVA_HOME /jdk1.8.0_71
RUN apt-get install -y wget git unzip vim bash rpm subversion openssh-client curl 

 
RUN wget  http://10.58.182.187:8080/jdk-8u71-linux-x64.gz 
RUN tar zxvf jdk-8u71-linux-x64.gz

RUN wget  http://10.58.182.187:8080/settings.xml
RUN mkdir ~/.m2
RUN mv settings.xml ~/.m2/ 
RUN ssh-keygen -t rsa -b 4096 -N "" -f ~/.ssh/id_rsa -C "wanhua.liu01@sap.com" 
RUN wget http://apache.mesi.com.ar/tomcat/tomcat-8/v8.0.30/bin/apache-tomcat-8.0.30.zip && unzip apache-tomcat-8.0.30.zip
RUN wget http://mirrors.jenkins-ci.org/war/latest/jenkins.war
RUN cp jenkins.war /apache-tomcat-8.0.30/webapps/
EXPOSE 8080
WORKDIR /apache-tomcat-8.0.30/bin
RUN chmod +x *.sh
CMD ["./catalina.sh", "run"]

