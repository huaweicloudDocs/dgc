# CloudTable连接<a name="dgc_02_0268"></a>

## 介绍<a name="zh-cn_topic_0108272788_section12903857173911"></a>

通过CloudTable连接，可以对CloudTable服务抽取、加载数据。

## 连接样例<a name="zh-cn_topic_0108272788_section6163607716523"></a>

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
                "value": "CloudTable"
              },
              {
                "name": "linkConfig.zookeeperQuorum",
                "value": "cloudtable-pass-zk2-bae54VGN.cloudtable.com:2181,cloudtable-pass-zk1-Fu828so2.cloudtable.com:2181"
              },
              {
                "name": "linkConfig.iamAuth",
                "value": "true"
              },
              {
                "name": "linkConfig.cloudtableUser",
                "value": "zane"
              },
              {
                "name": "linkConfig.accessKey",
                "value": "GRC2WR0IxxxxxxxYLWU2"
              },
              {
                "name": "linkConfig.securityKey",
                "value": "Add password here"
              },
              {
                "name": "linkConfig.runMode",
                "value": "EMBEDDED"
              }
            ],
            "name": "linkConfig"
          }
        ]
      },
      "name": "cloudtablelink",
      "connector-name": "hbase-connector"
    }
  ]
}
```

## 连接参数<a name="zh-cn_topic_0108272788_section37929003173911"></a>

<a name="zh-cn_topic_0108272788_table52350397173911"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108272788_row42443862173911"><th class="cellrowborder" valign="top" width="19.84%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272788_p15400793173911"><a name="zh-cn_topic_0108272788_p15400793173911"></a><a name="zh-cn_topic_0108272788_p15400793173911"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20.34%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272788_p39504729173911"><a name="zh-cn_topic_0108272788_p39504729173911"></a><a name="zh-cn_topic_0108272788_p39504729173911"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="16.68%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272788_p45766461173911"><a name="zh-cn_topic_0108272788_p45766461173911"></a><a name="zh-cn_topic_0108272788_p45766461173911"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="43.14%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272788_p16095854173911"><a name="zh-cn_topic_0108272788_p16095854173911"></a><a name="zh-cn_topic_0108272788_p16095854173911"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108272788_row28695763173911"><td class="cellrowborder" valign="top" width="19.84%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272788_p42655444173911"><a name="zh-cn_topic_0108272788_p42655444173911"></a><a name="zh-cn_topic_0108272788_p42655444173911"></a>linkConfig.hbaseType</p>
</td>
<td class="cellrowborder" valign="top" width="20.34%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272788_p32538971173911"><a name="zh-cn_topic_0108272788_p32538971173911"></a><a name="zh-cn_topic_0108272788_p32538971173911"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.68%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272788_p18410957173911"><a name="zh-cn_topic_0108272788_p18410957173911"></a><a name="zh-cn_topic_0108272788_p18410957173911"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="43.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272788_p42728221113647"><a name="zh-cn_topic_0108272788_p42728221113647"></a><a name="zh-cn_topic_0108272788_p42728221113647"></a>HBase类型：</p>
<a name="zh-cn_topic_0108272788_ul23819850113656"></a><a name="zh-cn_topic_0108272788_ul23819850113656"></a><ul id="zh-cn_topic_0108272788_ul23819850113656"><li>CloudTable：表示连接CloudTable服务。</li><li>MRS：表示连接MRS。</li><li>FusionInsight HD：表示连接FusionInsight HD。</li><li>Apache Hadoop：表示连接开源Apache Hadoop。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0108272788_row66924219173911"><td class="cellrowborder" valign="top" width="19.84%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272788_p52152668173911"><a name="zh-cn_topic_0108272788_p52152668173911"></a><a name="zh-cn_topic_0108272788_p52152668173911"></a>linkConfig.zookeeperQuorum</p>
</td>
<td class="cellrowborder" valign="top" width="20.34%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272788_p63616581173911"><a name="zh-cn_topic_0108272788_p63616581173911"></a><a name="zh-cn_topic_0108272788_p63616581173911"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.68%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272788_p52669471173911"><a name="zh-cn_topic_0108272788_p52669471173911"></a><a name="zh-cn_topic_0108272788_p52669471173911"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272788_p38368786173911"><a name="zh-cn_topic_0108272788_p38368786173911"></a><a name="zh-cn_topic_0108272788_p38368786173911"></a>连接<span class="parmvalue" id="zh-cn_topic_0108272788_parmvalue4216650316234"><a name="zh-cn_topic_0108272788_parmvalue4216650316234"></a><a name="zh-cn_topic_0108272788_parmvalue4216650316234"></a>“CloudTable”</span>时必选，表示CloudTable的ZooKeeper链接地址。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272788_row112101312133212"><td class="cellrowborder" valign="top" width="19.84%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272788_p72121912133212"><a name="zh-cn_topic_0108272788_p72121912133212"></a><a name="zh-cn_topic_0108272788_p72121912133212"></a>linkConfig.iamAuth</p>
</td>
<td class="cellrowborder" valign="top" width="20.34%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272788_p8212312183216"><a name="zh-cn_topic_0108272788_p8212312183216"></a><a name="zh-cn_topic_0108272788_p8212312183216"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.68%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272788_p621215129321"><a name="zh-cn_topic_0108272788_p621215129321"></a><a name="zh-cn_topic_0108272788_p621215129321"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="43.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272788_p11212161217321"><a name="zh-cn_topic_0108272788_p11212161217321"></a><a name="zh-cn_topic_0108272788_p11212161217321"></a>当选择IAM统一身份认证时，需要输入用户名、AK和SK。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272788_row14704131223213"><td class="cellrowborder" valign="top" width="19.84%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272788_p070420125326"><a name="zh-cn_topic_0108272788_p070420125326"></a><a name="zh-cn_topic_0108272788_p070420125326"></a>linkConfig.runMode</p>
</td>
<td class="cellrowborder" valign="top" width="20.34%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272788_p970441210322"><a name="zh-cn_topic_0108272788_p970441210322"></a><a name="zh-cn_topic_0108272788_p970441210322"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.68%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272788_p4704512113211"><a name="zh-cn_topic_0108272788_p4704512113211"></a><a name="zh-cn_topic_0108272788_p4704512113211"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="43.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272788_p121733311504"><a name="zh-cn_topic_0108272788_p121733311504"></a><a name="zh-cn_topic_0108272788_p121733311504"></a>选择HBase连接的运行模式：</p>
<a name="zh-cn_topic_0108272788_ul192118325256"></a><a name="zh-cn_topic_0108272788_ul192118325256"></a><ul id="zh-cn_topic_0108272788_ul192118325256"><li>EMBEDDED：连接实例与CDM运行在一起，该模式性能较好。</li><li>STANDALONE：连接实例运行在独立进程。如果CDM需要对接多个Hadoop数据源（MRS、Hadoop或CloudTable），并且既有KERBEROS认证模式又有SIMPLE认证模式，只能使用STANDALONE模式。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0108272788_row614271373215"><td class="cellrowborder" valign="top" width="19.84%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272788_p1014251383219"><a name="zh-cn_topic_0108272788_p1014251383219"></a><a name="zh-cn_topic_0108272788_p1014251383219"></a>linkConfig.cloudtableUser</p>
</td>
<td class="cellrowborder" valign="top" width="20.34%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272788_p10142613123214"><a name="zh-cn_topic_0108272788_p10142613123214"></a><a name="zh-cn_topic_0108272788_p10142613123214"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.68%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272788_p9754171773815"><a name="zh-cn_topic_0108272788_p9754171773815"></a><a name="zh-cn_topic_0108272788_p9754171773815"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272788_p13952124417392"><a name="zh-cn_topic_0108272788_p13952124417392"></a><a name="zh-cn_topic_0108272788_p13952124417392"></a>登录CloudTable集群的用户名。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272788_row5580181373217"><td class="cellrowborder" valign="top" width="19.84%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272788_p658231312328"><a name="zh-cn_topic_0108272788_p658231312328"></a><a name="zh-cn_topic_0108272788_p658231312328"></a>linkConfig.accessKey</p>
</td>
<td class="cellrowborder" valign="top" width="20.34%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272788_p5582913123217"><a name="zh-cn_topic_0108272788_p5582913123217"></a><a name="zh-cn_topic_0108272788_p5582913123217"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.68%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272788_p1467312185387"><a name="zh-cn_topic_0108272788_p1467312185387"></a><a name="zh-cn_topic_0108272788_p1467312185387"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272788_p8527134543910"><a name="zh-cn_topic_0108272788_p8527134543910"></a><a name="zh-cn_topic_0108272788_p8527134543910"></a>登录CloudTable集群的访问标识。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272788_row980131415322"><td class="cellrowborder" valign="top" width="19.84%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272788_p1380114153212"><a name="zh-cn_topic_0108272788_p1380114153212"></a><a name="zh-cn_topic_0108272788_p1380114153212"></a>linkConfig.securityKey</p>
</td>
<td class="cellrowborder" valign="top" width="20.34%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272788_p13801914193210"><a name="zh-cn_topic_0108272788_p13801914193210"></a><a name="zh-cn_topic_0108272788_p13801914193210"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.68%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272788_p183301919143814"><a name="zh-cn_topic_0108272788_p183301919143814"></a><a name="zh-cn_topic_0108272788_p183301919143814"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272788_p813194633919"><a name="zh-cn_topic_0108272788_p813194633919"></a><a name="zh-cn_topic_0108272788_p813194633919"></a>登录CloudTable集群的秘钥。</p>
</td>
</tr>
</tbody>
</table>

