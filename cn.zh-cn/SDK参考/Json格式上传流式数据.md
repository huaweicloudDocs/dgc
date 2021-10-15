# Json格式上传流式数据<a name="dgc_06_2002"></a>

参见[初始化DIS客户端](初始化DIS客户端-2.md#dgc_06_0026)的操作初始化一个DIS客户端实例。

配置参数如下：

```
streamname="dis-test1"| #已存在的通道名
```

putRecords\_sample.py文件中的putRecords\_test方法中的records为需要上传的数据内容，数据上传格式如下：

```
records=[{"data": "abcdefd", "partition_key": “1”}]
#"data"："xxx"为上传的数据值，请自定义；“partition_key”:“1”为数据写入的分区值，请自定义。
 record1 = {"data": "xxx","partition_key": partition_key}   
#可写入多条数据，数据格式如record1所示，每写一条数据使用下面的append方法传入records中。
```

配置好以上参数后，执行putRecords\_sample.py文件调用putRecords\_test方法，响应结果如下：

```
200
{'failed_record_count': 0, 'records': [{'partition_id': 'shardId-0000000001', 'sequence_number': '15'}]}
```

