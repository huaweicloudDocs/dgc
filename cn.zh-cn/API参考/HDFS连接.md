# HDFS连接<a name="dgc_02_0266"></a>

## 介绍<a name="zh-cn_topic_0108272817_section621837"></a>

通过HDFS连接，可以对MRS、FusionInsight HD或开源Hadoop的HDFS抽取、加载文件，支持CSV、Parquet和二进制格式。

## 连接样例<a name="zh-cn_topic_0108272817_section6163607716523"></a>

```
{
    "links": [
        {
            "link-config-values": {
                "configs": [
                    {
                        "inputs": [
                            {
                                "name": "linkConfig.hadoopType",
                                "value": "FusionInsight HD"
                            },
                            {
                                "name": "linkConfig.host",
                                "value": "10.120.205.143"
                            },
                            {
                                "name": "linkConfig.casPort",
                                "value": "20009"
                            },
                            {
                                "name": "linkConfig.port",
                                "value": "28443"
                            },
                            {
                                "name": "linkConfig.authType",
                                "value": "KERBEROS"
                            },
                            {
                                "name": "linkConfig.user",
                                "value": "admin"
                            },
                            {
                                "name": "linkConfig.password",
                                "value": "Add password here"
                            },
                            {
                                "name": "linkConfig.runMode",
                                "value": "STANDALONE"
                            }
                        ],
                        "name": "linkConfig"
                    }
                ]
            },
            "name": "hdfslink",
            "connector-name": "hdfs-connector"
        }
    ]
}
```

## 连接参数<a name="zh-cn_topic_0108272817_section5035508012043"></a>

