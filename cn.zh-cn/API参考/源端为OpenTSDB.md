# 源端为OpenTSDB<a name="dgc_02_0294"></a>

## JSON样例<a name="zh-cn_topic_0133491666_section33401108172339"></a>

```
      "from-config-values": {
        "configs": [
          {
            "inputs": [
              {
                "name": "fromJobConfig.start",
                "value": "0"
              },
              {
                "name": "fromJobConfig.metric",
                "value": "city.temp"
              },
              {
                "name": "fromJobConfig.aggregator",
                "value": "sum"
              },
              {
                "name": "fromJobConfig.columnList",
                "value": "ps.timestample&metric&aggregator&dps.value"
              }
            ],
            "name": "fromJobConfig"
          }
        ]
      }
```

## 参数说明<a name="zh-cn_topic_0133491666_section61808073174843"></a>

<a name="zh-cn_topic_0133491666_table6307873415412"></a>
<table><thead align="left"><tr id="zh-cn_topic_0133491666_row2882542015412"><th class="cellrowborder" valign="top" width="22.657734226577343%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0133491666_p5315765115412"><a name="zh-cn_topic_0133491666_p5315765115412"></a><a name="zh-cn_topic_0133491666_p5315765115412"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20.157984201579843%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0133491666_p1080249515412"><a name="zh-cn_topic_0133491666_p1080249515412"></a><a name="zh-cn_topic_0133491666_p1080249515412"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="16.2983701629837%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0133491666_p258693615412"><a name="zh-cn_topic_0133491666_p258693615412"></a><a name="zh-cn_topic_0133491666_p258693615412"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="40.885911408859116%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0133491666_p821526915412"><a name="zh-cn_topic_0133491666_p821526915412"></a><a name="zh-cn_topic_0133491666_p821526915412"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0133491666_row3532522715412"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0133491666_p31423427144217"><a name="zh-cn_topic_0133491666_p31423427144217"></a><a name="zh-cn_topic_0133491666_p31423427144217"></a>fromJobConfig.start</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0133491666_p62269650144217"><a name="zh-cn_topic_0133491666_p62269650144217"></a><a name="zh-cn_topic_0133491666_p62269650144217"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.2983701629837%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0133491666_p10676914144217"><a name="zh-cn_topic_0133491666_p10676914144217"></a><a name="zh-cn_topic_0133491666_p10676914144217"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.885911408859116%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0133491666_p59523723144217"><a name="zh-cn_topic_0133491666_p59523723144217"></a><a name="zh-cn_topic_0133491666_p59523723144217"></a>查询的起始时间，格式为yyyyMMddHHmmdd的字符串或时间戳。</p>
</td>
</tr>
<tr id="zh-cn_topic_0133491666_row2888033144824"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0133491666_p6384845162617"><a name="zh-cn_topic_0133491666_p6384845162617"></a><a name="zh-cn_topic_0133491666_p6384845162617"></a>fromJobConfig.end</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0133491666_p23688773144824"><a name="zh-cn_topic_0133491666_p23688773144824"></a><a name="zh-cn_topic_0133491666_p23688773144824"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.2983701629837%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0133491666_p39742454144824"><a name="zh-cn_topic_0133491666_p39742454144824"></a><a name="zh-cn_topic_0133491666_p39742454144824"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.885911408859116%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0133491666_p65022171144824"><a name="zh-cn_topic_0133491666_p65022171144824"></a><a name="zh-cn_topic_0133491666_p65022171144824"></a>查询的终止时间，格式为yyyyMMddHHmmdd的字串或时间戳。</p>
</td>
</tr>
<tr id="zh-cn_topic_0133491666_row612111115270"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0133491666_p31212110273"><a name="zh-cn_topic_0133491666_p31212110273"></a><a name="zh-cn_topic_0133491666_p31212110273"></a>fromJobConfig.metric</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0133491666_p11121119272"><a name="zh-cn_topic_0133491666_p11121119272"></a><a name="zh-cn_topic_0133491666_p11121119272"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.2983701629837%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0133491666_p61409541292"><a name="zh-cn_topic_0133491666_p61409541292"></a><a name="zh-cn_topic_0133491666_p61409541292"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.885911408859116%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0133491666_p14813655143413"><a name="zh-cn_topic_0133491666_p14813655143413"></a><a name="zh-cn_topic_0133491666_p14813655143413"></a>设置迁移哪个指标的数据。</p>
</td>
</tr>
<tr id="zh-cn_topic_0133491666_row16731144613273"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0133491666_p14731124619271"><a name="zh-cn_topic_0133491666_p14731124619271"></a><a name="zh-cn_topic_0133491666_p14731124619271"></a>fromJobConfig.aggregator</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0133491666_p673154618271"><a name="zh-cn_topic_0133491666_p673154618271"></a><a name="zh-cn_topic_0133491666_p673154618271"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.2983701629837%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0133491666_p14578155562914"><a name="zh-cn_topic_0133491666_p14578155562914"></a><a name="zh-cn_topic_0133491666_p14578155562914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.885911408859116%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0133491666_p1631810574340"><a name="zh-cn_topic_0133491666_p1631810574340"></a><a name="zh-cn_topic_0133491666_p1631810574340"></a>设置聚合函数。</p>
</td>
</tr>
<tr id="zh-cn_topic_0133491666_row208121339114512"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0133491666_p18560626141527"><a name="zh-cn_topic_0133491666_p18560626141527"></a><a name="zh-cn_topic_0133491666_p18560626141527"></a>fromJobConfig.tags</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0133491666_p27015713141527"><a name="zh-cn_topic_0133491666_p27015713141527"></a><a name="zh-cn_topic_0133491666_p27015713141527"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.2983701629837%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0133491666_p50167516142856"><a name="zh-cn_topic_0133491666_p50167516142856"></a><a name="zh-cn_topic_0133491666_p50167516142856"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.885911408859116%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0133491666_p32605071143018"><a name="zh-cn_topic_0133491666_p32605071143018"></a><a name="zh-cn_topic_0133491666_p32605071143018"></a>如果这里有输入标记，则只迁移标记的数据。</p>
</td>
</tr>
<tr id="zh-cn_topic_0133491666_row5037735615412"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0133491666_p52978520144217"><a name="zh-cn_topic_0133491666_p52978520144217"></a><a name="zh-cn_topic_0133491666_p52978520144217"></a>fromJobConfig.columnList</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0133491666_p63401693144217"><a name="zh-cn_topic_0133491666_p63401693144217"></a><a name="zh-cn_topic_0133491666_p63401693144217"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.2983701629837%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0133491666_p35263486144217"><a name="zh-cn_topic_0133491666_p35263486144217"></a><a name="zh-cn_topic_0133491666_p35263486144217"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.885911408859116%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0133491666_p091005834018"><a name="zh-cn_topic_0133491666_p091005834018"></a><a name="zh-cn_topic_0133491666_p091005834018"></a>字段列表。</p>
</td>
</tr>
</tbody>
</table>

