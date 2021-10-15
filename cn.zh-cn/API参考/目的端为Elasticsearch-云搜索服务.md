# 目的端为Elasticsearch/云搜索服务<a name="dgc_02_0304"></a>

## JSON样例<a name="zh-cn_topic_0108272837_section33401108172339"></a>

```
"to-config-values": {
                "configs": [
                    {
                        "inputs": [
                            {
                              "name": "toJobConfig.index",
                              "value": "cdm"
                            },
                            {
                              "name": "toJobConfig.type",
                              "value": "type1"
                            },
                            {
                              "name": "toJobConfig.shouldClearType",
                              "value": "false"
                            },
                           {
                              "name": "toJobConfig.pipeLine",
                              "value": "es_03"
                           }
                        ],
                        "name": "toJobConfig"
                    }
                ]
            }
```

## 参数说明<a name="zh-cn_topic_0108272837_section60129242115832"></a>

<a name="zh-cn_topic_0108272837_table6307873415412"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108272837_row2882542015412"><th class="cellrowborder" valign="top" width="22.657734226577343%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272837_p5315765115412"><a name="zh-cn_topic_0108272837_p5315765115412"></a><a name="zh-cn_topic_0108272837_p5315765115412"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20.157984201579843%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272837_p1080249515412"><a name="zh-cn_topic_0108272837_p1080249515412"></a><a name="zh-cn_topic_0108272837_p1080249515412"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="16.2983701629837%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272837_p258693615412"><a name="zh-cn_topic_0108272837_p258693615412"></a><a name="zh-cn_topic_0108272837_p258693615412"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="40.885911408859116%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272837_p821526915412"><a name="zh-cn_topic_0108272837_p821526915412"></a><a name="zh-cn_topic_0108272837_p821526915412"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108272837_row3532522715412"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272837_p31423427144217"><a name="zh-cn_topic_0108272837_p31423427144217"></a><a name="zh-cn_topic_0108272837_p31423427144217"></a>toJobConfig.index</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272837_p62269650144217"><a name="zh-cn_topic_0108272837_p62269650144217"></a><a name="zh-cn_topic_0108272837_p62269650144217"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.2983701629837%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272837_p10676914144217"><a name="zh-cn_topic_0108272837_p10676914144217"></a><a name="zh-cn_topic_0108272837_p10676914144217"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.885911408859116%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272837_p59523723144217"><a name="zh-cn_topic_0108272837_p59523723144217"></a><a name="zh-cn_topic_0108272837_p59523723144217"></a>写入数据的索引，类似关系数据库中的数据库名称。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272837_row2888033144824"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272837_p32604129144824"><a name="zh-cn_topic_0108272837_p32604129144824"></a><a name="zh-cn_topic_0108272837_p32604129144824"></a>toJobConfig.type</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272837_p23688773144824"><a name="zh-cn_topic_0108272837_p23688773144824"></a><a name="zh-cn_topic_0108272837_p23688773144824"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.2983701629837%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272837_p39742454144824"><a name="zh-cn_topic_0108272837_p39742454144824"></a><a name="zh-cn_topic_0108272837_p39742454144824"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.885911408859116%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272837_p65022171144824"><a name="zh-cn_topic_0108272837_p65022171144824"></a><a name="zh-cn_topic_0108272837_p65022171144824"></a>写入数据的类型，类似关系数据库中的表名。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272837_row56184745141343"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272837_p54670509141343"><a name="zh-cn_topic_0108272837_p54670509141343"></a><a name="zh-cn_topic_0108272837_p54670509141343"></a>toJobConfig.shouldClearType</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272837_p66235072141343"><a name="zh-cn_topic_0108272837_p66235072141343"></a><a name="zh-cn_topic_0108272837_p66235072141343"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.2983701629837%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272837_p63440653141343"><a name="zh-cn_topic_0108272837_p63440653141343"></a><a name="zh-cn_topic_0108272837_p63440653141343"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="40.885911408859116%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272837_p38419258141343"><a name="zh-cn_topic_0108272837_p38419258141343"></a><a name="zh-cn_topic_0108272837_p38419258141343"></a>导入前是否清除数据。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272837_row130765815412"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272837_p40468004144217"><a name="zh-cn_topic_0108272837_p40468004144217"></a><a name="zh-cn_topic_0108272837_p40468004144217"></a>toJobConfig.primaryKey</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272837_p56682864144217"><a name="zh-cn_topic_0108272837_p56682864144217"></a><a name="zh-cn_topic_0108272837_p56682864144217"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.2983701629837%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272837_p27909297144217"><a name="zh-cn_topic_0108272837_p27909297144217"></a><a name="zh-cn_topic_0108272837_p27909297144217"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.885911408859116%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272837_p18776402152853"><a name="zh-cn_topic_0108272837_p18776402152853"></a><a name="zh-cn_topic_0108272837_p18776402152853"></a>主键或唯一索引。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272837_row5037735615412"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272837_p52978520144217"><a name="zh-cn_topic_0108272837_p52978520144217"></a><a name="zh-cn_topic_0108272837_p52978520144217"></a>toJobConfig.columnList</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272837_p63401693144217"><a name="zh-cn_topic_0108272837_p63401693144217"></a><a name="zh-cn_topic_0108272837_p63401693144217"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.2983701629837%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272837_p35263486144217"><a name="zh-cn_topic_0108272837_p35263486144217"></a><a name="zh-cn_topic_0108272837_p35263486144217"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.885911408859116%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272837_p37770149144217"><a name="zh-cn_topic_0108272837_p37770149144217"></a><a name="zh-cn_topic_0108272837_p37770149144217"></a>需要写入的字段列表，字段名之间使用<span class="parmvalue" id="zh-cn_topic_0108272837_parmvalue1296851616438"><a name="zh-cn_topic_0108272837_parmvalue1296851616438"></a><a name="zh-cn_topic_0108272837_parmvalue1296851616438"></a>“&amp;”</span>分隔，例如：<span class="parmvalue" id="zh-cn_topic_0108272837_parmvalue2845770316447"><a name="zh-cn_topic_0108272837_parmvalue2845770316447"></a><a name="zh-cn_topic_0108272837_parmvalue2845770316447"></a>“id&amp;gid&amp;name”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272837_row663119528426"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272837_p26311852144211"><a name="zh-cn_topic_0108272837_p26311852144211"></a><a name="zh-cn_topic_0108272837_p26311852144211"></a>toJobConfig.pipeLine</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272837_p17631195244219"><a name="zh-cn_topic_0108272837_p17631195244219"></a><a name="zh-cn_topic_0108272837_p17631195244219"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.2983701629837%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272837_p66311752114215"><a name="zh-cn_topic_0108272837_p66311752114215"></a><a name="zh-cn_topic_0108272837_p66311752114215"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.885911408859116%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272837_p8755914553"><a name="zh-cn_topic_0108272837_p8755914553"></a><a name="zh-cn_topic_0108272837_p8755914553"></a>需要先在kibana中创建管道ID，这里才可以选择，该参数用于数据传到云搜索服务/Elasticsearch后，通过Elasticsearch的数据转换pipeline进行数据格式变换。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272837_row186852037173515"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272837_p1668573773512"><a name="zh-cn_topic_0108272837_p1668573773512"></a><a name="zh-cn_topic_0108272837_p1668573773512"></a>toJobConfig.createIndexStrategy</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272837_p468615374355"><a name="zh-cn_topic_0108272837_p468615374355"></a><a name="zh-cn_topic_0108272837_p468615374355"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.2983701629837%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272837_p1168663717353"><a name="zh-cn_topic_0108272837_p1168663717353"></a><a name="zh-cn_topic_0108272837_p1168663717353"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="40.885911408859116%" headers="mcps1.1.5.1.4 "><div class="p" id="zh-cn_topic_0108272837_p53511015420"><a name="zh-cn_topic_0108272837_p53511015420"></a><a name="zh-cn_topic_0108272837_p53511015420"></a>对于持续写入数据到Elasticsearch的流式作业，CDM支持在Elasticsearch中定时创建新索引并写入数据，方便用户后期删除过期的数据。支持按以下周期创建新索引：<a name="zh-cn_topic_0108272837_ul112848823812"></a><a name="zh-cn_topic_0108272837_ul112848823812"></a><ul id="zh-cn_topic_0108272837_ul112848823812"><li>EveryHour：每小时整点创建新索引，新索引的命名格式为<span class="parmvalue" id="zh-cn_topic_0108272837_parmvalue166091542527"><a name="zh-cn_topic_0108272837_parmvalue166091542527"></a><a name="zh-cn_topic_0108272837_parmvalue166091542527"></a>“索引名+年+月+日+小时”</span>，例如<span class="parmvalue" id="zh-cn_topic_0108272837_parmvalue97280286527"><a name="zh-cn_topic_0108272837_parmvalue97280286527"></a><a name="zh-cn_topic_0108272837_parmvalue97280286527"></a>“index2018121709”</span>。</li><li>EveryDay：每天零点零分创建新索引，新索引的命名格式为<span class="parmvalue" id="zh-cn_topic_0108272837_parmvalue13376104820546"><a name="zh-cn_topic_0108272837_parmvalue13376104820546"></a><a name="zh-cn_topic_0108272837_parmvalue13376104820546"></a>“索引名+年+月+日”</span>，例如<span class="parmvalue" id="zh-cn_topic_0108272837_parmvalue83912311554"><a name="zh-cn_topic_0108272837_parmvalue83912311554"></a><a name="zh-cn_topic_0108272837_parmvalue83912311554"></a>“index20181217”</span>。</li><li>EveryWeek：每周周一的零点零分创建新索引，新索引的命名格式为<span class="parmvalue" id="zh-cn_topic_0108272837_parmvalue125511630145612"><a name="zh-cn_topic_0108272837_parmvalue125511630145612"></a><a name="zh-cn_topic_0108272837_parmvalue125511630145612"></a>“索引名+年+周”</span>，例如<span class="parmvalue" id="zh-cn_topic_0108272837_parmvalue19461055135616"><a name="zh-cn_topic_0108272837_parmvalue19461055135616"></a><a name="zh-cn_topic_0108272837_parmvalue19461055135616"></a>“index201842”</span>。</li><li>EveryMonth：每月一号零点零分创建新索引，新索引的命名格式为<span class="parmvalue" id="zh-cn_topic_0108272837_parmvalue5856103018585"><a name="zh-cn_topic_0108272837_parmvalue5856103018585"></a><a name="zh-cn_topic_0108272837_parmvalue5856103018585"></a>“索引名+年+月”</span>，例如<span class="parmvalue" id="zh-cn_topic_0108272837_parmvalue43841656105818"><a name="zh-cn_topic_0108272837_parmvalue43841656105818"></a><a name="zh-cn_topic_0108272837_parmvalue43841656105818"></a>“index201812”</span>。</li></ul>
</div>
<p id="zh-cn_topic_0108272837_p837316411590"><a name="zh-cn_topic_0108272837_p837316411590"></a><a name="zh-cn_topic_0108272837_p837316411590"></a>从文件类抽取数据时，必须配置单个抽取（<span class="parmname" id="zh-cn_topic_0108272837_parmname51503147198"><a name="zh-cn_topic_0108272837_parmname51503147198"></a><a name="zh-cn_topic_0108272837_parmname51503147198"></a>“抽取并发数”</span>参数配置为1），否则该参数无效。</p>
</td>
</tr>
</tbody>
</table>

