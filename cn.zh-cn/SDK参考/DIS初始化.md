# DIS初始化<a name="dayu_06_0076"></a>

下面是main函数，其中包含dis参数配置，dis初始化，dis传输方式的设置以及上传下载示例的调用，回收处理操作等。

```
int main()
{
int ret = 0;
FILE *logFile = NULL;
//通道所在的资源ID
char *projectId = "c159a24641da49b2a729ea6f57647888";
//用户使用通道所在的区域
char *region = "******";
// DIS的访问地址
char *host = "dis.cn-north-1.myhuaweicloud.com:20004";
//通道名称
char *streamName = "lifei_test";

srand((unsigned) time(NULL ));
logFile = fopen("log.txt", "a+");
if(NULL == logFile)
{
printf("open file error\r\n");
return 1;
}
printf("step 1\r\n");
ret = DisInit(logFile, GetUserAuthInfo);
if(0 != ret)
{
printf("init error: %d\r\n", ret);
getchar();
return ret;
}
printf("start test\r\n");

logPrint(1, "this is a test: %d", ret);
DISSetSerializedMode("protobuf");//设置为protobuf的方式上传、下载数据
testSendRecord(streamName);
testGetRecord(streamName);

getchar();
DisDeinit();

return 0;
}
```

-   DIS的初始化方法： DisInit\(logFile, GetUserAuthInfo\);
-   设置数据传送的序列化的方式是protobuf： DISSetSerializedMode\("protobuf"\);
-   设置数据传送的序列化的方式是base64： DISSetSerializedMode\("base64"\);
-   发送数据： testSendRecord\(streamName\);
-   下载数据： testGetRecord\(streamName\);

