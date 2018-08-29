
# 分布式系统设计要点

## 基础设施
```
  dns负载均衡(静态资源)
  反向代理+负载均衡(nginx主备)
  全链路日志(https://www.elastic.co/cn/elk-stack)
  数据库集群(mysql)
  缓存集群(redis,memcached)
  nosql存储(mongodb,hbase)
  分布式文件系统(ceph)
  消息集群(rocketmq,rabbitmq)
  分布式协调(zookeeper)
  大数据存储(spark+hdfs)
  搜索引擎(elasticsearch)
  风控
  数据分析
  实时计算
```
## 开发框架
```
  web框架(springmvc)
  restful框架(resteasy)
  rpc框架(dubbo,grpc)
  分库分表(shardingjdbc,mybaits)
  服务集成框架(springboot)
  服务治理(限流,降级,熔断)
  安全框架()
  分布式任务调度框架(quartz)
  批处理框架(springbatch)
  服务监控(命中,错误,异常,响应时间)
  后台管理(数据聚合查询,数据修复,动态开关)
  oauth2认证框架
  单点登录
  调用链
  动态配置中心
  状态机(Spring Statemachine)
  流程引擎()
```
[分布式系统理论](https://zhuanlan.zhihu.com/distributed?utm_source=com.jianshu.haruki&utm_medium=social)

[elasticjob.io](http://elasticjob.io/)

[shardingsphere.io](shardingsphere.io)

[elk](https://www.elastic.co/cn/elk-stack)

[Spring Statemachine](https://projects.spring.io/spring-statemachine/)

[spring状态机参考-1](https://www.jianshu.com/p/bbee41d8defb)

[spring状态机参考-2](https://www.jianshu.com/p/326bd3ac2bf2)




## 设计要素
```
  restful api(授权信息,md5摘要)
  结果对象(结果对象,错误码,错误信息)
  入参对象(requestId,anwserId,transId,traceId)
  幂等方案
  并发控制(分布式锁)
  数据条件更新
  服务端消息排重(缓存msgId)
  失败重试(注册调度任务,重试时间)
  异步(返回transId)
  dto,domain,dao分离
  领域驱动(领域服务,领域对象,领域事件)
  查询,命令分离
  分布式id
  缓存更新策略
  消息解耦(消息排序,事务性)
  报警(短信-防疲劳)
```
## 数据表设计要点
```
   主表+扩展表
   快照存储(hbase)
   版本号,分库分表键,删除标志,不可见标志
```






