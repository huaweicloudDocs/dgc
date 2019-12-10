# 转储至CloudTable<a name="dayu_01_0217"></a>

## 源数据类型JSON/CSV==\>CloudTable类型HBase<a name="zh-cn_topic_0165739441_section5760185410392"></a>

**表 1**  转储相关配置参数

<a name="zh-cn_topic_0165739441_table18468165816451"></a>
<table><thead align="left"><tr id="zh-cn_topic_0165739441_row15468165811456"><th class="cellrowborder" valign="top" width="21.08210821082108%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0165739441_p1746865813454"><a name="zh-cn_topic_0165739441_p1746865813454"></a><a name="zh-cn_topic_0165739441_p1746865813454"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="56.66566656665667%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0165739441_p1746811580453"><a name="zh-cn_topic_0165739441_p1746811580453"></a><a name="zh-cn_topic_0165739441_p1746811580453"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="22.252225222522252%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0165739441_p184682582458"><a name="zh-cn_topic_0165739441_p184682582458"></a><a name="zh-cn_topic_0165739441_p184682582458"></a>取值</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0165739441_row846805820453"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739441_p4468195810455"><a name="zh-cn_topic_0165739441_p4468195810455"></a><a name="zh-cn_topic_0165739441_p4468195810455"></a>任务名称</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p15371132211357"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p15371132211357"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p15371132211357"></a>用户创建转储任务时，需要指定转储任务名称，同一通道的转储任务名称不可重复。任务名称由<span id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_text2371822163519"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_text2371822163519"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_text2371822163519"></a>英文字母、数字、中划线和下划线组成。</span>长度为1～64个字符。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p9371522113518"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p9371522113518"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p9371522113518"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739441_row118972181498"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739441_p188972181392"><a name="zh-cn_topic_0165739441_p188972181392"></a><a name="zh-cn_topic_0165739441_p188972181392"></a>源数据Schema</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739441_p5969122711441"><a name="zh-cn_topic_0165739441_p5969122711441"></a><a name="zh-cn_topic_0165739441_p5969122711441"></a>用户的JSON或CSV数据样例，用于描述JSON或CSV数据格式。DIS可以根据此JSON或CSV数据样例生成Avro schema。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739441_p1689718181896"><a name="zh-cn_topic_0165739441_p1689718181896"></a><a name="zh-cn_topic_0165739441_p1689718181896"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739441_row346865813454"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739441_p181884311917"><a name="zh-cn_topic_0165739441_p181884311917"></a><a name="zh-cn_topic_0165739441_p181884311917"></a>CloudTable集群</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p93873227356"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p93873227356"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p93873227356"></a>单击“选择”，在“选择CloudTable集群”窗口选择一个集群名称。</p>
<p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p1738713222358"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p1738713222358"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p1738713222358"></a>此配置项不可配置为空。仅支持选择，不可手动输入。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p14387122133517"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p14387122133517"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p14387122133517"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739441_row17888513010"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739441_p111316431994"><a name="zh-cn_topic_0165739441_p111316431994"></a><a name="zh-cn_topic_0165739441_p111316431994"></a>CloudTable表类型</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p17387132215359"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p17387132215359"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p17387132215359"></a>HBase和openTSDB两种。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739441_p10955233814"><a name="zh-cn_topic_0165739441_p10955233814"></a><a name="zh-cn_topic_0165739441_p10955233814"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739441_row174699584459"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739441_p076434910"><a name="zh-cn_topic_0165739441_p076434910"></a><a name="zh-cn_topic_0165739441_p076434910"></a>CloudTable数据表</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p838762253514"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p838762253514"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p838762253514"></a>CloudTable数据表：单击“选择”，在“选择CloudTable数据表”窗口选择一个数据表。</p>
<p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p538742283514"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p538742283514"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p538742283514"></a>此处路径仅支持选择，不可手动输入。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p1238752263513"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p1238752263513"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p1238752263513"></a>配置此项必须已配置“CloudTable集群”并创建了HBase表。</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739441_row154692588456"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739441_p121943297"><a name="zh-cn_topic_0165739441_p121943297"></a><a name="zh-cn_topic_0165739441_p121943297"></a>偏移量</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul19387202217353"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul19387202217353"></a><ul id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul19387202217353"><li>最新：最大偏移量，即获取最新的有效数据。</li><li>最早：最小偏移量，即读取最早的有效数据。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739441_p199115253816"><a name="zh-cn_topic_0165739441_p199115253816"></a><a name="zh-cn_topic_0165739441_p199115253816"></a>最新</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739441_row14351951154713"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739441_p16997642190"><a name="zh-cn_topic_0165739441_p16997642190"></a><a name="zh-cn_topic_0165739441_p16997642190"></a>备份开关</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p11387142253513"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p11387142253513"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p11387142253513"></a>用户数据转储CloudTable服务失败时，是否将转储失败的数据备份至OBS服务。</p>
<a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul838717220358"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul838717220358"></a><ul id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul838717220358"><li>开启：是，转储失败的数据备份至OBS服务。</li><li>关闭：否，转储失败的数据不备份至OBS服务。</li></ul>
<p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p6387122213517"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p6387122213517"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p6387122213517"></a>开关默认关闭。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p5387112223517"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p5387112223517"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p5387112223517"></a>关闭开关，转储失败的数据会存储在DIS中，并在<span class="parmname" id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_parmname203871822133518"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_parmname203871822133518"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_parmname203871822133518"></a>“生命周期”</span>配置的时间到达时将数据清除。</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739441_row7508810153116"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739441_p189906421918"><a name="zh-cn_topic_0165739441_p189906421918"></a><a name="zh-cn_topic_0165739441_p189906421918"></a>失败记录备份桶</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p438782211354"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p438782211354"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p438782211354"></a>转储失败记录会存储在用户指定的OBS桶中。</p>
<p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p1138720221351"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p1138720221351"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p1138720221351"></a>此配置项仅支持选择，不可手动输入。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p438716228356"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p438716228356"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p438716228356"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739441_row119451913118"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739441_p1998715421994"><a name="zh-cn_topic_0165739441_p1998715421994"></a><a name="zh-cn_topic_0165739441_p1998715421994"></a>失败记录备份目录</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p11387202243514"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p11387202243514"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p11387202243514"></a>转储失败记录存储在OBS桶下该配置项配置的目录中。</p>
<p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p53871522193514"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p53871522193514"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p53871522193514"></a>配置为空，则转储失败记录存储在<span class="parmname" id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_parmname9387162213352"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_parmname9387162213352"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_parmname9387162213352"></a>“失败记录备份桶”</span>内。</p>
<p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p1438713229359"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p1438713229359"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p1438713229359"></a>取值范围：英文字母、数字、“_”和“/”，且不可以“/”开头。</p>
<p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p438772215352"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p438772215352"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p438772215352"></a>最大长度：最大长度为50个字符。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p7387112220350"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p7387112220350"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p7387112220350"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739441_row14501443353"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739441_p1045074143511"><a name="zh-cn_topic_0165739441_p1045074143511"></a><a name="zh-cn_topic_0165739441_p1045074143511"></a>Row Key</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul9387102213351"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul9387102213351"></a><ul id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul9387102213351"><li>Json属性名，取值范围为英文字母、数字、下划线和小数点，最大取值为32个字符，不可为空，不可以小数点开头，不可包含连续的小数点 且不可以小数点结尾。最多可添加64个属性。</li><li>数据类型，从下拉框选择。<a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul63874222350"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul63874222350"></a><ul id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul63874222350"><li>Bigint</li><li>Double</li><li>Boolean</li><li>Timestamp</li><li>String</li><li>Decimal</li></ul>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p038711227351"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p038711227351"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p038711227351"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739441_row10711819143511"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739441_p8711419173516"><a name="zh-cn_topic_0165739441_p8711419173516"></a><a name="zh-cn_topic_0165739441_p8711419173516"></a>Row Key分隔符</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p1038702263515"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p1038702263515"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p1038702263515"></a>支持<span class="parmvalue" id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_parmvalue4387122113519"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_parmvalue4387122113519"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_parmvalue4387122113519"></a>“.”</span>、<span class="parmvalue" id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_parmvalue838714221354"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_parmvalue838714221354"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_parmvalue838714221354"></a>“,”</span>、<span class="parmvalue" id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_parmvalue43872022103510"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_parmvalue43872022103510"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_parmvalue43872022103510"></a>“|”</span>、<span class="parmvalue" id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_parmvalue1338732210350"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_parmvalue1338732210350"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_parmvalue1338732210350"></a>“;”</span>、<span class="parmvalue" id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_parmvalue03871822183513"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_parmvalue03871822183513"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_parmvalue03871822183513"></a>“-”</span>、<span class="parmvalue" id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_parmvalue1638720224353"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_parmvalue1638720224353"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_parmvalue1638720224353"></a>“_”</span>、和<span class="parmvalue" id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_parmvalue438752243516"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_parmvalue438752243516"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_parmvalue438752243516"></a>“~”</span>七种字符取值，也可配置为NULL。</p>
<p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p738702253511"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p738702253511"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p738702253511"></a>最大长度为一个字符。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p1638716225351"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p1638716225351"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p1638716225351"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739441_row37321934123510"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739441_p1773318347352"><a name="zh-cn_topic_0165739441_p1773318347352"></a><a name="zh-cn_topic_0165739441_p1773318347352"></a>Schema列</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul3434622103513"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul3434622103513"></a><ul id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul3434622103513"><li>列名，取值范围为英文字母、数字和下划线，最大取值为32个字符，不可为空。最多可添加4096个列。</li><li>数据类型，从下拉框选择。<a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul124343223355"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul124343223355"></a><ul id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul124343223355"><li>Bigint</li><li>Double</li><li>Boolean</li><li>Timestamp</li><li>String</li><li>Decimal</li></ul>
</li><li>Json属性名，取值范围为英文字母、数字、下划线和小数点，最大取值为32个字符，不可为空，不可以小数点开头，不可包含连续的小数点 且不可以小数点结尾。</li><li>所属列族，从下拉框选择，不可为空。配置此项必须已配置“CloudTable 集群”、“CloudTable 数据表”且CloudTable表类型为HBase。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p16434202219352"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p16434202219352"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p16434202219352"></a>-</p>
</td>
</tr>
</tbody>
</table>

