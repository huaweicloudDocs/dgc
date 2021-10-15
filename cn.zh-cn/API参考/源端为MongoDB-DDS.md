# 源端为MongoDB/DDS<a name="dgc_02_0289"></a>

## JSON样例<a name="zh-cn_topic_0108272801_section33401108172339"></a>

```
"from-config-values": {
        "configs": [
          {
            "inputs": [
              {
                "name": "fromJobConfig.database",
                "value": "cdm"
              },
              {
                "name": "fromJobConfig.collectionName",
                "value": "rf_from"
              },
              {
                "name": "fromJobConfig.columnList",
                "value": "TINYTEST&SMALLTEST&INTTEST&INTEGERTEST&BIGINTTEST&FLOATTEST"
              },
              {
                "name": "fromJobConfig.isBatchMigration",
                "value": "false"
              },
              {
                "name": "fromJobConfig.filters",
                "value": "{'last_name': 'Smith'}"
              }
            ],
            "name": "fromJobConfig"
          }
        ]
      }
```

## 参数说明<a name="zh-cn_topic_0108272801_section57802592174657"></a>

<a name="zh-cn_topic_0108272801_table13922888141527"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108272801_row229143141527"><th class="cellrowborder" valign="top" width="22.66%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272801_p66756185141527"><a name="zh-cn_topic_0108272801_p66756185141527"></a><a name="zh-cn_topic_0108272801_p66756185141527"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="19.78%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272801_p38541938141527"><a name="zh-cn_topic_0108272801_p38541938141527"></a><a name="zh-cn_topic_0108272801_p38541938141527"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.05%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272801_p34889279141527"><a name="zh-cn_topic_0108272801_p34889279141527"></a><a name="zh-cn_topic_0108272801_p34889279141527"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="40.510000000000005%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272801_p7459369141527"><a name="zh-cn_topic_0108272801_p7459369141527"></a><a name="zh-cn_topic_0108272801_p7459369141527"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108272801_row353218783220"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272801_p175321273324"><a name="zh-cn_topic_0108272801_p175321273324"></a><a name="zh-cn_topic_0108272801_p175321273324"></a>fromJobConfig.database</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272801_p1753267183217"><a name="zh-cn_topic_0108272801_p1753267183217"></a><a name="zh-cn_topic_0108272801_p1753267183217"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272801_p2691102813354"><a name="zh-cn_topic_0108272801_p2691102813354"></a><a name="zh-cn_topic_0108272801_p2691102813354"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272801_p1053219733211"><a name="zh-cn_topic_0108272801_p1053219733211"></a><a name="zh-cn_topic_0108272801_p1053219733211"></a>MongoDB/DDS的数据库名称。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272801_row62628929141527"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272801_p9831304162518"><a name="zh-cn_topic_0108272801_p9831304162518"></a><a name="zh-cn_topic_0108272801_p9831304162518"></a>fromJobConfig.collectionName</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272801_p33528469162518"><a name="zh-cn_topic_0108272801_p33528469162518"></a><a name="zh-cn_topic_0108272801_p33528469162518"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272801_p30716554162817"><a name="zh-cn_topic_0108272801_p30716554162817"></a><a name="zh-cn_topic_0108272801_p30716554162817"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272801_p32355904162824"><a name="zh-cn_topic_0108272801_p32355904162824"></a><a name="zh-cn_topic_0108272801_p32355904162824"></a>MongoDB/DDS的集合名称。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272801_row42094113141527"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272801_p34470963162721"><a name="zh-cn_topic_0108272801_p34470963162721"></a><a name="zh-cn_topic_0108272801_p34470963162721"></a>fromJobConfig.columnList</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272801_p40684644162721"><a name="zh-cn_topic_0108272801_p40684644162721"></a><a name="zh-cn_topic_0108272801_p40684644162721"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272801_p7121906162721"><a name="zh-cn_topic_0108272801_p7121906162721"></a><a name="zh-cn_topic_0108272801_p7121906162721"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272801_p40003524162721"><a name="zh-cn_topic_0108272801_p40003524162721"></a><a name="zh-cn_topic_0108272801_p40003524162721"></a>需要抽取的字段列表，字段名之间使用<span class="parmvalue" id="zh-cn_topic_0108272801_parmvalue24487403162721"><a name="zh-cn_topic_0108272801_parmvalue24487403162721"></a><a name="zh-cn_topic_0108272801_parmvalue24487403162721"></a>“&amp;”</span>分割，例如：<span class="parmvalue" id="zh-cn_topic_0108272801_parmvalue19060035162721"><a name="zh-cn_topic_0108272801_parmvalue19060035162721"></a><a name="zh-cn_topic_0108272801_parmvalue19060035162721"></a>“id&amp;gid&amp;name”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272801_row19544111519403"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272801_p17544111514014"><a name="zh-cn_topic_0108272801_p17544111514014"></a><a name="zh-cn_topic_0108272801_p17544111514014"></a>fromJobConfig.isBatchMigration</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272801_p6544515104010"><a name="zh-cn_topic_0108272801_p6544515104010"></a><a name="zh-cn_topic_0108272801_p6544515104010"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272801_p854416152400"><a name="zh-cn_topic_0108272801_p854416152400"></a><a name="zh-cn_topic_0108272801_p854416152400"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272801_p954491510403"><a name="zh-cn_topic_0108272801_p954491510403"></a><a name="zh-cn_topic_0108272801_p954491510403"></a>是否为整库迁移。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272801_row1558641518358"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272801_p1158861563517"><a name="zh-cn_topic_0108272801_p1158861563517"></a><a name="zh-cn_topic_0108272801_p1158861563517"></a>fromJobConfig.filters</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272801_p175881415123511"><a name="zh-cn_topic_0108272801_p175881415123511"></a><a name="zh-cn_topic_0108272801_p175881415123511"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272801_p14588191510356"><a name="zh-cn_topic_0108272801_p14588191510356"></a><a name="zh-cn_topic_0108272801_p14588191510356"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><div class="p" id="zh-cn_topic_0108272801_p241710321259"><a name="zh-cn_topic_0108272801_p241710321259"></a><a name="zh-cn_topic_0108272801_p241710321259"></a>创建用于匹配文档的筛选条件，CDM只迁移符合条件的数据。例如：<a name="zh-cn_topic_0108272801_ol6793125415558"></a><a name="zh-cn_topic_0108272801_ol6793125415558"></a><ol id="zh-cn_topic_0108272801_ol6793125415558"><li>按表达式对象筛选：例如{'last_name': 'Smith'}，表示查找所有<span class="parmname" id="zh-cn_topic_0108272801_parmname0657201595916"><a name="zh-cn_topic_0108272801_parmname0657201595916"></a><a name="zh-cn_topic_0108272801_parmname0657201595916"></a>“last_name”</span>属性值为<span class="parmvalue" id="zh-cn_topic_0108272801_parmvalue21701627155916"><a name="zh-cn_topic_0108272801_parmvalue21701627155916"></a><a name="zh-cn_topic_0108272801_parmvalue21701627155916"></a>“Smith”</span>的文档。</li><li>按参数选项筛选：例如{ x : "john" }, { z : 1 }，表示查找x=john的所有z字段。</li><li>按条件筛选：例如{ "field" : { $gt: 5 } }，表示查找field字段中大于5的值。</li></ol>
</div>
</td>
</tr>
</tbody>
</table>

