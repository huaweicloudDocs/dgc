# Hive连接<a name="dgc_02_0269"></a>

## 介绍<a name="zh-cn_topic_0108272815_section621837"></a>

通过Hive连接，可以对MRS的Hive数据源进行抽取、加载数据。

## 连接样例<a name="zh-cn_topic_0108272815_section6163607716523"></a>

```
{
  "links": [
    {
      "link-config-values": {
        "configs": [
          {
            "inputs": [
              {
                "name": "linkConfig.host",
                "value": "10.120.205.230"
              },
			  {
                "name": "linkConfig.authType",
                "value": "KERBEROS"
              },
              {
                "name": "linkConfig.user",
                "value": "cdm"
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
      "name": "hive_link",
      "connector-name": "hive-connector"
    }
  ]
}
```

## 连接参数<a name="zh-cn_topic_0108272815_section5035508012043"></a>

<a name="zh-cn_topic_0108272815_table52350397173911"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108272815_row42443862173911"><th class="cellrowborder" valign="top" width="19.84%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272815_p15400793173911"><a name="zh-cn_topic_0108272815_p15400793173911"></a><a name="zh-cn_topic_0108272815_p15400793173911"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20.34%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272815_p39504729173911"><a name="zh-cn_topic_0108272815_p39504729173911"></a><a name="zh-cn_topic_0108272815_p39504729173911"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="16.68%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272815_p45766461173911"><a name="zh-cn_topic_0108272815_p45766461173911"></a><a name="zh-cn_topic_0108272815_p45766461173911"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="43.14%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272815_p16095854173911"><a name="zh-cn_topic_0108272815_p16095854173911"></a><a name="zh-cn_topic_0108272815_p16095854173911"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108272815_row66924219173911"><td class="cellrowborder" valign="top" width="19.84%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272815_p52152668173911"><a name="zh-cn_topic_0108272815_p52152668173911"></a><a name="zh-cn_topic_0108272815_p52152668173911"></a>llinkConfig.host</p>
</td>
<td class="cellrowborder" valign="top" width="20.34%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272815_p63616581173911"><a name="zh-cn_topic_0108272815_p63616581173911"></a><a name="zh-cn_topic_0108272815_p63616581173911"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.68%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272815_p52669471173911"><a name="zh-cn_topic_0108272815_p52669471173911"></a><a name="zh-cn_topic_0108272815_p52669471173911"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272815_p117731251522"><a name="zh-cn_topic_0108272815_p117731251522"></a><a name="zh-cn_topic_0108272815_p117731251522"></a>MRS Manager的IP地址。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272815_row159351483434"><td class="cellrowborder" valign="top" width="19.84%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272815_p17935138204310"><a name="zh-cn_topic_0108272815_p17935138204310"></a><a name="zh-cn_topic_0108272815_p17935138204310"></a>linkConfig.authType</p>
</td>
<td class="cellrowborder" valign="top" width="20.34%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272815_p43871655175124"><a name="zh-cn_topic_0108272815_p43871655175124"></a><a name="zh-cn_topic_0108272815_p43871655175124"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.68%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272815_p32281241175124"><a name="zh-cn_topic_0108272815_p32281241175124"></a><a name="zh-cn_topic_0108272815_p32281241175124"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="43.14%" headers="mcps1.1.5.1.4 "><div class="p" id="zh-cn_topic_0108272815_p121015210521"><a name="zh-cn_topic_0108272815_p121015210521"></a><a name="zh-cn_topic_0108272815_p121015210521"></a>访问MRS的认证类型：<a name="zh-cn_topic_0108272815_ul131011722520"></a><a name="zh-cn_topic_0108272815_ul131011722520"></a><ul id="zh-cn_topic_0108272815_ul131011722520"><li>SIMPLE：非安全模式选择Simple鉴权。</li><li>KERBEROS：安全模式选择Kerberos鉴权。</li></ul>
</div>
</td>
</tr>
<tr id="zh-cn_topic_0108272815_row15471111273613"><td class="cellrowborder" valign="top" width="19.84%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272815_p46966235175124"><a name="zh-cn_topic_0108272815_p46966235175124"></a><a name="zh-cn_topic_0108272815_p46966235175124"></a>linkConfig.principal</p>
</td>
<td class="cellrowborder" valign="top" width="20.34%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272815_p11678433175124"><a name="zh-cn_topic_0108272815_p11678433175124"></a><a name="zh-cn_topic_0108272815_p11678433175124"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.68%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272815_p22966577175124"><a name="zh-cn_topic_0108272815_p22966577175124"></a><a name="zh-cn_topic_0108272815_p22966577175124"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272815_p35669338174624"><a name="zh-cn_topic_0108272815_p35669338174624"></a><a name="zh-cn_topic_0108272815_p35669338174624"></a>Kerberos认证所需的Principal，您可以联系管理员获取此帐号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272815_row16231593439"><td class="cellrowborder" valign="top" width="19.84%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272815_p4482790922835"><a name="zh-cn_topic_0108272815_p4482790922835"></a><a name="zh-cn_topic_0108272815_p4482790922835"></a>linkConfig.keytab</p>
</td>
<td class="cellrowborder" valign="top" width="20.34%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272815_p718200822835"><a name="zh-cn_topic_0108272815_p718200822835"></a><a name="zh-cn_topic_0108272815_p718200822835"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.68%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272815_p58832454114040"><a name="zh-cn_topic_0108272815_p58832454114040"></a><a name="zh-cn_topic_0108272815_p58832454114040"></a>FileContent</p>
</td>
<td class="cellrowborder" valign="top" width="43.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272815_p37696402174620"><a name="zh-cn_topic_0108272815_p37696402174620"></a><a name="zh-cn_topic_0108272815_p37696402174620"></a>Kerberos认证所需的keytab文件的本地绝对路径，您可以联系管理员获取此文件。</p>
</td>
</tr>
</tbody>
</table>

