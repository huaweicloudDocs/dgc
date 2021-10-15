# 源端为Elasticsearch/云搜索服务<a name="dgc_02_0293"></a>

## JSON样例<a name="zh-cn_topic_0108272828_section33401108172339"></a>

```
"from-config-values": {
                "configs": [
                    {
                        "inputs": [
                            {
                                "name": "fromJobConfig.index",
                                "value": "cdm"
                            },
                            {
                                "name": "fromJobConfig.type",
                                "value": "es"
                            },
                            {
                                "name": "fromJobConfig.columnList",
                                "value": "a1:numeric&s1:string"
                            },
                           {
                               "name": "fromJobConfig.splitNestedField",
                               "value": "true"
                           },
                           {
                               "name": "fromJobConfig.queryString",
                               "value": "last_name:Smith"
                           }
                        ],
                        "name": "fromJobConfig"
                    }
                ]
            }
```

## 参数说明<a name="zh-cn_topic_0108272828_section61808073174843"></a>

<a name="zh-cn_topic_0108272828_table6307873415412"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108272828_row2882542015412"><th class="cellrowborder" valign="top" width="22.657734226577343%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272828_p5315765115412"><a name="zh-cn_topic_0108272828_p5315765115412"></a><a name="zh-cn_topic_0108272828_p5315765115412"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20.157984201579843%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272828_p1080249515412"><a name="zh-cn_topic_0108272828_p1080249515412"></a><a name="zh-cn_topic_0108272828_p1080249515412"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="16.2983701629837%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272828_p258693615412"><a name="zh-cn_topic_0108272828_p258693615412"></a><a name="zh-cn_topic_0108272828_p258693615412"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="40.885911408859116%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272828_p821526915412"><a name="zh-cn_topic_0108272828_p821526915412"></a><a name="zh-cn_topic_0108272828_p821526915412"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108272828_row3532522715412"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272828_p31423427144217"><a name="zh-cn_topic_0108272828_p31423427144217"></a><a name="zh-cn_topic_0108272828_p31423427144217"></a>fromJobConfig.index</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272828_p62269650144217"><a name="zh-cn_topic_0108272828_p62269650144217"></a><a name="zh-cn_topic_0108272828_p62269650144217"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.2983701629837%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272828_p10676914144217"><a name="zh-cn_topic_0108272828_p10676914144217"></a><a name="zh-cn_topic_0108272828_p10676914144217"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.885911408859116%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272828_p59523723144217"><a name="zh-cn_topic_0108272828_p59523723144217"></a><a name="zh-cn_topic_0108272828_p59523723144217"></a>抽取数据的索引，类似关系数据库中的数据库名称。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272828_row2888033144824"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272828_p32604129144824"><a name="zh-cn_topic_0108272828_p32604129144824"></a><a name="zh-cn_topic_0108272828_p32604129144824"></a>fromJobConfig.type</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272828_p23688773144824"><a name="zh-cn_topic_0108272828_p23688773144824"></a><a name="zh-cn_topic_0108272828_p23688773144824"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.2983701629837%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272828_p39742454144824"><a name="zh-cn_topic_0108272828_p39742454144824"></a><a name="zh-cn_topic_0108272828_p39742454144824"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.885911408859116%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272828_p65022171144824"><a name="zh-cn_topic_0108272828_p65022171144824"></a><a name="zh-cn_topic_0108272828_p65022171144824"></a>抽取数据的类型，类似关系数据库中的表名。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272828_row5037735615412"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272828_p52978520144217"><a name="zh-cn_topic_0108272828_p52978520144217"></a><a name="zh-cn_topic_0108272828_p52978520144217"></a>fromJobConfig.columnList</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272828_p63401693144217"><a name="zh-cn_topic_0108272828_p63401693144217"></a><a name="zh-cn_topic_0108272828_p63401693144217"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.2983701629837%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272828_p35263486144217"><a name="zh-cn_topic_0108272828_p35263486144217"></a><a name="zh-cn_topic_0108272828_p35263486144217"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.885911408859116%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272828_p37770149144217"><a name="zh-cn_topic_0108272828_p37770149144217"></a><a name="zh-cn_topic_0108272828_p37770149144217"></a>需要抽取的字段列表，字段名之间使用<span class="parmvalue" id="zh-cn_topic_0108272828_parmvalue1296851616438"><a name="zh-cn_topic_0108272828_parmvalue1296851616438"></a><a name="zh-cn_topic_0108272828_parmvalue1296851616438"></a>“&amp;”</span>分隔，例如：<span class="parmvalue" id="zh-cn_topic_0108272828_parmvalue2845770316447"><a name="zh-cn_topic_0108272828_parmvalue2845770316447"></a><a name="zh-cn_topic_0108272828_parmvalue2845770316447"></a>“id&amp;gid&amp;name”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272828_row1583494418571"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272828_p16834174416571"><a name="zh-cn_topic_0108272828_p16834174416571"></a><a name="zh-cn_topic_0108272828_p16834174416571"></a>fromJobConfig.splitNestedField</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272828_p883484425711"><a name="zh-cn_topic_0108272828_p883484425711"></a><a name="zh-cn_topic_0108272828_p883484425711"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.2983701629837%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272828_p8057768172040"><a name="zh-cn_topic_0108272828_p8057768172040"></a><a name="zh-cn_topic_0108272828_p8057768172040"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="40.885911408859116%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272828_p9286172411394"><a name="zh-cn_topic_0108272828_p9286172411394"></a><a name="zh-cn_topic_0108272828_p9286172411394"></a>选择是否将nested字段的json内容拆分，例如：将<span class="uicontrol" id="zh-cn_topic_0108272828_uicontrol2957184253017"><a name="zh-cn_topic_0108272828_uicontrol2957184253017"></a><a name="zh-cn_topic_0108272828_uicontrol2957184253017"></a>“a:{ b:{ c:1, d:{ e:2, f:3 } } }”</span> 拆成三个字段<span class="uicontrol" id="zh-cn_topic_0108272828_uicontrol139867186304"><a name="zh-cn_topic_0108272828_uicontrol139867186304"></a><a name="zh-cn_topic_0108272828_uicontrol139867186304"></a>“a.b.c”</span>、<span class="uicontrol" id="zh-cn_topic_0108272828_uicontrol62201525173012"><a name="zh-cn_topic_0108272828_uicontrol62201525173012"></a><a name="zh-cn_topic_0108272828_uicontrol62201525173012"></a>“a.b.d.e”</span>、<span class="uicontrol" id="zh-cn_topic_0108272828_uicontrol6379733173013"><a name="zh-cn_topic_0108272828_uicontrol6379733173013"></a><a name="zh-cn_topic_0108272828_uicontrol6379733173013"></a>“a.b.d.f”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272828_row135064715715"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272828_p1235024712574"><a name="zh-cn_topic_0108272828_p1235024712574"></a><a name="zh-cn_topic_0108272828_p1235024712574"></a>fromJobConfig.queryString</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272828_p2035074705717"><a name="zh-cn_topic_0108272828_p2035074705717"></a><a name="zh-cn_topic_0108272828_p2035074705717"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.2983701629837%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272828_p13400129013"><a name="zh-cn_topic_0108272828_p13400129013"></a><a name="zh-cn_topic_0108272828_p13400129013"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.885911408859116%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272828_p16865173219416"><a name="zh-cn_topic_0108272828_p16865173219416"></a><a name="zh-cn_topic_0108272828_p16865173219416"></a>使用Elasticsearch的查询字符串（query string）对源数据进行过滤，CDM只迁移满足过滤条件的数据。</p>
</td>
</tr>
</tbody>
</table>

