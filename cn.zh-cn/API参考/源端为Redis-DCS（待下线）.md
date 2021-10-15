# 源端为Redis/DCS（待下线）<a name="dgc_02_0290"></a>

## JSON样例<a name="zh-cn_topic_0108272845_section33401108172339"></a>

```
"from-config-values": {
        "configs": [
          {
            "inputs": [
              {
                "name": "fromJobConfig.isBatchMigration",
                "value": "false"
              },
              {
                "name": "fromJobConfig.keyPrefix",
                "value": "rf_string_from"
              },
              {
                "name": "fromJobConfig.keySeparator",
                "value": ":"
              },
              {
                "name": "fromJobConfig.valueStoreType",
                "value": "STRING"
              },
              {
                "name": "fromJobConfig.valueSeparator",
                "value": ","
              },
              {
                "name": "fromJobConfig.columnList",
                "value": "1&2&3&4&5&6&7&8&9&10&11&12"
              }
            ],
            "name": "fromJobConfig"
          }
        ]
      }
```

## 参数说明<a name="zh-cn_topic_0108272845_section3697070174723"></a>

-   Redis源端作业参数说明

    <a name="zh-cn_topic_0108272845_table29568914174737"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0108272845_row37517852174737"><th class="cellrowborder" valign="top" width="22.66%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272845_p19047209174737"><a name="zh-cn_topic_0108272845_p19047209174737"></a><a name="zh-cn_topic_0108272845_p19047209174737"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.78%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272845_p66428950174737"><a name="zh-cn_topic_0108272845_p66428950174737"></a><a name="zh-cn_topic_0108272845_p66428950174737"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.05%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272845_p12035851174737"><a name="zh-cn_topic_0108272845_p12035851174737"></a><a name="zh-cn_topic_0108272845_p12035851174737"></a>类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="40.510000000000005%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272845_p35379889174737"><a name="zh-cn_topic_0108272845_p35379889174737"></a><a name="zh-cn_topic_0108272845_p35379889174737"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0108272845_row954802520320"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272845_p3519257420320"><a name="zh-cn_topic_0108272845_p3519257420320"></a><a name="zh-cn_topic_0108272845_p3519257420320"></a>fromJobConfig.isBatchMigration</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272845_p3202623120320"><a name="zh-cn_topic_0108272845_p3202623120320"></a><a name="zh-cn_topic_0108272845_p3202623120320"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272845_p4398791720320"><a name="zh-cn_topic_0108272845_p4398791720320"></a><a name="zh-cn_topic_0108272845_p4398791720320"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272845_p625149520320"><a name="zh-cn_topic_0108272845_p625149520320"></a><a name="zh-cn_topic_0108272845_p625149520320"></a>是否为整库迁移。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272845_row47198767174737"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272845_p65003822174737"><a name="zh-cn_topic_0108272845_p65003822174737"></a><a name="zh-cn_topic_0108272845_p65003822174737"></a>fromJobConfig.keyPrefix</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272845_p30818262174737"><a name="zh-cn_topic_0108272845_p30818262174737"></a><a name="zh-cn_topic_0108272845_p30818262174737"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272845_p13251278174737"><a name="zh-cn_topic_0108272845_p13251278174737"></a><a name="zh-cn_topic_0108272845_p13251278174737"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272845_p66720574174737"><a name="zh-cn_topic_0108272845_p66720574174737"></a><a name="zh-cn_topic_0108272845_p66720574174737"></a>key前缀，对应关系表的表名。</p>
    <p id="zh-cn_topic_0108272845_p63614259174737"><a name="zh-cn_topic_0108272845_p63614259174737"></a><a name="zh-cn_topic_0108272845_p63614259174737"></a>Redis和关系表的映射：用关系表的<span class="uicontrol" id="zh-cn_topic_0108272845_uicontrol35657423174737"><a name="zh-cn_topic_0108272845_uicontrol35657423174737"></a><a name="zh-cn_topic_0108272845_uicontrol35657423174737"></a>“表名+分隔符”</span>来对应Redis的Key；关系表的一行数据对应Redis的Value。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272845_row52481355174737"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272845_p23131376174737"><a name="zh-cn_topic_0108272845_p23131376174737"></a><a name="zh-cn_topic_0108272845_p23131376174737"></a>fromJobConfig.keySeparator</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272845_p61702153174737"><a name="zh-cn_topic_0108272845_p61702153174737"></a><a name="zh-cn_topic_0108272845_p61702153174737"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272845_p31818495174737"><a name="zh-cn_topic_0108272845_p31818495174737"></a><a name="zh-cn_topic_0108272845_p31818495174737"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272845_p27161273174737"><a name="zh-cn_topic_0108272845_p27161273174737"></a><a name="zh-cn_topic_0108272845_p27161273174737"></a>key分隔符，一般用来分割关系表和主键。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272845_row43124867174737"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272845_p3453343174737"><a name="zh-cn_topic_0108272845_p3453343174737"></a><a name="zh-cn_topic_0108272845_p3453343174737"></a>fromJobConfig.valueStoreType</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272845_p11285363174737"><a name="zh-cn_topic_0108272845_p11285363174737"></a><a name="zh-cn_topic_0108272845_p11285363174737"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272845_p41699240174737"><a name="zh-cn_topic_0108272845_p41699240174737"></a><a name="zh-cn_topic_0108272845_p41699240174737"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272845_p22195302174737"><a name="zh-cn_topic_0108272845_p22195302174737"></a><a name="zh-cn_topic_0108272845_p22195302174737"></a>关系表行数据在Redis中的存储方式分为<span class="parmvalue" id="zh-cn_topic_0108272845_parmvalue65539991174737"><a name="zh-cn_topic_0108272845_parmvalue65539991174737"></a><a name="zh-cn_topic_0108272845_parmvalue65539991174737"></a>“string”</span>和<span class="parmvalue" id="zh-cn_topic_0108272845_parmvalue52989012174737"><a name="zh-cn_topic_0108272845_parmvalue52989012174737"></a><a name="zh-cn_topic_0108272845_parmvalue52989012174737"></a>“hash”</span>两种存储方式。</p>
    <a name="zh-cn_topic_0108272845_ul7139060174737"></a><a name="zh-cn_topic_0108272845_ul7139060174737"></a><ul id="zh-cn_topic_0108272845_ul7139060174737"><li>STRING：表示用字符串通过分隔符来表示一行数据的各列，可以有效节省存储空间。</li><li>HASH：表示一行数据通过<span class="uicontrol" id="zh-cn_topic_0108272845_uicontrol36992737174737"><a name="zh-cn_topic_0108272845_uicontrol36992737174737"></a><a name="zh-cn_topic_0108272845_uicontrol36992737174737"></a>“列名：列值”</span>的方式存储在hash表中。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272845_row64499180174737"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272845_p57051095174737"><a name="zh-cn_topic_0108272845_p57051095174737"></a><a name="zh-cn_topic_0108272845_p57051095174737"></a>fromJobConfig.valueSeparator</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272845_p57735958174737"><a name="zh-cn_topic_0108272845_p57735958174737"></a><a name="zh-cn_topic_0108272845_p57735958174737"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272845_p46101010174737"><a name="zh-cn_topic_0108272845_p46101010174737"></a><a name="zh-cn_topic_0108272845_p46101010174737"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272845_p43194290174737"><a name="zh-cn_topic_0108272845_p43194290174737"></a><a name="zh-cn_topic_0108272845_p43194290174737"></a>值分隔符号，当<span class="parmname" id="zh-cn_topic_0108272845_parmname53204291174737"><a name="zh-cn_topic_0108272845_parmname53204291174737"></a><a name="zh-cn_topic_0108272845_parmname53204291174737"></a>“valueStoreType”</span>为<span class="parmvalue" id="zh-cn_topic_0108272845_parmvalue9076574174737"><a name="zh-cn_topic_0108272845_parmvalue9076574174737"></a><a name="zh-cn_topic_0108272845_parmvalue9076574174737"></a>“STRING”</span>时此参数有效，默认值为：<span class="parmvalue" id="zh-cn_topic_0108272845_parmvalue14580309174737"><a name="zh-cn_topic_0108272845_parmvalue14580309174737"></a><a name="zh-cn_topic_0108272845_parmvalue14580309174737"></a>“\tab”</span>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272845_row64113919174737"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272845_p25844989174737"><a name="zh-cn_topic_0108272845_p25844989174737"></a><a name="zh-cn_topic_0108272845_p25844989174737"></a>fromJobConfig.columnList</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272845_p13069375174737"><a name="zh-cn_topic_0108272845_p13069375174737"></a><a name="zh-cn_topic_0108272845_p13069375174737"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272845_p51986478174737"><a name="zh-cn_topic_0108272845_p51986478174737"></a><a name="zh-cn_topic_0108272845_p51986478174737"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272845_p50155185174737"><a name="zh-cn_topic_0108272845_p50155185174737"></a><a name="zh-cn_topic_0108272845_p50155185174737"></a>需要抽取的字段列表，字段名之间使用<span class="parmvalue" id="zh-cn_topic_0108272845_parmvalue48743486174737"><a name="zh-cn_topic_0108272845_parmvalue48743486174737"></a><a name="zh-cn_topic_0108272845_parmvalue48743486174737"></a>“&amp;”</span>分割，例如：<span class="parmvalue" id="zh-cn_topic_0108272845_parmvalue36038193174737"><a name="zh-cn_topic_0108272845_parmvalue36038193174737"></a><a name="zh-cn_topic_0108272845_parmvalue36038193174737"></a>“id&amp;gid&amp;name”</span>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272845_row55908283174737"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272845_p32277056174737"><a name="zh-cn_topic_0108272845_p32277056174737"></a><a name="zh-cn_topic_0108272845_p32277056174737"></a>fromJobConfig.formats</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272845_p64304758174737"><a name="zh-cn_topic_0108272845_p64304758174737"></a><a name="zh-cn_topic_0108272845_p64304758174737"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272845_p41302916174737"><a name="zh-cn_topic_0108272845_p41302916174737"></a><a name="zh-cn_topic_0108272845_p41302916174737"></a>数据结构</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272845_p57201939174737"><a name="zh-cn_topic_0108272845_p57201939174737"></a><a name="zh-cn_topic_0108272845_p57201939174737"></a>时间格式，请参见<a href="#zh-cn_topic_0108272845_li45055411174737">fromJobConfig.formats参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="zh-cn_topic_0108272845_li45055411174737"></a>fromJobConfig.formats参数说明

    <a name="zh-cn_topic_0108272845_table37875375203058"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0108272845_row57939309203058"><th class="cellrowborder" valign="top" width="20.987901209879013%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272845_p62572456203058"><a name="zh-cn_topic_0108272845_p62572456203058"></a><a name="zh-cn_topic_0108272845_p62572456203058"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.567843215678433%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272845_p35204151203058"><a name="zh-cn_topic_0108272845_p35204151203058"></a><a name="zh-cn_topic_0108272845_p35204151203058"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.25827417258274%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272845_p32963971203058"><a name="zh-cn_topic_0108272845_p32963971203058"></a><a name="zh-cn_topic_0108272845_p32963971203058"></a>类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="40.18598140185981%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272845_p52835955203058"><a name="zh-cn_topic_0108272845_p52835955203058"></a><a name="zh-cn_topic_0108272845_p52835955203058"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0108272845_row51853935203058"><td class="cellrowborder" valign="top" width="20.987901209879013%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272845_p39419232203058"><a name="zh-cn_topic_0108272845_p39419232203058"></a><a name="zh-cn_topic_0108272845_p39419232203058"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.567843215678433%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272845_p38841262203058"><a name="zh-cn_topic_0108272845_p38841262203058"></a><a name="zh-cn_topic_0108272845_p38841262203058"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.25827417258274%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272845_p59134528203058"><a name="zh-cn_topic_0108272845_p59134528203058"></a><a name="zh-cn_topic_0108272845_p59134528203058"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.18598140185981%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272845_p25167487203058"><a name="zh-cn_topic_0108272845_p25167487203058"></a><a name="zh-cn_topic_0108272845_p25167487203058"></a>列号，例如：<span class="parmvalue" id="zh-cn_topic_0108272845_parmvalue25180794203058"><a name="zh-cn_topic_0108272845_parmvalue25180794203058"></a><a name="zh-cn_topic_0108272845_parmvalue25180794203058"></a>“1”</span>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272845_row25300562203058"><td class="cellrowborder" valign="top" width="20.987901209879013%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272845_p36079650203058"><a name="zh-cn_topic_0108272845_p36079650203058"></a><a name="zh-cn_topic_0108272845_p36079650203058"></a>value</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.567843215678433%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272845_p36770518203058"><a name="zh-cn_topic_0108272845_p36770518203058"></a><a name="zh-cn_topic_0108272845_p36770518203058"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.25827417258274%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272845_p25621975203058"><a name="zh-cn_topic_0108272845_p25621975203058"></a><a name="zh-cn_topic_0108272845_p25621975203058"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.18598140185981%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272845_p62114060203058"><a name="zh-cn_topic_0108272845_p62114060203058"></a><a name="zh-cn_topic_0108272845_p62114060203058"></a>时间格式，例如：<span class="parmvalue" id="zh-cn_topic_0108272845_parmvalue22155629203058"><a name="zh-cn_topic_0108272845_parmvalue22155629203058"></a><a name="zh-cn_topic_0108272845_parmvalue22155629203058"></a>“yyyy-MM-dd”</span>。</p>
    </td>
    </tr>
    </tbody>
    </table>


