## Server服务器端存储配置
  * 原始配置 examples
  * Ignite自带配置
  * 第三方存储，采用jdbc mysql 配置

## DDL 配置

  * DDL Based Configuration  
  * 通过Java Annotations定义DDL  
  * QueryEntity Based Configuration  
  
## Application中Ignite.start()的方式  
  * 没有参数
  * 通过指定spring xml路径
  * 通过指定IgniteConfiguration
  
## Run代码运行  
  * 在Java Application里面运行 
  * 在服务器里面运行
  
## Result结果  
  *insert 或者 put 语句是否执行成功
  *get是否执行成功
  *query是否执行成功

| Server           | DDL             | Ignite.start      | Run       | Insert | Get| Query|
| ---------------- |:---------------:| -----------------:|-----------|--------|-----|------|
| examples         |Distributed DDL  | No Arguments      |Application|pass    |pass |pass  |
|                  |                 |                   |Runnable   |pass    |pass |pass  |
|                  |                 | Spring XML Path   |Application|pass    |pass |pass  |
|                  |                 |                   |Runnable   |pass    |pass |pass  |
|                  |                 |IgniteConfiguration|Application|pass    |pass |pass  |
|                  |                 |                   |Runnable   |pass    |pass |pass  |
|                  |Java Annotation  | No Arguments      |Application|pass    |pass |pass  |
|                  |                 |                   |Runnable   |pass    |pass |pass  |
|                  |                 | Spring XML Path   |Application|pass    |pass |pass  |
|                  |                 |                   |Runnable   |pass    |pass |pass  |
|                  |                 |IgniteConfiguration|Application|pass    |pass |pass  |
|                  |                 |                   |Runnable   |pass    |pass |pass  |
|                  |QueryEntity Based| No Arguments      |Application|pass    |pass |pass  |
|                  |                 |                   |Runnable   |pass    |pass |pass  |
|                  |                 | Spring XML Path   |Application|pass    |pass |pass  |
|                  |                 |                   |Runnable   |pass    |pass |pass  |
|                  |                 |IgniteConfiguration|Application|pass    |pass |pass  |
|                  |                 |                   |Runnable   |pass    |pass |pass  |
|Ignite Persistence|Distributed DDL  | No Arguments      |Application|pass    |pass |pass  |
|                  |                 |                   |Runnable   |pass    |pass |pass  |
|                  |                 | Spring XML Path   |Application|pass    |pass |pass  |
|                  |                 |                   |Runnable   |pass    |pass |pass  |
|                  |                 |IgniteConfiguration|Application|pass    |pass |pass  |
|                  |                 |                   |Runnable   |pass    |pass |pass  |
|                  |Java Annotation  | No Arguments      |Application|pass    |pass |pass  |
|                  |                 |                   |Runnable   |pass    |pass |pass  |
|                  |                 | Spring XML Path   |Application|pass    |pass |pass  |
|                  |                 |                   |Runnable   |pass    |pass |pass  |
|                  |                 |IgniteConfiguration|Application|pass    |pass |pass  |
|                  |                 |                   |Runnable   |pass    |pass |pass  |
|                  |QueryEntity Based| No Arguments      |Application|pass    |pass |pass  |
|                  |                 |                   |Runnable   |pass    |pass |pass  |
|                  |                 | Spring XML Path   |Application|pass    |pass |pass  |
|                  |                 |                   |Runnable   |pass    |pass |pass  |
|                  |                 |IgniteConfiguration|Application|pass    |pass |pass  |
|                  |                 |                   |Runnable   |pass    |pass |pass  |
| jdbc mysql       |Distributed DDL  | No Arguments      |Application|pass    |pass |pass  |
|                  |                 |                   |Runnable   |pass    |pass |pass  |
|                  |                 | Spring XML Path   |Application|pass    |pass |pass  |
|                  |                 |                   |Runnable   |pass    |pass |pass  |
|                  |                 |IgniteConfiguration|Application|pass    |pass |pass  |
|                  |                 |                   |Runnable   |pass    |pass |pass  |
|                  |Java Annotation  | No Arguments      |Application|pass    |pass |pass  |
|                  |                 |                   |Runnable   |pass    |pass |pass  |
|                  |                 | Spring XML Path   |Application|pass    |pass |pass  |
|                  |                 |                   |Runnable   |pass    |pass |pass  |
|                  |                 |IgniteConfiguration|Application|pass    |pass |pass  |
|                  |                 |                   |Runnable   |pass    |pass |pass  |
|                  |QueryEntity Based| No Arguments      |Application|pass    |pass |pass  |
|                  |                 |                   |Runnable   |pass    |pass |pass  |
|                  |                 | Spring XML Path   |Application|pass    |pass |pass  |
|                  |                 |                   |Runnable   |pass    |pass |pass  |
|                  |                 |IgniteConfiguration|Application|pass    |pass |pass  |
|                  |                 |                   |Runnable   |pass    |pass |pass  |
