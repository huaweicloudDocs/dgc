# 配置DMS Kafka连接<a name="dayu_01_0038"></a>

连接DMS的Kafka队列时，相关参数如[表1](#zh-cn_topic_0143085538_table22075105144748)所示。

**表 1**  DMS Kafka连接参数

<a name="zh-cn_topic_0143085538_table22075105144748"></a>
<table><thead align="left"><tr id="zh-cn_topic_0143085538_row19905440144748"><th class="cellrowborder" valign="top" width="20.62%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0143085538_p1727937144748"><a name="zh-cn_topic_0143085538_p1727937144748"></a><a name="zh-cn_topic_0143085538_p1727937144748"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="58.19%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0143085538_p5745174144748"><a name="zh-cn_topic_0143085538_p5745174144748"></a><a name="zh-cn_topic_0143085538_p5745174144748"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="21.19%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0143085538_p62705927144748"><a name="zh-cn_topic_0143085538_p62705927144748"></a><a name="zh-cn_topic_0143085538_p62705927144748"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0143085538_row11298866916"><td class="cellrowborder" valign="top" width="20.62%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0143085538_p15298176296"><a name="zh-cn_topic_0143085538_p15298176296"></a><a name="zh-cn_topic_0143085538_p15298176296"></a>名称</p>
</td>
<td class="cellrowborder" valign="top" width="58.19%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0143085538_p1369564463813"><a name="zh-cn_topic_0143085538_p1369564463813"></a><a name="zh-cn_topic_0143085538_p1369564463813"></a>连接的名称，根据连接的数据源类型，用户可自定义便于记忆、区分的连接名。</p>
</td>
<td class="cellrowborder" valign="top" width="21.19%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0143085538_p19298156493"><a name="zh-cn_topic_0143085538_p19298156493"></a><a name="zh-cn_topic_0143085538_p19298156493"></a>dms_link</p>
</td>
</tr>
<tr id="zh-cn_topic_0143085538_row87539715534"><td class="cellrowborder" valign="top" width="20.62%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0143085538_p1375357165315"><a name="zh-cn_topic_0143085538_p1375357165315"></a><a name="zh-cn_topic_0143085538_p1375357165315"></a>版本</p>
</td>
<td class="cellrowborder" valign="top" width="58.19%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0143085538_p147692714538"><a name="zh-cn_topic_0143085538_p147692714538"></a><a name="zh-cn_topic_0143085538_p147692714538"></a>选择DMS Kafka版本：</p>
<a name="zh-cn_topic_0143085538_ul182931744102816"></a><a name="zh-cn_topic_0143085538_ul182931744102816"></a><ul id="zh-cn_topic_0143085538_ul182931744102816"><li>Basic：指DMS Kafka普通队列。</li><li>Platinum：指DMS Kafka专享版。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="21.19%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0143085538_p2076910795316"><a name="zh-cn_topic_0143085538_p2076910795316"></a><a name="zh-cn_topic_0143085538_p2076910795316"></a>Basic</p>
</td>
</tr>
<tr id="zh-cn_topic_0143085538_row1634161118531"><td class="cellrowborder" valign="top" width="20.62%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0143085538_p134191195311"><a name="zh-cn_topic_0143085538_p134191195311"></a><a name="zh-cn_topic_0143085538_p134191195311"></a>终端节点</p>
</td>
<td class="cellrowborder" valign="top" width="58.19%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0143085538_p10479147165612"><a name="zh-cn_topic_0143085538_p10479147165612"></a><a name="zh-cn_topic_0143085538_p10479147165612"></a>这里需要配置的DMS Endpoint格式为host:port。</p>
</td>
<td class="cellrowborder" valign="top" width="21.19%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0143085538_p1674519527376"><a name="zh-cn_topic_0143085538_p1674519527376"></a><a name="zh-cn_topic_0143085538_p1674519527376"></a>dms-kafka.cn-north-1.myhuaweicloud.com:37000</p>
</td>
</tr>
<tr id="zh-cn_topic_0143085538_row745662217380"><td class="cellrowborder" valign="top" width="20.62%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0143085538_p31612872145433"><a name="zh-cn_topic_0143085538_p31612872145433"></a><a name="zh-cn_topic_0143085538_p31612872145433"></a>访问标识（AK）</p>
</td>
<td class="cellrowborder" valign="top" width="58.19%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0143085538_p181471423104"><a name="zh-cn_topic_0143085538_p181471423104"></a><a name="zh-cn_topic_0143085538_p181471423104"></a>访问DMS Kafka的凭证AK。</p>
</td>
<td class="cellrowborder" valign="top" width="21.19%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0143085538_p5195678145433"><a name="zh-cn_topic_0143085538_p5195678145433"></a><a name="zh-cn_topic_0143085538_p5195678145433"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0143085538_row192672348380"><td class="cellrowborder" valign="top" width="20.62%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0143085538_p29552890145433"><a name="zh-cn_topic_0143085538_p29552890145433"></a><a name="zh-cn_topic_0143085538_p29552890145433"></a>密钥（SK）</p>
</td>
<td class="cellrowborder" valign="top" width="58.19%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0143085538_p5143112316010"><a name="zh-cn_topic_0143085538_p5143112316010"></a><a name="zh-cn_topic_0143085538_p5143112316010"></a>访问DMS Kafka的凭证SK。</p>
</td>
<td class="cellrowborder" valign="top" width="21.19%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0143085538_p32797946145433"><a name="zh-cn_topic_0143085538_p32797946145433"></a><a name="zh-cn_topic_0143085538_p32797946145433"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0143085538_row1392892065413"><td class="cellrowborder" valign="top" width="20.62%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0143085538_p1016019285015"><a name="zh-cn_topic_0143085538_p1016019285015"></a><a name="zh-cn_topic_0143085538_p1016019285015"></a>项目ID</p>
</td>
<td class="cellrowborder" valign="top" width="58.19%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0143085538_p1637616424613"><a name="zh-cn_topic_0143085538_p1637616424613"></a><a name="zh-cn_topic_0143085538_p1637616424613"></a>DMS所在区域的项目ID。</p>
</td>
<td class="cellrowborder" valign="top" width="21.19%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0143085538_p11608245019"><a name="zh-cn_topic_0143085538_p11608245019"></a><a name="zh-cn_topic_0143085538_p11608245019"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0143085538_row4287224185416"><td class="cellrowborder" valign="top" width="20.62%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0143085538_p10285208143916"><a name="zh-cn_topic_0143085538_p10285208143916"></a><a name="zh-cn_topic_0143085538_p10285208143916"></a>授权者的ProjectID</p>
</td>
<td class="cellrowborder" valign="top" width="58.19%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0143085538_p12287142410545"><a name="zh-cn_topic_0143085538_p12287142410545"></a><a name="zh-cn_topic_0143085538_p12287142410545"></a>如果需要访问其他用户授权的队列，则需要配置授权者的Project ID。</p>
</td>
<td class="cellrowborder" valign="top" width="21.19%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0143085538_p428782415548"><a name="zh-cn_topic_0143085538_p428782415548"></a><a name="zh-cn_topic_0143085538_p428782415548"></a>admin</p>
</td>
</tr>
</tbody>
</table>

