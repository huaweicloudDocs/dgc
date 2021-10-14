# 配置Cassandra连接<a name="dgc_01_004501"></a>

**表 1**  Cassandra连接参数

<a name="zh-cn_topic_0000001086742916_table34037531171418"></a>
<table><thead align="left"><tr id="zh-cn_topic_0000001086742916_row56630393171418"><th class="cellrowborder" valign="top" width="19.18%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0000001086742916_p23659124171418"><a name="zh-cn_topic_0000001086742916_p23659124171418"></a><a name="zh-cn_topic_0000001086742916_p23659124171418"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="60.540000000000006%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0000001086742916_p37340867171418"><a name="zh-cn_topic_0000001086742916_p37340867171418"></a><a name="zh-cn_topic_0000001086742916_p37340867171418"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="20.28%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0000001086742916_p4711375171418"><a name="zh-cn_topic_0000001086742916_p4711375171418"></a><a name="zh-cn_topic_0000001086742916_p4711375171418"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0000001086742916_row148131718155810"><td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001086742916_p1081471865814"><a name="zh-cn_topic_0000001086742916_p1081471865814"></a><a name="zh-cn_topic_0000001086742916_p1081471865814"></a>名称</p>
</td>
<td class="cellrowborder" valign="top" width="60.540000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001086742916_p1369564463813"><a name="zh-cn_topic_0000001086742916_p1369564463813"></a><a name="zh-cn_topic_0000001086742916_p1369564463813"></a>连接的名称，根据连接的数据源类型，用户可自定义便于记忆、区分的连接名。</p>
</td>
<td class="cellrowborder" valign="top" width="20.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001086742916_p1981416180585"><a name="zh-cn_topic_0000001086742916_p1981416180585"></a><a name="zh-cn_topic_0000001086742916_p1981416180585"></a>mongodb_link</p>
</td>
</tr>
<tr id="zh-cn_topic_0000001086742916_row19710159171418"><td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001086742916_p1560893315570"><a name="zh-cn_topic_0000001086742916_p1560893315570"></a><a name="zh-cn_topic_0000001086742916_p1560893315570"></a>服务节点</p>
</td>
<td class="cellrowborder" valign="top" width="60.540000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001086742916_p1963014245571"><a name="zh-cn_topic_0000001086742916_p1963014245571"></a><a name="zh-cn_topic_0000001086742916_p1963014245571"></a>一个或者多个节点的地址，以;分隔。建议同时配置多个节点。</p>
</td>
<td class="cellrowborder" valign="top" width="20.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001086742916_p639334617571"><a name="zh-cn_topic_0000001086742916_p639334617571"></a><a name="zh-cn_topic_0000001086742916_p639334617571"></a>192.168.0.1;192.168.0.2</p>
</td>
</tr>
<tr id="zh-cn_topic_0000001086742916_row11588738102344"><td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001086742916_p94244579576"><a name="zh-cn_topic_0000001086742916_p94244579576"></a><a name="zh-cn_topic_0000001086742916_p94244579576"></a>端口</p>
</td>
<td class="cellrowborder" valign="top" width="60.540000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001086742916_p66477930102344"><a name="zh-cn_topic_0000001086742916_p66477930102344"></a><a name="zh-cn_topic_0000001086742916_p66477930102344"></a>连接的Cassandra节点的端口号。</p>
</td>
<td class="cellrowborder" valign="top" width="20.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001086742916_p31421021155810"><a name="zh-cn_topic_0000001086742916_p31421021155810"></a><a name="zh-cn_topic_0000001086742916_p31421021155810"></a>9042</p>
</td>
</tr>
<tr id="zh-cn_topic_0000001086742916_row35421096102350"><td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001086742916_p50536504102350"><a name="zh-cn_topic_0000001086742916_p50536504102350"></a><a name="zh-cn_topic_0000001086742916_p50536504102350"></a>用户名</p>
</td>
<td class="cellrowborder" valign="top" width="60.540000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001086742916_p5438008102436"><a name="zh-cn_topic_0000001086742916_p5438008102436"></a><a name="zh-cn_topic_0000001086742916_p5438008102436"></a>连接Cassandra的用户名。</p>
</td>
<td class="cellrowborder" valign="top" width="20.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001086742916_p52218594102350"><a name="zh-cn_topic_0000001086742916_p52218594102350"></a><a name="zh-cn_topic_0000001086742916_p52218594102350"></a>cdm</p>
</td>
</tr>
<tr id="zh-cn_topic_0000001086742916_row21870968171418"><td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001086742916_p26718016171418"><a name="zh-cn_topic_0000001086742916_p26718016171418"></a><a name="zh-cn_topic_0000001086742916_p26718016171418"></a>密码</p>
</td>
<td class="cellrowborder" valign="top" width="60.540000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001086742916_p5950554015418"><a name="zh-cn_topic_0000001086742916_p5950554015418"></a><a name="zh-cn_topic_0000001086742916_p5950554015418"></a>连接Cassandra的密码。</p>
</td>
<td class="cellrowborder" valign="top" width="20.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001086742916_p38901992114142"><a name="zh-cn_topic_0000001086742916_p38901992114142"></a><a name="zh-cn_topic_0000001086742916_p38901992114142"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0000001086742916_row12724184313582"><td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001086742916_p10725543105813"><a name="zh-cn_topic_0000001086742916_p10725543105813"></a><a name="zh-cn_topic_0000001086742916_p10725543105813"></a>连接超时时长</p>
</td>
<td class="cellrowborder" valign="top" width="60.540000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001086742916_p1786004019351"><a name="zh-cn_topic_0000001086742916_p1786004019351"></a><a name="zh-cn_topic_0000001086742916_p1786004019351"></a>可选参数，单击<span class="uicontrol" id="zh-cn_topic_0000001086742916_uicontrol4860194019354"><a name="zh-cn_topic_0000001086742916_uicontrol4860194019354"></a><a name="zh-cn_topic_0000001086742916_uicontrol4860194019354"></a>“显示高级属性”</span>后显示。</p>
<p id="zh-cn_topic_0000001086742916_p37255439586"><a name="zh-cn_topic_0000001086742916_p37255439586"></a><a name="zh-cn_topic_0000001086742916_p37255439586"></a>连接超时时长，单位秒。</p>
</td>
<td class="cellrowborder" valign="top" width="20.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001086742916_p1272534355820"><a name="zh-cn_topic_0000001086742916_p1272534355820"></a><a name="zh-cn_topic_0000001086742916_p1272534355820"></a>5</p>
</td>
</tr>
<tr id="zh-cn_topic_0000001086742916_row14629948175817"><td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001086742916_p18629134835818"><a name="zh-cn_topic_0000001086742916_p18629134835818"></a><a name="zh-cn_topic_0000001086742916_p18629134835818"></a>读取超时时长</p>
</td>
<td class="cellrowborder" valign="top" width="60.540000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001086742916_p04959434352"><a name="zh-cn_topic_0000001086742916_p04959434352"></a><a name="zh-cn_topic_0000001086742916_p04959434352"></a>可选参数，单击<span class="uicontrol" id="zh-cn_topic_0000001086742916_uicontrol149534323520"><a name="zh-cn_topic_0000001086742916_uicontrol149534323520"></a><a name="zh-cn_topic_0000001086742916_uicontrol149534323520"></a>“显示高级属性”</span>后显示。</p>
<p id="zh-cn_topic_0000001086742916_p1662944815810"><a name="zh-cn_topic_0000001086742916_p1662944815810"></a><a name="zh-cn_topic_0000001086742916_p1662944815810"></a>读取超时时长，单位秒。小于或等于0表示不超时。</p>
</td>
<td class="cellrowborder" valign="top" width="20.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001086742916_p1662974817581"><a name="zh-cn_topic_0000001086742916_p1662974817581"></a><a name="zh-cn_topic_0000001086742916_p1662974817581"></a>12</p>
</td>
</tr>
</tbody>
</table>

