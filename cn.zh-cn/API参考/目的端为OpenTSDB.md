# 目的端为OpenTSDB<a name="dgc_02_0307"></a>

## JSON样例<a name="zh-cn_topic_0133491667_section33401108172339"></a>

```
"to-config-values": {
        "configs": [
          {
            "inputs": [
              {
                "name": "toJobConfig.metric",
                "value": "city.temp"
              },
              {
                "name": "toJobConfig.timeStamp",
                "value": "0"
              },
              {
                "name": "toJobConfig.tags",
                "value": "tagk1:tagv1"
              },
              {
                "name": "toJobConfig.columnList",
                "value": "metric:1&tag:2&timestamp&value"
              }
            ],
            "name": "toJobConfig"
          }
        ]
      }
```

## 参数说明<a name="zh-cn_topic_0133491667_section28186120174818"></a>

<a name="zh-cn_topic_0133491667_table13922888141527"></a>
<table><thead align="left"><tr id="zh-cn_topic_0133491667_row229143141527"><th class="cellrowborder" valign="top" width="22.66%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0133491667_p66756185141527"><a name="zh-cn_topic_0133491667_p66756185141527"></a><a name="zh-cn_topic_0133491667_p66756185141527"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="19.78%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0133491667_p38541938141527"><a name="zh-cn_topic_0133491667_p38541938141527"></a><a name="zh-cn_topic_0133491667_p38541938141527"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.05%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0133491667_p34889279141527"><a name="zh-cn_topic_0133491667_p34889279141527"></a><a name="zh-cn_topic_0133491667_p34889279141527"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="40.510000000000005%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0133491667_p7459369141527"><a name="zh-cn_topic_0133491667_p7459369141527"></a><a name="zh-cn_topic_0133491667_p7459369141527"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0133491667_row3332173310395"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0133491667_p1533263315395"><a name="zh-cn_topic_0133491667_p1533263315395"></a><a name="zh-cn_topic_0133491667_p1533263315395"></a>toJobConfig.metric</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0133491667_p173324335394"><a name="zh-cn_topic_0133491667_p173324335394"></a><a name="zh-cn_topic_0133491667_p173324335394"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0133491667_p1633283373913"><a name="zh-cn_topic_0133491667_p1633283373913"></a><a name="zh-cn_topic_0133491667_p1633283373913"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0133491667_p93321733173914"><a name="zh-cn_topic_0133491667_p93321733173914"></a><a name="zh-cn_topic_0133491667_p93321733173914"></a>数据的指标名称。</p>
</td>
</tr>
<tr id="zh-cn_topic_0133491667_row159149216431"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0133491667_p1914142114316"><a name="zh-cn_topic_0133491667_p1914142114316"></a><a name="zh-cn_topic_0133491667_p1914142114316"></a>toJobConfig.timeStamp</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0133491667_p209144217437"><a name="zh-cn_topic_0133491667_p209144217437"></a><a name="zh-cn_topic_0133491667_p209144217437"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0133491667_p11914122144314"><a name="zh-cn_topic_0133491667_p11914122144314"></a><a name="zh-cn_topic_0133491667_p11914122144314"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0133491667_p5914192124316"><a name="zh-cn_topic_0133491667_p5914192124316"></a><a name="zh-cn_topic_0133491667_p5914192124316"></a>记录数据的时间点，格式为yyyyMMddHHmmdd的字符串或时间戳。</p>
</td>
</tr>
<tr id="zh-cn_topic_0133491667_row62628929141527"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0133491667_p18560626141527"><a name="zh-cn_topic_0133491667_p18560626141527"></a><a name="zh-cn_topic_0133491667_p18560626141527"></a>toJobConfig.tags</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0133491667_p27015713141527"><a name="zh-cn_topic_0133491667_p27015713141527"></a><a name="zh-cn_topic_0133491667_p27015713141527"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0133491667_p50167516142856"><a name="zh-cn_topic_0133491667_p50167516142856"></a><a name="zh-cn_topic_0133491667_p50167516142856"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0133491667_p32605071143018"><a name="zh-cn_topic_0133491667_p32605071143018"></a><a name="zh-cn_topic_0133491667_p32605071143018"></a>数据的标签。</p>
</td>
</tr>
<tr id="zh-cn_topic_0133491667_row4268185173352"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0133491667_p1253517963912"><a name="zh-cn_topic_0133491667_p1253517963912"></a><a name="zh-cn_topic_0133491667_p1253517963912"></a>toJobConfig.columnList</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0133491667_p19169610173352"><a name="zh-cn_topic_0133491667_p19169610173352"></a><a name="zh-cn_topic_0133491667_p19169610173352"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0133491667_p9234573173352"><a name="zh-cn_topic_0133491667_p9234573173352"></a><a name="zh-cn_topic_0133491667_p9234573173352"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0133491667_p9802957173352"><a name="zh-cn_topic_0133491667_p9802957173352"></a><a name="zh-cn_topic_0133491667_p9802957173352"></a>字段列表。</p>
</td>
</tr>
</tbody>
</table>

