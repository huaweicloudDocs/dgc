# 查询Checkpoint<a name="dgc_06_0070"></a>

参考[初始化DIS客户端](初始化DIS客户端.md#dgc_06_0050)的操作初始化一个DIS客户端实例，实例名称为dic。

其中，“streamName”的配置值要与[开通DIS通道](https://support.huaweicloud.com/usermanual-dis/dis_01_0601.html)中“通道名称”的值一致，“endpoint”，“ak”，“sk”，“region”，“projectId”信息请参见[获取认证信息](获取认证信息.md#dgc_06_0005)。

```
GetCheckpointRequest getCheckpointRequest = new GetCheckpointRequest();
// 设置App名称(注: 1.3.0及以前版本使用setAppId，1.3.1及后续版本请使用setAppName
getCheckpointRequest.setAppName(appName);
getCheckpointRequest.setStreamName(streamName);
// 分区编号
getCheckpointRequest.setPartitionId("0");
// Checkpoint类型
getCheckpointRequest.setCheckpointType(CheckpointTypeEnum.LAST_READ.name());
System.out.println("getCheckpoint: " + JsonUtils.objToJson(dic.getCheckpoint(getCheckpointRequest)));
```

查询Checkpoint的返回信息如下。

```
getCheckpoint:
{"sequence_number": "10", "metadata": "metadata"}
```

