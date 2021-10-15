# DIS连接<a name="dgc_02_0275"></a>

## 介绍<a name="zh-cn_topic_0108272804_section6064778111258"></a>

通过DIS连接可以与DIS建立连接，并按照用户指定配置将DIS中的数据迁移到其他数据源。

## 连接样例<a name="zh-cn_topic_0108272804_section6163607716523"></a>

```
{
    "links": [
        {
            "link-config-values": {
                "configs": [
                    {
                        "inputs": [
                            {
                                "name": "linkConfig.region",
                                "value": "Region"
                            },
                            {
                                "name": "linkConfig.endpoint",
                                "value": "https://dis.cn-north-1.myhuaweiclouds.com"
                            },
                            {
                                "name": "linkConfig.ak",
                                "value": "RSO6TTEZMJ6TTFBBAACE"
                            },
                            {
                                "name": "linkConfig.sk",
                                "value": "Add password here"
                            },
                            {
                                "name": "linkConfig.projectId",
                                "value": "11d4d5af17c84660bc90b6631327d7c7"
                            }
                        ],
                        "name": "linkConfig"
                    }
                ]
            },
            "name": "dis_link",
            "connector-name": "dis-connector"
        }
    ]
}
```

## 连接参数<a name="zh-cn_topic_0108272804_section4905685211330"></a>

<a name="zh-cn_topic_0108272804_table13922888141527"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108272804_row229143141527"><th class="cellrowborder" valign="top" width="29.049999999999997%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272804_p66756185141527"><a name="zh-cn_topic_0108272804_p66756185141527"></a><a name="zh-cn_topic_0108272804_p66756185141527"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="19.6%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272804_p38541938141527"><a name="zh-cn_topic_0108272804_p38541938141527"></a><a name="zh-cn_topic_0108272804_p38541938141527"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.419999999999998%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272804_p34889279141527"><a name="zh-cn_topic_0108272804_p34889279141527"></a><a name="zh-cn_topic_0108272804_p34889279141527"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.93%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272804_p7459369141527"><a name="zh-cn_topic_0108272804_p7459369141527"></a><a name="zh-cn_topic_0108272804_p7459369141527"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108272804_row564934184343"><td class="cellrowborder" valign="top" width="29.049999999999997%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272804_p24689642184346"><a name="zh-cn_topic_0108272804_p24689642184346"></a><a name="zh-cn_topic_0108272804_p24689642184346"></a>linkConfig.region</p>
</td>
<td class="cellrowborder" valign="top" width="19.6%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272804_p53703963184346"><a name="zh-cn_topic_0108272804_p53703963184346"></a><a name="zh-cn_topic_0108272804_p53703963184346"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272804_p55053778184346"><a name="zh-cn_topic_0108272804_p55053778184346"></a><a name="zh-cn_topic_0108272804_p55053778184346"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.93%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272804_p30170996184346"><a name="zh-cn_topic_0108272804_p30170996184346"></a><a name="zh-cn_topic_0108272804_p30170996184346"></a>DIS服务所属地域。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272804_row2725489141730"><td class="cellrowborder" valign="top" width="29.049999999999997%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272804_p28492222171138"><a name="zh-cn_topic_0108272804_p28492222171138"></a><a name="zh-cn_topic_0108272804_p28492222171138"></a>linkConfig.endpoint</p>
</td>
<td class="cellrowborder" valign="top" width="19.6%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272804_p2813219141730"><a name="zh-cn_topic_0108272804_p2813219141730"></a><a name="zh-cn_topic_0108272804_p2813219141730"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272804_p26544197141730"><a name="zh-cn_topic_0108272804_p26544197141730"></a><a name="zh-cn_topic_0108272804_p26544197141730"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.93%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272804_p2596372141730"><a name="zh-cn_topic_0108272804_p2596372141730"></a><a name="zh-cn_topic_0108272804_p2596372141730"></a>待连接DIS的URL，URL格式为https://Endpoint。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272804_row53856530141730"><td class="cellrowborder" valign="top" width="29.049999999999997%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272804_p43117167171152"><a name="zh-cn_topic_0108272804_p43117167171152"></a><a name="zh-cn_topic_0108272804_p43117167171152"></a>linkConfig.ak</p>
</td>
<td class="cellrowborder" valign="top" width="19.6%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272804_p26039827141730"><a name="zh-cn_topic_0108272804_p26039827141730"></a><a name="zh-cn_topic_0108272804_p26039827141730"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272804_p28851277141730"><a name="zh-cn_topic_0108272804_p28851277141730"></a><a name="zh-cn_topic_0108272804_p28851277141730"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.93%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272804_p55252128141730"><a name="zh-cn_topic_0108272804_p55252128141730"></a><a name="zh-cn_topic_0108272804_p55252128141730"></a>DIS服务端的AK。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272804_row38134078171211"><td class="cellrowborder" valign="top" width="29.049999999999997%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272804_p1852576171211"><a name="zh-cn_topic_0108272804_p1852576171211"></a><a name="zh-cn_topic_0108272804_p1852576171211"></a>linkConfig.sk</p>
</td>
<td class="cellrowborder" valign="top" width="19.6%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272804_p15840983171211"><a name="zh-cn_topic_0108272804_p15840983171211"></a><a name="zh-cn_topic_0108272804_p15840983171211"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272804_p8051275171211"><a name="zh-cn_topic_0108272804_p8051275171211"></a><a name="zh-cn_topic_0108272804_p8051275171211"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.93%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272804_p48173539171211"><a name="zh-cn_topic_0108272804_p48173539171211"></a><a name="zh-cn_topic_0108272804_p48173539171211"></a>DIS服务端的SK。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272804_row3643675171217"><td class="cellrowborder" valign="top" width="29.049999999999997%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272804_p65139020184339"><a name="zh-cn_topic_0108272804_p65139020184339"></a><a name="zh-cn_topic_0108272804_p65139020184339"></a>linkConfig.projectId</p>
</td>
<td class="cellrowborder" valign="top" width="19.6%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272804_p22547918184339"><a name="zh-cn_topic_0108272804_p22547918184339"></a><a name="zh-cn_topic_0108272804_p22547918184339"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272804_p23433084184339"><a name="zh-cn_topic_0108272804_p23433084184339"></a><a name="zh-cn_topic_0108272804_p23433084184339"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.93%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272804_p47250101"><a name="zh-cn_topic_0108272804_p47250101"></a><a name="zh-cn_topic_0108272804_p47250101"></a>项目ID。</p>
</td>
</tr>
</tbody>
</table>

