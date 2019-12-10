# 配置Elasticsearch或云搜索服务目的端参数<a name="dayu_01_0071"></a>

作业中目的连接为[配置Elasticsearch/CSS连接](配置Elasticsearch-CSS连接.md)，即将数据导入到云搜索服务或Elasticsearch时，目的端作业参数如[表1](#zh-cn_topic_0108275347_table5046103815165)所示。

**表 1**  Elasticsearch作为目的端时的作业参数

<a name="zh-cn_topic_0108275347_table5046103815165"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108275347_row585315215165"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108275347_p1626397215165"><a name="zh-cn_topic_0108275347_p1626397215165"></a><a name="zh-cn_topic_0108275347_p1626397215165"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="55.00000000000001%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108275347_p4231334915165"><a name="zh-cn_topic_0108275347_p4231334915165"></a><a name="zh-cn_topic_0108275347_p4231334915165"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108275347_p482921015165"><a name="zh-cn_topic_0108275347_p482921015165"></a><a name="zh-cn_topic_0108275347_p482921015165"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108275347_row4012116315165"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275347_p2858877215165"><a name="zh-cn_topic_0108275347_p2858877215165"></a><a name="zh-cn_topic_0108275347_p2858877215165"></a>索引</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275347_p15492661577"><a name="zh-cn_topic_0108275347_p15492661577"></a><a name="zh-cn_topic_0108275347_p15492661577"></a>待写入数据的Elasticsearch的索引，类似关系数据库中的数据库名称。<span id="zh-cn_topic_0108275347_ph1997374045914"><a name="zh-cn_topic_0108275347_ph1997374045914"></a><a name="zh-cn_topic_0108275347_ph1997374045914"></a>CDM支持自动创建索引和类型，索引和类型名称只能全部小写，不能有大写。</span></p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275347_p166427315165"><a name="zh-cn_topic_0108275347_p166427315165"></a><a name="zh-cn_topic_0108275347_p166427315165"></a>index</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275347_row1497845915165"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275347_p529563715165"><a name="zh-cn_topic_0108275347_p529563715165"></a><a name="zh-cn_topic_0108275347_p529563715165"></a>类型</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275347_p527763715824"><a name="zh-cn_topic_0108275347_p527763715824"></a><a name="zh-cn_topic_0108275347_p527763715824"></a>待写入数据的Elasticsearch的类型，类似关系数据库中的表名称。类型名称只能全部小写，不能有大写。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275347_p3753014815165"><a name="zh-cn_topic_0108275347_p3753014815165"></a><a name="zh-cn_topic_0108275347_p3753014815165"></a>type</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275347_row1271559105513"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275347_p57115925517"><a name="zh-cn_topic_0108275347_p57115925517"></a><a name="zh-cn_topic_0108275347_p57115925517"></a>管道ID</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275347_p8755914553"><a name="zh-cn_topic_0108275347_p8755914553"></a><a name="zh-cn_topic_0108275347_p8755914553"></a>需要先在kibana中创建管道ID，这里才可以选择，该参数用于数据传到Elasticsearch后，通过Elasticsearch的数据转换pipeline进行数据格式变换。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275347_p1171859185510"><a name="zh-cn_topic_0108275347_p1171859185510"></a><a name="zh-cn_topic_0108275347_p1171859185510"></a>pipeline_id</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275347_row1435112005414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275347_p935120165411"><a name="zh-cn_topic_0108275347_p935120165411"></a><a name="zh-cn_topic_0108275347_p935120165411"></a>定时创索引</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108275347_p53511015420"><a name="zh-cn_topic_0108275347_p53511015420"></a><a name="zh-cn_topic_0108275347_p53511015420"></a>对于持续写入数据到Elasticsearch的流式作业，CDM支持在Elasticsearch中定时创建新索引并写入数据，方便用户后期删除过期的数据。支持按以下周期创建新索引：<a name="zh-cn_topic_0108275347_ul112848823812"></a><a name="zh-cn_topic_0108275347_ul112848823812"></a><ul id="zh-cn_topic_0108275347_ul112848823812"><li>每小时：每小时整点创建新索引，新索引的命名格式为<span class="parmvalue" id="zh-cn_topic_0108275347_parmvalue166091542527"><a name="zh-cn_topic_0108275347_parmvalue166091542527"></a><a name="zh-cn_topic_0108275347_parmvalue166091542527"></a>“索引名+年+月+日+小时”</span>，例如<span class="parmvalue" id="zh-cn_topic_0108275347_parmvalue97280286527"><a name="zh-cn_topic_0108275347_parmvalue97280286527"></a><a name="zh-cn_topic_0108275347_parmvalue97280286527"></a>“index2018121709”</span>。</li><li>每天：每天零点零分创建新索引，新索引的命名格式为<span class="parmvalue" id="zh-cn_topic_0108275347_parmvalue13376104820546"><a name="zh-cn_topic_0108275347_parmvalue13376104820546"></a><a name="zh-cn_topic_0108275347_parmvalue13376104820546"></a>“索引名+年+月+日”</span>，例如<span class="parmvalue" id="zh-cn_topic_0108275347_parmvalue83912311554"><a name="zh-cn_topic_0108275347_parmvalue83912311554"></a><a name="zh-cn_topic_0108275347_parmvalue83912311554"></a>“index20181217”</span>。</li><li>每周：每周周一的零点零分创建新索引，新索引的命名格式为<span class="parmvalue" id="zh-cn_topic_0108275347_parmvalue125511630145612"><a name="zh-cn_topic_0108275347_parmvalue125511630145612"></a><a name="zh-cn_topic_0108275347_parmvalue125511630145612"></a>“索引名+年+周”</span>，例如<span class="parmvalue" id="zh-cn_topic_0108275347_parmvalue19461055135616"><a name="zh-cn_topic_0108275347_parmvalue19461055135616"></a><a name="zh-cn_topic_0108275347_parmvalue19461055135616"></a>“index201842”</span>。</li><li>每月：每月一号零点零分创建新索引，新索引的命名格式为<span class="parmvalue" id="zh-cn_topic_0108275347_parmvalue5856103018585"><a name="zh-cn_topic_0108275347_parmvalue5856103018585"></a><a name="zh-cn_topic_0108275347_parmvalue5856103018585"></a>“索引名+年+月”</span>，例如<span class="parmvalue" id="zh-cn_topic_0108275347_parmvalue43841656105818"><a name="zh-cn_topic_0108275347_parmvalue43841656105818"></a><a name="zh-cn_topic_0108275347_parmvalue43841656105818"></a>“index201812”</span>。</li></ul>
</div>
<p id="zh-cn_topic_0108275347_p837316411590"><a name="zh-cn_topic_0108275347_p837316411590"></a><a name="zh-cn_topic_0108275347_p837316411590"></a>从文件类抽取数据时，必须配置单个抽取（<span class="parmname" id="zh-cn_topic_0108275347_parmname51503147198"><a name="zh-cn_topic_0108275347_parmname51503147198"></a><a name="zh-cn_topic_0108275347_parmname51503147198"></a>“抽取并发数”</span>参数配置为1），否则该参数无效。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275347_p19351806548"><a name="zh-cn_topic_0108275347_p19351806548"></a><a name="zh-cn_topic_0108275347_p19351806548"></a>每小时</p>
</td>
</tr>
</tbody>
</table>

