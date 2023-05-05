## Kafka Log

Kafka是基于page cache来实现文件的写入，至于什么时候把page cache里的数据刷到磁盘里，这是由操作系统来决定

### 零拷贝技术



## producer

### 重要参数

```
batch.size
linger.ms
buffer.memory
```





## doSend

### waitOnMetadata

获取topic的原数据信息，如果没有缓存，就会去从leader节点拉取topic的信息？

### serializedKey

### 计算partition

如果没有指定partition，那么就会根据key的hash值与partition的数量，取余

### Check  the message size 

maxRequestSize 和 totalMemorySize

### Call back function

## Network

### NIO

在启动Kafka client 的时候，会通过多线程的方式，

#### KafkaClient



### Selector

