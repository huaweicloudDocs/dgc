# 目的端为Hive<a name="dgc_02_0299"></a>

## JSON样例<a name="zh-cn_topic_0108272785_section33401108172339"></a>

```
"to-config-values": {
        "configs": [
          {
            "inputs": [
              {
                "name": "toJobConfig.hive",
                "value": "hive"
              },
              {
                "name": "toJobConfig.database",
                "value": "rf_database"
              },
              {
                "name": "toJobConfig.table",
                "value": "rf_to"
              },
              {
                "name": "toJobConfig.tablePreparation",
                "value": "DO_NOTHING"
              },
              {
                "name": "toJobConfig.columnList",
                "value": "aa&bb&cc&dd"
              },
              {
                "name": "toJobConfig.shouldClearTable",
                "value": "true"
              }
            ],
            "name": "toJobConfig"
          }
        ]
      }
```

## 参数说明<a name="zh-cn_topic_0108272785_section4352042310388"></a>

<a name="zh-cn_topic_0108272785_table13922888141527"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108272785_row229143141527"><th class="cellrowborder" valign="top" width="20.78%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272785_p66756185141527"><a name="zh-cn_topic_0108272785_p66756185141527"></a><a name="zh-cn_topic_0108272785_p66756185141527"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20.72%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272785_p38541938141527"><a name="zh-cn_topic_0108272785_p38541938141527"></a><a name="zh-cn_topic_0108272785_p38541938141527"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="19.68%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272785_p34889279141527"><a name="zh-cn_topic_0108272785_p34889279141527"></a><a name="zh-cn_topic_0108272785_p34889279141527"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="38.82%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272785_p7459369141527"><a name="zh-cn_topic_0108272785_p7459369141527"></a><a name="zh-cn_topic_0108272785_p7459369141527"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108272785_row1610024133611"><td class="cellrowborder" valign="top" width="20.78%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272785_p6100349368"><a name="zh-cn_topic_0108272785_p6100349368"></a><a name="zh-cn_topic_0108272785_p6100349368"></a>toJobConfig.hive</p>
</td>
<td class="cellrowborder" valign="top" width="20.72%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272785_p171001348369"><a name="zh-cn_topic_0108272785_p171001348369"></a><a name="zh-cn_topic_0108272785_p171001348369"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.68%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272785_p61009423615"><a name="zh-cn_topic_0108272785_p61009423615"></a><a name="zh-cn_topic_0108272785_p61009423615"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.82%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272785_p91006483617"><a name="zh-cn_topic_0108272785_p91006483617"></a><a name="zh-cn_topic_0108272785_p91006483617"></a>写入数据的数据源。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272785_row62628929141527"><td class="cellrowborder" valign="top" width="20.78%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272785_p5713207712229"><a name="zh-cn_topic_0108272785_p5713207712229"></a><a name="zh-cn_topic_0108272785_p5713207712229"></a>toJobConfig.database</p>
</td>
<td class="cellrowborder" valign="top" width="20.72%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272785_p6429552912229"><a name="zh-cn_topic_0108272785_p6429552912229"></a><a name="zh-cn_topic_0108272785_p6429552912229"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.68%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272785_p4055535712229"><a name="zh-cn_topic_0108272785_p4055535712229"></a><a name="zh-cn_topic_0108272785_p4055535712229"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.82%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272785_p6375851412229"><a name="zh-cn_topic_0108272785_p6375851412229"></a><a name="zh-cn_topic_0108272785_p6375851412229"></a>写入数据的数据库名称，例如：<span class="parmvalue" id="zh-cn_topic_0108272785_parmvalue6167159810621"><a name="zh-cn_topic_0108272785_parmvalue6167159810621"></a><a name="zh-cn_topic_0108272785_parmvalue6167159810621"></a>“default”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272785_row42094113141527"><td class="cellrowborder" valign="top" width="20.78%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272785_p4062337712229"><a name="zh-cn_topic_0108272785_p4062337712229"></a><a name="zh-cn_topic_0108272785_p4062337712229"></a>toJobConfig.table</p>
</td>
<td class="cellrowborder" valign="top" width="20.72%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272785_p215924612229"><a name="zh-cn_topic_0108272785_p215924612229"></a><a name="zh-cn_topic_0108272785_p215924612229"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.68%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272785_p4068125612229"><a name="zh-cn_topic_0108272785_p4068125612229"></a><a name="zh-cn_topic_0108272785_p4068125612229"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.82%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272785_p684743012229"><a name="zh-cn_topic_0108272785_p684743012229"></a><a name="zh-cn_topic_0108272785_p684743012229"></a>写入数据的表名。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272785_row3293911421"><td class="cellrowborder" valign="top" width="20.78%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272785_p132917924210"><a name="zh-cn_topic_0108272785_p132917924210"></a><a name="zh-cn_topic_0108272785_p132917924210"></a>toJobConfig.tablePreparation</p>
</td>
<td class="cellrowborder" valign="top" width="20.72%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272785_p510510189594"><a name="zh-cn_topic_0108272785_p510510189594"></a><a name="zh-cn_topic_0108272785_p510510189594"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.68%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272785_p414918119594"><a name="zh-cn_topic_0108272785_p414918119594"></a><a name="zh-cn_topic_0108272785_p414918119594"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="38.82%" headers="mcps1.1.5.1.4 "><div class="p" id="zh-cn_topic_0108272785_p2035898817235"><a name="zh-cn_topic_0108272785_p2035898817235"></a><a name="zh-cn_topic_0108272785_p2035898817235"></a>写入表数据时，用户选择的操作：<a name="zh-cn_topic_0108272785_ul12109569172733"></a><a name="zh-cn_topic_0108272785_ul12109569172733"></a><ul id="zh-cn_topic_0108272785_ul12109569172733"><li>DO_NOTHING：不自动建表。</li><li>CREATE_WHEN_NOT_EXIST：当目的端的数据库没有<span class="parmname" id="zh-cn_topic_0108272785_parmname42948736113514"><a name="zh-cn_topic_0108272785_parmname42948736113514"></a><a name="zh-cn_topic_0108272785_parmname42948736113514"></a>“tableName”</span>参数中指定的表时，CDM会自动创建该表。</li><li>DROP_AND_CREATE：先删除<span class="parmname" id="zh-cn_topic_0108272785_parmname55972483114928"><a name="zh-cn_topic_0108272785_parmname55972483114928"></a><a name="zh-cn_topic_0108272785_parmname55972483114928"></a>“tableName”</span>参数中指定的表，然后再重新创建该表。</li></ul>
</div>
</td>
</tr>
<tr id="zh-cn_topic_0108272785_row183798934210"><td class="cellrowborder" valign="top" width="20.78%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272785_p173796944218"><a name="zh-cn_topic_0108272785_p173796944218"></a><a name="zh-cn_topic_0108272785_p173796944218"></a>toJobConfig.columnList</p>
</td>
<td class="cellrowborder" valign="top" width="20.72%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272785_p55393515141527"><a name="zh-cn_topic_0108272785_p55393515141527"></a><a name="zh-cn_topic_0108272785_p55393515141527"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.68%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272785_p57689731141527"><a name="zh-cn_topic_0108272785_p57689731141527"></a><a name="zh-cn_topic_0108272785_p57689731141527"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.82%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272785_p42356648141527"><a name="zh-cn_topic_0108272785_p42356648141527"></a><a name="zh-cn_topic_0108272785_p42356648141527"></a>需要加载的字段列表，字段名之间使用<span class="parmvalue" id="zh-cn_topic_0108272785_parmvalue6030650210259"><a name="zh-cn_topic_0108272785_parmvalue6030650210259"></a><a name="zh-cn_topic_0108272785_parmvalue6030650210259"></a>“&amp;”</span>分割，例如：<span class="parmvalue" id="zh-cn_topic_0108272785_parmvalue292934391039"><a name="zh-cn_topic_0108272785_parmvalue292934391039"></a><a name="zh-cn_topic_0108272785_parmvalue292934391039"></a>“id&amp;gid&amp;name”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272785_row37521698421"><td class="cellrowborder" valign="top" width="20.78%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272785_p13752179174217"><a name="zh-cn_topic_0108272785_p13752179174217"></a><a name="zh-cn_topic_0108272785_p13752179174217"></a>toJobConfig.shouldClearTable</p>
</td>
<td class="cellrowborder" valign="top" width="20.72%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272785_p574414144219"><a name="zh-cn_topic_0108272785_p574414144219"></a><a name="zh-cn_topic_0108272785_p574414144219"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.68%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272785_p11745113421"><a name="zh-cn_topic_0108272785_p11745113421"></a><a name="zh-cn_topic_0108272785_p11745113421"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="38.82%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272785_p1175289144212"><a name="zh-cn_topic_0108272785_p1175289144212"></a><a name="zh-cn_topic_0108272785_p1175289144212"></a>导入前是否清空目标表的数据，如果设置为true，任务启动前会清除目标表中数据。</p>
</td>
</tr>
</tbody>
</table>

