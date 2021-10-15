# 查询APP列表<a name="dgc_06_0040"></a>

参见[初始化DIS客户端](初始化DIS客户端-2.md#dgc_06_0026)的操作初始化一个DIS客户端实例。

listApp\_test  方法中的（limit可设置单次请求返回APP列表的最大数量取值范围：1\~100）。

配置参数如下：

```
startAppName="app1"    #APP名称（从该通道开始返回app列表，返回的app列表不包括此app名称。）
```

配置好以上参数，执行listApp\_sample.py文件调用Applist\_test方法。

响应结果如下：

```
200
{'has_more_app': False, 'apps': [{'app_id': 'kpvGNrFYfKjpqTSdPIX', 'create_time': 1543301301992, 'app_name': 'sadfghjkl'}, {'app_id': 'MtPG1lD1E7IesDuOcNt', 'create_time': 1542765418080, 'app_name': 'testAppName2'}]}
```

