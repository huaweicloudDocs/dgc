# 配置DMS Kafka连接<a name="dgc_01_0038"></a>

连接DMS的Kafka队列时，相关参数如[表1](#zh-cn_topic_0143085538_table22075105144748)所示。

**表 1**  DMS Kafka连接参数

<a name="zh-cn_topic_0143085538_table22075105144748"></a>
<table><thead align="left"><tr id="zh-cn_topic_0143085538_row19905440144748"><th class="cellrowborder" valign="top" width="20.68%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0143085538_p1727937144748"><a name="zh-cn_topic_0143085538_p1727937144748"></a><a name="zh-cn_topic_0143085538_p1727937144748"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="58.13%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0143085538_p5745174144748"><a name="zh-cn_topic_0143085538_p5745174144748"></a><a name="zh-cn_topic_0143085538_p5745174144748"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="21.19%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0143085538_p62705927144748"><a name="zh-cn_topic_0143085538_p62705927144748"></a><a name="zh-cn_topic_0143085538_p62705927144748"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0143085538_row11298866916"><td class="cellrowborder" valign="top" width="20.68%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0143085538_p15298176296"><a name="zh-cn_topic_0143085538_p15298176296"></a><a name="zh-cn_topic_0143085538_p15298176296"></a>名称</p>
</td>
<td class="cellrowborder" valign="top" width="58.13%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0143085538_p1369564463813"><a name="zh-cn_topic_0143085538_p1369564463813"></a><a name="zh-cn_topic_0143085538_p1369564463813"></a>连接的名称，根据连接的数据源类型，用户可自定义便于记忆、区分的连接名。</p>
</td>
<td class="cellrowborder" valign="top" width="21.19%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0143085538_p19298156493"><a name="zh-cn_topic_0143085538_p19298156493"></a><a name="zh-cn_topic_0143085538_p19298156493"></a>dms_link</p>
</td>
</tr>
<tr id="zh-cn_topic_0143085538_row87539715534"><td class="cellrowborder" valign="top" width="20.68%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0143085538_p1375357165315"><a name="zh-cn_topic_0143085538_p1375357165315"></a><a name="zh-cn_topic_0143085538_p1375357165315"></a>服务类型</p>
</td>
<td class="cellrowborder" valign="top" width="58.13%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0143085538_p147692714538"><a name="zh-cn_topic_0143085538_p147692714538"></a><a name="zh-cn_topic_0143085538_p147692714538"></a>选择DMS Kafka版本，目前只有专享版。</p>
</td>
<td class="cellrowborder" valign="top" width="21.19%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0143085538_p2076910795316"><a name="zh-cn_topic_0143085538_p2076910795316"></a><a name="zh-cn_topic_0143085538_p2076910795316"></a>专享版</p>
</td>
</tr>
<tr id="zh-cn_topic_0143085538_row1351774015574"><td class="cellrowborder" valign="top" width="20.68%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0143085538_p132674594583"><a name="zh-cn_topic_0143085538_p132674594583"></a><a name="zh-cn_topic_0143085538_p132674594583"></a>Kafka Broker</p>
</td>
<td class="cellrowborder" valign="top" width="58.13%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0143085538_p55181140195712"><a name="zh-cn_topic_0143085538_p55181140195712"></a><a name="zh-cn_topic_0143085538_p55181140195712"></a>Kafka专享版实例的地址，格式为 host:port。</p>
</td>
<td class="cellrowborder" valign="top" width="21.19%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0143085538_p17518440165713"><a name="zh-cn_topic_0143085538_p17518440165713"></a><a name="zh-cn_topic_0143085538_p17518440165713"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0143085538_row4239164445710"><td class="cellrowborder" valign="top" width="20.68%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0143085538_p082419415916"><a name="zh-cn_topic_0143085538_p082419415916"></a><a name="zh-cn_topic_0143085538_p082419415916"></a>Kafka SASL_SSL</p>
</td>
<td class="cellrowborder" valign="top" width="58.13%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0143085538_p112168292347"><a name="zh-cn_topic_0143085538_p112168292347"></a><a name="zh-cn_topic_0143085538_p112168292347"></a>选择是否打开客户端连接Kafka专享版实例时SSL认证的开关。</p>
<p id="zh-cn_topic_0143085538_p1563192753418"><a name="zh-cn_topic_0143085538_p1563192753418"></a><a name="zh-cn_topic_0143085538_p1563192753418"></a>开启Kafka SASL_SSL，则数据加密传输，安全性更高，但性能会下降。</p>
</td>
<td class="cellrowborder" valign="top" width="21.19%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0143085538_p42402440579"><a name="zh-cn_topic_0143085538_p42402440579"></a><a name="zh-cn_topic_0143085538_p42402440579"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0143085538_row1521465119"><td class="cellrowborder" valign="top" width="20.68%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0143085538_p181416274499"><a name="zh-cn_topic_0143085538_p181416274499"></a><a name="zh-cn_topic_0143085538_p181416274499"></a>用户名</p>
</td>
<td class="cellrowborder" valign="top" width="58.13%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0143085538_p814182718498"><a name="zh-cn_topic_0143085538_p814182718498"></a><a name="zh-cn_topic_0143085538_p814182718498"></a>开启Kafka SASL_SSL时显示该参数，表示连接DMS Kafka的用户名。</p>
</td>
<td class="cellrowborder" valign="top" width="21.19%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0143085538_p1522641120"><a name="zh-cn_topic_0143085538_p1522641120"></a><a name="zh-cn_topic_0143085538_p1522641120"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0143085538_row1831717229110"><td class="cellrowborder" valign="top" width="20.68%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0143085538_p11141202744912"><a name="zh-cn_topic_0143085538_p11141202744912"></a><a name="zh-cn_topic_0143085538_p11141202744912"></a>密码</p>
</td>
<td class="cellrowborder" valign="top" width="58.13%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0143085538_p1376018356512"><a name="zh-cn_topic_0143085538_p1376018356512"></a><a name="zh-cn_topic_0143085538_p1376018356512"></a>开启Kafka SASL_SSL时显示该参数，表示连接DMS Kafka的密码。</p>
</td>
<td class="cellrowborder" valign="top" width="21.19%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0143085538_p4317522121118"><a name="zh-cn_topic_0143085538_p4317522121118"></a><a name="zh-cn_topic_0143085538_p4317522121118"></a>-</p>
</td>
</tr>
</tbody>
</table>

