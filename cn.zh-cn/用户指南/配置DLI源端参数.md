# 配置DLI源端参数<a name="dgc_01_0120"></a>

作业中源连接为[配置DLI连接](配置DLI连接.md#dgc_01_0036)时，源端作业参数如[表1](#zh-cn_topic_0000001145417420_table5046103815165)所示。

**表 1**  DLI作为源端时的作业参数

<a name="zh-cn_topic_0000001145417420_table5046103815165"></a>
<table><thead align="left"><tr id="zh-cn_topic_0000001145417420_row585315215165"><th class="cellrowborder" valign="top" width="17.169999999999998%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0000001145417420_p1626397215165"><a name="zh-cn_topic_0000001145417420_p1626397215165"></a><a name="zh-cn_topic_0000001145417420_p1626397215165"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="63.77%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0000001145417420_p4231334915165"><a name="zh-cn_topic_0000001145417420_p4231334915165"></a><a name="zh-cn_topic_0000001145417420_p4231334915165"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="19.06%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0000001145417420_p482921015165"><a name="zh-cn_topic_0000001145417420_p482921015165"></a><a name="zh-cn_topic_0000001145417420_p482921015165"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0000001145417420_row61343144519"><td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001145417420_p21341141357"><a name="zh-cn_topic_0000001145417420_p21341141357"></a><a name="zh-cn_topic_0000001145417420_p21341141357"></a>资源队列</p>
</td>
<td class="cellrowborder" valign="top" width="63.77%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001145417420_p713417141954"><a name="zh-cn_topic_0000001145417420_p713417141954"></a><a name="zh-cn_topic_0000001145417420_p713417141954"></a>选择目的表所属的资源队列。</p>
<p id="zh-cn_topic_0000001145417420_p7755261865"><a name="zh-cn_topic_0000001145417420_p7755261865"></a><a name="zh-cn_topic_0000001145417420_p7755261865"></a>DLI的default队列无法在迁移作业中使用，您需要在DLI中新建SQL队列。</p>
</td>
<td class="cellrowborder" valign="top" width="19.06%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001145417420_p131341314654"><a name="zh-cn_topic_0000001145417420_p131341314654"></a><a name="zh-cn_topic_0000001145417420_p131341314654"></a>cdm</p>
</td>
</tr>
<tr id="zh-cn_topic_0000001145417420_row4012116315165"><td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001145417420_p2858877215165"><a name="zh-cn_topic_0000001145417420_p2858877215165"></a><a name="zh-cn_topic_0000001145417420_p2858877215165"></a>数据库名称</p>
</td>
<td class="cellrowborder" valign="top" width="63.77%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001145417420_p188281713155918"><a name="zh-cn_topic_0000001145417420_p188281713155918"></a><a name="zh-cn_topic_0000001145417420_p188281713155918"></a>写入数据的数据库名称。</p>
</td>
<td class="cellrowborder" valign="top" width="19.06%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001145417420_p166427315165"><a name="zh-cn_topic_0000001145417420_p166427315165"></a><a name="zh-cn_topic_0000001145417420_p166427315165"></a>dli</p>
</td>
</tr>
<tr id="zh-cn_topic_0000001145417420_row660232720546"><td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001145417420_p5602172785412"><a name="zh-cn_topic_0000001145417420_p5602172785412"></a><a name="zh-cn_topic_0000001145417420_p5602172785412"></a>表名</p>
</td>
<td class="cellrowborder" valign="top" width="63.77%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001145417420_p8823111311598"><a name="zh-cn_topic_0000001145417420_p8823111311598"></a><a name="zh-cn_topic_0000001145417420_p8823111311598"></a>写入数据的表名。</p>
</td>
<td class="cellrowborder" valign="top" width="19.06%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001145417420_p116025271541"><a name="zh-cn_topic_0000001145417420_p116025271541"></a><a name="zh-cn_topic_0000001145417420_p116025271541"></a>car_detail</p>
</td>
</tr>
<tr id="zh-cn_topic_0000001145417420_row7651152211319"><td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001145417420_p2651122181312"><a name="zh-cn_topic_0000001145417420_p2651122181312"></a><a name="zh-cn_topic_0000001145417420_p2651122181312"></a>分区</p>
</td>
<td class="cellrowborder" valign="top" width="63.77%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001145417420_p6622439171414"><a name="zh-cn_topic_0000001145417420_p6622439171414"></a><a name="zh-cn_topic_0000001145417420_p6622439171414"></a>导入前清空数据，如果设置为true时，呈现此参数。</p>
<p id="zh-cn_topic_0000001145417420_p196521522121320"><a name="zh-cn_topic_0000001145417420_p196521522121320"></a><a name="zh-cn_topic_0000001145417420_p196521522121320"></a>表示分区信息。</p>
</td>
<td class="cellrowborder" valign="top" width="19.06%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001145417420_p12652112231311"><a name="zh-cn_topic_0000001145417420_p12652112231311"></a><a name="zh-cn_topic_0000001145417420_p12652112231311"></a>year=2020,location=sun</p>
</td>
</tr>
</tbody>
</table>

