# 目的端为DCS<a name="dgc_02_0303"></a>

## JSON样例<a name="zh-cn_topic_0108272802_section33401108172339"></a>

```
 "to-config-values": {
           "configs": [
               {
                   "inputs": [
                       {
                          "name": "toJobConfig.isBatchMigration",
                          "value": "false"
                       },
                       {
                          "name": "toJobConfig.shouldClearDatabase",
                          "value": "false"
                       },
                       {
                           "name": "toJobConfig.keyPrefix",
                           "value": "cdm_string"
                       },
                       {
                           "name": "toJobConfig.keySeparator",
                           "value": ":"
                       },
                       {
                           "name": "toJobConfig.primaryKeyList",
                           "value": "1"
                       },
                       {
                           "name": "toJobConfig.valueStoreType",
                           "value": "STRING"
                       },
                       {
                           "name": "toJobConfig.valueSeparator",
                           "value": ","
                       },
                       {
                           "name": "toJobConfig.columnList",
                           "value": "1&2&3&4&5&6&7&8&9&10&11&12"
                       }
                   ],
                   "name": "toJobConfig"
               }
           ]
       }
```

## 参数说明<a name="zh-cn_topic_0108272802_section16885145112454"></a>

-   参数说明

    <a name="zh-cn_topic_0108272802_table6307873415412"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0108272802_row2882542015412"><th class="cellrowborder" valign="top" width="22.657734226577343%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272802_p5315765115412"><a name="zh-cn_topic_0108272802_p5315765115412"></a><a name="zh-cn_topic_0108272802_p5315765115412"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="20.157984201579843%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272802_p1080249515412"><a name="zh-cn_topic_0108272802_p1080249515412"></a><a name="zh-cn_topic_0108272802_p1080249515412"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="16.2983701629837%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272802_p258693615412"><a name="zh-cn_topic_0108272802_p258693615412"></a><a name="zh-cn_topic_0108272802_p258693615412"></a>类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="40.885911408859116%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272802_p821526915412"><a name="zh-cn_topic_0108272802_p821526915412"></a><a name="zh-cn_topic_0108272802_p821526915412"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0108272802_row51350293114814"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272802_p65733030114814"><a name="zh-cn_topic_0108272802_p65733030114814"></a><a name="zh-cn_topic_0108272802_p65733030114814"></a>toJobConfig.isBatchMigration</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272802_p22775208114814"><a name="zh-cn_topic_0108272802_p22775208114814"></a><a name="zh-cn_topic_0108272802_p22775208114814"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.2983701629837%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272802_p32852546114814"><a name="zh-cn_topic_0108272802_p32852546114814"></a><a name="zh-cn_topic_0108272802_p32852546114814"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.885911408859116%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272802_p43810589114814"><a name="zh-cn_topic_0108272802_p43810589114814"></a><a name="zh-cn_topic_0108272802_p43810589114814"></a>是否为整库迁移。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272802_row53262839115011"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272802_p19322672115011"><a name="zh-cn_topic_0108272802_p19322672115011"></a><a name="zh-cn_topic_0108272802_p19322672115011"></a>toJobConfig.shouldClearDatabase</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272802_p21632561115011"><a name="zh-cn_topic_0108272802_p21632561115011"></a><a name="zh-cn_topic_0108272802_p21632561115011"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.2983701629837%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272802_p7407011115011"><a name="zh-cn_topic_0108272802_p7407011115011"></a><a name="zh-cn_topic_0108272802_p7407011115011"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.885911408859116%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272802_p63097005115011"><a name="zh-cn_topic_0108272802_p63097005115011"></a><a name="zh-cn_topic_0108272802_p63097005115011"></a>导入前是否清空数据。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272802_row6145707115412"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272802_p40748341144217"><a name="zh-cn_topic_0108272802_p40748341144217"></a><a name="zh-cn_topic_0108272802_p40748341144217"></a>toJobConfig.keyPrefix</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272802_p12281354144217"><a name="zh-cn_topic_0108272802_p12281354144217"></a><a name="zh-cn_topic_0108272802_p12281354144217"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.2983701629837%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272802_p55265640144217"><a name="zh-cn_topic_0108272802_p55265640144217"></a><a name="zh-cn_topic_0108272802_p55265640144217"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.885911408859116%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272802_p32290553155944"><a name="zh-cn_topic_0108272802_p32290553155944"></a><a name="zh-cn_topic_0108272802_p32290553155944"></a>key前缀，类似关系数据库的表名。</p>
    <p id="zh-cn_topic_0108272802_p47331830144217"><a name="zh-cn_topic_0108272802_p47331830144217"></a><a name="zh-cn_topic_0108272802_p47331830144217"></a>Redis和关系表的映射：用关系表的<span class="uicontrol" id="zh-cn_topic_0108272802_uicontrol4962522916020"><a name="zh-cn_topic_0108272802_uicontrol4962522916020"></a><a name="zh-cn_topic_0108272802_uicontrol4962522916020"></a>“表名+分隔符”</span>来对应Redis的Key；关系表的一行数据对应Redis的Value。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272802_row3532522715412"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272802_p31423427144217"><a name="zh-cn_topic_0108272802_p31423427144217"></a><a name="zh-cn_topic_0108272802_p31423427144217"></a>toJobConfig.keySeparator</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272802_p62269650144217"><a name="zh-cn_topic_0108272802_p62269650144217"></a><a name="zh-cn_topic_0108272802_p62269650144217"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.2983701629837%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272802_p10676914144217"><a name="zh-cn_topic_0108272802_p10676914144217"></a><a name="zh-cn_topic_0108272802_p10676914144217"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.885911408859116%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272802_p59523723144217"><a name="zh-cn_topic_0108272802_p59523723144217"></a><a name="zh-cn_topic_0108272802_p59523723144217"></a>key分隔符，一般用来分隔关系表和主键。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272802_row2888033144824"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272802_p32604129144824"><a name="zh-cn_topic_0108272802_p32604129144824"></a><a name="zh-cn_topic_0108272802_p32604129144824"></a>toJobConfig.primaryKeyList</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272802_p23688773144824"><a name="zh-cn_topic_0108272802_p23688773144824"></a><a name="zh-cn_topic_0108272802_p23688773144824"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.2983701629837%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272802_p39742454144824"><a name="zh-cn_topic_0108272802_p39742454144824"></a><a name="zh-cn_topic_0108272802_p39742454144824"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.885911408859116%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272802_p65022171144824"><a name="zh-cn_topic_0108272802_p65022171144824"></a><a name="zh-cn_topic_0108272802_p65022171144824"></a>主键列表，字段名之间使用<span class="parmvalue" id="zh-cn_topic_0108272802_parmvalue5724612216115"><a name="zh-cn_topic_0108272802_parmvalue5724612216115"></a><a name="zh-cn_topic_0108272802_parmvalue5724612216115"></a>“&amp;”</span>分割，例如：<span class="parmvalue" id="zh-cn_topic_0108272802_parmvalue6284347216122"><a name="zh-cn_topic_0108272802_parmvalue6284347216122"></a><a name="zh-cn_topic_0108272802_parmvalue6284347216122"></a>“id&amp;gid”</span>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272802_row130765815412"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272802_p40468004144217"><a name="zh-cn_topic_0108272802_p40468004144217"></a><a name="zh-cn_topic_0108272802_p40468004144217"></a>toJobConfig.valueStoreType</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272802_p56682864144217"><a name="zh-cn_topic_0108272802_p56682864144217"></a><a name="zh-cn_topic_0108272802_p56682864144217"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.2983701629837%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272802_p27909297144217"><a name="zh-cn_topic_0108272802_p27909297144217"></a><a name="zh-cn_topic_0108272802_p27909297144217"></a>枚举</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.885911408859116%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272802_p31296545154541"><a name="zh-cn_topic_0108272802_p31296545154541"></a><a name="zh-cn_topic_0108272802_p31296545154541"></a>关系表行数据在Redis中的存储方式分为<span class="parmvalue" id="zh-cn_topic_0108272802_parmvalue52897852154541"><a name="zh-cn_topic_0108272802_parmvalue52897852154541"></a><a name="zh-cn_topic_0108272802_parmvalue52897852154541"></a>“string”</span>和<span class="parmvalue" id="zh-cn_topic_0108272802_parmvalue6318622154541"><a name="zh-cn_topic_0108272802_parmvalue6318622154541"></a><a name="zh-cn_topic_0108272802_parmvalue6318622154541"></a>“hash”</span>两种存储方式。</p>
    <a name="zh-cn_topic_0108272802_ul1233069154545"></a><a name="zh-cn_topic_0108272802_ul1233069154545"></a><ul id="zh-cn_topic_0108272802_ul1233069154545"><li>STRING：表示一行数据通过字符串方式存储，每列之间通过<span class="uicontrol" id="zh-cn_topic_0108272802_uicontrol1613916411081"><a name="zh-cn_topic_0108272802_uicontrol1613916411081"></a><a name="zh-cn_topic_0108272802_uicontrol1613916411081"></a>“值分隔符”</span>分隔。</li><li>HASH：表示一行数据通过<span class="uicontrol" id="zh-cn_topic_0108272802_uicontrol5976945816353"><a name="zh-cn_topic_0108272802_uicontrol5976945816353"></a><a name="zh-cn_topic_0108272802_uicontrol5976945816353"></a>“列名：列值”</span>的方式存储在hash表中。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272802_row6489782015412"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272802_p23762624144217"><a name="zh-cn_topic_0108272802_p23762624144217"></a><a name="zh-cn_topic_0108272802_p23762624144217"></a>toJobConfig.valueSeparator</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272802_p45724355144217"><a name="zh-cn_topic_0108272802_p45724355144217"></a><a name="zh-cn_topic_0108272802_p45724355144217"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.2983701629837%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272802_p12685312144217"><a name="zh-cn_topic_0108272802_p12685312144217"></a><a name="zh-cn_topic_0108272802_p12685312144217"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.885911408859116%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272802_p20877341144217"><a name="zh-cn_topic_0108272802_p20877341144217"></a><a name="zh-cn_topic_0108272802_p20877341144217"></a>值分隔符号，当<span class="parmname" id="zh-cn_topic_0108272802_parmname293446771647"><a name="zh-cn_topic_0108272802_parmname293446771647"></a><a name="zh-cn_topic_0108272802_parmname293446771647"></a>“valueStoreType”</span>为<span class="parmvalue" id="zh-cn_topic_0108272802_parmvalue4607463416412"><a name="zh-cn_topic_0108272802_parmvalue4607463416412"></a><a name="zh-cn_topic_0108272802_parmvalue4607463416412"></a>“string”</span>时此参数有效，默认值为：<span class="parmvalue" id="zh-cn_topic_0108272802_parmvalue936926916419"><a name="zh-cn_topic_0108272802_parmvalue936926916419"></a><a name="zh-cn_topic_0108272802_parmvalue936926916419"></a>“\tab”</span>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272802_row5037735615412"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272802_p52978520144217"><a name="zh-cn_topic_0108272802_p52978520144217"></a><a name="zh-cn_topic_0108272802_p52978520144217"></a>toJobConfig.columnList</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272802_p63401693144217"><a name="zh-cn_topic_0108272802_p63401693144217"></a><a name="zh-cn_topic_0108272802_p63401693144217"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.2983701629837%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272802_p35263486144217"><a name="zh-cn_topic_0108272802_p35263486144217"></a><a name="zh-cn_topic_0108272802_p35263486144217"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.885911408859116%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272802_p37770149144217"><a name="zh-cn_topic_0108272802_p37770149144217"></a><a name="zh-cn_topic_0108272802_p37770149144217"></a>需要写入的字段列表，字段名之间使用<span class="parmvalue" id="zh-cn_topic_0108272802_parmvalue1296851616438"><a name="zh-cn_topic_0108272802_parmvalue1296851616438"></a><a name="zh-cn_topic_0108272802_parmvalue1296851616438"></a>“&amp;”</span>分割，例如：<span class="parmvalue" id="zh-cn_topic_0108272802_parmvalue2845770316447"><a name="zh-cn_topic_0108272802_parmvalue2845770316447"></a><a name="zh-cn_topic_0108272802_parmvalue2845770316447"></a>“id&amp;gid&amp;name”</span>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272802_row5114066314427"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272802_p19804405144217"><a name="zh-cn_topic_0108272802_p19804405144217"></a><a name="zh-cn_topic_0108272802_p19804405144217"></a>toJobConfig.formats</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272802_p60652949144217"><a name="zh-cn_topic_0108272802_p60652949144217"></a><a name="zh-cn_topic_0108272802_p60652949144217"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.2983701629837%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272802_p13941846144217"><a name="zh-cn_topic_0108272802_p13941846144217"></a><a name="zh-cn_topic_0108272802_p13941846144217"></a>数据结构</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.885911408859116%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272802_p55547743144217"><a name="zh-cn_topic_0108272802_p55547743144217"></a><a name="zh-cn_topic_0108272802_p55547743144217"></a>时间格式，请参见<a href="#zh-cn_topic_0108272802_li27488828155343">toJobConfig.formats参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="zh-cn_topic_0108272802_li27488828155343"></a>toJobConfig.formats参数说明

    <a name="zh-cn_topic_0108272802_t4477f05d1bc94e6585dbf45b426fe73b"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0108272802_r006f9b6d73e34ee38a8da48d147b1c3d"><th class="cellrowborder" valign="top" width="20.987901209879013%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272802_a618d428378ff442781fa69141f57133c"><a name="zh-cn_topic_0108272802_a618d428378ff442781fa69141f57133c"></a><a name="zh-cn_topic_0108272802_a618d428378ff442781fa69141f57133c"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.567843215678433%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272802_a96a07b646a644893909fe84615e3bbc6"><a name="zh-cn_topic_0108272802_a96a07b646a644893909fe84615e3bbc6"></a><a name="zh-cn_topic_0108272802_a96a07b646a644893909fe84615e3bbc6"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.25827417258274%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272802_a3da9057af16440649870696d74c7ef77"><a name="zh-cn_topic_0108272802_a3da9057af16440649870696d74c7ef77"></a><a name="zh-cn_topic_0108272802_a3da9057af16440649870696d74c7ef77"></a>类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="40.18598140185981%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272802_ac62dfcfb79394987b66d2878c3613c57"><a name="zh-cn_topic_0108272802_ac62dfcfb79394987b66d2878c3613c57"></a><a name="zh-cn_topic_0108272802_ac62dfcfb79394987b66d2878c3613c57"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0108272802_rf8412f8b38204d1aaffe11495490bbdf"><td class="cellrowborder" valign="top" width="20.987901209879013%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272802_a08e134ceba9449b2966538d4df4370c1"><a name="zh-cn_topic_0108272802_a08e134ceba9449b2966538d4df4370c1"></a><a name="zh-cn_topic_0108272802_a08e134ceba9449b2966538d4df4370c1"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.567843215678433%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272802_abd29c5b76a954984b63731ec0cfd8a3e"><a name="zh-cn_topic_0108272802_abd29c5b76a954984b63731ec0cfd8a3e"></a><a name="zh-cn_topic_0108272802_abd29c5b76a954984b63731ec0cfd8a3e"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.25827417258274%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272802_aff5ea15506b343b8a2bb3b643da845e7"><a name="zh-cn_topic_0108272802_aff5ea15506b343b8a2bb3b643da845e7"></a><a name="zh-cn_topic_0108272802_aff5ea15506b343b8a2bb3b643da845e7"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.18598140185981%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272802_ab83a5ff86b694422a9ddcff4c2ac3f83"><a name="zh-cn_topic_0108272802_ab83a5ff86b694422a9ddcff4c2ac3f83"></a><a name="zh-cn_topic_0108272802_ab83a5ff86b694422a9ddcff4c2ac3f83"></a>列号，例如：<span class="parmvalue" id="zh-cn_topic_0108272802_pb23c9f7a2da0470dacd54efded1f0766"><a name="zh-cn_topic_0108272802_pb23c9f7a2da0470dacd54efded1f0766"></a><a name="zh-cn_topic_0108272802_pb23c9f7a2da0470dacd54efded1f0766"></a>“1”</span>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272802_r3a96a7d4a75244d597ac1fdc77be8d63"><td class="cellrowborder" valign="top" width="20.987901209879013%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272802_ab915fc2b472b492c82e9567cb97a6fb5"><a name="zh-cn_topic_0108272802_ab915fc2b472b492c82e9567cb97a6fb5"></a><a name="zh-cn_topic_0108272802_ab915fc2b472b492c82e9567cb97a6fb5"></a>value</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.567843215678433%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272802_a648e844f17ec4610919a4724b588a213"><a name="zh-cn_topic_0108272802_a648e844f17ec4610919a4724b588a213"></a><a name="zh-cn_topic_0108272802_a648e844f17ec4610919a4724b588a213"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.25827417258274%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272802_ade2ba95d5ebb47928f648480dd039c4e"><a name="zh-cn_topic_0108272802_ade2ba95d5ebb47928f648480dd039c4e"></a><a name="zh-cn_topic_0108272802_ade2ba95d5ebb47928f648480dd039c4e"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.18598140185981%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272802_a48836c62e216482a9f510b0d7401dc3a"><a name="zh-cn_topic_0108272802_a48836c62e216482a9f510b0d7401dc3a"></a><a name="zh-cn_topic_0108272802_a48836c62e216482a9f510b0d7401dc3a"></a>时间格式，例如：<span class="parmvalue" id="zh-cn_topic_0108272802_p2723e15ad7b04a7ab2b817b91f055254"><a name="zh-cn_topic_0108272802_p2723e15ad7b04a7ab2b817b91f055254"></a><a name="zh-cn_topic_0108272802_p2723e15ad7b04a7ab2b817b91f055254"></a>“yyyy-MM-dd”</span>。</p>
    </td>
    </tr>
    </tbody>
    </table>


