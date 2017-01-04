#this is docker file for jboss server
#build command
#docker build -t wanhua/jboss/v8 .
FROM ubuntu:15.10
MAINTAINER wanhua liu <wanhua.liu01@sap.com>
ENV http_proxy http://proxy.tyo.sap.corp:8080
ENV https_proxy http://proxy.tyo.sap.corp:8080
ENV no_proxy .apj.global.corp.sap,.dhcp.pvgl.sap.corp,127.0.0.1,localhost,10.59.163.167
ENV JAVA_HOME /usr/lib/jdk/jdk1.6.0_45
ENV JAVA_OPTS=-DCSI.Home=/QU2
RUN apt-get install -y wget && apt-get install -y unzip &&apt-get install &&apt-get install -y vim &&apt-get install -y bash
RUN wget -nv http://10.58.182.187:8080/jdk-6u45-linux-x64.bin && chmod +x jdk-6u45-linux-x64.bin && ./jdk-6u45-linux-x64.bin &&mkdir /usr/lib/jdk && mv jdk1.6.0_45 /usr/lib/jdk
RUN wget -nv http://10.58.182.187:8080/jboss_jocelyn.zip &&unzip jboss_jocelyn.zip 

RUN wget -nv http://10.58.182.187:8080/FS-PRO.ear && cp FS-PRO.ear /jboss_jocelyn/server/default/
RUN wget -nv http://10.58.182.187:8080/QU2.zip && unzip QU2.zip
RUN cd jboss_jocelyn/bin &&chmod +x *.sh
#&&sleep 1 &&nohup ./run.sh
