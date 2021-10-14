# 配置Elasticsearch/云搜索服务（CSS）连接<a name="dgc_01_0035"></a>

## Elasticsearch<a name="zh-cn_topic_0108275341_section72131053165214"></a>

Elasticsearch连接适用于Elasticsearch服务，以及用户在本地数据中心或ECS上自建的Elasticsearch。

>![](public_sys-resources/icon-note.gif) **说明：** 
>Elasticsearch连接器只支持非安全模式。

连接Elasticsearch时，相关参数如[表1](#zh-cn_topic_0108275341_table22075105144748)所示。

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
<td class="cellrowborder" valign="top" width="55.17999999999999%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275341_p10505843145433"><a name="zh-cn_topic_0108275341_p10505843145433"></a><a name="zh-cn_topic_0108275341_p10505843145433"></a>配置为一个或多个Elasticsearch服务器的IP地址或域名，包括端口号，格式为<span class="parmvalue" id="zh-cn_topic_0108275341_parmvalue757313251129"><a name="zh-cn_topic_0108275341_parmvalue757313251129"></a><a name="zh-cn_topic_0108275341_parmvalue757313251129"></a>“ip:port”</span>，多个地址之间使用分号（;）分隔。</p>
</td>
<td class="cellrowborder" valign="top" width="22.97%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275341_p5195678145433"><a name="zh-cn_topic_0108275341_p5195678145433"></a><a name="zh-cn_topic_0108275341_p5195678145433"></a>192.168.0.1:9200;192.168.0.2:9200</p>
</td>
</tr>
</tbody>
</table>

## 云搜索服务（CSS）<a name="zh-cn_topic_0108275341_section13755123284814"></a>

华为云云搜索服务基于Elasticsearch引擎，该连接适用于将各类日志文件或数据库记录迁移到Elasticsearch引擎进行搜索和分析。

连接云搜索服务\(CSS\)时，相关参数如[表2](#zh-cn_topic_0108275341_table1714082724917)所示。

**表 2**  云搜索服务\(CSS\)连接参数

<a name="zh-cn_topic_0108275341_table1714082724917"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108275341_row15140927124910"><th class="cellrowborder" valign="top" width="21.85%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108275341_p17140122718493"><a name="zh-cn_topic_0108275341_p17140122718493"></a><a name="zh-cn_topic_0108275341_p17140122718493"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="55.17999999999999%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108275341_p1014062724920"><a name="zh-cn_topic_0108275341_p1014062724920"></a><a name="zh-cn_topic_0108275341_p1014062724920"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="22.97%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108275341_p01404275496"><a name="zh-cn_topic_0108275341_p01404275496"></a><a name="zh-cn_topic_0108275341_p01404275496"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108275341_row414013271491"><td class="cellrowborder" valign="top" width="21.85%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275341_p514062710494"><a name="zh-cn_topic_0108275341_p514062710494"></a><a name="zh-cn_topic_0108275341_p514062710494"></a>名称</p>
</td>
<td class="cellrowborder" valign="top" width="55.17999999999999%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275341_p61401527104919"><a name="zh-cn_topic_0108275341_p61401527104919"></a><a name="zh-cn_topic_0108275341_p61401527104919"></a>连接的名称，根据连接的数据源类型，用户可自定义便于记忆、区分的连接名。</p>
</td>
<td class="cellrowborder" valign="top" width="22.97%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275341_p914042717492"><a name="zh-cn_topic_0108275341_p914042717492"></a><a name="zh-cn_topic_0108275341_p914042717492"></a>css_link</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275341_row12140727174912"><td class="cellrowborder" valign="top" width="21.85%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275341_p1514017277496"><a name="zh-cn_topic_0108275341_p1514017277496"></a><a name="zh-cn_topic_0108275341_p1514017277496"></a>Elasticsearch服务器列表</p>
</td>
<td class="cellrowborder" valign="top" width="55.17999999999999%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275341_p1140122719498"><a name="zh-cn_topic_0108275341_p1140122719498"></a><a name="zh-cn_topic_0108275341_p1140122719498"></a>配置为一个或多个Elasticsearch服务器的IP地址或域名，包括端口号，格式为<span class="parmvalue" id="zh-cn_topic_0108275341_parmvalue1114015275497"><a name="zh-cn_topic_0108275341_parmvalue1114015275497"></a><a name="zh-cn_topic_0108275341_parmvalue1114015275497"></a>“ip:port”</span>，多个地址之间使用分号（;）分隔。</p>
</td>
<td class="cellrowborder" valign="top" width="22.97%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275341_p181411027144911"><a name="zh-cn_topic_0108275341_p181411027144911"></a><a name="zh-cn_topic_0108275341_p181411027144911"></a>192.168.0.1:9200;192.168.0.2:9200</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275341_row7141112784917"><td class="cellrowborder" valign="top" width="21.85%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275341_p11415277496"><a name="zh-cn_topic_0108275341_p11415277496"></a><a name="zh-cn_topic_0108275341_p11415277496"></a>安全模式认证</p>
</td>
<td class="cellrowborder" valign="top" width="55.17999999999999%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275341_p3141202734910"><a name="zh-cn_topic_0108275341_p3141202734910"></a><a name="zh-cn_topic_0108275341_p3141202734910"></a>是否开启安全模式认证。</p>
<p id="zh-cn_topic_0108275341_p1712015325114"><a name="zh-cn_topic_0108275341_p1712015325114"></a><a name="zh-cn_topic_0108275341_p1712015325114"></a>如果所需连接的CSS集群在创建时开启了<span class="parmname" id="zh-cn_topic_0108275341_parmname6621256019"><a name="zh-cn_topic_0108275341_parmname6621256019"></a><a name="zh-cn_topic_0108275341_parmname6621256019"></a>“安全模式”</span>，该参数需设置为<span class="parmvalue" id="zh-cn_topic_0108275341_parmvalue978203214523"><a name="zh-cn_topic_0108275341_parmvalue978203214523"></a><a name="zh-cn_topic_0108275341_parmvalue978203214523"></a>“是”</span>，否则设置为<span class="parmvalue" id="zh-cn_topic_0108275341_parmvalue17601034125214"><a name="zh-cn_topic_0108275341_parmvalue17601034125214"></a><a name="zh-cn_topic_0108275341_parmvalue17601034125214"></a>“否”</span>。</p>
</td>
<td class="cellrowborder" valign="top" width="22.97%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275341_p61413275497"><a name="zh-cn_topic_0108275341_p61413275497"></a><a name="zh-cn_topic_0108275341_p61413275497"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275341_row61411427124915"><td class="cellrowborder" valign="top" width="21.85%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275341_p181416274499"><a name="zh-cn_topic_0108275341_p181416274499"></a><a name="zh-cn_topic_0108275341_p181416274499"></a>用户名</p>
</td>
<td class="cellrowborder" valign="top" width="55.17999999999999%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275341_p814182718498"><a name="zh-cn_topic_0108275341_p814182718498"></a><a name="zh-cn_topic_0108275341_p814182718498"></a>CSS集群开启安全认证模式时显示此参数。该参数表示连接云搜索服务的用户名。</p>
</td>
<td class="cellrowborder" valign="top" width="22.97%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275341_p10141327194913"><a name="zh-cn_topic_0108275341_p10141327194913"></a><a name="zh-cn_topic_0108275341_p10141327194913"></a>admin</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275341_row414122716499"><td class="cellrowborder" valign="top" width="21.85%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275341_p11141202744912"><a name="zh-cn_topic_0108275341_p11141202744912"></a><a name="zh-cn_topic_0108275341_p11141202744912"></a>密码</p>
</td>
<td class="cellrowborder" valign="top" width="55.17999999999999%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275341_p1376018356512"><a name="zh-cn_topic_0108275341_p1376018356512"></a><a name="zh-cn_topic_0108275341_p1376018356512"></a>CSS集群开启安全认证模式时显示此参数。该参数表示连接云搜索服务的密码。</p>
</td>
<td class="cellrowborder" valign="top" width="22.97%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275341_p6141427104919"><a name="zh-cn_topic_0108275341_p6141427104919"></a><a name="zh-cn_topic_0108275341_p6141427104919"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275341_row83091712451"><td class="cellrowborder" valign="top" width="21.85%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275341_p591311246511"><a name="zh-cn_topic_0108275341_p591311246511"></a><a name="zh-cn_topic_0108275341_p591311246511"></a>https访问</p>
</td>
<td class="cellrowborder" valign="top" width="55.17999999999999%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275341_p663711151553"><a name="zh-cn_topic_0108275341_p663711151553"></a><a name="zh-cn_topic_0108275341_p663711151553"></a>CSS集群开启安全认证模式时显示此参数。该参数表示开启https访问，https访问相较于http访问更安全。</p>
</td>
<td class="cellrowborder" valign="top" width="22.97%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275341_p86372015554"><a name="zh-cn_topic_0108275341_p86372015554"></a><a name="zh-cn_topic_0108275341_p86372015554"></a>是</p>
</td>
</tr>
</tbody>
</table>

