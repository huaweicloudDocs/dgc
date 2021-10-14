# 配置OpenTSDB源端参数<a name="dgc_01_0060"></a>

作业中源连接为[配置CloudTable OpenTSDB连接](配置CloudTable-OpenTSDB连接.md#dgc_01_0037)时，源端作业参数如[表1](#zh-cn_topic_0133467989_table5046103815165)所示。

**表 1**  OpenTSDB作为源端时的作业参数

<a name="zh-cn_topic_0133467989_table5046103815165"></a>
<table><thead align="left"><tr id="zh-cn_topic_0133467989_row585315215165"><th class="cellrowborder" valign="top" width="18.279999999999998%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0133467989_p1626397215165"><a name="zh-cn_topic_0133467989_p1626397215165"></a><a name="zh-cn_topic_0133467989_p1626397215165"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="61.199999999999996%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0133467989_p4231334915165"><a name="zh-cn_topic_0133467989_p4231334915165"></a><a name="zh-cn_topic_0133467989_p4231334915165"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="20.52%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0133467989_p482921015165"><a name="zh-cn_topic_0133467989_p482921015165"></a><a name="zh-cn_topic_0133467989_p482921015165"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0133467989_row4012116315165"><td class="cellrowborder" valign="top" width="18.279999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0133467989_p2858877215165"><a name="zh-cn_topic_0133467989_p2858877215165"></a><a name="zh-cn_topic_0133467989_p2858877215165"></a>开始时间</p>
</td>
<td class="cellrowborder" valign="top" width="61.199999999999996%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0133467989_p18424347134812"><a name="zh-cn_topic_0133467989_p18424347134812"></a><a name="zh-cn_topic_0133467989_p18424347134812"></a>查询的起始时间，格式为yyyyMMddHHmmdd的字符串或时间戳。</p>
</td>
<td class="cellrowborder" valign="top" width="20.52%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0133467989_p166427315165"><a name="zh-cn_topic_0133467989_p166427315165"></a><a name="zh-cn_topic_0133467989_p166427315165"></a>20180920145505</p>
</td>
</tr>
<tr id="zh-cn_topic_0133467989_row2085795312515"><td class="cellrowborder" valign="top" width="18.279999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0133467989_p7355104195318"><a name="zh-cn_topic_0133467989_p7355104195318"></a><a name="zh-cn_topic_0133467989_p7355104195318"></a>结束时间</p>
</td>
<td class="cellrowborder" valign="top" width="61.199999999999996%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0133467989_p93554465319"><a name="zh-cn_topic_0133467989_p93554465319"></a><a name="zh-cn_topic_0133467989_p93554465319"></a>可选参数，查询的终止时间，格式为yyyyMMddHHmmdd的字串或时间戳。</p>
</td>
<td class="cellrowborder" valign="top" width="20.52%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0133467989_p13665124217387"><a name="zh-cn_topic_0133467989_p13665124217387"></a><a name="zh-cn_topic_0133467989_p13665124217387"></a>20180921145505</p>
</td>
</tr>
<tr id="zh-cn_topic_0133467989_row68131455163415"><td class="cellrowborder" valign="top" width="18.279999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0133467989_p16748133795415"><a name="zh-cn_topic_0133467989_p16748133795415"></a><a name="zh-cn_topic_0133467989_p16748133795415"></a>指标</p>
</td>
<td class="cellrowborder" valign="top" width="61.199999999999996%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0133467989_p14813655143413"><a name="zh-cn_topic_0133467989_p14813655143413"></a><a name="zh-cn_topic_0133467989_p14813655143413"></a>输入迁移哪个指标的数据，或选择OpenTSDB中已存在的指标。</p>
</td>
<td class="cellrowborder" valign="top" width="20.52%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0133467989_p881355511346"><a name="zh-cn_topic_0133467989_p881355511346"></a><a name="zh-cn_topic_0133467989_p881355511346"></a>city.temp</p>
</td>
</tr>
<tr id="zh-cn_topic_0133467989_row1431725743415"><td class="cellrowborder" valign="top" width="18.279999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0133467989_p3317457133416"><a name="zh-cn_topic_0133467989_p3317457133416"></a><a name="zh-cn_topic_0133467989_p3317457133416"></a>聚合函数</p>
</td>
<td class="cellrowborder" valign="top" width="61.199999999999996%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0133467989_p1631810574340"><a name="zh-cn_topic_0133467989_p1631810574340"></a><a name="zh-cn_topic_0133467989_p1631810574340"></a>输入聚合函数。</p>
</td>
<td class="cellrowborder" valign="top" width="20.52%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0133467989_p15318175714341"><a name="zh-cn_topic_0133467989_p15318175714341"></a><a name="zh-cn_topic_0133467989_p15318175714341"></a>sum</p>
</td>
</tr>
<tr id="zh-cn_topic_0133467989_row667043895219"><td class="cellrowborder" valign="top" width="18.279999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0133467989_p1967023835217"><a name="zh-cn_topic_0133467989_p1967023835217"></a><a name="zh-cn_topic_0133467989_p1967023835217"></a>标记</p>
</td>
<td class="cellrowborder" valign="top" width="61.199999999999996%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0133467989_p091005834018"><a name="zh-cn_topic_0133467989_p091005834018"></a><a name="zh-cn_topic_0133467989_p091005834018"></a>可选参数，如果这里有输入标记，则只迁移标记的数据。</p>
</td>
<td class="cellrowborder" valign="top" width="20.52%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0133467989_p49421616115718"><a name="zh-cn_topic_0133467989_p49421616115718"></a><a name="zh-cn_topic_0133467989_p49421616115718"></a>tagk1:tagv1,tagk2:tagv2</p>
</td>
</tr>
</tbody>
</table>

