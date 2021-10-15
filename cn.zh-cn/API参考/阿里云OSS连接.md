# 阿里云OSS连接<a name="dgc_02_0264"></a>

## 介绍<a name="zh-cn_topic_0108272818_section621837"></a>

通过OSS连接，可以对阿里云对象存储服务（Object Storage Service，简称 OSS）抽取文件，支持CSV、JSON和二进制格式。

## 连接样例<a name="zh-cn_topic_0108272818_section6163607716523"></a>

```
{
    "links": [
        {
            "link-config-values": {
                "configs": [
                    {
                        "inputs": [
                            {
                                "name": "linkConfig.storageType",
                                "value": "OSS"
                            },
                            {
                                "name": "linkConfig.ossEndpoint",
                                "value": "oss-cn-qingdao.aliyuncs.com"
                            },
                            {
                                "name": "linkConfig.ossAuthType",
                                "value": "ACCESS_KEY"
                            },
                            {
                                "name": "linkConfig.accessKey",
                                "value": "LTAI1mR805IE0cVr"
                            },
                            {
                                "name": "linkConfig.securityKey",
                                "value": "Add password here"
                            }
                        ],
                        "name": "linkConfig"
                    }
                ]
            },
            "name": "op_oss_link",
            "connector-name": "obs-connector"
        }
    ]
}
```

## 连接参数<a name="zh-cn_topic_0108272818_section5035508012043"></a>

