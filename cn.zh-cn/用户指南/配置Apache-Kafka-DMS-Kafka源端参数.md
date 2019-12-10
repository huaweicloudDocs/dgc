# 配置Apache Kafka/DMS Kafka源端参数<a name="dayu_01_0058"></a>

目前仅支持从Kafka导出数据到云搜索服务、DMS Kafka、DIS。

作业中源连接为[配置Kafka连接](配置Kafka连接.md)或[配置DMS Kafka连接](配置DMS-Kafka连接.md)时，源端作业参数如[表1](#zh-cn_topic_0108275337_table45985388113529)所示。

**表 1**  Kafka作为源端时的作业参数

<a name="zh-cn_topic_0108275337_table45985388113529"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108275337_row1499348113529"><th class="cellrowborder" valign="top" width="24.54%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108275337_p54338376113529"><a name="zh-cn_topic_0108275337_p54338376113529"></a><a name="zh-cn_topic_0108275337_p54338376113529"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="56.48%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108275337_p39332299113529"><a name="zh-cn_topic_0108275337_p39332299113529"></a><a name="zh-cn_topic_0108275337_p39332299113529"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="18.98%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108275337_p31799688113529"><a name="zh-cn_topic_0108275337_p31799688113529"></a><a name="zh-cn_topic_0108275337_p31799688113529"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108275337_row29414735113529"><td class="cellrowborder" valign="top" width="24.54%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275337_p33783328113529"><a name="zh-cn_topic_0108275337_p33783328113529"></a><a name="zh-cn_topic_0108275337_p33783328113529"></a>Topics</p>
</td>
<td class="cellrowborder" valign="top" width="56.48%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275337_p52095013113529"><a name="zh-cn_topic_0108275337_p52095013113529"></a><a name="zh-cn_topic_0108275337_p52095013113529"></a>支持单个或多个topic。</p>
</td>
<td class="cellrowborder" valign="top" width="18.98%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275337_p58946502113529"><a name="zh-cn_topic_0108275337_p58946502113529"></a><a name="zh-cn_topic_0108275337_p58946502113529"></a>est1,est2</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275337_row60756477113529"><td class="cellrowborder" valign="top" width="24.54%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275337_p22327637113529"><a name="zh-cn_topic_0108275337_p22327637113529"></a><a name="zh-cn_topic_0108275337_p22327637113529"></a>偏移量参数</p>
</td>
<td class="cellrowborder" valign="top" width="56.48%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275337_p63708157113529"><a name="zh-cn_topic_0108275337_p63708157113529"></a><a name="zh-cn_topic_0108275337_p63708157113529"></a>从Kafka拉取数据时的初始偏移量：</p>
<a name="zh-cn_topic_0108275337_ul36502502113529"></a><a name="zh-cn_topic_0108275337_ul36502502113529"></a><ul id="zh-cn_topic_0108275337_ul36502502113529"><li>最新：最大偏移量，即拉取最新的数据。</li><li>最早：最小偏移量，即拉取最早的数据。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="18.98%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275337_p33796583113529"><a name="zh-cn_topic_0108275337_p33796583113529"></a><a name="zh-cn_topic_0108275337_p33796583113529"></a>最新</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275337_row35733799113529"><td class="cellrowborder" valign="top" width="24.54%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275337_p8756592113529"><a name="zh-cn_topic_0108275337_p8756592113529"></a><a name="zh-cn_topic_0108275337_p8756592113529"></a>是否持久运行</p>
</td>
<td class="cellrowborder" valign="top" width="56.48%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275337_p38195350113529"><a name="zh-cn_topic_0108275337_p38195350113529"></a><a name="zh-cn_topic_0108275337_p38195350113529"></a>用户自定义是否永久运行。</p>
</td>
<td class="cellrowborder" valign="top" width="18.98%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275337_p6815616113529"><a name="zh-cn_topic_0108275337_p6815616113529"></a><a name="zh-cn_topic_0108275337_p6815616113529"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275337_row15194006113529"><td class="cellrowborder" valign="top" width="24.54%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275337_p22755010113529"><a name="zh-cn_topic_0108275337_p22755010113529"></a><a name="zh-cn_topic_0108275337_p22755010113529"></a>消费组ID</p>
</td>
<td class="cellrowborder" valign="top" width="56.48%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275337_p1638011885013"><a name="zh-cn_topic_0108275337_p1638011885013"></a><a name="zh-cn_topic_0108275337_p1638011885013"></a>用户指定消费组ID。</p>
<p id="zh-cn_topic_0108275337_p1114017325017"><a name="zh-cn_topic_0108275337_p1114017325017"></a><a name="zh-cn_topic_0108275337_p1114017325017"></a>如果是从DMS Kafka导出数据，专享版请任意输入，标准版请输入有效的消费组ID。</p>
</td>
<td class="cellrowborder" valign="top" width="18.98%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275337_p45507701113529"><a name="zh-cn_topic_0108275337_p45507701113529"></a><a name="zh-cn_topic_0108275337_p45507701113529"></a>sumer-group</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275337_row9228163115910"><td class="cellrowborder" valign="top" width="24.54%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275337_p72289311596"><a name="zh-cn_topic_0108275337_p72289311596"></a><a name="zh-cn_topic_0108275337_p72289311596"></a>数据格式</p>
</td>
<td class="cellrowborder" valign="top" width="56.48%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275337_p111321138622"><a name="zh-cn_topic_0108275337_p111321138622"></a><a name="zh-cn_topic_0108275337_p111321138622"></a>解析数据时使用的格式：</p>
<a name="zh-cn_topic_0108275337_ul59573391929"></a><a name="zh-cn_topic_0108275337_ul59573391929"></a><ul id="zh-cn_topic_0108275337_ul59573391929"><li>二进制格式：适用于文件迁移场景，不解析数据内容原样传输。</li><li>CSV格式：以CSV格式解析源数据。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="18.98%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275337_p182286311598"><a name="zh-cn_topic_0108275337_p182286311598"></a><a name="zh-cn_topic_0108275337_p182286311598"></a>二进制格式</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275337_row62245198113529"><td class="cellrowborder" valign="top" width="24.54%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275337_p8696283113529"><a name="zh-cn_topic_0108275337_p8696283113529"></a><a name="zh-cn_topic_0108275337_p8696283113529"></a>字段分隔符</p>
</td>
<td class="cellrowborder" valign="top" width="56.48%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275337_p9802957173352"><a name="zh-cn_topic_0108275337_p9802957173352"></a><a name="zh-cn_topic_0108275337_p9802957173352"></a>默认为空格，使用Tab键作为分隔符请输入<span class="parmvalue" id="zh-cn_topic_0108275337_parmvalue6198888511118"><a name="zh-cn_topic_0108275337_parmvalue6198888511118"></a><a name="zh-cn_topic_0108275337_parmvalue6198888511118"></a>“\t”</span>。</p>
</td>
<td class="cellrowborder" valign="top" width="18.98%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275337_p56938959113529"><a name="zh-cn_topic_0108275337_p56938959113529"></a><a name="zh-cn_topic_0108275337_p56938959113529"></a>,</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275337_row48652991113529"><td class="cellrowborder" valign="top" width="24.54%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275337_p48578216113529"><a name="zh-cn_topic_0108275337_p48578216113529"></a><a name="zh-cn_topic_0108275337_p48578216113529"></a>最大消息数/poll</p>
</td>
<td class="cellrowborder" valign="top" width="56.48%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275337_p42521393113529"><a name="zh-cn_topic_0108275337_p42521393113529"></a><a name="zh-cn_topic_0108275337_p42521393113529"></a>可选参数，每次向Kafka请求数据限制最大请求记录数。</p>
</td>
<td class="cellrowborder" valign="top" width="18.98%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275337_p21680770113529"><a name="zh-cn_topic_0108275337_p21680770113529"></a><a name="zh-cn_topic_0108275337_p21680770113529"></a>100</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275337_row6670289111413"><td class="cellrowborder" valign="top" width="24.54%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275337_p3422508911413"><a name="zh-cn_topic_0108275337_p3422508911413"></a><a name="zh-cn_topic_0108275337_p3422508911413"></a>最大时间间隔/poll</p>
</td>
<td class="cellrowborder" valign="top" width="56.48%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275337_p2076879511413"><a name="zh-cn_topic_0108275337_p2076879511413"></a><a name="zh-cn_topic_0108275337_p2076879511413"></a>可选参数，向Kafka请求数据的最大时间间隔。</p>
</td>
<td class="cellrowborder" valign="top" width="18.98%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275337_p455081711413"><a name="zh-cn_topic_0108275337_p455081711413"></a><a name="zh-cn_topic_0108275337_p455081711413"></a>100</p>
</td>
</tr>
</tbody>
</table>

