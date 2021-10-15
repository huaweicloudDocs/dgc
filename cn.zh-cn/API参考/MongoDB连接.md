# MongoDB连接<a name="dgc_02_0271"></a>

## 介绍<a name="zh-cn_topic_0108272832_section621837"></a>

通过MongoDB连接，可以对MongoDB服务器抽取、加载数据。

## 连接样例<a name="zh-cn_topic_0108272832_section6163607716523"></a>

```
{
    "links": [
        {
            "link-config-values": {
                "configs": [
                    {
                        "inputs": [
                            {
                                "name": "linkConfig.serverList",
                                "value": "10.120.84.149:27017"
                            },
                            {
                                "name": "linkConfig.database",
                                "value": "DB_name"
                            },
                            {
                                "name": "linkConfig.userName",
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
            "name": "mongo_link",
            "connector-name": "mongodb-connector"
        }
    ]
}
```

## 连接参数<a name="zh-cn_topic_0108272832_section5035508012043"></a>

<a name="zh-cn_topic_0108272832_table13922888141527"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108272832_row229143141527"><th class="cellrowborder" valign="top" width="19.84%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272832_p66756185141527"><a name="zh-cn_topic_0108272832_p66756185141527"></a><a name="zh-cn_topic_0108272832_p66756185141527"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20.34%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272832_p38541938141527"><a name="zh-cn_topic_0108272832_p38541938141527"></a><a name="zh-cn_topic_0108272832_p38541938141527"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="16.68%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272832_p34889279141527"><a name="zh-cn_topic_0108272832_p34889279141527"></a><a name="zh-cn_topic_0108272832_p34889279141527"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="43.14%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272832_p7459369141527"><a name="zh-cn_topic_0108272832_p7459369141527"></a><a name="zh-cn_topic_0108272832_p7459369141527"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108272832_row2725489141730"><td class="cellrowborder" valign="top" width="19.84%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272832_p64025194161338"><a name="zh-cn_topic_0108272832_p64025194161338"></a><a name="zh-cn_topic_0108272832_p64025194161338"></a>linkConfig.serverList</p>
</td>
<td class="cellrowborder" valign="top" width="20.34%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272832_p18658186161338"><a name="zh-cn_topic_0108272832_p18658186161338"></a><a name="zh-cn_topic_0108272832_p18658186161338"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.68%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272832_p34918070161338"><a name="zh-cn_topic_0108272832_p34918070161338"></a><a name="zh-cn_topic_0108272832_p34918070161338"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272832_p9791447161338"><a name="zh-cn_topic_0108272832_p9791447161338"></a><a name="zh-cn_topic_0108272832_p9791447161338"></a>服务器地址列表，格式如：<span class="parmvalue" id="zh-cn_topic_0108272832_parmvalue21014167161338"><a name="zh-cn_topic_0108272832_parmvalue21014167161338"></a><a name="zh-cn_topic_0108272832_parmvalue21014167161338"></a>“host1:port1;host2:port2”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272832_row302832141730"><td class="cellrowborder" valign="top" width="19.84%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272832_p18431456161929"><a name="zh-cn_topic_0108272832_p18431456161929"></a><a name="zh-cn_topic_0108272832_p18431456161929"></a>linkConfig.database</p>
</td>
<td class="cellrowborder" valign="top" width="20.34%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272832_p16553004161929"><a name="zh-cn_topic_0108272832_p16553004161929"></a><a name="zh-cn_topic_0108272832_p16553004161929"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.68%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272832_p65724915161929"><a name="zh-cn_topic_0108272832_p65724915161929"></a><a name="zh-cn_topic_0108272832_p65724915161929"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272832_p22117919161929"><a name="zh-cn_topic_0108272832_p22117919161929"></a><a name="zh-cn_topic_0108272832_p22117919161929"></a>MongoDB的数据库名称。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272832_row14946728141730"><td class="cellrowborder" valign="top" width="19.84%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272832_p2311093316183"><a name="zh-cn_topic_0108272832_p2311093316183"></a><a name="zh-cn_topic_0108272832_p2311093316183"></a>linkConfig.userName</p>
</td>
<td class="cellrowborder" valign="top" width="20.34%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272832_p6004628016183"><a name="zh-cn_topic_0108272832_p6004628016183"></a><a name="zh-cn_topic_0108272832_p6004628016183"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.68%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272832_p3191052016183"><a name="zh-cn_topic_0108272832_p3191052016183"></a><a name="zh-cn_topic_0108272832_p3191052016183"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272832_p3461530816183"><a name="zh-cn_topic_0108272832_p3461530816183"></a><a name="zh-cn_topic_0108272832_p3461530816183"></a>连接MongoDB服务器的用户名。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272832_row53856530141730"><td class="cellrowborder" valign="top" width="19.84%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272832_p28305123161714"><a name="zh-cn_topic_0108272832_p28305123161714"></a><a name="zh-cn_topic_0108272832_p28305123161714"></a>linkConfig.password</p>
</td>
<td class="cellrowborder" valign="top" width="20.34%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272832_p11013606161714"><a name="zh-cn_topic_0108272832_p11013606161714"></a><a name="zh-cn_topic_0108272832_p11013606161714"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.68%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272832_p19686865161714"><a name="zh-cn_topic_0108272832_p19686865161714"></a><a name="zh-cn_topic_0108272832_p19686865161714"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272832_p51132237161714"><a name="zh-cn_topic_0108272832_p51132237161714"></a><a name="zh-cn_topic_0108272832_p51132237161714"></a>连接MongoDB服务器的密码。</p>
</td>
</tr>
</tbody>
</table>

