# 查询APP详情<a name="dgc_06_0039"></a>

参见[初始化DIS客户端](初始化DIS客户端-2.md#dgc_06_0026)的操作初始化一个DIS客户端实例。

配置参数如下：

```
appname=”app1”      #查询的APP名称  
```

配置好以上参数，执行describeApp\_sample.py文件调用describeApp\_test方法。

响应结果如下：

```
200
{'app_name': 'app1', 'app_id': 'OPKQuggQVtfqhyvK0cs', 'create_time': 1532425956631}
```

