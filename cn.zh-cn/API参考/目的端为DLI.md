# 目的端为DLI<a name="dgc_02_0305"></a>

## JSON样例<a name="zh-cn_topic_0108272819_section33401108172339"></a>

```
"to-config-values": {
                "configs": [
                    {
                        "inputs": [
                            {
                                "name": "toJobConfig.queue",
                                "value": "cdm"
                            },
                            {
                                "name": "toJobConfig.database",
                                "value": "sqoop"
                            },
                            {
                                "name": "toJobConfig.table",
                                "value": "est1"
                            },
                            {
                                "name": "toJobConfig.columnList",
                                "value": "string_&int_&date_&double_&boolean_&short_&timestamp_&long_&smallint_&bigint_"
                            },
                            {
                                "name": "toJobConfig.shouldClearTable",
                                "value": "false"
                            }
                        ],
                        "name": "toJobConfig"
                    }
                ]
            }
```

## 参数说明<a name="zh-cn_topic_0108272819_section60129242115832"></a>

<a name="zh-cn_topic_0108272819_table6307873415412"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108272819_row2882542015412"><th class="cellrowborder" valign="top" width="22.657734226577343%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272819_p5315765115412"><a name="zh-cn_topic_0108272819_p5315765115412"></a><a name="zh-cn_topic_0108272819_p5315765115412"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20.157984201579843%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272819_p1080249515412"><a name="zh-cn_topic_0108272819_p1080249515412"></a><a name="zh-cn_topic_0108272819_p1080249515412"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="16.2983701629837%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272819_p258693615412"><a name="zh-cn_topic_0108272819_p258693615412"></a><a name="zh-cn_topic_0108272819_p258693615412"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="40.885911408859116%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272819_p821526915412"><a name="zh-cn_topic_0108272819_p821526915412"></a><a name="zh-cn_topic_0108272819_p821526915412"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108272819_row1592012572154"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272819_p682241305919"><a name="zh-cn_topic_0108272819_p682241305919"></a><a name="zh-cn_topic_0108272819_p682241305919"></a>toJobConfig.queue</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272819_p282119130591"><a name="zh-cn_topic_0108272819_p282119130591"></a><a name="zh-cn_topic_0108272819_p282119130591"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.2983701629837%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272819_p39742454144824"><a name="zh-cn_topic_0108272819_p39742454144824"></a><a name="zh-cn_topic_0108272819_p39742454144824"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.885911408859116%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272819_p138199136592"><a name="zh-cn_topic_0108272819_p138199136592"></a><a name="zh-cn_topic_0108272819_p138199136592"></a>写入数据的资源队列。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272819_row3532522715412"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272819_p383251310597"><a name="zh-cn_topic_0108272819_p383251310597"></a><a name="zh-cn_topic_0108272819_p383251310597"></a>toJobConfig.database</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272819_p1683119136599"><a name="zh-cn_topic_0108272819_p1683119136599"></a><a name="zh-cn_topic_0108272819_p1683119136599"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.2983701629837%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272819_p11830101315911"><a name="zh-cn_topic_0108272819_p11830101315911"></a><a name="zh-cn_topic_0108272819_p11830101315911"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.885911408859116%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272819_p188281713155918"><a name="zh-cn_topic_0108272819_p188281713155918"></a><a name="zh-cn_topic_0108272819_p188281713155918"></a>写入数据到数据湖探索（DLI）的哪个数据库。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272819_row2888033144824"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272819_p19827171355920"><a name="zh-cn_topic_0108272819_p19827171355920"></a><a name="zh-cn_topic_0108272819_p19827171355920"></a>toJobConfig.table</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272819_p18825161385913"><a name="zh-cn_topic_0108272819_p18825161385913"></a><a name="zh-cn_topic_0108272819_p18825161385913"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.2983701629837%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272819_p1824181305916"><a name="zh-cn_topic_0108272819_p1824181305916"></a><a name="zh-cn_topic_0108272819_p1824181305916"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.885911408859116%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272819_p8823111311598"><a name="zh-cn_topic_0108272819_p8823111311598"></a><a name="zh-cn_topic_0108272819_p8823111311598"></a>写入数据的表名。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272819_row56184745141343"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272819_p1511117156162"><a name="zh-cn_topic_0108272819_p1511117156162"></a><a name="zh-cn_topic_0108272819_p1511117156162"></a>toJobConfig.columnList</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272819_p55393515141527"><a name="zh-cn_topic_0108272819_p55393515141527"></a><a name="zh-cn_topic_0108272819_p55393515141527"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.2983701629837%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272819_p57689731141527"><a name="zh-cn_topic_0108272819_p57689731141527"></a><a name="zh-cn_topic_0108272819_p57689731141527"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.885911408859116%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272819_p42356648141527"><a name="zh-cn_topic_0108272819_p42356648141527"></a><a name="zh-cn_topic_0108272819_p42356648141527"></a>需要加载的字段列表，字段名之间使用<span class="parmvalue" id="zh-cn_topic_0108272819_parmvalue6030650210259"><a name="zh-cn_topic_0108272819_parmvalue6030650210259"></a><a name="zh-cn_topic_0108272819_parmvalue6030650210259"></a>“&amp;”</span>分割，例如：<span class="parmvalue" id="zh-cn_topic_0108272819_parmvalue292934391039"><a name="zh-cn_topic_0108272819_parmvalue292934391039"></a><a name="zh-cn_topic_0108272819_parmvalue292934391039"></a>“id&amp;gid&amp;name”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272819_row130765815412"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272819_p11817111355911"><a name="zh-cn_topic_0108272819_p11817111355911"></a><a name="zh-cn_topic_0108272819_p11817111355911"></a>toJobConfig.shouldClearTable</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272819_p17816813135917"><a name="zh-cn_topic_0108272819_p17816813135917"></a><a name="zh-cn_topic_0108272819_p17816813135917"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.2983701629837%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272819_p63440653141343"><a name="zh-cn_topic_0108272819_p63440653141343"></a><a name="zh-cn_topic_0108272819_p63440653141343"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="40.885911408859116%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272819_p98148138591"><a name="zh-cn_topic_0108272819_p98148138591"></a><a name="zh-cn_topic_0108272819_p98148138591"></a>导入前是否清空资源队列的数据。</p>
</td>
</tr>
</tbody>
</table>

