# 七牛云KODO/腾讯云COS连接<a name="dgc_02_0265"></a>

## 介绍<a name="zh-cn_topic_0119683600_section621837"></a>

通过KODO//COS连接，可以对七牛云对象存储服务（KODO）或者腾讯云对象存储（COS）抽取文件，支持CSV、JSON和二进制格式。

## 连接样例<a name="zh-cn_topic_0119683600_section6163607716523"></a>

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
                "value": "KODO_COS"
              },
              {
                "name": "linkConfig.zone",
                "value": "z1"
              },
              {
                "name": "linkConfig.accessKey",
                "value": "xib1R_oeN4KBYTA-yNoV0Kd3AbUwi1yuvzbPF4LE"
              },
              {
                "name": "linkConfig.securityKey",
                "value": "Add password here"
              },
              {
                "name": "linkConfig.useCustomDomain",
                "value": "false"
              }
            ],
            "name": "linkConfig"
          }
        ]
      },
      "name": "kodo_link",
      "connector-name": "thirdparty-obs-connector"
    }
  ]
}
```

## 连接参数<a name="zh-cn_topic_0119683600_section5035508012043"></a>

<a name="zh-cn_topic_0119683600_table13922888141527"></a>
<table><thead align="left"><tr id="zh-cn_topic_0119683600_row229143141527"><th class="cellrowborder" valign="top" width="22.09%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0119683600_p66756185141527"><a name="zh-cn_topic_0119683600_p66756185141527"></a><a name="zh-cn_topic_0119683600_p66756185141527"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="21.84%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0119683600_p38541938141527"><a name="zh-cn_topic_0119683600_p38541938141527"></a><a name="zh-cn_topic_0119683600_p38541938141527"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.43%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0119683600_p34889279141527"><a name="zh-cn_topic_0119683600_p34889279141527"></a><a name="zh-cn_topic_0119683600_p34889279141527"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="38.64%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0119683600_p7459369141527"><a name="zh-cn_topic_0119683600_p7459369141527"></a><a name="zh-cn_topic_0119683600_p7459369141527"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0119683600_row2725489141730"><td class="cellrowborder" valign="top" width="22.09%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0119683600_p177932511744"><a name="zh-cn_topic_0119683600_p177932511744"></a><a name="zh-cn_topic_0119683600_p177932511744"></a>linkConfig.storageType</p>
</td>
<td class="cellrowborder" valign="top" width="21.84%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0119683600_p2813219141730"><a name="zh-cn_topic_0119683600_p2813219141730"></a><a name="zh-cn_topic_0119683600_p2813219141730"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.43%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0119683600_p26544197141730"><a name="zh-cn_topic_0119683600_p26544197141730"></a><a name="zh-cn_topic_0119683600_p26544197141730"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.64%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0119683600_p2596372141730"><a name="zh-cn_topic_0119683600_p2596372141730"></a><a name="zh-cn_topic_0119683600_p2596372141730"></a>对象存储的类型。</p>
</td>
</tr>
<tr id="zh-cn_topic_0119683600_row302832141730"><td class="cellrowborder" valign="top" width="22.09%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0119683600_p18998152382"><a name="zh-cn_topic_0119683600_p18998152382"></a><a name="zh-cn_topic_0119683600_p18998152382"></a>linkConfig.zone</p>
</td>
<td class="cellrowborder" valign="top" width="21.84%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0119683600_p36550801141730"><a name="zh-cn_topic_0119683600_p36550801141730"></a><a name="zh-cn_topic_0119683600_p36550801141730"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.43%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0119683600_p7824886141730"><a name="zh-cn_topic_0119683600_p7824886141730"></a><a name="zh-cn_topic_0119683600_p7824886141730"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.64%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0119683600_p29836044141730"><a name="zh-cn_topic_0119683600_p29836044141730"></a><a name="zh-cn_topic_0119683600_p29836044141730"></a>KODO/COS的存储区域。</p>
</td>
</tr>
<tr id="zh-cn_topic_0119683600_row14946728141730"><td class="cellrowborder" valign="top" width="22.09%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0119683600_p7204562141730"><a name="zh-cn_topic_0119683600_p7204562141730"></a><a name="zh-cn_topic_0119683600_p7204562141730"></a>linkConfig.accessKey</p>
</td>
<td class="cellrowborder" valign="top" width="21.84%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0119683600_p46698681141730"><a name="zh-cn_topic_0119683600_p46698681141730"></a><a name="zh-cn_topic_0119683600_p46698681141730"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.43%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0119683600_p24496779141730"><a name="zh-cn_topic_0119683600_p24496779141730"></a><a name="zh-cn_topic_0119683600_p24496779141730"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.64%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0119683600_p1585198617219"><a name="zh-cn_topic_0119683600_p1585198617219"></a><a name="zh-cn_topic_0119683600_p1585198617219"></a>访问标识（AK）。</p>
</td>
</tr>
<tr id="zh-cn_topic_0119683600_row53856530141730"><td class="cellrowborder" valign="top" width="22.09%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0119683600_p45889226141730"><a name="zh-cn_topic_0119683600_p45889226141730"></a><a name="zh-cn_topic_0119683600_p45889226141730"></a>linkConfig.securityKey</p>
</td>
<td class="cellrowborder" valign="top" width="21.84%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0119683600_p26039827141730"><a name="zh-cn_topic_0119683600_p26039827141730"></a><a name="zh-cn_topic_0119683600_p26039827141730"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.43%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0119683600_p28851277141730"><a name="zh-cn_topic_0119683600_p28851277141730"></a><a name="zh-cn_topic_0119683600_p28851277141730"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.64%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0119683600_p1549749917230"><a name="zh-cn_topic_0119683600_p1549749917230"></a><a name="zh-cn_topic_0119683600_p1549749917230"></a>密钥（SK）。</p>
</td>
</tr>
<tr id="zh-cn_topic_0119683600_row1346855713511"><td class="cellrowborder" valign="top" width="22.09%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0119683600_p15499742595"><a name="zh-cn_topic_0119683600_p15499742595"></a><a name="zh-cn_topic_0119683600_p15499742595"></a>linkConfig.useCustomDomain</p>
</td>
<td class="cellrowborder" valign="top" width="21.84%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0119683600_p174685570511"><a name="zh-cn_topic_0119683600_p174685570511"></a><a name="zh-cn_topic_0119683600_p174685570511"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.43%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0119683600_p1777619171514"><a name="zh-cn_topic_0119683600_p1777619171514"></a><a name="zh-cn_topic_0119683600_p1777619171514"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="38.64%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0119683600_p1538717341111"><a name="zh-cn_topic_0119683600_p1538717341111"></a><a name="zh-cn_topic_0119683600_p1538717341111"></a>KODO连接才有该参数，选择是否优先使用自定义域名下载对象。</p>
</td>
</tr>
</tbody>
</table>

