调用JCoDestinationManager.getDestination,Java错误日志栈如下  
Exception in thread "main" com.sap.conn.jco.JCoException: (106) JCO_ERROR_RESOURCE: Destination ABAP_AS does not exist  
	at com.sap.conn.jco.rt.DefaultDestinationManager.update(DefaultDestinationManager.java:217)  
	at com.sap.conn.jco.rt.DefaultDestinationManager.searchDestination(DefaultDestinationManager.java:381)  
	at com.sap.conn.jco.rt.DefaultDestinationManager.getDestinationInstance(DefaultDestinationManager.java:100)  
	at com.sap.conn.jco.JCoDestinationManager.getDestination(JCoDestinationManager.java:104)  
	at bbb.DestTest.main(DestTest.java:15)  

查看代码，简单的逻辑是从DestinationDataProvider根据destinationName 获取Properties,然后根据Properties来创建RfcDestination  
所以要创建一个DestinationDataProvider

# DestinationDataProvider的实现
JCO自带了
  * FileDestinationsDataProvider构造函数不可见
  * PropertyFileDestinationDataProvider构造函数不可见
  * SimpleDataProviderImpl构造函数不可见
  * CustomDestinationDataProvider.MyDestinationDataProvider 这是例子中的代码

## FileDestinationsDataProvider
  构造函数的参数是目录d  
  然后在目录下查找属性文件{destName}.jcoDestination
   
## PropertyFileDestinationDataProvider
  感觉和FileDestinationsDataProvider类似

JCoDestinationManager是在DefaultJCoRuntime中创建出来的，使用了PropertyFileDestinationDataProvider，并且使用了环境变量jco.destinations.dir，所以把配置文件放在目录jco.destinations.dir下

String directory = System.getProperty("jco.destinations.dir", ".");
DestinationDataProvider defProvider = new PropertyFileDestinationDataProvider(directory);

      
