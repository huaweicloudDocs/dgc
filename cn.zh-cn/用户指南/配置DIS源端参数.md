# 配置DIS源端参数<a name="dayu_01_0057"></a>

目前仅支持从DIS导出数据到云搜索服务、Apache Kafka、DMS Kafka。

消息体中的数据是一条类似CSV格式的记录，可以支持多种分隔符。不支持二进制格式或其他格式的消息内容解析。

作业中源连接为[配置DIS连接](配置DIS连接.md)时，源端作业参数如所[表1](#zh-cn_topic_0108275320_table13922888141527)示。

**表 1**  DIS作为源端时的作业参数

<a name="zh-cn_topic_0108275320_table13922888141527"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108275320_row229143141527"><th class="cellrowborder" valign="top" width="24.54%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108275320_p66756185141527"><a name="zh-cn_topic_0108275320_p66756185141527"></a><a name="zh-cn_topic_0108275320_p66756185141527"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="56.48%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108275320_p7459369141527"><a name="zh-cn_topic_0108275320_p7459369141527"></a><a name="zh-cn_topic_0108275320_p7459369141527"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="18.98%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108275320_p51516676172428"><a name="zh-cn_topic_0108275320_p51516676172428"></a><a name="zh-cn_topic_0108275320_p51516676172428"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108275320_row62628929141527"><td class="cellrowborder" valign="top" width="24.54%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275320_p18560626141527"><a name="zh-cn_topic_0108275320_p18560626141527"></a><a name="zh-cn_topic_0108275320_p18560626141527"></a>DIS通道</p>
</td>
<td class="cellrowborder" valign="top" width="56.48%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275320_p32605071143018"><a name="zh-cn_topic_0108275320_p32605071143018"></a><a name="zh-cn_topic_0108275320_p32605071143018"></a>DIS的通道名。</p>
</td>
<td class="cellrowborder" valign="top" width="18.98%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275320_p12101217172428"><a name="zh-cn_topic_0108275320_p12101217172428"></a><a name="zh-cn_topic_0108275320_p12101217172428"></a>dis</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275320_row42094113141527"><td class="cellrowborder" valign="top" width="24.54%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275320_p26789449141527"><a name="zh-cn_topic_0108275320_p26789449141527"></a><a name="zh-cn_topic_0108275320_p26789449141527"></a>偏移量参数</p>
</td>
<td class="cellrowborder" valign="top" width="56.48%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108275320_p1561824172319"><a name="zh-cn_topic_0108275320_p1561824172319"></a><a name="zh-cn_topic_0108275320_p1561824172319"></a>设置从DIS拉取数据时的初始偏移量：<a name="zh-cn_topic_0108275320_ul4823568317828"></a><a name="zh-cn_topic_0108275320_ul4823568317828"></a><ul id="zh-cn_topic_0108275320_ul4823568317828"><li>最新：最大偏移量，即拉取最新的数据。</li><li>上次停止处：从上次停止处继续读取。</li><li>最早：最小偏移量，即拉取最早的数据。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="18.98%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275320_p40674502172428"><a name="zh-cn_topic_0108275320_p40674502172428"></a><a name="zh-cn_topic_0108275320_p40674502172428"></a>最新</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275320_row8336449141527"><td class="cellrowborder" valign="top" width="24.54%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275320_p29681527141527"><a name="zh-cn_topic_0108275320_p29681527141527"></a><a name="zh-cn_topic_0108275320_p29681527141527"></a>是否持久运行</p>
</td>
<td class="cellrowborder" valign="top" width="56.48%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275320_p31296545154541"><a name="zh-cn_topic_0108275320_p31296545154541"></a><a name="zh-cn_topic_0108275320_p31296545154541"></a>用户自定义是否永久运行。<span id="zh-cn_topic_0108275320_ph132881132114210"><a name="zh-cn_topic_0108275320_ph132881132114210"></a><a name="zh-cn_topic_0108275320_ph132881132114210"></a>设置为长久运行的任务，如果DIS系统发生中断，任务也会失败结束。</span></p>
</td>
<td class="cellrowborder" valign="top" width="18.98%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275320_p6300380172428"><a name="zh-cn_topic_0108275320_p6300380172428"></a><a name="zh-cn_topic_0108275320_p6300380172428"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275320_row4065400315124"><td class="cellrowborder" valign="top" width="24.54%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275320_p2824781215124"><a name="zh-cn_topic_0108275320_p2824781215124"></a><a name="zh-cn_topic_0108275320_p2824781215124"></a>DIS分区ID</p>
</td>
<td class="cellrowborder" valign="top" width="56.48%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275320_p6135724015124"><a name="zh-cn_topic_0108275320_p6135724015124"></a><a name="zh-cn_topic_0108275320_p6135724015124"></a>DIS分区ID，该参数支持输入多个分区ID，使用英文逗号（,）分隔。</p>
</td>
<td class="cellrowborder" valign="top" width="18.98%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275320_p40568778172428"><a name="zh-cn_topic_0108275320_p40568778172428"></a><a name="zh-cn_topic_0108275320_p40568778172428"></a>0,1,2</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275320_row110671119568"><td class="cellrowborder" valign="top" width="24.54%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275320_p72289311596"><a name="zh-cn_topic_0108275320_p72289311596"></a><a name="zh-cn_topic_0108275320_p72289311596"></a>数据格式</p>
</td>
<td class="cellrowborder" valign="top" width="56.48%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275320_p111321138622"><a name="zh-cn_topic_0108275320_p111321138622"></a><a name="zh-cn_topic_0108275320_p111321138622"></a>解析数据时使用的格式：</p>
<a name="zh-cn_topic_0108275320_ul59573391929"></a><a name="zh-cn_topic_0108275320_ul59573391929"></a><ul id="zh-cn_topic_0108275320_ul59573391929"><li>二进制格式：适用于文件迁移场景，不解析数据内容原样传输。</li><li>CSV格式：以CSV格式解析源数据。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="18.98%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275320_p182286311598"><a name="zh-cn_topic_0108275320_p182286311598"></a><a name="zh-cn_topic_0108275320_p182286311598"></a>二进制格式</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275320_row4268185173352"><td class="cellrowborder" valign="top" width="24.54%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275320_p10178715173352"><a name="zh-cn_topic_0108275320_p10178715173352"></a><a name="zh-cn_topic_0108275320_p10178715173352"></a>字段分隔符</p>
</td>
<td class="cellrowborder" valign="top" width="56.48%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275320_p9802957173352"><a name="zh-cn_topic_0108275320_p9802957173352"></a><a name="zh-cn_topic_0108275320_p9802957173352"></a>默认为空格，使用Tab键作为分隔符请输入<span class="parmvalue" id="zh-cn_topic_0108275320_parmvalue6198888511118"><a name="zh-cn_topic_0108275320_parmvalue6198888511118"></a><a name="zh-cn_topic_0108275320_parmvalue6198888511118"></a>“\t”</span>。</p>
</td>
<td class="cellrowborder" valign="top" width="18.98%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275320_p18004305172428"><a name="zh-cn_topic_0108275320_p18004305172428"></a><a name="zh-cn_topic_0108275320_p18004305172428"></a>,</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275320_row58484443172332"><td class="cellrowborder" valign="top" width="24.54%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275320_p52123033172339"><a name="zh-cn_topic_0108275320_p52123033172339"></a><a name="zh-cn_topic_0108275320_p52123033172339"></a>最大消息数/poll</p>
</td>
<td class="cellrowborder" valign="top" width="56.48%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275320_p61216145172339"><a name="zh-cn_topic_0108275320_p61216145172339"></a><a name="zh-cn_topic_0108275320_p61216145172339"></a>可选参数，每次向DIS请求数据限制最大请求记录数。</p>
</td>
<td class="cellrowborder" valign="top" width="18.98%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275320_p49062585172428"><a name="zh-cn_topic_0108275320_p49062585172428"></a><a name="zh-cn_topic_0108275320_p49062585172428"></a>100</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275320_row194441839154117"><td class="cellrowborder" valign="top" width="24.54%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275320_p1744413916416"><a name="zh-cn_topic_0108275320_p1744413916416"></a><a name="zh-cn_topic_0108275320_p1744413916416"></a>APP名字</p>
</td>
<td class="cellrowborder" valign="top" width="56.48%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275320_p444412398415"><a name="zh-cn_topic_0108275320_p444412398415"></a><a name="zh-cn_topic_0108275320_p444412398415"></a>配置用户数据消费程序的唯一标识符，不存在时会自动创建。</p>
</td>
<td class="cellrowborder" valign="top" width="18.98%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275320_p11444639184119"><a name="zh-cn_topic_0108275320_p11444639184119"></a><a name="zh-cn_topic_0108275320_p11444639184119"></a>cdm</p>
</td>
</tr>
</tbody>
</table>

