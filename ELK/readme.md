#安装
https://www.elastic.co/downloads/kibana

https://www.elastic.co/downloads/elasticsearch

https://www.elastic.co/downloads/logstash
//需要在每个datasource机器上安装filebeat
https://www.elastic.co/downloads/beats/filebeat

#logstash  

配置文件分成 input, filter, output, codec

其中codec放在input里面的

filter可以支持条件表达式
https://www.elastic.co/guide/en/logstash/5.x/event-dependent-configuration.html

支持多行日志  
https://www.elastic.co/guide/en/logstash/current/multiline.html

