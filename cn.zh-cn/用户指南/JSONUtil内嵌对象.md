# JSONUtil内嵌对象<a name="dgc_01_0501"></a>

JSONUtil内嵌对象提供了JSON对象方法。

## 方法<a name="zh-cn_topic_0132846500_section18267348332"></a>

**表 1**  方法说明

<a name="zh-cn_topic_0132846500_table874717402336"></a>
<table><thead align="left"><tr id="zh-cn_topic_0132846500_row167470408331"><th class="cellrowborder" valign="top" width="42%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0132846500_p1774714014337"><a name="zh-cn_topic_0132846500_p1774714014337"></a><a name="zh-cn_topic_0132846500_p1774714014337"></a>方法</p>
</th>
<th class="cellrowborder" valign="top" width="57.99999999999999%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0132846500_p177471640193311"><a name="zh-cn_topic_0132846500_p177471640193311"></a><a name="zh-cn_topic_0132846500_p177471640193311"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0132846500_row1747740123312"><td class="cellrowborder" valign="top" width="42%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0132846500_p127471840153312"><a name="zh-cn_topic_0132846500_p127471840153312"></a><a name="zh-cn_topic_0132846500_p127471840153312"></a>Object parse(String jsonStr)</p>
</td>
<td class="cellrowborder" valign="top" width="57.99999999999999%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0132846500_p1874724010332"><a name="zh-cn_topic_0132846500_p1874724010332"></a><a name="zh-cn_topic_0132846500_p1874724010332"></a>将json字符串转换为对象。</p>
</td>
</tr>
<tr id="zh-cn_topic_0132846500_row3747154018335"><td class="cellrowborder" valign="top" width="42%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0132846500_p11747184043316"><a name="zh-cn_topic_0132846500_p11747184043316"></a><a name="zh-cn_topic_0132846500_p11747184043316"></a>String toString(Object jsonObject)</p>
</td>
<td class="cellrowborder" valign="top" width="57.99999999999999%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0132846500_p17747184016331"><a name="zh-cn_topic_0132846500_p17747184016331"></a><a name="zh-cn_topic_0132846500_p17747184016331"></a>将对象转换为json字符串。</p>
</td>
</tr>
<tr id="zh-cn_topic_0132846500_row197471240123319"><td class="cellrowborder" valign="top" width="42%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0132846500_p1974794003313"><a name="zh-cn_topic_0132846500_p1974794003313"></a><a name="zh-cn_topic_0132846500_p1974794003313"></a>Object path(String jsonStr,String jsonPath)</p>
</td>
<td class="cellrowborder" valign="top" width="57.99999999999999%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0132846500_p107471840133310"><a name="zh-cn_topic_0132846500_p107471840133310"></a><a name="zh-cn_topic_0132846500_p107471840133310"></a>返回json字符串指定路径下的字段值。类似于XPath，path方法可以通过路径检索或设置JSON，其路径中可以使用.或[]等访问成员、数值，例如：tables[0].table_name。</p>
</td>
</tr>
</tbody>
</table>

## 举例<a name="zh-cn_topic_0132846500_section115011297442"></a>

字符串变量str的内容如下：

```
{
            "cities": [{
                        "name": "Shenzhen",
                        "areaCode": "0755"
            },
            {
                        "name": "city2",
                        "areaCode": "010"
            },
            {
                        "name": "Shanghai",
                        "areaCode": "021"
            }]
}
```

获取深圳的电话区号，EL表达式如下：

```
#{JSONUtil.path(str,"cities[0].areaCode")}
```

