# CloudTable OpenTSDB连接<a name="dgc_02_0278"></a>

## 介绍<a name="zh-cn_topic_0133483914_section621837"></a>

通过OpenTSDB连接，可以从CloudTable OpenTSDB导入导出数据。

## 连接样例<a name="zh-cn_topic_0133483914_section6163607716523"></a>

```
{
  "links": [
    {
      "link-config-values": {
        "configs": [
          {
            "inputs": [
              {
                "name": "linkConfig.openTSDBQuorum",
                "value": "opentsdb-sp8afz7bgbps5ur.cloudtable.com:4242"
              },
              {
                "name": "linkConfig.securityMode",
                "value": "UNSAFE"
              }
            ],
            "name": "linkConfig"
          }
        ]
      },
      "name": "opentsdb",
      "connector-name": "opentsdb-connector"
    }
  ]
}
```

## 连接参数<a name="zh-cn_topic_0133483914_section5035508012043"></a>

<a name="zh-cn_topic_0133483914_table13922888141527"></a>
<table><thead align="left"><tr id="zh-cn_topic_0133483914_row229143141527"><th class="cellrowborder" valign="top" width="20.03%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0133483914_p66756185141527"><a name="zh-cn_topic_0133483914_p66756185141527"></a><a name="zh-cn_topic_0133483914_p66756185141527"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="21.099999999999998%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0133483914_p38541938141527"><a name="zh-cn_topic_0133483914_p38541938141527"></a><a name="zh-cn_topic_0133483914_p38541938141527"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="16.669999999999998%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0133483914_p34889279141527"><a name="zh-cn_topic_0133483914_p34889279141527"></a><a name="zh-cn_topic_0133483914_p34889279141527"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.199999999999996%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0133483914_p7459369141527"><a name="zh-cn_topic_0133483914_p7459369141527"></a><a name="zh-cn_topic_0133483914_p7459369141527"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0133483914_row335915114596"><td class="cellrowborder" valign="top" width="20.03%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0133483914_p63595113593"><a name="zh-cn_topic_0133483914_p63595113593"></a><a name="zh-cn_topic_0133483914_p63595113593"></a>linkConfig.openTSDBQuorum</p>
</td>
<td class="cellrowborder" valign="top" width="21.099999999999998%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0133483914_p514515141813"><a name="zh-cn_topic_0133483914_p514515141813"></a><a name="zh-cn_topic_0133483914_p514515141813"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.669999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0133483914_p14145614316"><a name="zh-cn_topic_0133483914_p14145614316"></a><a name="zh-cn_topic_0133483914_p14145614316"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.199999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0133483914_p1035981145911"><a name="zh-cn_topic_0133483914_p1035981145911"></a><a name="zh-cn_topic_0133483914_p1035981145911"></a>OpenTSDB的ZooKeeper链接地址。</p>
</td>
</tr>
<tr id="zh-cn_topic_0133483914_row1331858125819"><td class="cellrowborder" valign="top" width="20.03%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0133483914_p631258185815"><a name="zh-cn_topic_0133483914_p631258185815"></a><a name="zh-cn_topic_0133483914_p631258185815"></a>linkConfig.securityMode</p>
</td>
<td class="cellrowborder" valign="top" width="21.099999999999998%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0133483914_p1214519141012"><a name="zh-cn_topic_0133483914_p1214519141012"></a><a name="zh-cn_topic_0133483914_p1214519141012"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.669999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0133483914_p1214512142114"><a name="zh-cn_topic_0133483914_p1214512142114"></a><a name="zh-cn_topic_0133483914_p1214512142114"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.199999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0133483914_p73481116533"><a name="zh-cn_topic_0133483914_p73481116533"></a><a name="zh-cn_topic_0133483914_p73481116533"></a>选择安全或非安全模式。</p>
<p id="zh-cn_topic_0133483914_p10479147165612"><a name="zh-cn_topic_0133483914_p10479147165612"></a><a name="zh-cn_topic_0133483914_p10479147165612"></a>选择安全模式时，需要输入项目ID、用户名、AK/SK。</p>
</td>
</tr>
<tr id="zh-cn_topic_0133483914_row2902138195911"><td class="cellrowborder" valign="top" width="20.03%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0133483914_p107618216186"><a name="zh-cn_topic_0133483914_p107618216186"></a><a name="zh-cn_topic_0133483914_p107618216186"></a>linkConfig.user</p>
</td>
<td class="cellrowborder" valign="top" width="21.099999999999998%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0133483914_p19761112141817"><a name="zh-cn_topic_0133483914_p19761112141817"></a><a name="zh-cn_topic_0133483914_p19761112141817"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.669999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0133483914_p18293152252611"><a name="zh-cn_topic_0133483914_p18293152252611"></a><a name="zh-cn_topic_0133483914_p18293152252611"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.199999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0133483914_p12287142410545"><a name="zh-cn_topic_0133483914_p12287142410545"></a><a name="zh-cn_topic_0133483914_p12287142410545"></a>访问CloudTable服务的用户名。</p>
</td>
</tr>
<tr id="zh-cn_topic_0133483914_row035741185516"><td class="cellrowborder" valign="top" width="20.03%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0133483914_p43117167171152"><a name="zh-cn_topic_0133483914_p43117167171152"></a><a name="zh-cn_topic_0133483914_p43117167171152"></a>linkConfig.ak</p>
</td>
<td class="cellrowborder" valign="top" width="21.099999999999998%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0133483914_p26039827141730"><a name="zh-cn_topic_0133483914_p26039827141730"></a><a name="zh-cn_topic_0133483914_p26039827141730"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.669999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0133483914_p28851277141730"><a name="zh-cn_topic_0133483914_p28851277141730"></a><a name="zh-cn_topic_0133483914_p28851277141730"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.199999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0133483914_p55252128141730"><a name="zh-cn_topic_0133483914_p55252128141730"></a><a name="zh-cn_topic_0133483914_p55252128141730"></a>访问CloudTable服务的AK。</p>
</td>
</tr>
<tr id="zh-cn_topic_0133483914_row17643511195518"><td class="cellrowborder" valign="top" width="20.03%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0133483914_p1852576171211"><a name="zh-cn_topic_0133483914_p1852576171211"></a><a name="zh-cn_topic_0133483914_p1852576171211"></a>linkConfig.sk</p>
</td>
<td class="cellrowborder" valign="top" width="21.099999999999998%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0133483914_p15840983171211"><a name="zh-cn_topic_0133483914_p15840983171211"></a><a name="zh-cn_topic_0133483914_p15840983171211"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.669999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0133483914_p8051275171211"><a name="zh-cn_topic_0133483914_p8051275171211"></a><a name="zh-cn_topic_0133483914_p8051275171211"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.199999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0133483914_p48173539171211"><a name="zh-cn_topic_0133483914_p48173539171211"></a><a name="zh-cn_topic_0133483914_p48173539171211"></a>访问CloudTable服务的SK。</p>
</td>
</tr>
<tr id="zh-cn_topic_0133483914_row1149141210552"><td class="cellrowborder" valign="top" width="20.03%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0133483914_p65139020184339"><a name="zh-cn_topic_0133483914_p65139020184339"></a><a name="zh-cn_topic_0133483914_p65139020184339"></a>linkConfig.projectId</p>
</td>
<td class="cellrowborder" valign="top" width="21.099999999999998%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0133483914_p22547918184339"><a name="zh-cn_topic_0133483914_p22547918184339"></a><a name="zh-cn_topic_0133483914_p22547918184339"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.669999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0133483914_p23433084184339"><a name="zh-cn_topic_0133483914_p23433084184339"></a><a name="zh-cn_topic_0133483914_p23433084184339"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.199999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0133483914_p33128214184339"><a name="zh-cn_topic_0133483914_p33128214184339"></a><a name="zh-cn_topic_0133483914_p33128214184339"></a>CloudTable服务的项目ID。</p>
</td>
</tr>
</tbody>
</table>

