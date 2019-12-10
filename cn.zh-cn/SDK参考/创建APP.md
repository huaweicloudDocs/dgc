# 创建APP<a name="dayu_06_0018"></a>

参考[初始化DIS客户端](初始化DIS客户端.md)的操作初始化一个DIS客户端实例。

使用DIS SDK创建APP。

```
String appName = “appName”;
            var dic = new DISIngestionClient();
            var request = new CreateAppRequest
            {
//APP的名称，用户数据消费程序的唯一标识符
                AppName = appName,
            };
            ResponseResult response = dic.CreateApp(request);
Console.Out.WriteLine(response);
```

## 运行结果<a name="zh-cn_topic_0124367681_section15291113301214"></a>

可以在控制台查看到类似如下信息：

```
{ResponseResult{status_code='201 Created', content='', errorCode='', message=''}}
```

**表 1**  ResponseResult响应参数说明

<a name="zh-cn_topic_0124367681_table548315553111"></a>
<table><thead align="left"><tr id="zh-cn_topic_0124367681_row20483105143110"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0124367681_p82498194316"><a name="zh-cn_topic_0124367681_p82498194316"></a><a name="zh-cn_topic_0124367681_p82498194316"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0124367681_p15249319153112"><a name="zh-cn_topic_0124367681_p15249319153112"></a><a name="zh-cn_topic_0124367681_p15249319153112"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0124367681_p1924991943115"><a name="zh-cn_topic_0124367681_p1924991943115"></a><a name="zh-cn_topic_0124367681_p1924991943115"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0124367681_row16483185113113"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0124367681_p182656199318"><a name="zh-cn_topic_0124367681_p182656199318"></a><a name="zh-cn_topic_0124367681_p182656199318"></a>content</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0124367681_p9265131943110"><a name="zh-cn_topic_0124367681_p9265131943110"></a><a name="zh-cn_topic_0124367681_p9265131943110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0124367681_p326501911319"><a name="zh-cn_topic_0124367681_p326501911319"></a><a name="zh-cn_topic_0124367681_p326501911319"></a>响应消息体</p>
</td>
</tr>
<tr id="zh-cn_topic_0124367681_row0483185183116"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0124367681_p18265101953111"><a name="zh-cn_topic_0124367681_p18265101953111"></a><a name="zh-cn_topic_0124367681_p18265101953111"></a>errorCode</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0124367681_p4265111919310"><a name="zh-cn_topic_0124367681_p4265111919310"></a><a name="zh-cn_topic_0124367681_p4265111919310"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0124367681_p12651019153119"><a name="zh-cn_topic_0124367681_p12651019153119"></a><a name="zh-cn_topic_0124367681_p12651019153119"></a>错误码</p>
</td>
</tr>
<tr id="zh-cn_topic_0124367681_row7483153313"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0124367681_p226517198318"><a name="zh-cn_topic_0124367681_p226517198318"></a><a name="zh-cn_topic_0124367681_p226517198318"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0124367681_p1028011923114"><a name="zh-cn_topic_0124367681_p1028011923114"></a><a name="zh-cn_topic_0124367681_p1028011923114"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0124367681_p13280101903112"><a name="zh-cn_topic_0124367681_p13280101903112"></a><a name="zh-cn_topic_0124367681_p13280101903112"></a>错误响应消息体</p>
</td>
</tr>
<tr id="zh-cn_topic_0124367681_row348365143118"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0124367681_p22801019183118"><a name="zh-cn_topic_0124367681_p22801019183118"></a><a name="zh-cn_topic_0124367681_p22801019183118"></a>status_code</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0124367681_p1928081911315"><a name="zh-cn_topic_0124367681_p1928081911315"></a><a name="zh-cn_topic_0124367681_p1928081911315"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0124367681_p12280111953110"><a name="zh-cn_topic_0124367681_p12280111953110"></a><a name="zh-cn_topic_0124367681_p12280111953110"></a>状态码</p>
</td>
</tr>
</tbody>
</table>

