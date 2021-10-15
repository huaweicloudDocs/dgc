# 删除APP<a name="dgc_06_0068"></a>

参考[初始化DIS客户端](初始化DIS客户端.md#dgc_06_0050)的操作初始化一个DIS客户端实例，实例名称为dic。

使用DIS SDK创建DIS通道，需要指定APP名称。

```
// 待删除APP名称 
String appName = "myApp"; 
```

配置APP名称之后，通过调用deleteApp的方法删除APP。

```
dic.deleteApp(myApp);
```