<a name="zh-cn_topic_0108272818_table13922888141527"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108272818_row229143141527"><th class="cellrowborder" valign="top" width="22.09%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272818_p66756185141527"><a name="zh-cn_topic_0108272818_p66756185141527"></a><a name="zh-cn_topic_0108272818_p66756185141527"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="21.84%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272818_p38541938141527"><a name="zh-cn_topic_0108272818_p38541938141527"></a><a name="zh-cn_topic_0108272818_p38541938141527"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.43%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272818_p34889279141527"><a name="zh-cn_topic_0108272818_p34889279141527"></a><a name="zh-cn_topic_0108272818_p34889279141527"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="38.64%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272818_p7459369141527"><a name="zh-cn_topic_0108272818_p7459369141527"></a><a name="zh-cn_topic_0108272818_p7459369141527"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108272818_row2725489141730"><td class="cellrowborder" valign="top" width="22.09%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272818_p177932511744"><a name="zh-cn_topic_0108272818_p177932511744"></a><a name="zh-cn_topic_0108272818_p177932511744"></a>linkConfig.storageType</p>
</td>
<td class="cellrowborder" valign="top" width="21.84%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272818_p2813219141730"><a name="zh-cn_topic_0108272818_p2813219141730"></a><a name="zh-cn_topic_0108272818_p2813219141730"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.43%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272818_p26544197141730"><a name="zh-cn_topic_0108272818_p26544197141730"></a><a name="zh-cn_topic_0108272818_p26544197141730"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.64%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272818_p2596372141730"><a name="zh-cn_topic_0108272818_p2596372141730"></a><a name="zh-cn_topic_0108272818_p2596372141730"></a>对象存储的类型。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272818_row302832141730"><td class="cellrowborder" valign="top" width="22.09%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272818_p11340626153"><a name="zh-cn_topic_0108272818_p11340626153"></a><a name="zh-cn_topic_0108272818_p11340626153"></a>linkConfig.ossEndpoint</p>
</td>
<td class="cellrowborder" valign="top" width="21.84%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272818_p36550801141730"><a name="zh-cn_topic_0108272818_p36550801141730"></a><a name="zh-cn_topic_0108272818_p36550801141730"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.43%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272818_p7824886141730"><a name="zh-cn_topic_0108272818_p7824886141730"></a><a name="zh-cn_topic_0108272818_p7824886141730"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.64%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272818_p29836044141730"><a name="zh-cn_topic_0108272818_p29836044141730"></a><a name="zh-cn_topic_0108272818_p29836044141730"></a>OSS的域名。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272818_row6277630954"><td class="cellrowborder" valign="top" width="22.09%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272818_p327743017513"><a name="zh-cn_topic_0108272818_p327743017513"></a><a name="zh-cn_topic_0108272818_p327743017513"></a>linkConfig.ossAuthType</p>
</td>
<td class="cellrowborder" valign="top" width="21.84%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272818_p027763016512"><a name="zh-cn_topic_0108272818_p027763016512"></a><a name="zh-cn_topic_0108272818_p027763016512"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.43%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272818_p5277730752"><a name="zh-cn_topic_0108272818_p5277730752"></a><a name="zh-cn_topic_0108272818_p5277730752"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="38.64%" headers="mcps1.1.5.1.4 "><div class="p" id="zh-cn_topic_0108272818_p152770301554"><a name="zh-cn_topic_0108272818_p152770301554"></a><a name="zh-cn_topic_0108272818_p152770301554"></a>身份认证方式。<a name="zh-cn_topic_0108272818_ul773418615139"></a><a name="zh-cn_topic_0108272818_ul773418615139"></a><ul id="zh-cn_topic_0108272818_ul773418615139"><li>ACCESS_KEY：使用长期密钥访问OSS。</li><li>STS：使用临时密钥和安全令牌访问OSS。</li></ul>
</div>
</td>
</tr>
<tr id="zh-cn_topic_0108272818_row14946728141730"><td class="cellrowborder" valign="top" width="22.09%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272818_p7204562141730"><a name="zh-cn_topic_0108272818_p7204562141730"></a><a name="zh-cn_topic_0108272818_p7204562141730"></a>linkConfig.accessKey</p>
</td>
<td class="cellrowborder" valign="top" width="21.84%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272818_p46698681141730"><a name="zh-cn_topic_0108272818_p46698681141730"></a><a name="zh-cn_topic_0108272818_p46698681141730"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.43%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272818_p24496779141730"><a name="zh-cn_topic_0108272818_p24496779141730"></a><a name="zh-cn_topic_0108272818_p24496779141730"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.64%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272818_p1585198617219"><a name="zh-cn_topic_0108272818_p1585198617219"></a><a name="zh-cn_topic_0108272818_p1585198617219"></a>访问标识（AK）。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272818_row53856530141730"><td class="cellrowborder" valign="top" width="22.09%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272818_p45889226141730"><a name="zh-cn_topic_0108272818_p45889226141730"></a><a name="zh-cn_topic_0108272818_p45889226141730"></a>linkConfig.securityKey</p>
</td>
<td class="cellrowborder" valign="top" width="21.84%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272818_p26039827141730"><a name="zh-cn_topic_0108272818_p26039827141730"></a><a name="zh-cn_topic_0108272818_p26039827141730"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.43%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272818_p28851277141730"><a name="zh-cn_topic_0108272818_p28851277141730"></a><a name="zh-cn_topic_0108272818_p28851277141730"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.64%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272818_p1549749917230"><a name="zh-cn_topic_0108272818_p1549749917230"></a><a name="zh-cn_topic_0108272818_p1549749917230"></a>密钥（SK）。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272818_row1346855713511"><td class="cellrowborder" valign="top" width="22.09%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272818_p1468257353"><a name="zh-cn_topic_0108272818_p1468257353"></a><a name="zh-cn_topic_0108272818_p1468257353"></a>linkConfig.securityToken</p>
</td>
<td class="cellrowborder" valign="top" width="21.84%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272818_p174685570511"><a name="zh-cn_topic_0108272818_p174685570511"></a><a name="zh-cn_topic_0108272818_p174685570511"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.43%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272818_p12741256191514"><a name="zh-cn_topic_0108272818_p12741256191514"></a><a name="zh-cn_topic_0108272818_p12741256191514"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.64%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272818_p1538717341111"><a name="zh-cn_topic_0108272818_p1538717341111"></a><a name="zh-cn_topic_0108272818_p1538717341111"></a>使用临时访问凭证登录OSS时，还需要提供临时令牌。</p>
</td>
</tr>
</tbody>
</table>

