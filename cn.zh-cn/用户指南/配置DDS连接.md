# 配置DDS连接<a name="dgc_01_0031"></a>

DDS连接适用于华为云上的文档数据库服务，常用于从DDS同步数据到大数据平台。

连接云服务DDS时，相关参数如[表1](#zh-cn_topic_0173586864_table34037531171418)所示。

**表 1**  DDS连接参数

<a name="zh-cn_topic_0173586864_table34037531171418"></a>
<table><thead align="left"><tr id="zh-cn_topic_0173586864_row56630393171418"><th class="cellrowborder" valign="top" width="18.509999999999998%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0173586864_p23659124171418"><a name="zh-cn_topic_0173586864_p23659124171418"></a><a name="zh-cn_topic_0173586864_p23659124171418"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="61.309999999999995%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0173586864_p37340867171418"><a name="zh-cn_topic_0173586864_p37340867171418"></a><a name="zh-cn_topic_0173586864_p37340867171418"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="20.18%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0173586864_p4711375171418"><a name="zh-cn_topic_0173586864_p4711375171418"></a><a name="zh-cn_topic_0173586864_p4711375171418"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0173586864_row148131718155810"><td class="cellrowborder" valign="top" width="18.509999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0173586864_p1081471865814"><a name="zh-cn_topic_0173586864_p1081471865814"></a><a name="zh-cn_topic_0173586864_p1081471865814"></a>名称</p>
</td>
<td class="cellrowborder" valign="top" width="61.309999999999995%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0173586864_p1369564463813"><a name="zh-cn_topic_0173586864_p1369564463813"></a><a name="zh-cn_topic_0173586864_p1369564463813"></a>连接的名称，根据连接的数据源类型，用户可自定义便于记忆、区分的连接名。</p>
</td>
<td class="cellrowborder" valign="top" width="20.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0173586864_p1981416180585"><a name="zh-cn_topic_0173586864_p1981416180585"></a><a name="zh-cn_topic_0173586864_p1981416180585"></a>dds_link</p>
</td>
</tr>
<tr id="zh-cn_topic_0173586864_row19710159171418"><td class="cellrowborder" valign="top" width="18.509999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0173586864_p62657656114131"><a name="zh-cn_topic_0173586864_p62657656114131"></a><a name="zh-cn_topic_0173586864_p62657656114131"></a>服务器列表</p>
</td>
<td class="cellrowborder" valign="top" width="61.309999999999995%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0173586864_p733031416592"><a name="zh-cn_topic_0173586864_p733031416592"></a><a name="zh-cn_topic_0173586864_p733031416592"></a>服务器地址列表，输入格式为<span class="uicontrol" id="zh-cn_topic_0173586864_uicontrol11588628155916"><a name="zh-cn_topic_0173586864_uicontrol11588628155916"></a><a name="zh-cn_topic_0173586864_uicontrol11588628155916"></a>“数据库服务器域名或IP地址：端口”</span>。多个服务器列表间以<span class="uicontrol" id="zh-cn_topic_0173586864_uicontrol1126413469590"><a name="zh-cn_topic_0173586864_uicontrol1126413469590"></a><a name="zh-cn_topic_0173586864_uicontrol1126413469590"></a>“;”</span>分隔。</p>
</td>
<td class="cellrowborder" valign="top" width="20.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0173586864_p3891070991628"><a name="zh-cn_topic_0173586864_p3891070991628"></a><a name="zh-cn_topic_0173586864_p3891070991628"></a>192.168.0.1:7300;192.168.0.2:7301</p>
</td>
</tr>
<tr id="zh-cn_topic_0173586864_row11588738102344"><td class="cellrowborder" valign="top" width="18.509999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0173586864_p66272570102344"><a name="zh-cn_topic_0173586864_p66272570102344"></a><a name="zh-cn_topic_0173586864_p66272570102344"></a>数据库名称</p>
</td>
<td class="cellrowborder" valign="top" width="61.309999999999995%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0173586864_p66477930102344"><a name="zh-cn_topic_0173586864_p66477930102344"></a><a name="zh-cn_topic_0173586864_p66477930102344"></a>要连接的DDS数据库名称。</p>
</td>
<td class="cellrowborder" valign="top" width="20.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0173586864_p16003259102344"><a name="zh-cn_topic_0173586864_p16003259102344"></a><a name="zh-cn_topic_0173586864_p16003259102344"></a>DB_dds</p>
</td>
</tr>
<tr id="zh-cn_topic_0173586864_row35421096102350"><td class="cellrowborder" valign="top" width="18.509999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0173586864_p50536504102350"><a name="zh-cn_topic_0173586864_p50536504102350"></a><a name="zh-cn_topic_0173586864_p50536504102350"></a>用户名</p>
</td>
<td class="cellrowborder" valign="top" width="61.309999999999995%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0173586864_p5438008102436"><a name="zh-cn_topic_0173586864_p5438008102436"></a><a name="zh-cn_topic_0173586864_p5438008102436"></a>连接DDS的用户名。</p>
</td>
<td class="cellrowborder" valign="top" width="20.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0173586864_p52218594102350"><a name="zh-cn_topic_0173586864_p52218594102350"></a><a name="zh-cn_topic_0173586864_p52218594102350"></a>cdm</p>
</td>
</tr>
<tr id="zh-cn_topic_0173586864_row21870968171418"><td class="cellrowborder" valign="top" width="18.509999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0173586864_p26718016171418"><a name="zh-cn_topic_0173586864_p26718016171418"></a><a name="zh-cn_topic_0173586864_p26718016171418"></a>密码</p>
</td>
<td class="cellrowborder" valign="top" width="61.309999999999995%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0173586864_p5950554015418"><a name="zh-cn_topic_0173586864_p5950554015418"></a><a name="zh-cn_topic_0173586864_p5950554015418"></a>连接DDS的密码。</p>
</td>
<td class="cellrowborder" valign="top" width="20.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0173586864_p38901992114142"><a name="zh-cn_topic_0173586864_p38901992114142"></a><a name="zh-cn_topic_0173586864_p38901992114142"></a>-</p>
</td>
</tr>
</tbody>
</table>

