# FTP/SFTP连接<a name="dgc_02_0270"></a>

## 介绍<a name="zh-cn_topic_0108272835_section621837"></a>

通过FTP或SFTP连接，可以对FTP或SFTP服务器抽取或加载文件，支持CSV、二进制和JSON格式。

## 连接样例<a name="zh-cn_topic_0108272835_section6163607716523"></a>

```
{
    "links": [
        {
            "link-config-values": {
                "configs": [
                    {
                        "inputs": [
                            {
                                "name": "linkConfig.server",
                                "value": "10.120.85.167"
                            },
                            {
                                "name": "linkConfig.port",
                                "value": "22"
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
            "name": "sftp_link",
            "connector-name": "sftp-connector"
        }
    ]
}
```

## 连接参数<a name="zh-cn_topic_0108272835_section5035508012043"></a>

FTP和SFTP的连接参数相同。

<a name="zh-cn_topic_0108272835_table13922888141527"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108272835_row229143141527"><th class="cellrowborder" valign="top" width="25.292529252925295%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272835_p66756185141527"><a name="zh-cn_topic_0108272835_p66756185141527"></a><a name="zh-cn_topic_0108272835_p66756185141527"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="19.21192119211921%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272835_p38541938141527"><a name="zh-cn_topic_0108272835_p38541938141527"></a><a name="zh-cn_topic_0108272835_p38541938141527"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.431743174317432%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272835_p34889279141527"><a name="zh-cn_topic_0108272835_p34889279141527"></a><a name="zh-cn_topic_0108272835_p34889279141527"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="38.06380638063806%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272835_p7459369141527"><a name="zh-cn_topic_0108272835_p7459369141527"></a><a name="zh-cn_topic_0108272835_p7459369141527"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108272835_row2725489141730"><td class="cellrowborder" valign="top" width="25.292529252925295%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272835_p18261829141730"><a name="zh-cn_topic_0108272835_p18261829141730"></a><a name="zh-cn_topic_0108272835_p18261829141730"></a>linkConfig.server</p>
</td>
<td class="cellrowborder" valign="top" width="19.21192119211921%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272835_p2813219141730"><a name="zh-cn_topic_0108272835_p2813219141730"></a><a name="zh-cn_topic_0108272835_p2813219141730"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.431743174317432%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272835_p26544197141730"><a name="zh-cn_topic_0108272835_p26544197141730"></a><a name="zh-cn_topic_0108272835_p26544197141730"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.06380638063806%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272835_p2596372141730"><a name="zh-cn_topic_0108272835_p2596372141730"></a><a name="zh-cn_topic_0108272835_p2596372141730"></a>FTP或SFTP服务器的地址。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272835_row302832141730"><td class="cellrowborder" valign="top" width="25.292529252925295%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272835_p13707316141730"><a name="zh-cn_topic_0108272835_p13707316141730"></a><a name="zh-cn_topic_0108272835_p13707316141730"></a>linkConfig.port</p>
</td>
<td class="cellrowborder" valign="top" width="19.21192119211921%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272835_p36550801141730"><a name="zh-cn_topic_0108272835_p36550801141730"></a><a name="zh-cn_topic_0108272835_p36550801141730"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.431743174317432%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272835_p7824886141730"><a name="zh-cn_topic_0108272835_p7824886141730"></a><a name="zh-cn_topic_0108272835_p7824886141730"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.06380638063806%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272835_p29836044141730"><a name="zh-cn_topic_0108272835_p29836044141730"></a><a name="zh-cn_topic_0108272835_p29836044141730"></a>FTP或SFTP服务器端口号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272835_row14946728141730"><td class="cellrowborder" valign="top" width="25.292529252925295%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272835_p7204562141730"><a name="zh-cn_topic_0108272835_p7204562141730"></a><a name="zh-cn_topic_0108272835_p7204562141730"></a>linkConfig.username</p>
</td>
<td class="cellrowborder" valign="top" width="19.21192119211921%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272835_p46698681141730"><a name="zh-cn_topic_0108272835_p46698681141730"></a><a name="zh-cn_topic_0108272835_p46698681141730"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.431743174317432%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272835_p24496779141730"><a name="zh-cn_topic_0108272835_p24496779141730"></a><a name="zh-cn_topic_0108272835_p24496779141730"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.06380638063806%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272835_p38082098141730"><a name="zh-cn_topic_0108272835_p38082098141730"></a><a name="zh-cn_topic_0108272835_p38082098141730"></a>登录FTP或SFTP服务器的用户名。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272835_row53856530141730"><td class="cellrowborder" valign="top" width="25.292529252925295%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272835_p45889226141730"><a name="zh-cn_topic_0108272835_p45889226141730"></a><a name="zh-cn_topic_0108272835_p45889226141730"></a>linkConfig.password</p>
</td>
<td class="cellrowborder" valign="top" width="19.21192119211921%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272835_p26039827141730"><a name="zh-cn_topic_0108272835_p26039827141730"></a><a name="zh-cn_topic_0108272835_p26039827141730"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.431743174317432%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272835_p28851277141730"><a name="zh-cn_topic_0108272835_p28851277141730"></a><a name="zh-cn_topic_0108272835_p28851277141730"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.06380638063806%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272835_p55252128141730"><a name="zh-cn_topic_0108272835_p55252128141730"></a><a name="zh-cn_topic_0108272835_p55252128141730"></a>登录用户的密码。</p>
</td>
</tr>
</tbody>
</table>

