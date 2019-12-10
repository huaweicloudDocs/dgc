# 新增Checkpoint<a name="dayu_06_0069"></a>

参考[初始化DIS客户端](初始化DIS客户端-14.md)的操作初始化一个DIS客户端实例，实例名称为dic。

使用DIS SDK创建Checkpoint，需要指定通道名称、APP名称、分区编号、序列号以及Checkpoint类型。

其中，“streamName“的配置值要与[开通DIS通道](https://support.huaweicloud.com/usermanual-dis/zh-cn_topic_0034903799.html)中“Stream Name“的值一致。

```
// 通道名称 
String streamName = "myStream"; 
// APP名称
String appName = "myApp";
CommitCheckpointRequest commitCheckpointRequest = new CommitCheckpointRequest();
commitCheckpointRequest.setStreamName(streamName);
commitCheckpointRequest.setAppName(appName);
// 需要提交的sequenceNumber
commitCheckpointRequest.setSequenceNumber("100");
// 分区编号
commitCheckpointRequest.setPartitionId("0");
// Checkpoint类型
commitCheckpointRequest.setCheckpointType(CheckpointTypeEnum.LAST_READ.name());
```

配置“CommitCheckpointRequest”对象之后，通过调用 commitCheckpoint 提交checkpoint。

```
dic.commitCheckpoint(commitCheckpointRequest);
```

