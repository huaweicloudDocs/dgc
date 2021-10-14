# Env内嵌对象<a name="dgc_01_0497"></a>

Env内嵌对象提供了获取环境变量值的方法。

## 方法<a name="zh-cn_topic_0172161190_section18267348332"></a>

**表 1**  方法说明

<a name="zh-cn_topic_0172161190_table874717402336"></a>
<table><thead align="left"><tr id="zh-cn_topic_0172161190_row167470408331"><th class="cellrowborder" valign="top" width="42%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0172161190_p1774714014337"><a name="zh-cn_topic_0172161190_p1774714014337"></a><a name="zh-cn_topic_0172161190_p1774714014337"></a>方法</p>
</th>
<th class="cellrowborder" valign="top" width="57.99999999999999%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0172161190_p177471640193311"><a name="zh-cn_topic_0172161190_p177471640193311"></a><a name="zh-cn_topic_0172161190_p177471640193311"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0172161190_row1747740123312"><td class="cellrowborder" valign="top" width="42%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0172161190_p127471840153312"><a name="zh-cn_topic_0172161190_p127471840153312"></a><a name="zh-cn_topic_0172161190_p127471840153312"></a>String get(String name)</p>
</td>
<td class="cellrowborder" valign="top" width="57.99999999999999%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0172161190_p1874724010332"><a name="zh-cn_topic_0172161190_p1874724010332"></a><a name="zh-cn_topic_0172161190_p1874724010332"></a>获取指定名称环境变量值。</p>
</td>
</tr>
</tbody>
</table>

## 举例<a name="zh-cn_topic_0172161190_section1259817279715"></a>

获取环境变量名称为**test**的参数值，EL表达式如下：

```
#{Env.get("test")}
```