<a name="zh-cn_topic_0108272817_table13922888141527"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108272817_row229143141527"><th class="cellrowborder" valign="top" width="20.96%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272817_p66756185141527"><a name="zh-cn_topic_0108272817_p66756185141527"></a><a name="zh-cn_topic_0108272817_p66756185141527"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20.91%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272817_p38541938141527"><a name="zh-cn_topic_0108272817_p38541938141527"></a><a name="zh-cn_topic_0108272817_p38541938141527"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.73%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272817_p34889279141527"><a name="zh-cn_topic_0108272817_p34889279141527"></a><a name="zh-cn_topic_0108272817_p34889279141527"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.4%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272817_p7459369141527"><a name="zh-cn_topic_0108272817_p7459369141527"></a><a name="zh-cn_topic_0108272817_p7459369141527"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108272817_row2725489141730"><td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272817_p31327482175124"><a name="zh-cn_topic_0108272817_p31327482175124"></a><a name="zh-cn_topic_0108272817_p31327482175124"></a>linkConfig.hadoopType</p>
</td>
<td class="cellrowborder" valign="top" width="20.91%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272817_p19211512175124"><a name="zh-cn_topic_0108272817_p19211512175124"></a><a name="zh-cn_topic_0108272817_p19211512175124"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.73%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272817_p19590909175124"><a name="zh-cn_topic_0108272817_p19590909175124"></a><a name="zh-cn_topic_0108272817_p19590909175124"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="42.4%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272817_p40849601113150"><a name="zh-cn_topic_0108272817_p40849601113150"></a><a name="zh-cn_topic_0108272817_p40849601113150"></a>Hadoop类型：</p>
<a name="zh-cn_topic_0108272817_ul49344411321"></a><a name="zh-cn_topic_0108272817_ul49344411321"></a><ul id="zh-cn_topic_0108272817_ul49344411321"><li>MRS：表示连接MRS的HDFS。</li><li>FusionInsight HD：表示连接FusionInsight HD的HDFS。</li><li>Apache Hadoop：表示连接开源Apache Hadoop的HDFS。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0108272817_row302832141730"><td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272817_p30068829175124"><a name="zh-cn_topic_0108272817_p30068829175124"></a><a name="zh-cn_topic_0108272817_p30068829175124"></a>linkConfig.uri</p>
</td>
<td class="cellrowborder" valign="top" width="20.91%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272817_p379375175124"><a name="zh-cn_topic_0108272817_p379375175124"></a><a name="zh-cn_topic_0108272817_p379375175124"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.73%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272817_p46443378175124"><a name="zh-cn_topic_0108272817_p46443378175124"></a><a name="zh-cn_topic_0108272817_p46443378175124"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.4%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272817_p50220406175124"><a name="zh-cn_topic_0108272817_p50220406175124"></a><a name="zh-cn_topic_0108272817_p50220406175124"></a>连接Apache Hadoop时的Namenode URI地址，格式为<span class="uicontrol" id="zh-cn_topic_0108272817_uicontrol9492030193730"><a name="zh-cn_topic_0108272817_uicontrol9492030193730"></a><a name="zh-cn_topic_0108272817_uicontrol9492030193730"></a>“ip:port”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272817_row50442567191550"><td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272817_p59316094191550"><a name="zh-cn_topic_0108272817_p59316094191550"></a><a name="zh-cn_topic_0108272817_p59316094191550"></a>linkConfig.host</p>
</td>
<td class="cellrowborder" valign="top" width="20.91%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272817_p782000191843"><a name="zh-cn_topic_0108272817_p782000191843"></a><a name="zh-cn_topic_0108272817_p782000191843"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.73%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272817_p63342026191843"><a name="zh-cn_topic_0108272817_p63342026191843"></a><a name="zh-cn_topic_0108272817_p63342026191843"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.4%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272817_p25133216191550"><a name="zh-cn_topic_0108272817_p25133216191550"></a><a name="zh-cn_topic_0108272817_p25133216191550"></a>连接MRS或FusionInsight HD时，需要配置Manager平台的IP地址。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272817_row23965116817"><td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272817_p51105455191612"><a name="zh-cn_topic_0108272817_p51105455191612"></a><a name="zh-cn_topic_0108272817_p51105455191612"></a>linkConfig.port</p>
</td>
<td class="cellrowborder" valign="top" width="20.91%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272817_p56079990191848"><a name="zh-cn_topic_0108272817_p56079990191848"></a><a name="zh-cn_topic_0108272817_p56079990191848"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.73%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272817_p46185322191848"><a name="zh-cn_topic_0108272817_p46185322191848"></a><a name="zh-cn_topic_0108272817_p46185322191848"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.4%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272817_p3913811183515"><a name="zh-cn_topic_0108272817_p3913811183515"></a><a name="zh-cn_topic_0108272817_p3913811183515"></a>连接FusionInsight HD时，需要配置Manager平台的端口。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272817_row44965011191611"><td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272817_p18287275191611"><a name="zh-cn_topic_0108272817_p18287275191611"></a><a name="zh-cn_topic_0108272817_p18287275191611"></a>linkConfig.casPort</p>
</td>
<td class="cellrowborder" valign="top" width="20.91%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272817_p42854722191846"><a name="zh-cn_topic_0108272817_p42854722191846"></a><a name="zh-cn_topic_0108272817_p42854722191846"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.73%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272817_p48680453191846"><a name="zh-cn_topic_0108272817_p48680453191846"></a><a name="zh-cn_topic_0108272817_p48680453191846"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.4%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272817_p36596319191611"><a name="zh-cn_topic_0108272817_p36596319191611"></a><a name="zh-cn_topic_0108272817_p36596319191611"></a>连接FusionInsight HD时，需要配置与FusionInsight HD对接的CAS Server的端口。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272817_row12723067191613"><td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272817_p23935469191613"><a name="zh-cn_topic_0108272817_p23935469191613"></a><a name="zh-cn_topic_0108272817_p23935469191613"></a>linkConfig.user</p>
</td>
<td class="cellrowborder" valign="top" width="20.91%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272817_p44715260191850"><a name="zh-cn_topic_0108272817_p44715260191850"></a><a name="zh-cn_topic_0108272817_p44715260191850"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.73%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272817_p65166273191850"><a name="zh-cn_topic_0108272817_p65166273191850"></a><a name="zh-cn_topic_0108272817_p65166273191850"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.4%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272817_p15481183410599"><a name="zh-cn_topic_0108272817_p15481183410599"></a><a name="zh-cn_topic_0108272817_p15481183410599"></a>登录Manager平台的用户名。连接MRS时，如果使用Simple认证，则不用输入Manager用户名、密码。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272817_row27957086191613"><td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272817_p49931487191613"><a name="zh-cn_topic_0108272817_p49931487191613"></a><a name="zh-cn_topic_0108272817_p49931487191613"></a>linkConfig.password</p>
</td>
<td class="cellrowborder" valign="top" width="20.91%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272817_p7575218191852"><a name="zh-cn_topic_0108272817_p7575218191852"></a><a name="zh-cn_topic_0108272817_p7575218191852"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.73%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272817_p9612954191852"><a name="zh-cn_topic_0108272817_p9612954191852"></a><a name="zh-cn_topic_0108272817_p9612954191852"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.4%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272817_p199057357597"><a name="zh-cn_topic_0108272817_p199057357597"></a><a name="zh-cn_topic_0108272817_p199057357597"></a>登录Manager平台的密码。连接MRS时，如果使用Simple认证，则不用输入Manager用户名、密码。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272817_row57133381612"><td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272817_p10494739175124"><a name="zh-cn_topic_0108272817_p10494739175124"></a><a name="zh-cn_topic_0108272817_p10494739175124"></a>linkConfig.authType</p>
</td>
<td class="cellrowborder" valign="top" width="20.91%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272817_p43871655175124"><a name="zh-cn_topic_0108272817_p43871655175124"></a><a name="zh-cn_topic_0108272817_p43871655175124"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.73%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272817_p32281241175124"><a name="zh-cn_topic_0108272817_p32281241175124"></a><a name="zh-cn_topic_0108272817_p32281241175124"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="42.4%" headers="mcps1.1.5.1.4 "><div class="p" id="zh-cn_topic_0108272817_p31363547113238"><a name="zh-cn_topic_0108272817_p31363547113238"></a><a name="zh-cn_topic_0108272817_p31363547113238"></a>认证类型，分为以下两种：<a name="zh-cn_topic_0108272817_ul320611711334"></a><a name="zh-cn_topic_0108272817_ul320611711334"></a><ul id="zh-cn_topic_0108272817_ul320611711334"><li>Simple：非安全模式选择Simple鉴权。</li><li>Kerberos：安全模式选择Kerberos鉴权。</li></ul>
</div>
</td>
</tr>
<tr id="zh-cn_topic_0108272817_row5821133914163"><td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272817_p46966235175124"><a name="zh-cn_topic_0108272817_p46966235175124"></a><a name="zh-cn_topic_0108272817_p46966235175124"></a>linkConfig.principal</p>
</td>
<td class="cellrowborder" valign="top" width="20.91%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272817_p11678433175124"><a name="zh-cn_topic_0108272817_p11678433175124"></a><a name="zh-cn_topic_0108272817_p11678433175124"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.73%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272817_p22966577175124"><a name="zh-cn_topic_0108272817_p22966577175124"></a><a name="zh-cn_topic_0108272817_p22966577175124"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.4%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272817_p35669338174624"><a name="zh-cn_topic_0108272817_p35669338174624"></a><a name="zh-cn_topic_0108272817_p35669338174624"></a>Kerberos认证所需的Principal，您可以联系管理员获取此帐号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272817_row468115404169"><td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272817_p4482790922835"><a name="zh-cn_topic_0108272817_p4482790922835"></a><a name="zh-cn_topic_0108272817_p4482790922835"></a>linkConfig.keytab</p>
</td>
<td class="cellrowborder" valign="top" width="20.91%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272817_p718200822835"><a name="zh-cn_topic_0108272817_p718200822835"></a><a name="zh-cn_topic_0108272817_p718200822835"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.73%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272817_p58832454114040"><a name="zh-cn_topic_0108272817_p58832454114040"></a><a name="zh-cn_topic_0108272817_p58832454114040"></a>FileContent</p>
</td>
<td class="cellrowborder" valign="top" width="42.4%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272817_p37696402174620"><a name="zh-cn_topic_0108272817_p37696402174620"></a><a name="zh-cn_topic_0108272817_p37696402174620"></a>Kerberos认证所需的keytab文件的本地绝对路径，您可以联系管理员获取此文件。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272817_row769418475561"><td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272817_p7694174735610"><a name="zh-cn_topic_0108272817_p7694174735610"></a><a name="zh-cn_topic_0108272817_p7694174735610"></a>linkConfig.runMode</p>
</td>
<td class="cellrowborder" valign="top" width="20.91%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272817_p8694164755614"><a name="zh-cn_topic_0108272817_p8694164755614"></a><a name="zh-cn_topic_0108272817_p8694164755614"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.73%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272817_p3694174725618"><a name="zh-cn_topic_0108272817_p3694174725618"></a><a name="zh-cn_topic_0108272817_p3694174725618"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="42.4%" headers="mcps1.1.5.1.4 "><div class="p" id="zh-cn_topic_0108272817_p8372165910575"><a name="zh-cn_topic_0108272817_p8372165910575"></a><a name="zh-cn_topic_0108272817_p8372165910575"></a>选择HDFS连接的运行模式：<a name="zh-cn_topic_0108272817_ul1747017597574"></a><a name="zh-cn_topic_0108272817_ul1747017597574"></a><ul id="zh-cn_topic_0108272817_ul1747017597574"><li>EMBEDDED：连接实例与CDM运行在一起，该模式性能较好。</li><li>STANDALONE：连接实例运行在独立进程。如果CDM需要对接多个Hadoop数据源（MRS、Hadoop或CloudTable），并且既有KERBEROS认证模式又有SIMPLE认证模式，只能使用STANDALONE模式。</li></ul>
</div>
<p id="zh-cn_topic_0108272817_p5211105873913"><a name="zh-cn_topic_0108272817_p5211105873913"></a><a name="zh-cn_topic_0108272817_p5211105873913"></a>选择STANDALONE模式时，CDM支持在多个MRS集群的HDFS之间迁移数据。</p>
</td>
</tr>
</tbody>
</table>

