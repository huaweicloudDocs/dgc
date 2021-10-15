# DLI连接<a name="dgc_02_0277"></a>

## 介绍<a name="zh-cn_topic_0108272810_section621837"></a>

通过DLI连接，可以导入数据到数据湖探索（DLI）服务，CDM暂不支持从DLI服务导出数据。

## 连接样例<a name="zh-cn_topic_0108272810_section6163607716523"></a>

```
{
    "links": [
        {
            "link-config-values": {
                "configs": [
                    {
                        "inputs": [
                            {
                                "name": "linkConfig.ak",
                                "value": "GRC2WR0IDC6NGROYLWU2"
                            },
                            {
                                "name": "linkConfig.sk",
                                "value": "Add password here"
                            },
                            {
                                "name": "linkConfig.region",
                                "value": "cn-north-1"
                            },
                            {
                                "name": "linkConfig.projectId",
                                "value": "c48475ce8e174a7a9f775706a3d5ebe2"
                            }
                        ],
                        "name": "linkConfig"
                    }
                ]
            },
            "name": "dli",
            "connector-name": "dli-connector"
        }
    ]
}
```

## 连接参数<a name="zh-cn_topic_0108272810_section5035508012043"></a>

<a name="zh-cn_topic_0108272810_table13922888141527"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108272810_row229143141527"><th class="cellrowborder" valign="top" width="20.03%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272810_p66756185141527"><a name="zh-cn_topic_0108272810_p66756185141527"></a><a name="zh-cn_topic_0108272810_p66756185141527"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="21.099999999999998%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272810_p38541938141527"><a name="zh-cn_topic_0108272810_p38541938141527"></a><a name="zh-cn_topic_0108272810_p38541938141527"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="16.669999999999998%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272810_p34889279141527"><a name="zh-cn_topic_0108272810_p34889279141527"></a><a name="zh-cn_topic_0108272810_p34889279141527"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.199999999999996%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272810_p7459369141527"><a name="zh-cn_topic_0108272810_p7459369141527"></a><a name="zh-cn_topic_0108272810_p7459369141527"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108272810_row2725489141730"><td class="cellrowborder" valign="top" width="20.03%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272810_p19149122318018"><a name="zh-cn_topic_0108272810_p19149122318018"></a><a name="zh-cn_topic_0108272810_p19149122318018"></a>linkConfig.ak</p>
</td>
<td class="cellrowborder" valign="top" width="21.099999999999998%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272810_p17149182317017"><a name="zh-cn_topic_0108272810_p17149182317017"></a><a name="zh-cn_topic_0108272810_p17149182317017"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.669999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272810_p26544197141730"><a name="zh-cn_topic_0108272810_p26544197141730"></a><a name="zh-cn_topic_0108272810_p26544197141730"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.199999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272810_p181471423104"><a name="zh-cn_topic_0108272810_p181471423104"></a><a name="zh-cn_topic_0108272810_p181471423104"></a>登录DLI数据库的AK。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272810_row53856530141730"><td class="cellrowborder" valign="top" width="20.03%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272810_p2014610231007"><a name="zh-cn_topic_0108272810_p2014610231007"></a><a name="zh-cn_topic_0108272810_p2014610231007"></a>linkConfig.sk</p>
</td>
<td class="cellrowborder" valign="top" width="21.099999999999998%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272810_p7145162319012"><a name="zh-cn_topic_0108272810_p7145162319012"></a><a name="zh-cn_topic_0108272810_p7145162319012"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.669999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272810_p1118311915475"><a name="zh-cn_topic_0108272810_p1118311915475"></a><a name="zh-cn_topic_0108272810_p1118311915475"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.199999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272810_p5143112316010"><a name="zh-cn_topic_0108272810_p5143112316010"></a><a name="zh-cn_topic_0108272810_p5143112316010"></a>登录DLI数据库的SK。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272810_row1563612597453"><td class="cellrowborder" valign="top" width="20.03%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272810_p86361859104514"><a name="zh-cn_topic_0108272810_p86361859104514"></a><a name="zh-cn_topic_0108272810_p86361859104514"></a>linkConfig.region</p>
</td>
<td class="cellrowborder" valign="top" width="21.099999999999998%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272810_p36368596454"><a name="zh-cn_topic_0108272810_p36368596454"></a><a name="zh-cn_topic_0108272810_p36368596454"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.669999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272810_p1616132054716"><a name="zh-cn_topic_0108272810_p1616132054716"></a><a name="zh-cn_topic_0108272810_p1616132054716"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.199999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272810_p12636155914459"><a name="zh-cn_topic_0108272810_p12636155914459"></a><a name="zh-cn_topic_0108272810_p12636155914459"></a>DLI服务所在的区域。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272810_row13756414611"><td class="cellrowborder" valign="top" width="20.03%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272810_p53763418465"><a name="zh-cn_topic_0108272810_p53763418465"></a><a name="zh-cn_topic_0108272810_p53763418465"></a>linkConfig.projectId</p>
</td>
<td class="cellrowborder" valign="top" width="21.099999999999998%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272810_p6376644466"><a name="zh-cn_topic_0108272810_p6376644466"></a><a name="zh-cn_topic_0108272810_p6376644466"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.669999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272810_p118111202475"><a name="zh-cn_topic_0108272810_p118111202475"></a><a name="zh-cn_topic_0108272810_p118111202475"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.199999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272810_p1637616424613"><a name="zh-cn_topic_0108272810_p1637616424613"></a><a name="zh-cn_topic_0108272810_p1637616424613"></a>DLI服务的项目ID。</p>
</td>
</tr>
</tbody>
</table>

