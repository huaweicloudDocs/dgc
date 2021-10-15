# HBase连接<a name="dgc_02_0267"></a>

## 介绍<a name="zh-cn_topic_0109665329_section12903857173911"></a>

通过HBase连接，可以对MRS、FusionInsight HD、Apache Hadoop的HBase抽取、加载数据。

## 连接样例<a name="zh-cn_topic_0109665329_section6163607716523"></a>

```
{
  "links": [
    {
      "link-config-values": {
        "configs": [
          {
            "inputs": [
              {
                "name": "linkConfig.hbaseType",
                "value": "MRS"
              },
              {
                "name": "linkConfig.host",
                "value": "192.168.2.23"
              },
              {
                "name": "linkConfig.authType",
                "value": "SIMPLE"
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
      "name": "mrshbase",
      "connector-name": "hbase-connector"
    }
  ]
}
```

## 连接参数<a name="zh-cn_topic_0109665329_section37929003173911"></a>

<a name="zh-cn_topic_0109665329_table52350397173911"></a>
<table><thead align="left"><tr id="zh-cn_topic_0109665329_row42443862173911"><th class="cellrowborder" valign="top" width="19.84%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0109665329_p15400793173911"><a name="zh-cn_topic_0109665329_p15400793173911"></a><a name="zh-cn_topic_0109665329_p15400793173911"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20.34%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0109665329_p39504729173911"><a name="zh-cn_topic_0109665329_p39504729173911"></a><a name="zh-cn_topic_0109665329_p39504729173911"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="16.68%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0109665329_p45766461173911"><a name="zh-cn_topic_0109665329_p45766461173911"></a><a name="zh-cn_topic_0109665329_p45766461173911"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="43.14%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0109665329_p16095854173911"><a name="zh-cn_topic_0109665329_p16095854173911"></a><a name="zh-cn_topic_0109665329_p16095854173911"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0109665329_row28695763173911"><td class="cellrowborder" valign="top" width="19.84%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0109665329_p42655444173911"><a name="zh-cn_topic_0109665329_p42655444173911"></a><a name="zh-cn_topic_0109665329_p42655444173911"></a>linkConfig.hbaseType</p>
</td>
<td class="cellrowborder" valign="top" width="20.34%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0109665329_p32538971173911"><a name="zh-cn_topic_0109665329_p32538971173911"></a><a name="zh-cn_topic_0109665329_p32538971173911"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.68%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0109665329_p18410957173911"><a name="zh-cn_topic_0109665329_p18410957173911"></a><a name="zh-cn_topic_0109665329_p18410957173911"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="43.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0109665329_p42728221113647"><a name="zh-cn_topic_0109665329_p42728221113647"></a><a name="zh-cn_topic_0109665329_p42728221113647"></a>HBase类型：</p>
<a name="zh-cn_topic_0109665329_ul23819850113656"></a><a name="zh-cn_topic_0109665329_ul23819850113656"></a><ul id="zh-cn_topic_0109665329_ul23819850113656"><li>CloudTable：表示连接CloudTable服务。</li><li>MRS：表示连接MRS的HBase。</li><li>FusionInsight HD：表示连接FusionInsight HD的HBase。</li><li>Apache Hadoop：表示连接开源Apache Hadoop的HBase。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0109665329_row19735109203218"><td class="cellrowborder" valign="top" width="19.84%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0109665329_p30068829175124"><a name="zh-cn_topic_0109665329_p30068829175124"></a><a name="zh-cn_topic_0109665329_p30068829175124"></a>linkConfig.uri</p>
</td>
<td class="cellrowborder" valign="top" width="20.34%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0109665329_p379375175124"><a name="zh-cn_topic_0109665329_p379375175124"></a><a name="zh-cn_topic_0109665329_p379375175124"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.68%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0109665329_p46443378175124"><a name="zh-cn_topic_0109665329_p46443378175124"></a><a name="zh-cn_topic_0109665329_p46443378175124"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0109665329_p1975013933212"><a name="zh-cn_topic_0109665329_p1975013933212"></a><a name="zh-cn_topic_0109665329_p1975013933212"></a>连接Apache Hadoop时的Namenode URI地址，格式为<span class="uicontrol" id="zh-cn_topic_0109665329_zh-cn_topic_0108272817_uicontrol9492030193730"><a name="zh-cn_topic_0109665329_zh-cn_topic_0108272817_uicontrol9492030193730"></a><a name="zh-cn_topic_0109665329_zh-cn_topic_0108272817_uicontrol9492030193730"></a>“ip:port”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0109665329_row66924219173911"><td class="cellrowborder" valign="top" width="19.84%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0109665329_p52152668173911"><a name="zh-cn_topic_0109665329_p52152668173911"></a><a name="zh-cn_topic_0109665329_p52152668173911"></a>llinkConfig.host</p>
</td>
<td class="cellrowborder" valign="top" width="20.34%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0109665329_p63616581173911"><a name="zh-cn_topic_0109665329_p63616581173911"></a><a name="zh-cn_topic_0109665329_p63616581173911"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.68%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0109665329_p52669471173911"><a name="zh-cn_topic_0109665329_p52669471173911"></a><a name="zh-cn_topic_0109665329_p52669471173911"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0109665329_p38368786173911"><a name="zh-cn_topic_0109665329_p38368786173911"></a><a name="zh-cn_topic_0109665329_p38368786173911"></a>连接MRS或FusionInsight HD时，需要配置Manager平台的IP地址。</p>
</td>
</tr>
<tr id="zh-cn_topic_0109665329_row15568114462"><td class="cellrowborder" valign="top" width="19.84%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0109665329_p197211134613"><a name="zh-cn_topic_0109665329_p197211134613"></a><a name="zh-cn_topic_0109665329_p197211134613"></a>linkConfig.port</p>
</td>
<td class="cellrowborder" valign="top" width="20.34%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0109665329_p5315558133512"><a name="zh-cn_topic_0109665329_p5315558133512"></a><a name="zh-cn_topic_0109665329_p5315558133512"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.68%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0109665329_p33154583355"><a name="zh-cn_topic_0109665329_p33154583355"></a><a name="zh-cn_topic_0109665329_p33154583355"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0109665329_p2072161164620"><a name="zh-cn_topic_0109665329_p2072161164620"></a><a name="zh-cn_topic_0109665329_p2072161164620"></a>连接FusionInsight HD时，需要配置Manager平台的端口。</p>
</td>
</tr>
<tr id="zh-cn_topic_0109665329_row14983106114314"><td class="cellrowborder" valign="top" width="19.84%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0109665329_p1998356124316"><a name="zh-cn_topic_0109665329_p1998356124316"></a><a name="zh-cn_topic_0109665329_p1998356124316"></a>linkConfig.casPort</p>
</td>
<td class="cellrowborder" valign="top" width="20.34%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0109665329_p268930133618"><a name="zh-cn_topic_0109665329_p268930133618"></a><a name="zh-cn_topic_0109665329_p268930133618"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.68%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0109665329_p17689009367"><a name="zh-cn_topic_0109665329_p17689009367"></a><a name="zh-cn_topic_0109665329_p17689009367"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0109665329_p18983136204311"><a name="zh-cn_topic_0109665329_p18983136204311"></a><a name="zh-cn_topic_0109665329_p18983136204311"></a>连接FusionInsight HD时，需要配置与FusionInsight HD对接的CAS Server的端口。</p>
</td>
</tr>
<tr id="zh-cn_topic_0109665329_row76704714314"><td class="cellrowborder" valign="top" width="19.84%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0109665329_p1567019719436"><a name="zh-cn_topic_0109665329_p1567019719436"></a><a name="zh-cn_topic_0109665329_p1567019719436"></a>linkConfig.user</p>
</td>
<td class="cellrowborder" valign="top" width="20.34%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0109665329_p154701718362"><a name="zh-cn_topic_0109665329_p154701718362"></a><a name="zh-cn_topic_0109665329_p154701718362"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.68%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0109665329_p1347051143620"><a name="zh-cn_topic_0109665329_p1347051143620"></a><a name="zh-cn_topic_0109665329_p1347051143620"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0109665329_p1167018744317"><a name="zh-cn_topic_0109665329_p1167018744317"></a><a name="zh-cn_topic_0109665329_p1167018744317"></a>登录Manager平台的用户名。连接MRS时，如果使用Simple认证，则不用输入Manager用户名、密码。</p>
</td>
</tr>
<tr id="zh-cn_topic_0109665329_row33434818432"><td class="cellrowborder" valign="top" width="19.84%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0109665329_p1234310844315"><a name="zh-cn_topic_0109665329_p1234310844315"></a><a name="zh-cn_topic_0109665329_p1234310844315"></a>linkConfig.password</p>
</td>
<td class="cellrowborder" valign="top" width="20.34%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0109665329_p4221926369"><a name="zh-cn_topic_0109665329_p4221926369"></a><a name="zh-cn_topic_0109665329_p4221926369"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.68%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0109665329_p1022116213365"><a name="zh-cn_topic_0109665329_p1022116213365"></a><a name="zh-cn_topic_0109665329_p1022116213365"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0109665329_p143436814315"><a name="zh-cn_topic_0109665329_p143436814315"></a><a name="zh-cn_topic_0109665329_p143436814315"></a>登录Manager平台的密码。连接MRS时，如果使用Simple认证，则不用输入Manager用户名、密码。</p>
</td>
</tr>
<tr id="zh-cn_topic_0109665329_row159351483434"><td class="cellrowborder" valign="top" width="19.84%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0109665329_p17935138204310"><a name="zh-cn_topic_0109665329_p17935138204310"></a><a name="zh-cn_topic_0109665329_p17935138204310"></a>linkConfig.authType</p>
</td>
<td class="cellrowborder" valign="top" width="20.34%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0109665329_p43871655175124"><a name="zh-cn_topic_0109665329_p43871655175124"></a><a name="zh-cn_topic_0109665329_p43871655175124"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.68%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0109665329_p32281241175124"><a name="zh-cn_topic_0109665329_p32281241175124"></a><a name="zh-cn_topic_0109665329_p32281241175124"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="43.14%" headers="mcps1.1.5.1.4 "><div class="p" id="zh-cn_topic_0109665329_p1793518134318"><a name="zh-cn_topic_0109665329_p1793518134318"></a><a name="zh-cn_topic_0109665329_p1793518134318"></a>认证类型，分为以下两种：<a name="zh-cn_topic_0109665329_zh-cn_topic_0108272817_ul320611711334"></a><a name="zh-cn_topic_0109665329_zh-cn_topic_0108272817_ul320611711334"></a><ul id="zh-cn_topic_0109665329_zh-cn_topic_0108272817_ul320611711334"><li>Simple：非安全模式选择Simple鉴权。</li><li>Kerberos：安全模式选择Kerberos鉴权。</li></ul>
</div>
</td>
</tr>
<tr id="zh-cn_topic_0109665329_row15471111273613"><td class="cellrowborder" valign="top" width="19.84%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0109665329_p46966235175124"><a name="zh-cn_topic_0109665329_p46966235175124"></a><a name="zh-cn_topic_0109665329_p46966235175124"></a>linkConfig.principal</p>
</td>
<td class="cellrowborder" valign="top" width="20.34%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0109665329_p11678433175124"><a name="zh-cn_topic_0109665329_p11678433175124"></a><a name="zh-cn_topic_0109665329_p11678433175124"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.68%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0109665329_p22966577175124"><a name="zh-cn_topic_0109665329_p22966577175124"></a><a name="zh-cn_topic_0109665329_p22966577175124"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0109665329_p35669338174624"><a name="zh-cn_topic_0109665329_p35669338174624"></a><a name="zh-cn_topic_0109665329_p35669338174624"></a>Kerberos认证所需的Principal，您可以联系管理员获取此帐号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0109665329_row16231593439"><td class="cellrowborder" valign="top" width="19.84%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0109665329_p4482790922835"><a name="zh-cn_topic_0109665329_p4482790922835"></a><a name="zh-cn_topic_0109665329_p4482790922835"></a>linkConfig.keytab</p>
</td>
<td class="cellrowborder" valign="top" width="20.34%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0109665329_p718200822835"><a name="zh-cn_topic_0109665329_p718200822835"></a><a name="zh-cn_topic_0109665329_p718200822835"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.68%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0109665329_p58832454114040"><a name="zh-cn_topic_0109665329_p58832454114040"></a><a name="zh-cn_topic_0109665329_p58832454114040"></a>FileContent</p>
</td>
<td class="cellrowborder" valign="top" width="43.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0109665329_p37696402174620"><a name="zh-cn_topic_0109665329_p37696402174620"></a><a name="zh-cn_topic_0109665329_p37696402174620"></a>Kerberos认证所需的keytab文件的本地绝对路径，您可以联系管理员获取此文件。</p>
</td>
</tr>
<tr id="zh-cn_topic_0109665329_row7439182225012"><td class="cellrowborder" valign="top" width="19.84%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0109665329_p1745472218507"><a name="zh-cn_topic_0109665329_p1745472218507"></a><a name="zh-cn_topic_0109665329_p1745472218507"></a>linkConfig.serviceType</p>
</td>
<td class="cellrowborder" valign="top" width="20.34%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0109665329_p84541522125017"><a name="zh-cn_topic_0109665329_p84541522125017"></a><a name="zh-cn_topic_0109665329_p84541522125017"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.68%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0109665329_p54541122125010"><a name="zh-cn_topic_0109665329_p54541122125010"></a><a name="zh-cn_topic_0109665329_p54541122125010"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0109665329_p1545462212507"><a name="zh-cn_topic_0109665329_p1545462212507"></a><a name="zh-cn_topic_0109665329_p1545462212507"></a>服务类型。</p>
</td>
</tr>
<tr id="zh-cn_topic_0109665329_row17224012592"><td class="cellrowborder" valign="top" width="19.84%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0109665329_p1972210155917"><a name="zh-cn_topic_0109665329_p1972210155917"></a><a name="zh-cn_topic_0109665329_p1972210155917"></a>linkConfig.runMode</p>
</td>
<td class="cellrowborder" valign="top" width="20.34%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0109665329_p77221014591"><a name="zh-cn_topic_0109665329_p77221014591"></a><a name="zh-cn_topic_0109665329_p77221014591"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.68%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0109665329_p572211055919"><a name="zh-cn_topic_0109665329_p572211055919"></a><a name="zh-cn_topic_0109665329_p572211055919"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="43.14%" headers="mcps1.1.5.1.4 "><div class="p" id="zh-cn_topic_0109665329_p31105185914"><a name="zh-cn_topic_0109665329_p31105185914"></a><a name="zh-cn_topic_0109665329_p31105185914"></a>选择HBase连接的运行模式：<a name="zh-cn_topic_0109665329_ul1747017597574"></a><a name="zh-cn_topic_0109665329_ul1747017597574"></a><ul id="zh-cn_topic_0109665329_ul1747017597574"><li>EMBEDDED：连接实例与CDM运行在一起，该模式性能较好。</li><li>STANDALONE：连接实例运行在独立进程。如果CDM需要对接多个Hadoop数据源（MRS、Hadoop或CloudTable），并且既有KERBEROS认证模式又有SIMPLE认证模式，只能使用STANDALONE模式。</li></ul>
</div>
</td>
</tr>
</tbody>
</table>