## 源数据类型JSON/CSV==\>CloudTable类型openTSDB<a name="zh-cn_topic_0165739441_section137712381462"></a>

**表 2**  转储相关配置参数

<a name="zh-cn_topic_0165739441_table167721381261"></a>
<table><thead align="left"><tr id="zh-cn_topic_0165739441_row1677216381068"><th class="cellrowborder" valign="top" width="21.08210821082108%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0165739441_p27722382066"><a name="zh-cn_topic_0165739441_p27722382066"></a><a name="zh-cn_topic_0165739441_p27722382066"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="56.66566656665667%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0165739441_p15772138663"><a name="zh-cn_topic_0165739441_p15772138663"></a><a name="zh-cn_topic_0165739441_p15772138663"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="22.252225222522252%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0165739441_p377223813614"><a name="zh-cn_topic_0165739441_p377223813614"></a><a name="zh-cn_topic_0165739441_p377223813614"></a>取值</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0165739441_row57728384620"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739441_p2077216380617"><a name="zh-cn_topic_0165739441_p2077216380617"></a><a name="zh-cn_topic_0165739441_p2077216380617"></a>任务名称</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739441_p11772638764"><a name="zh-cn_topic_0165739441_p11772638764"></a><a name="zh-cn_topic_0165739441_p11772638764"></a>用户创建转储任务时，需要指定转储任务名称，同一通道的转储任务名称不可重复。任务名称由<span id="zh-cn_topic_0165739441_text977211381762"><a name="zh-cn_topic_0165739441_text977211381762"></a><a name="zh-cn_topic_0165739441_text977211381762"></a>英文字母、数字、中划线和下划线组成。</span>长度为1～64个字符。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739441_p187722387615"><a name="zh-cn_topic_0165739441_p187722387615"></a><a name="zh-cn_topic_0165739441_p187722387615"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739441_row1877212386616"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739441_p1577219388613"><a name="zh-cn_topic_0165739441_p1577219388613"></a><a name="zh-cn_topic_0165739441_p1577219388613"></a>源数据Schema</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739441_p477210382063"><a name="zh-cn_topic_0165739441_p477210382063"></a><a name="zh-cn_topic_0165739441_p477210382063"></a>用户的JSON或CSV数据样例，用于描述JSON或CSV数据格式。DIS可以根据此JSON或CSV数据样例生成Avro schema。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739441_p177219383617"><a name="zh-cn_topic_0165739441_p177219383617"></a><a name="zh-cn_topic_0165739441_p177219383617"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739441_row15772123815615"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739441_p8773138769"><a name="zh-cn_topic_0165739441_p8773138769"></a><a name="zh-cn_topic_0165739441_p8773138769"></a>CloudTable集群</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739441_p1377311389614"><a name="zh-cn_topic_0165739441_p1377311389614"></a><a name="zh-cn_topic_0165739441_p1377311389614"></a>单击“选择”，在“选择CloudTable集群”窗口选择一个集群名称。</p>
<p id="zh-cn_topic_0165739441_p377313814618"><a name="zh-cn_topic_0165739441_p377313814618"></a><a name="zh-cn_topic_0165739441_p377313814618"></a>此配置项不可配置为空。仅支持选择，不可手动输入。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739441_p5773238362"><a name="zh-cn_topic_0165739441_p5773238362"></a><a name="zh-cn_topic_0165739441_p5773238362"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739441_row2773138664"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739441_p777312385610"><a name="zh-cn_topic_0165739441_p777312385610"></a><a name="zh-cn_topic_0165739441_p777312385610"></a>CloudTable表类型</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739441_p67736381164"><a name="zh-cn_topic_0165739441_p67736381164"></a><a name="zh-cn_topic_0165739441_p67736381164"></a>HBase和openTSDB两种。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739441_p1077313383611"><a name="zh-cn_topic_0165739441_p1077313383611"></a><a name="zh-cn_topic_0165739441_p1077313383611"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739441_row1177333811618"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739441_p18773038863"><a name="zh-cn_topic_0165739441_p18773038863"></a><a name="zh-cn_topic_0165739441_p18773038863"></a>CloudTable数据表</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739441_p77736381762"><a name="zh-cn_topic_0165739441_p77736381762"></a><a name="zh-cn_topic_0165739441_p77736381762"></a>CloudTable数据表：单击“选择”，在“选择CloudTable数据表”窗口选择一个数据表。</p>
<p id="zh-cn_topic_0165739441_p1977313381168"><a name="zh-cn_topic_0165739441_p1977313381168"></a><a name="zh-cn_topic_0165739441_p1977313381168"></a>此处路径仅支持选择，不可手动输入。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739441_p1677310381067"><a name="zh-cn_topic_0165739441_p1677310381067"></a><a name="zh-cn_topic_0165739441_p1677310381067"></a>配置此项必须已配置“CloudTable集群”并创建了openTSDB表。</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739441_row177310381666"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739441_p6773173817613"><a name="zh-cn_topic_0165739441_p6773173817613"></a><a name="zh-cn_topic_0165739441_p6773173817613"></a>偏移量</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><a name="zh-cn_topic_0165739441_ul1377315381367"></a><a name="zh-cn_topic_0165739441_ul1377315381367"></a><ul id="zh-cn_topic_0165739441_ul1377315381367"><li>最新：最大偏移量，即获取最新的有效数据。</li><li>最早：最小偏移量，即读取最早的有效数据。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739441_p187744381968"><a name="zh-cn_topic_0165739441_p187744381968"></a><a name="zh-cn_topic_0165739441_p187744381968"></a>最新</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739441_row107741838664"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739441_p57745381768"><a name="zh-cn_topic_0165739441_p57745381768"></a><a name="zh-cn_topic_0165739441_p57745381768"></a>备份开关</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739441_p377411382063"><a name="zh-cn_topic_0165739441_p377411382063"></a><a name="zh-cn_topic_0165739441_p377411382063"></a>用户数据转储CloudTable服务失败时，是否将转储失败的数据备份至OBS服务。</p>
<a name="zh-cn_topic_0165739441_ul877423818617"></a><a name="zh-cn_topic_0165739441_ul877423818617"></a><ul id="zh-cn_topic_0165739441_ul877423818617"><li>开启：是，转储失败的数据备份至OBS服务。</li><li>关闭：否，转储失败的数据不备份至OBS服务。</li></ul>
<p id="zh-cn_topic_0165739441_p17741638463"><a name="zh-cn_topic_0165739441_p17741638463"></a><a name="zh-cn_topic_0165739441_p17741638463"></a>开关默认关闭。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739441_p157741838560"><a name="zh-cn_topic_0165739441_p157741838560"></a><a name="zh-cn_topic_0165739441_p157741838560"></a>关闭开关，转储失败的数据会存储在DIS中，并在<span class="parmname" id="zh-cn_topic_0165739441_parmname1977415381260"><a name="zh-cn_topic_0165739441_parmname1977415381260"></a><a name="zh-cn_topic_0165739441_parmname1977415381260"></a>“生命周期”</span>配置的时间到达时将数据清除。</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739441_row1477411385619"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739441_p177747380615"><a name="zh-cn_topic_0165739441_p177747380615"></a><a name="zh-cn_topic_0165739441_p177747380615"></a>失败记录备份桶</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739441_p117758385617"><a name="zh-cn_topic_0165739441_p117758385617"></a><a name="zh-cn_topic_0165739441_p117758385617"></a>转储失败记录会存储在用户指定的OBS桶中。</p>
<p id="zh-cn_topic_0165739441_p977523813619"><a name="zh-cn_topic_0165739441_p977523813619"></a><a name="zh-cn_topic_0165739441_p977523813619"></a>此配置项仅支持选择，不可手动输入。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739441_p777514388618"><a name="zh-cn_topic_0165739441_p777514388618"></a><a name="zh-cn_topic_0165739441_p777514388618"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739441_row117751638564"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739441_p13775038264"><a name="zh-cn_topic_0165739441_p13775038264"></a><a name="zh-cn_topic_0165739441_p13775038264"></a>失败记录备份目录</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739441_p1775538263"><a name="zh-cn_topic_0165739441_p1775538263"></a><a name="zh-cn_topic_0165739441_p1775538263"></a>转储失败记录存储在OBS桶下该配置项配置的目录中。</p>
<p id="zh-cn_topic_0165739441_p17756382067"><a name="zh-cn_topic_0165739441_p17756382067"></a><a name="zh-cn_topic_0165739441_p17756382067"></a>配置为空，则转储失败记录存储在<span class="parmname" id="zh-cn_topic_0165739441_parmname1977573814615"><a name="zh-cn_topic_0165739441_parmname1977573814615"></a><a name="zh-cn_topic_0165739441_parmname1977573814615"></a>“失败记录备份桶”</span>内。</p>
<p id="zh-cn_topic_0165739441_p1277515381364"><a name="zh-cn_topic_0165739441_p1277515381364"></a><a name="zh-cn_topic_0165739441_p1277515381364"></a>取值范围：英文字母、数字、“_”和“/”，且不可以“/”开头。</p>
<p id="zh-cn_topic_0165739441_p1775113811610"><a name="zh-cn_topic_0165739441_p1775113811610"></a><a name="zh-cn_topic_0165739441_p1775113811610"></a>最大长度：最大长度为50个字符。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739441_p97751738166"><a name="zh-cn_topic_0165739441_p97751738166"></a><a name="zh-cn_topic_0165739441_p97751738166"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739441_row11776133820617"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p1943422283514"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p1943422283514"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p1943422283514"></a>Metric：CloudTable集群OpenTSDB数据metric的Schema配置，用于将通道内的JSON数据进行格式转换生成OpenTSDB数据的metric。</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul14449172253514"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul14449172253514"></a><ul id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul14449172253514"><li>Json属性名，取值范围为英文字母、数字、下划线和小数点，最大取值为32个字符，不可为空，不可以小数点开头，不可包含连续的小数点 且不可以小数点结尾。</li><li>数据类型，从下拉框选择。<a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul24491122153510"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul24491122153510"></a><ul id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul24491122153510"><li>String</li><li>Constant</li></ul>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p1844992213358"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p1844992213358"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p1844992213358"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739441_row157771938965"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p74491322183513"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p74491322183513"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p74491322183513"></a>Timestamp：CloudTable集群OpenTSDB数据timestamp的Schema配置，用于将通道内的JSON数据进行格式转换生成OpenTSDB数据的timestamp。</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul1744912229353"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul1744912229353"></a><ul id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul1744912229353"><li>Json属性名，取值范围为英文字母、数字、下划线和小数点，最大取值为32个字符，不可为空，不可以小数点开头，不可包含连续的小数点 且不可以小数点结尾。</li><li>时间戳的格式，从下拉框中选择。<p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p3449122218353"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p3449122218353"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p3449122218353"></a>yyyy/MM/dd HH:mm:ss</p>
<p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p17449122218355"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p17449122218355"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p17449122218355"></a>MM/dd/yyyy HH:mm:ss</p>
<p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p14449192243511"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p14449192243511"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p14449192243511"></a>dd/MM/yyyy HH:mm:ss</p>
<p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p444992223514"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p444992223514"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p444992223514"></a>yyyy-MM-dd HH:mm:ss</p>
<p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p1644992216353"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p1644992216353"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p1644992216353"></a>MM-dd-yyyy HH:mm:ss</p>
<p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p1944902243517"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p1944902243517"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p1944902243517"></a>dd-MM-yyyy HH:mm:ss</p>
</li><li>数据类型，从下拉框中选择。<a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul9449112253518"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul9449112253518"></a><ul id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul9449112253518"><li>String</li><li>Timestamp</li></ul>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p204492227353"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p204492227353"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p204492227353"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739441_row4779173811617"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p6449822153520"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p6449822153520"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p6449822153520"></a>Value：CloudTable集群OpenTSDB 数据value的Schema配置，用于将通道内的JSON数据进行格式转换生成OpenTSDB 数据的value</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul3449422123510"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul3449422123510"></a><ul id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul3449422123510"><li>Json属性名，取值范围为英文字母、数字、下划线和小数点，最大取值为32个字符，不可为空，不可以小数点开头，不可包含连续的小数点 且不可以小数点结尾。</li><li>数据类型，从下拉框选择。<a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul744972273512"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul744972273512"></a><ul id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul744972273512"><li>Bigint</li><li>Double</li><li>Boolean</li><li>Timestamp</li><li>String</li><li>Decimal</li></ul>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p1844916222351"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p1844916222351"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p1844916222351"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739441_row153163041613"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p144932283519"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p144932283519"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p144932283519"></a>Tags：CloudTable集群OpenTSDB数据tags的Schema配置，用于将通道内的JSON数据进行格式转换生成OpenTSDB数据的tags。</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul1344912215351"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul1344912215351"></a><ul id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul1344912215351"><li>Tag名：取值范围为英文字母、数字、下划线，最大取值为32个字符，不可为空。</li><li>数据类型，从下拉框选择。<a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul154491122133511"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul154491122133511"></a><ul id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_ul154491122133511"><li>Bigint</li><li>Double</li><li>Boolean</li><li>Timestamp</li><li>String</li><li>Decimal</li><li>Constant</li></ul>
</li><li>Json属性名，取值范围为英文字母、数字、下划线和小数点，最大取值为32个字符，不可为空，不可以小数点开头，不可包含连续的小数点 且不可以小数点结尾。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p12449192212353"><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p12449192212353"></a><a name="zh-cn_topic_0165739441_zh-cn_topic_0120206045_p12449192212353"></a>-</p>
</td>
</tr>
</tbody>
</table>

