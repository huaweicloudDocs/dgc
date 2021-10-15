# DMS Kafka连接<a name="dgc_02_0280"></a>

## 介绍<a name="zh-cn_topic_0143158089_section621837"></a>

通过DMS Kafka连接，可以连接DMS Kafka普通队列或者专享版Kafka。目前仅支持从DMS Kafka导出数据到云搜索服务。

## 连接样例<a name="zh-cn_topic_0143158089_section6163607716523"></a>

```
{
  "links": [
    {
      "link-config-values": {
        "configs": [
          {
            "inputs": [
              {
                "name": "linkConfig.kafkaType",
                "value": "Basic"
              },
              {
                "name": "linkConfig.endpoint",
                "value": "dms-kafka.cn-north-1.myhuaweicloud.com:37000"
              },
              {
                "name": "linkConfig.ak",
                "value": "GRC2WR0IDC6NGROYLWU2"
              },
              {
                "name": "linkConfig.sk",
                "value": "Add password here"
              },
              {
                "name": "linkConfig.projectId",
                "value": "c48475ce8e174a7a9f775706a3d5ebe2"
              },
              {
                "name": "linkConfig.targetProjectId",
                "value": "be1a07648c074b948700a03fa3c0990e"
              }
            ],
            "name": "linkConfig"
          }
        ]
      },
      "name": "dms",
      "connector-name": "dms-kafka-connector"
    }
  ]
}
```

## 连接参数<a name="zh-cn_topic_0143158089_section5035508012043"></a>

