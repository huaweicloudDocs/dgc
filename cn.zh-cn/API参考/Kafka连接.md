# Kafka连接<a name="dgc_02_0274"></a>

## 介绍<a name="zh-cn_topic_0108272808_section621837"></a>

通过Kafka连接器可以与开源的Kafka数据源建立连接，并按照用户指定配置将Kafka中的数据迁移到其它数据源。目前仅支持从Kafka导出数据。

## 连接样例<a name="zh-cn_topic_0108272808_section6163607716523"></a>

```
{
    "links": [
        {
            "link-config-values": {
                "configs": [
                    {
                        "inputs": [
                            {
                                "name": "linkConfig.brokerList",
                                "value": "127.0.0.1:9092"
                            }
                        ],
                        "name": "linkConfig"
                    }
                ]
            },
            "name": "kafka_link",
            "connector-name": "kafka-connector"
        }
    ]
}
```

## 连接参数<a name="zh-cn_topic_0108272808_section5035508012043"></a>

<a name="zh-cn_topic_0108272808_table13922888141527"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108272808_row229143141527"><th class="cellrowborder" valign="top" width="20.22%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272808_p66756185141527"><a name="zh-cn_topic_0108272808_p66756185141527"></a><a name="zh-cn_topic_0108272808_p66756185141527"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20.16%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272808_p38541938141527"><a name="zh-cn_topic_0108272808_p38541938141527"></a><a name="zh-cn_topic_0108272808_p38541938141527"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.419999999999998%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272808_p34889279141527"><a name="zh-cn_topic_0108272808_p34889279141527"></a><a name="zh-cn_topic_0108272808_p34889279141527"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.199999999999996%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272808_p7459369141527"><a name="zh-cn_topic_0108272808_p7459369141527"></a><a name="zh-cn_topic_0108272808_p7459369141527"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108272808_row2725489141730"><td class="cellrowborder" valign="top" width="20.22%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272808_p28492222171138"><a name="zh-cn_topic_0108272808_p28492222171138"></a><a name="zh-cn_topic_0108272808_p28492222171138"></a>linkConfig.brokerList</p>
</td>
<td class="cellrowborder" valign="top" width="20.16%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272808_p2813219141730"><a name="zh-cn_topic_0108272808_p2813219141730"></a><a name="zh-cn_topic_0108272808_p2813219141730"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272808_p26544197141730"><a name="zh-cn_topic_0108272808_p26544197141730"></a><a name="zh-cn_topic_0108272808_p26544197141730"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.199999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272808_p2596372141730"><a name="zh-cn_topic_0108272808_p2596372141730"></a><a name="zh-cn_topic_0108272808_p2596372141730"></a>Kafka broker列表，格式如：<span class="parmvalue" id="zh-cn_topic_0108272808_parmvalue5393115815435"><a name="zh-cn_topic_0108272808_parmvalue5393115815435"></a><a name="zh-cn_topic_0108272808_parmvalue5393115815435"></a>“host1:port1,host2:port2”</span>。</p>
</td>
</tr>
</tbody>
</table>

