# 配置CloudTable OpenTSDB连接<a name="dayu_01_0037"></a>

连接CloudTable OpenTSDB时，相关参数如[表1](#zh-cn_topic_0133463138_table22075105144748)所示。

**表 1**  CloudTable OpenTSDB连接参数

<a name="zh-cn_topic_0133463138_table22075105144748"></a>
<table><thead align="left"><tr id="zh-cn_topic_0133463138_row19905440144748"><th class="cellrowborder" valign="top" width="20.07%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0133463138_p1727937144748"><a name="zh-cn_topic_0133463138_p1727937144748"></a><a name="zh-cn_topic_0133463138_p1727937144748"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="58.19%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0133463138_p5745174144748"><a name="zh-cn_topic_0133463138_p5745174144748"></a><a name="zh-cn_topic_0133463138_p5745174144748"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="21.740000000000002%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0133463138_p62705927144748"><a name="zh-cn_topic_0133463138_p62705927144748"></a><a name="zh-cn_topic_0133463138_p62705927144748"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0133463138_row11298866916"><td class="cellrowborder" valign="top" width="20.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0133463138_p15298176296"><a name="zh-cn_topic_0133463138_p15298176296"></a><a name="zh-cn_topic_0133463138_p15298176296"></a>名称</p>
</td>
<td class="cellrowborder" valign="top" width="58.19%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0133463138_p1369564463813"><a name="zh-cn_topic_0133463138_p1369564463813"></a><a name="zh-cn_topic_0133463138_p1369564463813"></a>连接的名称，根据连接的数据源类型，用户可自定义便于记忆、区分的连接名。</p>
</td>
<td class="cellrowborder" valign="top" width="21.740000000000002%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0133463138_p19298156493"><a name="zh-cn_topic_0133463138_p19298156493"></a><a name="zh-cn_topic_0133463138_p19298156493"></a>TSDB_link</p>
</td>
</tr>
<tr id="zh-cn_topic_0133463138_row87539715534"><td class="cellrowborder" valign="top" width="20.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0133463138_p1375357165315"><a name="zh-cn_topic_0133463138_p1375357165315"></a><a name="zh-cn_topic_0133463138_p1375357165315"></a>OpenTSDB链接地址</p>
</td>
<td class="cellrowborder" valign="top" width="58.19%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0133463138_p147692714538"><a name="zh-cn_topic_0133463138_p147692714538"></a><a name="zh-cn_topic_0133463138_p147692714538"></a>OpenTSDB的ZK链接地址。</p>
</td>
<td class="cellrowborder" valign="top" width="21.740000000000002%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0133463138_p2076910795316"><a name="zh-cn_topic_0133463138_p2076910795316"></a><a name="zh-cn_topic_0133463138_p2076910795316"></a>opentsdb-sp8afz7bgbps5ur.cloudtable.com:4242</p>
</td>
</tr>
<tr id="zh-cn_topic_0133463138_row1634161118531"><td class="cellrowborder" valign="top" width="20.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0133463138_p134191195311"><a name="zh-cn_topic_0133463138_p134191195311"></a><a name="zh-cn_topic_0133463138_p134191195311"></a>安全模式</p>
</td>
<td class="cellrowborder" valign="top" width="58.19%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0133463138_p73481116533"><a name="zh-cn_topic_0133463138_p73481116533"></a><a name="zh-cn_topic_0133463138_p73481116533"></a>选择安全或非安全模式。</p>
<p id="zh-cn_topic_0133463138_p10479147165612"><a name="zh-cn_topic_0133463138_p10479147165612"></a><a name="zh-cn_topic_0133463138_p10479147165612"></a>选择安全模式时，需要输入项目ID、用户名、AK/SK。</p>
</td>
<td class="cellrowborder" valign="top" width="21.740000000000002%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0133463138_p1674519527376"><a name="zh-cn_topic_0133463138_p1674519527376"></a><a name="zh-cn_topic_0133463138_p1674519527376"></a>Nonsecurity</p>
</td>
</tr>
<tr id="zh-cn_topic_0133463138_row1392892065413"><td class="cellrowborder" valign="top" width="20.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0133463138_p1016019285015"><a name="zh-cn_topic_0133463138_p1016019285015"></a><a name="zh-cn_topic_0133463138_p1016019285015"></a>项目ID</p>
</td>
<td class="cellrowborder" valign="top" width="58.19%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0133463138_p1637616424613"><a name="zh-cn_topic_0133463138_p1637616424613"></a><a name="zh-cn_topic_0133463138_p1637616424613"></a>CloudTable服务所在区域的项目ID。</p>
</td>
<td class="cellrowborder" valign="top" width="21.740000000000002%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0133463138_p11608245019"><a name="zh-cn_topic_0133463138_p11608245019"></a><a name="zh-cn_topic_0133463138_p11608245019"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0133463138_row4287224185416"><td class="cellrowborder" valign="top" width="20.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0133463138_p9287524205412"><a name="zh-cn_topic_0133463138_p9287524205412"></a><a name="zh-cn_topic_0133463138_p9287524205412"></a>用户名</p>
</td>
<td class="cellrowborder" valign="top" width="58.19%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0133463138_p12287142410545"><a name="zh-cn_topic_0133463138_p12287142410545"></a><a name="zh-cn_topic_0133463138_p12287142410545"></a>访问CloudTable服务的用户名。</p>
</td>
<td class="cellrowborder" valign="top" width="21.740000000000002%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0133463138_p428782415548"><a name="zh-cn_topic_0133463138_p428782415548"></a><a name="zh-cn_topic_0133463138_p428782415548"></a>admin</p>
</td>
</tr>
<tr id="zh-cn_topic_0133463138_row46015358144748"><td class="cellrowborder" valign="top" width="20.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0133463138_p31612872145433"><a name="zh-cn_topic_0133463138_p31612872145433"></a><a name="zh-cn_topic_0133463138_p31612872145433"></a>访问标识（AK）</p>
</td>
<td class="cellrowborder" valign="top" width="58.19%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0133463138_p181471423104"><a name="zh-cn_topic_0133463138_p181471423104"></a><a name="zh-cn_topic_0133463138_p181471423104"></a>访问CloudTable服务的AK。</p>
</td>
<td class="cellrowborder" valign="top" width="21.740000000000002%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0133463138_p5195678145433"><a name="zh-cn_topic_0133463138_p5195678145433"></a><a name="zh-cn_topic_0133463138_p5195678145433"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0133463138_row23643456144748"><td class="cellrowborder" valign="top" width="20.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0133463138_p29552890145433"><a name="zh-cn_topic_0133463138_p29552890145433"></a><a name="zh-cn_topic_0133463138_p29552890145433"></a>密钥（SK）</p>
</td>
<td class="cellrowborder" valign="top" width="58.19%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0133463138_p5143112316010"><a name="zh-cn_topic_0133463138_p5143112316010"></a><a name="zh-cn_topic_0133463138_p5143112316010"></a>访问CloudTable服务的SK。</p>
</td>
<td class="cellrowborder" valign="top" width="21.740000000000002%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0133463138_p32797946145433"><a name="zh-cn_topic_0133463138_p32797946145433"></a><a name="zh-cn_topic_0133463138_p32797946145433"></a>-</p>
</td>
</tr>
</tbody>
</table>