<a name="zh-cn_topic_0143158089_table13922888141527"></a>
<table><thead align="left"><tr id="zh-cn_topic_0143158089_row229143141527"><th class="cellrowborder" valign="top" width="27.777222277772225%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0143158089_p66756185141527"><a name="zh-cn_topic_0143158089_p66756185141527"></a><a name="zh-cn_topic_0143158089_p66756185141527"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="19.998000199980005%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0143158089_p38541938141527"><a name="zh-cn_topic_0143158089_p38541938141527"></a><a name="zh-cn_topic_0143158089_p38541938141527"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="16.66833316668333%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0143158089_p34889279141527"><a name="zh-cn_topic_0143158089_p34889279141527"></a><a name="zh-cn_topic_0143158089_p34889279141527"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="35.55644435556445%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0143158089_p7459369141527"><a name="zh-cn_topic_0143158089_p7459369141527"></a><a name="zh-cn_topic_0143158089_p7459369141527"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0143158089_row2725489141730"><td class="cellrowborder" valign="top" width="27.777222277772225%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0143158089_p28492222171138"><a name="zh-cn_topic_0143158089_p28492222171138"></a><a name="zh-cn_topic_0143158089_p28492222171138"></a>linkConfig.kafkaType</p>
</td>
<td class="cellrowborder" valign="top" width="19.998000199980005%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0143158089_p2813219141730"><a name="zh-cn_topic_0143158089_p2813219141730"></a><a name="zh-cn_topic_0143158089_p2813219141730"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.66833316668333%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0143158089_p26544197141730"><a name="zh-cn_topic_0143158089_p26544197141730"></a><a name="zh-cn_topic_0143158089_p26544197141730"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="35.55644435556445%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0143158089_p147692714538"><a name="zh-cn_topic_0143158089_p147692714538"></a><a name="zh-cn_topic_0143158089_p147692714538"></a>选择DMS Kafka版本：</p>
<a name="zh-cn_topic_0143158089_ul182931744102816"></a><a name="zh-cn_topic_0143158089_ul182931744102816"></a><ul id="zh-cn_topic_0143158089_ul182931744102816"><li>Basic：指DMS Kafka普通队列。</li><li>Platinum：指DMS Kafka专享版。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0143158089_row15083401734"><td class="cellrowborder" valign="top" width="27.777222277772225%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0143158089_p1550918404315"><a name="zh-cn_topic_0143158089_p1550918404315"></a><a name="zh-cn_topic_0143158089_p1550918404315"></a>linkConfig.endpoint</p>
</td>
<td class="cellrowborder" valign="top" width="19.998000199980005%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0143158089_p67951030103513"><a name="zh-cn_topic_0143158089_p67951030103513"></a><a name="zh-cn_topic_0143158089_p67951030103513"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.66833316668333%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0143158089_p13796133043517"><a name="zh-cn_topic_0143158089_p13796133043517"></a><a name="zh-cn_topic_0143158089_p13796133043517"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="35.55644435556445%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0143158089_p20509840330"><a name="zh-cn_topic_0143158089_p20509840330"></a><a name="zh-cn_topic_0143158089_p20509840330"></a>DMS Endpoint格式为host:port。</p>
</td>
</tr>
<tr id="zh-cn_topic_0143158089_row194813461330"><td class="cellrowborder" valign="top" width="27.777222277772225%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0143158089_p594810462317"><a name="zh-cn_topic_0143158089_p594810462317"></a><a name="zh-cn_topic_0143158089_p594810462317"></a>linkConfig.ak</p>
</td>
<td class="cellrowborder" valign="top" width="19.998000199980005%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0143158089_p16823152914352"><a name="zh-cn_topic_0143158089_p16823152914352"></a><a name="zh-cn_topic_0143158089_p16823152914352"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.66833316668333%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0143158089_p148243292357"><a name="zh-cn_topic_0143158089_p148243292357"></a><a name="zh-cn_topic_0143158089_p148243292357"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="35.55644435556445%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0143158089_p181471423104"><a name="zh-cn_topic_0143158089_p181471423104"></a><a name="zh-cn_topic_0143158089_p181471423104"></a>访问DMS Kafka的凭证AK。</p>
</td>
</tr>
<tr id="zh-cn_topic_0143158089_row928344716313"><td class="cellrowborder" valign="top" width="27.777222277772225%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0143158089_p132837471835"><a name="zh-cn_topic_0143158089_p132837471835"></a><a name="zh-cn_topic_0143158089_p132837471835"></a>linkConfig.sk</p>
</td>
<td class="cellrowborder" valign="top" width="19.998000199980005%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0143158089_p208451282357"><a name="zh-cn_topic_0143158089_p208451282357"></a><a name="zh-cn_topic_0143158089_p208451282357"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.66833316668333%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0143158089_p188461228103518"><a name="zh-cn_topic_0143158089_p188461228103518"></a><a name="zh-cn_topic_0143158089_p188461228103518"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="35.55644435556445%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0143158089_p5143112316010"><a name="zh-cn_topic_0143158089_p5143112316010"></a><a name="zh-cn_topic_0143158089_p5143112316010"></a>访问DMS Kafka的凭证SK。</p>
</td>
</tr>
<tr id="zh-cn_topic_0143158089_row195946471835"><td class="cellrowborder" valign="top" width="27.777222277772225%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0143158089_p135941447532"><a name="zh-cn_topic_0143158089_p135941447532"></a><a name="zh-cn_topic_0143158089_p135941447532"></a>linkConfig.projectId</p>
</td>
<td class="cellrowborder" valign="top" width="19.998000199980005%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0143158089_p26039827141730"><a name="zh-cn_topic_0143158089_p26039827141730"></a><a name="zh-cn_topic_0143158089_p26039827141730"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.66833316668333%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0143158089_p28851277141730"><a name="zh-cn_topic_0143158089_p28851277141730"></a><a name="zh-cn_topic_0143158089_p28851277141730"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="35.55644435556445%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0143158089_p1637616424613"><a name="zh-cn_topic_0143158089_p1637616424613"></a><a name="zh-cn_topic_0143158089_p1637616424613"></a>DMS所在区域的项目ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0143158089_row159371471239"><td class="cellrowborder" valign="top" width="27.777222277772225%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0143158089_p1493715478318"><a name="zh-cn_topic_0143158089_p1493715478318"></a><a name="zh-cn_topic_0143158089_p1493715478318"></a>linkConfig.targetProjectId</p>
</td>
<td class="cellrowborder" valign="top" width="19.998000199980005%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0143158089_p17937247334"><a name="zh-cn_topic_0143158089_p17937247334"></a><a name="zh-cn_topic_0143158089_p17937247334"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.66833316668333%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0143158089_p19371147538"><a name="zh-cn_topic_0143158089_p19371147538"></a><a name="zh-cn_topic_0143158089_p19371147538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="35.55644435556445%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0143158089_p12287142410545"><a name="zh-cn_topic_0143158089_p12287142410545"></a><a name="zh-cn_topic_0143158089_p12287142410545"></a>如果需要访问其他用户授权的队列，则需要配置授权者的Project ID。</p>
</td>
</tr>
</tbody>
</table>

