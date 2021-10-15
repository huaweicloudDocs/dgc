# Redis/DCS连接（待下线）<a name="dgc_02_0272"></a>

## 介绍<a name="zh-cn_topic_0108272833_section621837"></a>

通过Redis连接，可以对Redis服务器抽取或加载数据；通过DCS连接，可以加载数据到DCS（不支持从DCS抽取数据），支持“string“和“hash“两种数据存储格式。

## 连接样例<a name="zh-cn_topic_0108272833_section6163607716523"></a>

```
{
    "links": [
        {
            "link-config-values": {
                "configs": [
                    {
                        "inputs": [
                            {
                                "name": "linkConfig.deploymentMode",
                                "value": "Cluster"
                            },
                            {
                                "name": "linkConfig.serverlist",
                                "value": "10.120.84.149:7300"
                            },
                            {
                                "name": "linkConfig.password",
                                "value": "Add password here"
                            },
                            {
                                "name": "linkConfig.dbIndex",
                                "value": "0"
                            }
                        ],
                        "name": "linkConfig"
                    }
                ]
            },
            "name": "redis_link",
            "connector-name": "redis-connector"
        }
    ]
}
```

## 连接参数<a name="zh-cn_topic_0108272833_section5035508012043"></a>

<a name="zh-cn_topic_0108272833_table13922888141527"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108272833_row229143141527"><th class="cellrowborder" valign="top" width="28.672867286728675%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272833_p66756185141527"><a name="zh-cn_topic_0108272833_p66756185141527"></a><a name="zh-cn_topic_0108272833_p66756185141527"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="19.221922192219225%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272833_p38541938141527"><a name="zh-cn_topic_0108272833_p38541938141527"></a><a name="zh-cn_topic_0108272833_p38541938141527"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.981498149814982%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272833_p34889279141527"><a name="zh-cn_topic_0108272833_p34889279141527"></a><a name="zh-cn_topic_0108272833_p34889279141527"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="37.12371237123712%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272833_p7459369141527"><a name="zh-cn_topic_0108272833_p7459369141527"></a><a name="zh-cn_topic_0108272833_p7459369141527"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108272833_row29069648172636"><td class="cellrowborder" valign="top" width="28.672867286728675%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272833_p3324501172653"><a name="zh-cn_topic_0108272833_p3324501172653"></a><a name="zh-cn_topic_0108272833_p3324501172653"></a>linkConfig.deploymentMode</p>
</td>
<td class="cellrowborder" valign="top" width="19.221922192219225%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272833_p849189172653"><a name="zh-cn_topic_0108272833_p849189172653"></a><a name="zh-cn_topic_0108272833_p849189172653"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.981498149814982%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272833_p1675502172653"><a name="zh-cn_topic_0108272833_p1675502172653"></a><a name="zh-cn_topic_0108272833_p1675502172653"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="37.12371237123712%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272833_p1497943172653"><a name="zh-cn_topic_0108272833_p1497943172653"></a><a name="zh-cn_topic_0108272833_p1497943172653"></a>Redis部署方式：</p>
<a name="zh-cn_topic_0108272833_ul13481487172653"></a><a name="zh-cn_topic_0108272833_ul13481487172653"></a><ul id="zh-cn_topic_0108272833_ul13481487172653"><li>Single：表示单机部署。</li><li>Cluster：表示集群部署。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0108272833_row2725489141730"><td class="cellrowborder" valign="top" width="28.672867286728675%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272833_p18261829141730"><a name="zh-cn_topic_0108272833_p18261829141730"></a><a name="zh-cn_topic_0108272833_p18261829141730"></a>linkConfig.serverlist</p>
</td>
<td class="cellrowborder" valign="top" width="19.221922192219225%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272833_p2813219141730"><a name="zh-cn_topic_0108272833_p2813219141730"></a><a name="zh-cn_topic_0108272833_p2813219141730"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.981498149814982%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272833_p26544197141730"><a name="zh-cn_topic_0108272833_p26544197141730"></a><a name="zh-cn_topic_0108272833_p26544197141730"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="37.12371237123712%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272833_p2596372141730"><a name="zh-cn_topic_0108272833_p2596372141730"></a><a name="zh-cn_topic_0108272833_p2596372141730"></a>服务器地址列表，格式如：<span class="parmvalue" id="zh-cn_topic_0108272833_parmvalue31186725145645"><a name="zh-cn_topic_0108272833_parmvalue31186725145645"></a><a name="zh-cn_topic_0108272833_parmvalue31186725145645"></a>“host1:port1;host2:port2”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272833_row53856530141730"><td class="cellrowborder" valign="top" width="28.672867286728675%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272833_p45889226141730"><a name="zh-cn_topic_0108272833_p45889226141730"></a><a name="zh-cn_topic_0108272833_p45889226141730"></a>linkConfig.password</p>
</td>
<td class="cellrowborder" valign="top" width="19.221922192219225%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272833_p26039827141730"><a name="zh-cn_topic_0108272833_p26039827141730"></a><a name="zh-cn_topic_0108272833_p26039827141730"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.981498149814982%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272833_p28851277141730"><a name="zh-cn_topic_0108272833_p28851277141730"></a><a name="zh-cn_topic_0108272833_p28851277141730"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="37.12371237123712%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272833_p55252128141730"><a name="zh-cn_topic_0108272833_p55252128141730"></a><a name="zh-cn_topic_0108272833_p55252128141730"></a>连接Redis服务器的密码。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272833_row15539429151915"><td class="cellrowborder" valign="top" width="28.672867286728675%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272833_p55356658172646"><a name="zh-cn_topic_0108272833_p55356658172646"></a><a name="zh-cn_topic_0108272833_p55356658172646"></a>linkConfig.dbIndex</p>
</td>
<td class="cellrowborder" valign="top" width="19.221922192219225%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272833_p48938698172646"><a name="zh-cn_topic_0108272833_p48938698172646"></a><a name="zh-cn_topic_0108272833_p48938698172646"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.981498149814982%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272833_p13974271172646"><a name="zh-cn_topic_0108272833_p13974271172646"></a><a name="zh-cn_topic_0108272833_p13974271172646"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="37.12371237123712%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272833_p43475400172646"><a name="zh-cn_topic_0108272833_p43475400172646"></a><a name="zh-cn_topic_0108272833_p43475400172646"></a>Redis数据库索引。</p>
</td>
</tr>
</tbody>
</table>

