# 配置Redis/DCS连接<a name="dayu_01_0032"></a>

连接本地Redis数据库或DCS时，相关参数如[表1](#zh-cn_topic_0108275391_table34037531171418)所示。

**表 1**  Redis连接参数

<a name="zh-cn_topic_0108275391_table34037531171418"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108275391_row56630393171418"><th class="cellrowborder" valign="top" width="18.62%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108275391_p23659124171418"><a name="zh-cn_topic_0108275391_p23659124171418"></a><a name="zh-cn_topic_0108275391_p23659124171418"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="61.53999999999999%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108275391_p37340867171418"><a name="zh-cn_topic_0108275391_p37340867171418"></a><a name="zh-cn_topic_0108275391_p37340867171418"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="19.84%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108275391_p4711375171418"><a name="zh-cn_topic_0108275391_p4711375171418"></a><a name="zh-cn_topic_0108275391_p4711375171418"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108275391_row197082015910"><td class="cellrowborder" valign="top" width="18.62%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275391_p1670891512118"><a name="zh-cn_topic_0108275391_p1670891512118"></a><a name="zh-cn_topic_0108275391_p1670891512118"></a>名称</p>
</td>
<td class="cellrowborder" valign="top" width="61.53999999999999%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275391_p1369564463813"><a name="zh-cn_topic_0108275391_p1369564463813"></a><a name="zh-cn_topic_0108275391_p1369564463813"></a>连接的名称，根据连接的数据源类型，用户可自定义便于记忆、区分的连接名。</p>
</td>
<td class="cellrowborder" valign="top" width="19.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275391_p370819159116"><a name="zh-cn_topic_0108275391_p370819159116"></a><a name="zh-cn_topic_0108275391_p370819159116"></a>redis_link</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275391_row42099350112430"><td class="cellrowborder" valign="top" width="18.62%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275391_p54604217112430"><a name="zh-cn_topic_0108275391_p54604217112430"></a><a name="zh-cn_topic_0108275391_p54604217112430"></a>Redis部署方式</p>
</td>
<td class="cellrowborder" valign="top" width="61.53999999999999%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275391_p45863417112646"><a name="zh-cn_topic_0108275391_p45863417112646"></a><a name="zh-cn_topic_0108275391_p45863417112646"></a>Redis部署方式：</p>
<a name="zh-cn_topic_0108275391_ul54257378112542"></a><a name="zh-cn_topic_0108275391_ul54257378112542"></a><ul id="zh-cn_topic_0108275391_ul54257378112542"><li>Single：表示单机部署。</li><li>Cluster：表示集群部署。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="19.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275391_p31153255112430"><a name="zh-cn_topic_0108275391_p31153255112430"></a><a name="zh-cn_topic_0108275391_p31153255112430"></a>Single</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275391_row19710159171418"><td class="cellrowborder" valign="top" width="18.62%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275391_p62657656114131"><a name="zh-cn_topic_0108275391_p62657656114131"></a><a name="zh-cn_topic_0108275391_p62657656114131"></a>Redis服务器列表</p>
</td>
<td class="cellrowborder" valign="top" width="61.53999999999999%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275391_p3224914515418"><a name="zh-cn_topic_0108275391_p3224914515418"></a><a name="zh-cn_topic_0108275391_p3224914515418"></a>服务器地址列表，输入格式为<span class="uicontrol" id="zh-cn_topic_0108275391_zh-cn_topic_0108275382_uicontrol11588628155916"><a name="zh-cn_topic_0108275391_zh-cn_topic_0108275382_uicontrol11588628155916"></a><a name="zh-cn_topic_0108275391_zh-cn_topic_0108275382_uicontrol11588628155916"></a>“数据库服务器域名或IP地址：端口”</span>。多个服务器列表间以<span class="uicontrol" id="zh-cn_topic_0108275391_zh-cn_topic_0108275382_uicontrol1126413469590"><a name="zh-cn_topic_0108275391_zh-cn_topic_0108275382_uicontrol1126413469590"></a><a name="zh-cn_topic_0108275391_zh-cn_topic_0108275382_uicontrol1126413469590"></a>“;”</span>分隔。</p>
</td>
<td class="cellrowborder" valign="top" width="19.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275391_p3891070991628"><a name="zh-cn_topic_0108275391_p3891070991628"></a><a name="zh-cn_topic_0108275391_p3891070991628"></a>192.168.0.1:7300;192.168.0.2:7301</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275391_row21870968171418"><td class="cellrowborder" valign="top" width="18.62%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275391_p26718016171418"><a name="zh-cn_topic_0108275391_p26718016171418"></a><a name="zh-cn_topic_0108275391_p26718016171418"></a>密码</p>
</td>
<td class="cellrowborder" valign="top" width="61.53999999999999%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275391_p5950554015418"><a name="zh-cn_topic_0108275391_p5950554015418"></a><a name="zh-cn_topic_0108275391_p5950554015418"></a>连接Redis的密码。</p>
</td>
<td class="cellrowborder" valign="top" width="19.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275391_p38901992114142"><a name="zh-cn_topic_0108275391_p38901992114142"></a><a name="zh-cn_topic_0108275391_p38901992114142"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275391_row46725475164948"><td class="cellrowborder" valign="top" width="18.62%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275391_p26667143164948"><a name="zh-cn_topic_0108275391_p26667143164948"></a><a name="zh-cn_topic_0108275391_p26667143164948"></a>Redis数据库索引</p>
</td>
<td class="cellrowborder" valign="top" width="61.53999999999999%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275391_p12554938164948"><a name="zh-cn_topic_0108275391_p12554938164948"></a><a name="zh-cn_topic_0108275391_p12554938164948"></a>Redis分库的索引标识。</p>
<p id="zh-cn_topic_0108275391_p382084353413"><a name="zh-cn_topic_0108275391_p382084353413"></a><a name="zh-cn_topic_0108275391_p382084353413"></a>Redis的分库，相当于关系型数据库中的database。分库总数可以在Redis配置文件中设置，默认是16个，分库名称是一个整数（0～15），不是一个字符串。</p>
</td>
<td class="cellrowborder" valign="top" width="19.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275391_p10317095164948"><a name="zh-cn_topic_0108275391_p10317095164948"></a><a name="zh-cn_topic_0108275391_p10317095164948"></a>0</p>
</td>
</tr>
</tbody>
</table>

