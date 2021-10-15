# 查询Checkpoint<a name="dgc_06_0042"></a>

参见[初始化DIS客户端](初始化DIS客户端-2.md#dgc_06_0026)的操作初始化一个DIS客户端实例。

配置参数如下：

```
streamname = "" #通道名称
appName="xx"      # APP名称（APP是已存在状态）
partitionId="shardId-0000000000"  #分区的唯一标识符
```

>![](public_sys-resources/icon-note.gif) **说明：** 
>partitionId可通过[查询通道详情](查询通道详情-9.md#dgc_06_0033)获取，需要先传入当前设置的通道名称。

配置好以上参数，执行getCheckpoint\_sample.py文件调用getCheckpoint\_test方法，响应结果如下：

```
{  
  "sequence_number": "10", 
  "metadata": "metadata"   
}
```

