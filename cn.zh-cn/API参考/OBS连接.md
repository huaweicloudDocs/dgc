# OBS连接<a name="dgc_02_0263"></a>

## 介绍<a name="zh-cn_topic_0108272823_section621837"></a>

通过OBS连接，可以对对象存储服务（Object Storage Service，简称OBS）抽取或加载文件，支持CSV、JSON和二进制格式。

## 连接样例<a name="zh-cn_topic_0108272823_section6163607716523"></a>

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
                                "value": "OBS"
                            },
                            {
                                "name": "linkConfig.server",
                                "value": "10.121.16.183"
                            },
                            {
                                "name": "linkConfig.port",
                                "value": "443"
                            },
                            {
                                "name":"linkConfig.accessKey",
                                "value": "RSO6TTEZMJ6TTFBBAACE"
                            },
                            {
                                "name":"linkConfig.securityKey",
                                "value":"Add password here"
                            }
                        ],
                        "name": "linkConfig"
                    }
                ]
            },
            "name": "obs_link",
            "connector-name": "obs-connector"
        }
    ]
}
```

## 连接参数<a name="zh-cn_topic_0108272823_section5035508012043"></a>

<a name="zh-cn_topic_0108272823_table13922888141527"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108272823_row229143141527"><th class="cellrowborder" valign="top" width="22.09%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272823_p66756185141527"><a name="zh-cn_topic_0108272823_p66756185141527"></a><a name="zh-cn_topic_0108272823_p66756185141527"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="21.84%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272823_p38541938141527"><a name="zh-cn_topic_0108272823_p38541938141527"></a><a name="zh-cn_topic_0108272823_p38541938141527"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.43%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272823_p34889279141527"><a name="zh-cn_topic_0108272823_p34889279141527"></a><a name="zh-cn_topic_0108272823_p34889279141527"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="38.64%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272823_p7459369141527"><a name="zh-cn_topic_0108272823_p7459369141527"></a><a name="zh-cn_topic_0108272823_p7459369141527"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108272823_row5619468276"><td class="cellrowborder" valign="top" width="22.09%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272823_p1961446152715"><a name="zh-cn_topic_0108272823_p1961446152715"></a><a name="zh-cn_topic_0108272823_p1961446152715"></a>linkConfig.storageType</p>
</td>
<td class="cellrowborder" valign="top" width="21.84%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272823_p126104692710"><a name="zh-cn_topic_0108272823_p126104692710"></a><a name="zh-cn_topic_0108272823_p126104692710"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.43%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272823_p14804119102817"><a name="zh-cn_topic_0108272823_p14804119102817"></a><a name="zh-cn_topic_0108272823_p14804119102817"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.64%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272823_p11654612275"><a name="zh-cn_topic_0108272823_p11654612275"></a><a name="zh-cn_topic_0108272823_p11654612275"></a>对象存储的类型。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272823_row2725489141730"><td class="cellrowborder" valign="top" width="22.09%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272823_p18261829141730"><a name="zh-cn_topic_0108272823_p18261829141730"></a><a name="zh-cn_topic_0108272823_p18261829141730"></a>linkConfig.server</p>
</td>
<td class="cellrowborder" valign="top" width="21.84%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272823_p2813219141730"><a name="zh-cn_topic_0108272823_p2813219141730"></a><a name="zh-cn_topic_0108272823_p2813219141730"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.43%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272823_p26544197141730"><a name="zh-cn_topic_0108272823_p26544197141730"></a><a name="zh-cn_topic_0108272823_p26544197141730"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.64%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272823_p196911320142113"><a name="zh-cn_topic_0108272823_p196911320142113"></a><a name="zh-cn_topic_0108272823_p196911320142113"></a>OBS服务器的终端节点（Endpoint），这里支持用户输入桶级别的域名。</p>
<p id="zh-cn_topic_0108272823_p12996152342119"><a name="zh-cn_topic_0108272823_p12996152342119"></a><a name="zh-cn_topic_0108272823_p12996152342119"></a>例如：test.obs.myhuaweicloud.com，则在查询OBS桶的时候，只能查询到test这个桶。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272823_row302832141730"><td class="cellrowborder" valign="top" width="22.09%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272823_p13707316141730"><a name="zh-cn_topic_0108272823_p13707316141730"></a><a name="zh-cn_topic_0108272823_p13707316141730"></a>linkConfig.port</p>
</td>
<td class="cellrowborder" valign="top" width="21.84%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272823_p36550801141730"><a name="zh-cn_topic_0108272823_p36550801141730"></a><a name="zh-cn_topic_0108272823_p36550801141730"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.43%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272823_p7824886141730"><a name="zh-cn_topic_0108272823_p7824886141730"></a><a name="zh-cn_topic_0108272823_p7824886141730"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.64%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272823_p29836044141730"><a name="zh-cn_topic_0108272823_p29836044141730"></a><a name="zh-cn_topic_0108272823_p29836044141730"></a>数据传输协议端口，https是443，http是80。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272823_row14946728141730"><td class="cellrowborder" valign="top" width="22.09%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272823_p7204562141730"><a name="zh-cn_topic_0108272823_p7204562141730"></a><a name="zh-cn_topic_0108272823_p7204562141730"></a>linkConfig.accessKey</p>
</td>
<td class="cellrowborder" valign="top" width="21.84%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272823_p46698681141730"><a name="zh-cn_topic_0108272823_p46698681141730"></a><a name="zh-cn_topic_0108272823_p46698681141730"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.43%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272823_p24496779141730"><a name="zh-cn_topic_0108272823_p24496779141730"></a><a name="zh-cn_topic_0108272823_p24496779141730"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.64%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272823_p1585198617219"><a name="zh-cn_topic_0108272823_p1585198617219"></a><a name="zh-cn_topic_0108272823_p1585198617219"></a>访问标识（AK）。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272823_row53856530141730"><td class="cellrowborder" valign="top" width="22.09%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272823_p45889226141730"><a name="zh-cn_topic_0108272823_p45889226141730"></a><a name="zh-cn_topic_0108272823_p45889226141730"></a>linkConfig.securityKey</p>
</td>
<td class="cellrowborder" valign="top" width="21.84%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272823_p26039827141730"><a name="zh-cn_topic_0108272823_p26039827141730"></a><a name="zh-cn_topic_0108272823_p26039827141730"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.43%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272823_p28851277141730"><a name="zh-cn_topic_0108272823_p28851277141730"></a><a name="zh-cn_topic_0108272823_p28851277141730"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.64%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272823_p1549749917230"><a name="zh-cn_topic_0108272823_p1549749917230"></a><a name="zh-cn_topic_0108272823_p1549749917230"></a>密钥（SK）。</p>
</td>
</tr>
</tbody>
</table>

