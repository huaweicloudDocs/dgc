# 查询APP列表<a name="dayu_06_0040"></a>

参见[初始化DIS客户端](初始化DIS客户端-2.md)的操作初始化一个DIS客户端实例。

代码样例参考“Applist\_sample.py”文件，配置参数如下：

```
appname="app1"    #APP名称（从该通道开始返回app列表，返回的app列表不包括此app名称。）
```

配置好以上参数，执行Applist\_sample.py文件调用Applist\_test方法。

响应结果如下：

```
200
{'total_number': 2, 'apps_list': ['app1'], 'appinfo_list': [{'create_time': 1532425956631, 'app_id': 'OPKQuggQVtfqhyvK0cs', 'app_name': 'app1'}], 'has_more_app': False}
```

