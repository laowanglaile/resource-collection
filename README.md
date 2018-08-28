# resource-collection
article:
https://www.ibm.com/developerworks/cn/java/j-lo-jse61/

orderId:
```java
public long generateOrderId(long spliterKeyId) throws DAOException {
        long id = x;//获取基础id,通常数据库表保存一个递增的id
        //混淆，自增ID加大并混淆
        long a = 10;
        long b = 3;
        if (id % a > b) {
            id = generateByTddlSeq(ticketOrderSequence);
        }
        return id * 10000 + (spliterKeyId % 10000 % 1024);
    }
```
