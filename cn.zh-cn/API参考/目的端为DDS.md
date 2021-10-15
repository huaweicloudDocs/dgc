# 目的端为DDS<a name="dgc_02_0302"></a>

## JSON样例<a name="zh-cn_topic_0109634482_section33401108172339"></a>

```
"to-config-values": {
        "configs": [
          {
            "inputs": [
              {
                "name": "toJobConfig.database",
                "value": "demo"
              },
              {
                "name": "toJobConfig.collectionName",
                "value": "cdmbase"
              },
              {
                "name": "toJobConfig.columnList",
                "value": "_char&_varchar"
              },
              {
                "name": "toJobConfig.isBatchMigration",
                "value": "false"
              }
            ],
            "name": "toJobConfig"
          }
        ]
      }
```

## 参数说明<a name="zh-cn_topic_0109634482_section57802592174657"></a>

<a name="zh-cn_topic_0109634482_table13922888141527"></a>
<table><thead align="left"><tr id="zh-cn_topic_0109634482_row229143141527"><th class="cellrowborder" valign="top" width="22.66%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0109634482_p66756185141527"><a name="zh-cn_topic_0109634482_p66756185141527"></a><a name="zh-cn_topic_0109634482_p66756185141527"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="19.78%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0109634482_p38541938141527"><a name="zh-cn_topic_0109634482_p38541938141527"></a><a name="zh-cn_topic_0109634482_p38541938141527"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.05%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0109634482_p34889279141527"><a name="zh-cn_topic_0109634482_p34889279141527"></a><a name="zh-cn_topic_0109634482_p34889279141527"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="40.510000000000005%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0109634482_p7459369141527"><a name="zh-cn_topic_0109634482_p7459369141527"></a><a name="zh-cn_topic_0109634482_p7459369141527"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0109634482_row1471914424273"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0109634482_p137193425272"><a name="zh-cn_topic_0109634482_p137193425272"></a><a name="zh-cn_topic_0109634482_p137193425272"></a>toJobConfig.database</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0109634482_p18719154202716"><a name="zh-cn_topic_0109634482_p18719154202716"></a><a name="zh-cn_topic_0109634482_p18719154202716"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0109634482_p671914272717"><a name="zh-cn_topic_0109634482_p671914272717"></a><a name="zh-cn_topic_0109634482_p671914272717"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0109634482_p18719342172710"><a name="zh-cn_topic_0109634482_p18719342172710"></a><a name="zh-cn_topic_0109634482_p18719342172710"></a>MongoDB/DDS的数据库名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0109634482_row62628929141527"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0109634482_p1931090288"><a name="zh-cn_topic_0109634482_p1931090288"></a><a name="zh-cn_topic_0109634482_p1931090288"></a>toJobConfig.collectionName</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0109634482_p33528469162518"><a name="zh-cn_topic_0109634482_p33528469162518"></a><a name="zh-cn_topic_0109634482_p33528469162518"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0109634482_p30716554162817"><a name="zh-cn_topic_0109634482_p30716554162817"></a><a name="zh-cn_topic_0109634482_p30716554162817"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0109634482_p32355904162824"><a name="zh-cn_topic_0109634482_p32355904162824"></a><a name="zh-cn_topic_0109634482_p32355904162824"></a>MongoDB/DDS的集合名称。</p>
</td>
</tr>
<tr id="zh-cn_topic_0109634482_row42094113141527"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0109634482_p34470963162721"><a name="zh-cn_topic_0109634482_p34470963162721"></a><a name="zh-cn_topic_0109634482_p34470963162721"></a>toJobConfig.columnList</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0109634482_p40684644162721"><a name="zh-cn_topic_0109634482_p40684644162721"></a><a name="zh-cn_topic_0109634482_p40684644162721"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0109634482_p7121906162721"><a name="zh-cn_topic_0109634482_p7121906162721"></a><a name="zh-cn_topic_0109634482_p7121906162721"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0109634482_p40003524162721"><a name="zh-cn_topic_0109634482_p40003524162721"></a><a name="zh-cn_topic_0109634482_p40003524162721"></a>需要抽取的字段列表，字段名之间使用<span class="parmvalue" id="zh-cn_topic_0109634482_parmvalue24487403162721"><a name="zh-cn_topic_0109634482_parmvalue24487403162721"></a><a name="zh-cn_topic_0109634482_parmvalue24487403162721"></a>“&amp;”</span>分割，例如：<span class="parmvalue" id="zh-cn_topic_0109634482_parmvalue19060035162721"><a name="zh-cn_topic_0109634482_parmvalue19060035162721"></a><a name="zh-cn_topic_0109634482_parmvalue19060035162721"></a>“id&amp;gid&amp;name”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0109634482_row151561934172815"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0109634482_p1156133412285"><a name="zh-cn_topic_0109634482_p1156133412285"></a><a name="zh-cn_topic_0109634482_p1156133412285"></a>toJobConfig.isBatchMigration</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0109634482_p815603432814"><a name="zh-cn_topic_0109634482_p815603432814"></a><a name="zh-cn_topic_0109634482_p815603432814"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0109634482_p1815633414289"><a name="zh-cn_topic_0109634482_p1815633414289"></a><a name="zh-cn_topic_0109634482_p1815633414289"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0109634482_p015603432814"><a name="zh-cn_topic_0109634482_p015603432814"></a><a name="zh-cn_topic_0109634482_p015603432814"></a>是否为整库迁移。</p>
</td>
</tr>
</tbody>
</table>

