# 配置Elasticsearch/CSS连接<a name="dayu_01_0035"></a>

连接云搜索服务或Elasticsearch时，相关参数如[表1](#zh-cn_topic_0108275341_table22075105144748)所示。

**表 1**  Elasticsearch连接参数

<a name="zh-cn_topic_0108275341_table22075105144748"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108275341_row19905440144748"><th class="cellrowborder" valign="top" width="21.85%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108275341_p1727937144748"><a name="zh-cn_topic_0108275341_p1727937144748"></a><a name="zh-cn_topic_0108275341_p1727937144748"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="55.17999999999999%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108275341_p5745174144748"><a name="zh-cn_topic_0108275341_p5745174144748"></a><a name="zh-cn_topic_0108275341_p5745174144748"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="22.97%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108275341_p62705927144748"><a name="zh-cn_topic_0108275341_p62705927144748"></a><a name="zh-cn_topic_0108275341_p62705927144748"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108275341_row11298866916"><td class="cellrowborder" valign="top" width="21.85%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275341_p15298176296"><a name="zh-cn_topic_0108275341_p15298176296"></a><a name="zh-cn_topic_0108275341_p15298176296"></a>名称</p>
</td>
<td class="cellrowborder" valign="top" width="55.17999999999999%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275341_p1369564463813"><a name="zh-cn_topic_0108275341_p1369564463813"></a><a name="zh-cn_topic_0108275341_p1369564463813"></a>连接的名称，根据连接的数据源类型，用户可自定义便于记忆、区分的连接名。</p>
</td>
<td class="cellrowborder" valign="top" width="22.97%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275341_p19298156493"><a name="zh-cn_topic_0108275341_p19298156493"></a><a name="zh-cn_topic_0108275341_p19298156493"></a>css_link</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275341_row46015358144748"><td class="cellrowborder" valign="top" width="21.85%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275341_p31612872145433"><a name="zh-cn_topic_0108275341_p31612872145433"></a><a name="zh-cn_topic_0108275341_p31612872145433"></a>Elasticsearch服务器列表</p>
</td>
<td class="cellrowborder" valign="top" width="55.17999999999999%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275341_p10505843145433"><a name="zh-cn_topic_0108275341_p10505843145433"></a><a name="zh-cn_topic_0108275341_p10505843145433"></a>配置为一个或多个Elasticsearch服务器的IP地址或域名，包括端口号，格式为<span class="parmvalue" id="zh-cn_topic_0108275341_parmvalue757313251129"><a name="zh-cn_topic_0108275341_parmvalue757313251129"></a><a name="zh-cn_topic_0108275341_parmvalue757313251129"></a>“ip:port”</span>，多个地址之间使用分号（；）分隔。</p>
</td>
<td class="cellrowborder" valign="top" width="22.97%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275341_p5195678145433"><a name="zh-cn_topic_0108275341_p5195678145433"></a><a name="zh-cn_topic_0108275341_p5195678145433"></a>192.168.0.1:9200;192.168.0.2:9200</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275341_row17315161411152"><td class="cellrowborder" valign="top" width="21.85%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275341_p1087762218159"><a name="zh-cn_topic_0108275341_p1087762218159"></a><a name="zh-cn_topic_0108275341_p1087762218159"></a>用户名</p>
</td>
<td class="cellrowborder" valign="top" width="55.17999999999999%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275341_p2031520149157"><a name="zh-cn_topic_0108275341_p2031520149157"></a><a name="zh-cn_topic_0108275341_p2031520149157"></a>登录待连接数据库的用户名。</p>
</td>
<td class="cellrowborder" valign="top" width="22.97%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275341_p103151614141519"><a name="zh-cn_topic_0108275341_p103151614141519"></a><a name="zh-cn_topic_0108275341_p103151614141519"></a>cdm</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275341_row565818161516"><td class="cellrowborder" valign="top" width="21.85%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275341_p96531819155"><a name="zh-cn_topic_0108275341_p96531819155"></a><a name="zh-cn_topic_0108275341_p96531819155"></a>密码</p>
</td>
<td class="cellrowborder" valign="top" width="55.17999999999999%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275341_p8657186158"><a name="zh-cn_topic_0108275341_p8657186158"></a><a name="zh-cn_topic_0108275341_p8657186158"></a>登录数据库的密码。</p>
</td>
<td class="cellrowborder" valign="top" width="22.97%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275341_p165101871518"><a name="zh-cn_topic_0108275341_p165101871518"></a><a name="zh-cn_topic_0108275341_p165101871518"></a>-</p>
</td>
</tr>
</tbody>
</table>

