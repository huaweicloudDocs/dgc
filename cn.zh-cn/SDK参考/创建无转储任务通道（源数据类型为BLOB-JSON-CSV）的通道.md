# 创建无转储任务通道（源数据类型为BLOB、JSON、CSV）的通道<a name="dayu_06_0078"></a>

```
// 通道名称
char *pucStreamName = "myStream";
char *projectId = "d575b0b740e54221aeb9a165653b103d";
char *region = "southchina";
char *host = "XXX.XXX.XXX.XXX:XXX";
int ret = 0;
DISResponseInfo RspInfo = { 0 };
DISCreateStream *pstCreateStream = disMemAlloc(sizeof(DISCreateStream));
DISCreateStreamExpend *pstCreateStreamExpend = disMemAlloc(sizeof(DISCreateStreamExpend));
pstCreateStreamExpend->dataType = DISDataTypeBlob;
pstCreateStreamExpend->dataDuration = 2 * 24;

pstCreateStream->partitionCount = 10;
pstCreateStream->streamName = pucStreamName;
pstCreateStream->streamType = DISStreamTypeAdvanced;
pstCreateStream->pucReserved = pstCreateStreamExpend;

printf("===================%s Begin=======================\n", __FUNCTION__);
ret = CreateStream(host, projectId, region, pstCreateStream, &RspInfo);
if (ret != 0)
{
printf("Create Error: %d\r\n", ret);
printf("HttpResponseCode: %ld\r\n", RspInfo.HttpResponseCode);
printf("ErrorCode: %s\r\n", RspInfo.ErrorCode);
printf("ErrorDetail: %s\r\n", RspInfo.ErrorDetail);
}
else
{
printf("Create stream %s success\n", pstCreateStream->streamName);
printf("HttpResponseCode: %ld\r\n", RspInfo.HttpResponseCode);
}

disMemFree(pstCreateStream);
printf("===================%s End=======================\n", __FUNCTION__);

```

配置“DISCreateStream”对象之后，通过调用CreateStream的方法创建通道。

```
ret = CreateStream(host, projectId, region, pstCreateStream, &RspInfo);
```

## 运行结果<a name="zh-cn_topic_0131160809_zh-cn_topic_0131140743_section61337593"></a>

可以在控制台查看到类似如下信息：

```
Create stream myStream success
HttpResponseCode: 201
```

