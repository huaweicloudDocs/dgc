# NAS/SFS连接（待下线）<a name="dgc_02_0273"></a>

## 介绍<a name="zh-cn_topic_0108272792_section621837"></a>

通过NAS连接，可以对NAS服务器抽取或加载文件，目前支持SMB/CIFS/NFS协议，以及提供CIFS/SMB/NFS协议的文件系统的云服务，例如弹性文件服务SFS。文件格式支持CSV、JSON和二进制格式。

## 连接样例<a name="zh-cn_topic_0108272792_section6163607716523"></a>

```
{
    "links": [
        {
            "link-config-values": {
                "configs": [
                    {
                        "inputs": [
                            {
                                "name": "linkConfig.protocol",
                                "value": "CIFS"
                            },
                            {
                                "name": "linkConfig.server",
                                "value": "\\\\10.121.16.20\\data"
                            },
                            {
                                "name": "linkConfig.username",
                                "value": "username"
                            },
                            {
                                "name": "linkConfig.password",
                                "value": "Add password here"
                            }
                        ],
                        "name": "linkConfig"
                    }
                ]
            },
            "name": "nas_link",
            "connector-name": "nas-connector"
        }
    ]
}
```

## 连接参数<a name="zh-cn_topic_0108272792_section5035508012043"></a>

<a name="zh-cn_topic_0108272792_table13922888141527"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108272792_row229143141527"><th class="cellrowborder" valign="top" width="28.110000000000003%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272792_p66756185141527"><a name="zh-cn_topic_0108272792_p66756185141527"></a><a name="zh-cn_topic_0108272792_p66756185141527"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="19.02%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272792_p38541938141527"><a name="zh-cn_topic_0108272792_p38541938141527"></a><a name="zh-cn_topic_0108272792_p38541938141527"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.62%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272792_p34889279141527"><a name="zh-cn_topic_0108272792_p34889279141527"></a><a name="zh-cn_topic_0108272792_p34889279141527"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="35.25%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272792_p7459369141527"><a name="zh-cn_topic_0108272792_p7459369141527"></a><a name="zh-cn_topic_0108272792_p7459369141527"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108272792_row43782953195111"><td class="cellrowborder" valign="top" width="28.110000000000003%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272792_p20190464195123"><a name="zh-cn_topic_0108272792_p20190464195123"></a><a name="zh-cn_topic_0108272792_p20190464195123"></a>linkConfig.protocol</p>
</td>
<td class="cellrowborder" valign="top" width="19.02%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272792_p24814912195123"><a name="zh-cn_topic_0108272792_p24814912195123"></a><a name="zh-cn_topic_0108272792_p24814912195123"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.62%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272792_p63850873195123"><a name="zh-cn_topic_0108272792_p63850873195123"></a><a name="zh-cn_topic_0108272792_p63850873195123"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="35.25%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272792_p4538194195123"><a name="zh-cn_topic_0108272792_p4538194195123"></a><a name="zh-cn_topic_0108272792_p4538194195123"></a>NAS文件协议，目前只支持SMB/CIFS/NFS协议。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272792_row2725489141730"><td class="cellrowborder" valign="top" width="28.110000000000003%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272792_p18261829141730"><a name="zh-cn_topic_0108272792_p18261829141730"></a><a name="zh-cn_topic_0108272792_p18261829141730"></a>linkConfig.server</p>
</td>
<td class="cellrowborder" valign="top" width="19.02%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272792_p2813219141730"><a name="zh-cn_topic_0108272792_p2813219141730"></a><a name="zh-cn_topic_0108272792_p2813219141730"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.62%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272792_p26544197141730"><a name="zh-cn_topic_0108272792_p26544197141730"></a><a name="zh-cn_topic_0108272792_p26544197141730"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="35.25%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272792_p2596372141730"><a name="zh-cn_topic_0108272792_p2596372141730"></a><a name="zh-cn_topic_0108272792_p2596372141730"></a>NAS服务器的共享路径，<span class="uicontrol" id="zh-cn_topic_0108272792_uicontrol18465103004915"><a name="zh-cn_topic_0108272792_uicontrol18465103004915"></a><a name="zh-cn_topic_0108272792_uicontrol18465103004915"></a>“\\\\”</span>转义后为<span class="uicontrol" id="zh-cn_topic_0108272792_uicontrol1995184817498"><a name="zh-cn_topic_0108272792_uicontrol1995184817498"></a><a name="zh-cn_topic_0108272792_uicontrol1995184817498"></a>“\\”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272792_row14946728141730"><td class="cellrowborder" valign="top" width="28.110000000000003%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272792_p7204562141730"><a name="zh-cn_topic_0108272792_p7204562141730"></a><a name="zh-cn_topic_0108272792_p7204562141730"></a>linkConfig.username</p>
</td>
<td class="cellrowborder" valign="top" width="19.02%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272792_p46698681141730"><a name="zh-cn_topic_0108272792_p46698681141730"></a><a name="zh-cn_topic_0108272792_p46698681141730"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.62%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272792_p24496779141730"><a name="zh-cn_topic_0108272792_p24496779141730"></a><a name="zh-cn_topic_0108272792_p24496779141730"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="35.25%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272792_p38082098141730"><a name="zh-cn_topic_0108272792_p38082098141730"></a><a name="zh-cn_topic_0108272792_p38082098141730"></a>登录NAS服务器的用户名。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272792_row53856530141730"><td class="cellrowborder" valign="top" width="28.110000000000003%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272792_p45889226141730"><a name="zh-cn_topic_0108272792_p45889226141730"></a><a name="zh-cn_topic_0108272792_p45889226141730"></a>linkConfig.password</p>
</td>
<td class="cellrowborder" valign="top" width="19.02%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272792_p26039827141730"><a name="zh-cn_topic_0108272792_p26039827141730"></a><a name="zh-cn_topic_0108272792_p26039827141730"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.62%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272792_p28851277141730"><a name="zh-cn_topic_0108272792_p28851277141730"></a><a name="zh-cn_topic_0108272792_p28851277141730"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="35.25%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272792_p55252128141730"><a name="zh-cn_topic_0108272792_p55252128141730"></a><a name="zh-cn_topic_0108272792_p55252128141730"></a>登录用户的密码。</p>
</td>
</tr>
</tbody>
</table>

