https://github.com/apache/ignite  
https://github.com/srecon/ignite-book-code-samples  
https://github.com/apache/ignite/tree/master/examples  

# 设置Java虚拟机参数  
  参考 https://apacheignite.readme.io/docs/jvm-and-system-tuning  
  修改apache-ignite-fabric-2.1.0-bin/bin/control.bat，去掉set JVM_OPTS前的注释，并修改  
  
# 如果想使用Durable Memory或者  
  &lt;property name="memoryConfiguration"&gt;  
  &lt;bean class="org.apache.ignite.configuration.MemoryConfiguration"&gt;  
    &lt;!-- Set the size of default memory region to 4GB. --&gt;  
    &lt;property name="defaultMemoryPolicySize" value="#{4L * 1024 * 1024 * 1024}"/&gt;  
  &lt;/bean&gt;  
&lt;/property&gt;   
  参考 https://apacheignite.readme.io/docs/durable-memory  
  参考 https://apacheignite.readme.io/docs/distributed-persistent-store  
  
  
