# resource-collection
- article:

[Instrumentation 新功能](https://www.ibm.com/developerworks/cn/java/j-lo-jse61/)

[jvm attach机制实现](http://lovestblog.cn/blog/2014/06/18/jvm-attach/)

- orderId:
```java
public long generateOrderId(long spliterKeyId) throws DAOException {
        long id = x;//获取基础id,通常数据库表保存一个递增的id
        //混淆，自增ID加大并混淆
        return id * 10000 + (spliterKeyId % 10000 % 1024);
    }
```
