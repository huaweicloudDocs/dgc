# 创建APP<a name="dgc_06_0067"></a>

参考[初始化DIS客户端](初始化DIS客户端.md#dgc_06_0050)的操作初始化一个DIS客户端实例，实例名称为dic。

使用DIS SDK创建APP，需要指定APP名称。

```
// APP名称 
String appName = "myApp"; 
```

配置APP名称之后，通过调用createApp的方法创建APP。

```
dic.createApp(myApp);
```

