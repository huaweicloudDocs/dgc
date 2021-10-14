# 配置Elasticsearch或云搜索服务源端参数<a name="dgc_01_0059"></a>

作业中源连接为[配置Elasticsearch/云搜索服务（CSS）连接](配置Elasticsearch-云搜索服务（CSS）连接.md#dgc_01_0035)时，源端作业参数如[表1](#zh-cn_topic_0108275408_table5046103815165)所示。

**表 1**  Elasticsearch作为源端时的作业参数

<a name="zh-cn_topic_0108275408_table5046103815165"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108275408_row585315215165"><th class="cellrowborder" valign="top" width="17.948205179482052%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108275408_p1626397215165"><a name="zh-cn_topic_0108275408_p1626397215165"></a><a name="zh-cn_topic_0108275408_p1626397215165"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="63.313668633136686%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108275408_p4231334915165"><a name="zh-cn_topic_0108275408_p4231334915165"></a><a name="zh-cn_topic_0108275408_p4231334915165"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="18.738126187381262%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108275408_p482921015165"><a name="zh-cn_topic_0108275408_p482921015165"></a><a name="zh-cn_topic_0108275408_p482921015165"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108275408_row4012116315165"><td class="cellrowborder" valign="top" width="17.948205179482052%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275408_p2858877215165"><a name="zh-cn_topic_0108275408_p2858877215165"></a><a name="zh-cn_topic_0108275408_p2858877215165"></a>索引</p>
</td>
<td class="cellrowborder" valign="top" width="63.313668633136686%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275408_p15492661577"><a name="zh-cn_topic_0108275408_p15492661577"></a><a name="zh-cn_topic_0108275408_p15492661577"></a>Elasticsearch的索引，类似关系数据库中的数据库名称。索引名称只能全部小写，不能有大写。</p>
</td>
<td class="cellrowborder" valign="top" width="18.738126187381262%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275408_p166427315165"><a name="zh-cn_topic_0108275408_p166427315165"></a><a name="zh-cn_topic_0108275408_p166427315165"></a>index</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275408_row1497845915165"><td class="cellrowborder" valign="top" width="17.948205179482052%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275408_p529563715165"><a name="zh-cn_topic_0108275408_p529563715165"></a><a name="zh-cn_topic_0108275408_p529563715165"></a>类型</p>
</td>
<td class="cellrowborder" valign="top" width="63.313668633136686%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275408_p527763715824"><a name="zh-cn_topic_0108275408_p527763715824"></a><a name="zh-cn_topic_0108275408_p527763715824"></a>Elasticsearch的类型，类似关系数据库中的表名称。类型名称只能全部小写，不能有大写。</p>
</td>
<td class="cellrowborder" valign="top" width="18.738126187381262%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275408_p3753014815165"><a name="zh-cn_topic_0108275408_p3753014815165"></a><a name="zh-cn_topic_0108275408_p3753014815165"></a>type</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275408_row15286142463917"><td class="cellrowborder" valign="top" width="17.948205179482052%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275408_p142861324163913"><a name="zh-cn_topic_0108275408_p142861324163913"></a><a name="zh-cn_topic_0108275408_p142861324163913"></a>拆分nested类型字段</p>
</td>
<td class="cellrowborder" valign="top" width="63.313668633136686%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275408_p9286172411394"><a name="zh-cn_topic_0108275408_p9286172411394"></a><a name="zh-cn_topic_0108275408_p9286172411394"></a>可选参数，选择是否将nested字段的json内容拆分，例如：将<span class="uicontrol" id="zh-cn_topic_0108275408_uicontrol2957184253017"><a name="zh-cn_topic_0108275408_uicontrol2957184253017"></a><a name="zh-cn_topic_0108275408_uicontrol2957184253017"></a>“a:{ b:{ c:1, d:{ e:2, f:3 } } }”</span>拆成三个字段<span class="uicontrol" id="zh-cn_topic_0108275408_uicontrol139867186304"><a name="zh-cn_topic_0108275408_uicontrol139867186304"></a><a name="zh-cn_topic_0108275408_uicontrol139867186304"></a>“a.b.c”</span>、<span class="uicontrol" id="zh-cn_topic_0108275408_uicontrol62201525173012"><a name="zh-cn_topic_0108275408_uicontrol62201525173012"></a><a name="zh-cn_topic_0108275408_uicontrol62201525173012"></a>“a.b.d.e”</span>、<span class="uicontrol" id="zh-cn_topic_0108275408_uicontrol6379733173013"><a name="zh-cn_topic_0108275408_uicontrol6379733173013"></a><a name="zh-cn_topic_0108275408_uicontrol6379733173013"></a>“a.b.d.f”</span>。</p>
</td>
<td class="cellrowborder" valign="top" width="18.738126187381262%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275408_p728616244391"><a name="zh-cn_topic_0108275408_p728616244391"></a><a name="zh-cn_topic_0108275408_p728616244391"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275408_row4983279398"><td class="cellrowborder" valign="top" width="17.948205179482052%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275408_p169822715398"><a name="zh-cn_topic_0108275408_p169822715398"></a><a name="zh-cn_topic_0108275408_p169822715398"></a>过滤条件</p>
</td>
<td class="cellrowborder" valign="top" width="63.313668633136686%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275408_p16865173219416"><a name="zh-cn_topic_0108275408_p16865173219416"></a><a name="zh-cn_topic_0108275408_p16865173219416"></a>可选参数，使用Elasticsearch的查询字符串（query string）对源数据进行过滤，CDM只迁移满足过滤条件的数据。</p>
<p id="zh-cn_topic_0108275408_p12937154943213"><a name="zh-cn_topic_0108275408_p12937154943213"></a><a name="zh-cn_topic_0108275408_p12937154943213"></a>多条查询条件可以用大写“AND”分隔，且AND前后要有空格，例如：“last_name:Smith AND last_name:John”</p>
</td>
<td class="cellrowborder" valign="top" width="18.738126187381262%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275408_p398627133918"><a name="zh-cn_topic_0108275408_p398627133918"></a><a name="zh-cn_topic_0108275408_p398627133918"></a>last_name:Smith</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275408_row1969518119321"><td class="cellrowborder" valign="top" width="17.948205179482052%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275408_p413919913217"><a name="zh-cn_topic_0108275408_p413919913217"></a><a name="zh-cn_topic_0108275408_p413919913217"></a>抽取元字段</p>
</td>
<td class="cellrowborder" valign="top" width="63.313668633136686%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275408_p4695171163214"><a name="zh-cn_topic_0108275408_p4695171163214"></a><a name="zh-cn_topic_0108275408_p4695171163214"></a>表示是否抽取索引的元字段，目前只支持（_index、_type、_id、_score）例如：_index、_type、_id、_score</p>
</td>
<td class="cellrowborder" valign="top" width="18.738126187381262%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275408_p1269612110329"><a name="zh-cn_topic_0108275408_p1269612110329"></a><a name="zh-cn_topic_0108275408_p1269612110329"></a>是</p>
</td>
</tr>
</tbody>
</table>

在下一步的字段映射中，源端和目的端均支持配置自定义字段。

**图 1**  配置自定义字段<a name="zh-cn_topic_0108275408_fig19191631162510"></a>  
![](figures/配置自定义字段.png "配置自定义字段")

