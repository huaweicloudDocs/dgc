# Elasticsearch/云搜索服务连接<a name="dgc_02_0276"></a>

## 介绍<a name="zh-cn_topic_0108272849_section621837"></a>

通过Elasticsearch连接，可以对Elasticsearch服务器或云搜索服务抽取、加载数据。

## 连接样例<a name="zh-cn_topic_0108272849_section6163607716523"></a>

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
                "value": "192.168.0.1:9200;192.168.0.2:9200"
              },
              {
                "name": "linkConfig.user",
                "value": "cdm"
              },
              {
                "name": "linkConfig.password",
                "value": "Add password here"
              },
              {
                "name": "linkConfig.linkType",
                "value": "ElasticSearch"
              }
            ],
            "name": "linkConfig"
          }
        ]
      },
      "name": "es_link",
      "connector-name": "elasticsearch-connector"
    }
  ]
}
```

## 连接参数<a name="zh-cn_topic_0108272849_section5035508012043"></a>

<a name="zh-cn_topic_0108272849_table13922888141527"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108272849_row229143141527"><th class="cellrowborder" valign="top" width="20.03%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272849_p66756185141527"><a name="zh-cn_topic_0108272849_p66756185141527"></a><a name="zh-cn_topic_0108272849_p66756185141527"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="21.099999999999998%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272849_p38541938141527"><a name="zh-cn_topic_0108272849_p38541938141527"></a><a name="zh-cn_topic_0108272849_p38541938141527"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="16.669999999999998%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272849_p34889279141527"><a name="zh-cn_topic_0108272849_p34889279141527"></a><a name="zh-cn_topic_0108272849_p34889279141527"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.199999999999996%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272849_p7459369141527"><a name="zh-cn_topic_0108272849_p7459369141527"></a><a name="zh-cn_topic_0108272849_p7459369141527"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108272849_row2725489141730"><td class="cellrowborder" valign="top" width="20.03%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272849_p18261829141730"><a name="zh-cn_topic_0108272849_p18261829141730"></a><a name="zh-cn_topic_0108272849_p18261829141730"></a>linkConfig.host</p>
</td>
<td class="cellrowborder" valign="top" width="21.099999999999998%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272849_p2813219141730"><a name="zh-cn_topic_0108272849_p2813219141730"></a><a name="zh-cn_topic_0108272849_p2813219141730"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.669999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272849_p26544197141730"><a name="zh-cn_topic_0108272849_p26544197141730"></a><a name="zh-cn_topic_0108272849_p26544197141730"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.199999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272849_p10505843145433"><a name="zh-cn_topic_0108272849_p10505843145433"></a><a name="zh-cn_topic_0108272849_p10505843145433"></a>配置为Elasticsearch服务器的IP地址或域名，包括端口号，格式为<span class="parmvalue" id="zh-cn_topic_0108272849_parmvalue757313251129"><a name="zh-cn_topic_0108272849_parmvalue757313251129"></a><a name="zh-cn_topic_0108272849_parmvalue757313251129"></a>“ip:port”</span>，多个地址之间使用分号（；）分隔，例如：192.168.0.1:9200;192.168.0.2:9200。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272849_row1076119219183"><td class="cellrowborder" valign="top" width="20.03%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272849_p107618216186"><a name="zh-cn_topic_0108272849_p107618216186"></a><a name="zh-cn_topic_0108272849_p107618216186"></a>linkConfig.user</p>
</td>
<td class="cellrowborder" valign="top" width="21.099999999999998%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272849_p19761112141817"><a name="zh-cn_topic_0108272849_p19761112141817"></a><a name="zh-cn_topic_0108272849_p19761112141817"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.669999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272849_p18293152252611"><a name="zh-cn_topic_0108272849_p18293152252611"></a><a name="zh-cn_topic_0108272849_p18293152252611"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.199999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272849_p167615210188"><a name="zh-cn_topic_0108272849_p167615210188"></a><a name="zh-cn_topic_0108272849_p167615210188"></a>对于支持用户名密码鉴权的Elasticsearch，需要在创建连接时配置用户名和密码。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272849_row142925541817"><td class="cellrowborder" valign="top" width="20.03%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272849_p1929213551813"><a name="zh-cn_topic_0108272849_p1929213551813"></a><a name="zh-cn_topic_0108272849_p1929213551813"></a>linkConfig.password</p>
</td>
<td class="cellrowborder" valign="top" width="21.099999999999998%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272849_p18292185101814"><a name="zh-cn_topic_0108272849_p18292185101814"></a><a name="zh-cn_topic_0108272849_p18292185101814"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.669999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272849_p199112392615"><a name="zh-cn_topic_0108272849_p199112392615"></a><a name="zh-cn_topic_0108272849_p199112392615"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.199999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272849_p1629219515187"><a name="zh-cn_topic_0108272849_p1629219515187"></a><a name="zh-cn_topic_0108272849_p1629219515187"></a>登录Elasticsearch的密码。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272849_row195835288232"><td class="cellrowborder" valign="top" width="20.03%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272849_p55831328202315"><a name="zh-cn_topic_0108272849_p55831328202315"></a><a name="zh-cn_topic_0108272849_p55831328202315"></a>linkConfig.linkType</p>
</td>
<td class="cellrowborder" valign="top" width="21.099999999999998%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272849_p5583228202310"><a name="zh-cn_topic_0108272849_p5583228202310"></a><a name="zh-cn_topic_0108272849_p5583228202310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.669999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272849_p15763246269"><a name="zh-cn_topic_0108272849_p15763246269"></a><a name="zh-cn_topic_0108272849_p15763246269"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.199999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272849_p16583162820239"><a name="zh-cn_topic_0108272849_p16583162820239"></a><a name="zh-cn_topic_0108272849_p16583162820239"></a>连接类型，用于区分连接的是Elasticsearch或云搜索服务。</p>
</td>
</tr>
</tbody>
</table>

