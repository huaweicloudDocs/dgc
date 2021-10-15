# 源端为Hive<a name="dgc_02_0285"></a>

## JSON样例<a name="zh-cn_topic_0108272811_section33401108172339"></a>

```
"from-config-values": {
        "configs": [
          {
            "inputs": [
              {
                "name": "fromJobConfig.hive",
                "value": "hive"
              },
              {
                "name": "fromJobConfig.database",
                "value": "rf_database"
              },
              {
                "name": "fromJobConfig.table",
                "value": "rf_from"
              },
              {
                "name": "fromJobConfig.columnList",
                "value": "tiny&small&int&integer&bigint&float&double&timestamp&char&varchar&text"
              }
            ],
            "name": "fromJobConfig"
          }
        ]
      }
```

## 参数说明<a name="zh-cn_topic_0108272811_section25035823174041"></a>

<a name="zh-cn_topic_0108272811_table13922888141527"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108272811_row229143141527"><th class="cellrowborder" valign="top" width="19.838016198380164%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272811_p66756185141527"><a name="zh-cn_topic_0108272811_p66756185141527"></a><a name="zh-cn_topic_0108272811_p66756185141527"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20.34796520347965%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272811_p38541938141527"><a name="zh-cn_topic_0108272811_p38541938141527"></a><a name="zh-cn_topic_0108272811_p38541938141527"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.23827617238276%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272811_p34889279141527"><a name="zh-cn_topic_0108272811_p34889279141527"></a><a name="zh-cn_topic_0108272811_p34889279141527"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.575742425757426%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272811_p7459369141527"><a name="zh-cn_topic_0108272811_p7459369141527"></a><a name="zh-cn_topic_0108272811_p7459369141527"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108272811_row13229168113111"><td class="cellrowborder" valign="top" width="19.838016198380164%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272811_p132294883119"><a name="zh-cn_topic_0108272811_p132294883119"></a><a name="zh-cn_topic_0108272811_p132294883119"></a>fromJobConfig.hive</p>
</td>
<td class="cellrowborder" valign="top" width="20.34796520347965%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272811_p32298823113"><a name="zh-cn_topic_0108272811_p32298823113"></a><a name="zh-cn_topic_0108272811_p32298823113"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272811_p1822998203118"><a name="zh-cn_topic_0108272811_p1822998203118"></a><a name="zh-cn_topic_0108272811_p1822998203118"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.575742425757426%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272811_p162292089316"><a name="zh-cn_topic_0108272811_p162292089316"></a><a name="zh-cn_topic_0108272811_p162292089316"></a>待抽取数据的数据源，作业源端为Hive时，这里为<span class="parmvalue" id="zh-cn_topic_0108272811_parmvalue47081639143316"><a name="zh-cn_topic_0108272811_parmvalue47081639143316"></a><a name="zh-cn_topic_0108272811_parmvalue47081639143316"></a>“hive”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272811_row62628929141527"><td class="cellrowborder" valign="top" width="19.838016198380164%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272811_p18560626141527"><a name="zh-cn_topic_0108272811_p18560626141527"></a><a name="zh-cn_topic_0108272811_p18560626141527"></a>fromJobConfig.database</p>
</td>
<td class="cellrowborder" valign="top" width="20.34796520347965%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272811_p27015713141527"><a name="zh-cn_topic_0108272811_p27015713141527"></a><a name="zh-cn_topic_0108272811_p27015713141527"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272811_p50167516142856"><a name="zh-cn_topic_0108272811_p50167516142856"></a><a name="zh-cn_topic_0108272811_p50167516142856"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.575742425757426%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272811_p2430205141527"><a name="zh-cn_topic_0108272811_p2430205141527"></a><a name="zh-cn_topic_0108272811_p2430205141527"></a>待抽取数据的数据库，例如<span class="parmvalue" id="zh-cn_topic_0108272811_parmvalue5577088394823"><a name="zh-cn_topic_0108272811_parmvalue5577088394823"></a><a name="zh-cn_topic_0108272811_parmvalue5577088394823"></a>“default”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272811_row42094113141527"><td class="cellrowborder" valign="top" width="19.838016198380164%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272811_p26789449141527"><a name="zh-cn_topic_0108272811_p26789449141527"></a><a name="zh-cn_topic_0108272811_p26789449141527"></a>fromJobConfig.table</p>
</td>
<td class="cellrowborder" valign="top" width="20.34796520347965%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272811_p22461756141527"><a name="zh-cn_topic_0108272811_p22461756141527"></a><a name="zh-cn_topic_0108272811_p22461756141527"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272811_p7462956141527"><a name="zh-cn_topic_0108272811_p7462956141527"></a><a name="zh-cn_topic_0108272811_p7462956141527"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.575742425757426%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272811_p519680141527"><a name="zh-cn_topic_0108272811_p519680141527"></a><a name="zh-cn_topic_0108272811_p519680141527"></a>待抽取数据的表名，例如<span class="parmvalue" id="zh-cn_topic_0108272811_parmvalue43340352155026"><a name="zh-cn_topic_0108272811_parmvalue43340352155026"></a><a name="zh-cn_topic_0108272811_parmvalue43340352155026"></a>“cdm”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272811_row756089319291"><td class="cellrowborder" valign="top" width="19.838016198380164%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272811_p845261719291"><a name="zh-cn_topic_0108272811_p845261719291"></a><a name="zh-cn_topic_0108272811_p845261719291"></a>fromJobConfig.columnList</p>
</td>
<td class="cellrowborder" valign="top" width="20.34796520347965%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272811_p55393515141527"><a name="zh-cn_topic_0108272811_p55393515141527"></a><a name="zh-cn_topic_0108272811_p55393515141527"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272811_p57689731141527"><a name="zh-cn_topic_0108272811_p57689731141527"></a><a name="zh-cn_topic_0108272811_p57689731141527"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.575742425757426%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272811_p37985002193940"><a name="zh-cn_topic_0108272811_p37985002193940"></a><a name="zh-cn_topic_0108272811_p37985002193940"></a>需要抽取的列号，列号之间使用<span class="parmvalue" id="zh-cn_topic_0108272811_zh-cn_topic_0108272831_parmvalue36226019586"><a name="zh-cn_topic_0108272811_zh-cn_topic_0108272831_parmvalue36226019586"></a><a name="zh-cn_topic_0108272811_zh-cn_topic_0108272831_parmvalue36226019586"></a>“&amp;”</span>分割，并由小到大排序，例如：<span class="parmvalue" id="zh-cn_topic_0108272811_zh-cn_topic_0108272831_parmvalue6416671195818"><a name="zh-cn_topic_0108272811_zh-cn_topic_0108272831_parmvalue6416671195818"></a><a name="zh-cn_topic_0108272811_zh-cn_topic_0108272831_parmvalue6416671195818"></a>“1&amp;3&amp;5”</span>。</p>
</td>
</tr>
</tbody>
</table>

