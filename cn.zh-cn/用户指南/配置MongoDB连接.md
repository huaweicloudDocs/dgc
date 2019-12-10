# 配置MongoDB连接<a name="dayu_01_0030"></a>

连接本地MongoDB数据库时，相关参数如[表1](#zh-cn_topic_0108275382_table34037531171418)所示。

**表 1**  MongoDB连接参数

<a name="zh-cn_topic_0108275382_table34037531171418"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108275382_row56630393171418"><th class="cellrowborder" valign="top" width="19.18%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108275382_p23659124171418"><a name="zh-cn_topic_0108275382_p23659124171418"></a><a name="zh-cn_topic_0108275382_p23659124171418"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="60.540000000000006%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108275382_p37340867171418"><a name="zh-cn_topic_0108275382_p37340867171418"></a><a name="zh-cn_topic_0108275382_p37340867171418"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="20.28%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108275382_p4711375171418"><a name="zh-cn_topic_0108275382_p4711375171418"></a><a name="zh-cn_topic_0108275382_p4711375171418"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108275382_row148131718155810"><td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275382_p1081471865814"><a name="zh-cn_topic_0108275382_p1081471865814"></a><a name="zh-cn_topic_0108275382_p1081471865814"></a>名称</p>
</td>
<td class="cellrowborder" valign="top" width="60.540000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275382_p1369564463813"><a name="zh-cn_topic_0108275382_p1369564463813"></a><a name="zh-cn_topic_0108275382_p1369564463813"></a>连接的名称，根据连接的数据源类型，用户可自定义便于记忆、区分的连接名。</p>
</td>
<td class="cellrowborder" valign="top" width="20.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275382_p1981416180585"><a name="zh-cn_topic_0108275382_p1981416180585"></a><a name="zh-cn_topic_0108275382_p1981416180585"></a>mongodb_link</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275382_row19710159171418"><td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275382_p62657656114131"><a name="zh-cn_topic_0108275382_p62657656114131"></a><a name="zh-cn_topic_0108275382_p62657656114131"></a>MongoDB服务器列表</p>
</td>
<td class="cellrowborder" valign="top" width="60.540000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275382_p733031416592"><a name="zh-cn_topic_0108275382_p733031416592"></a><a name="zh-cn_topic_0108275382_p733031416592"></a>服务器地址列表，输入格式为<span class="uicontrol" id="zh-cn_topic_0108275382_uicontrol11588628155916"><a name="zh-cn_topic_0108275382_uicontrol11588628155916"></a><a name="zh-cn_topic_0108275382_uicontrol11588628155916"></a>“数据库服务器域名或IP地址：端口”</span>。多个服务器列表间以<span class="uicontrol" id="zh-cn_topic_0108275382_uicontrol1126413469590"><a name="zh-cn_topic_0108275382_uicontrol1126413469590"></a><a name="zh-cn_topic_0108275382_uicontrol1126413469590"></a>“;”</span>分隔。</p>
</td>
<td class="cellrowborder" valign="top" width="20.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275382_p3891070991628"><a name="zh-cn_topic_0108275382_p3891070991628"></a><a name="zh-cn_topic_0108275382_p3891070991628"></a>192.168.0.1:7300;192.168.0.2:7301</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275382_row11588738102344"><td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275382_p66272570102344"><a name="zh-cn_topic_0108275382_p66272570102344"></a><a name="zh-cn_topic_0108275382_p66272570102344"></a>数据库名称</p>
</td>
<td class="cellrowborder" valign="top" width="60.540000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275382_p66477930102344"><a name="zh-cn_topic_0108275382_p66477930102344"></a><a name="zh-cn_topic_0108275382_p66477930102344"></a>要连接的MongoDB数据库名称。</p>
</td>
<td class="cellrowborder" valign="top" width="20.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275382_p16003259102344"><a name="zh-cn_topic_0108275382_p16003259102344"></a><a name="zh-cn_topic_0108275382_p16003259102344"></a>DB_mongodb</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275382_row35421096102350"><td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275382_p50536504102350"><a name="zh-cn_topic_0108275382_p50536504102350"></a><a name="zh-cn_topic_0108275382_p50536504102350"></a>用户名</p>
</td>
<td class="cellrowborder" valign="top" width="60.540000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275382_p5438008102436"><a name="zh-cn_topic_0108275382_p5438008102436"></a><a name="zh-cn_topic_0108275382_p5438008102436"></a>连接MongoDB的用户名。</p>
</td>
<td class="cellrowborder" valign="top" width="20.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275382_p52218594102350"><a name="zh-cn_topic_0108275382_p52218594102350"></a><a name="zh-cn_topic_0108275382_p52218594102350"></a>cdm</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275382_row21870968171418"><td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275382_p26718016171418"><a name="zh-cn_topic_0108275382_p26718016171418"></a><a name="zh-cn_topic_0108275382_p26718016171418"></a>密码</p>
</td>
<td class="cellrowborder" valign="top" width="60.540000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275382_p5950554015418"><a name="zh-cn_topic_0108275382_p5950554015418"></a><a name="zh-cn_topic_0108275382_p5950554015418"></a>连接MongoDB的密码。</p>
</td>
<td class="cellrowborder" valign="top" width="20.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275382_p38901992114142"><a name="zh-cn_topic_0108275382_p38901992114142"></a><a name="zh-cn_topic_0108275382_p38901992114142"></a>-</p>
</td>
</tr>
</tbody>
</table>

