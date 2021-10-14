# 配置MongoDB/DDS源端参数<a name="dgc_01_0055"></a>

从MongoDB、DDS迁移到关系型数据库时，CDM会读取集合的首行数据作为字段列表样例，如果首行数据未包含该集合的所有字段，用户需要自己手工添加字段。

作业中源连接为[配置MongoDB连接](配置MongoDB连接.md#dgc_01_0030)，即从本地MongoDB或DDS导出数据时，源端作业参数如[表1](#zh-cn_topic_0108275308_table31823995163953)所示。

**表 1**  MongoDB/DDS作为源端时的作业参数

<a name="zh-cn_topic_0108275308_table31823995163953"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108275308_row18653487163953"><th class="cellrowborder" valign="top" width="15.61%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108275308_p15314298163953"><a name="zh-cn_topic_0108275308_p15314298163953"></a><a name="zh-cn_topic_0108275308_p15314298163953"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="64.88000000000001%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108275308_p32498630163953"><a name="zh-cn_topic_0108275308_p32498630163953"></a><a name="zh-cn_topic_0108275308_p32498630163953"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="19.509999999999998%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108275308_p15143370163953"><a name="zh-cn_topic_0108275308_p15143370163953"></a><a name="zh-cn_topic_0108275308_p15143370163953"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108275308_row2052684816261"><td class="cellrowborder" valign="top" width="15.61%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275308_p175265482261"><a name="zh-cn_topic_0108275308_p175265482261"></a><a name="zh-cn_topic_0108275308_p175265482261"></a>数据库名称</p>
</td>
<td class="cellrowborder" valign="top" width="64.88000000000001%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275308_p145261848192619"><a name="zh-cn_topic_0108275308_p145261848192619"></a><a name="zh-cn_topic_0108275308_p145261848192619"></a>选择待迁移的数据库。</p>
</td>
<td class="cellrowborder" valign="top" width="19.509999999999998%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275308_p452664812616"><a name="zh-cn_topic_0108275308_p452664812616"></a><a name="zh-cn_topic_0108275308_p452664812616"></a>mongodb</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275308_row34313000163953"><td class="cellrowborder" valign="top" width="15.61%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275308_p46804376161524"><a name="zh-cn_topic_0108275308_p46804376161524"></a><a name="zh-cn_topic_0108275308_p46804376161524"></a>集合名称</p>
</td>
<td class="cellrowborder" valign="top" width="64.88000000000001%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275308_p6187019816562"><a name="zh-cn_topic_0108275308_p6187019816562"></a><a name="zh-cn_topic_0108275308_p6187019816562"></a>相当于关系数据库的表名。单击输入框后面的按钮可进入选择集合名的界面，用户也可以直接输入集合名称。</p>
<p id="zh-cn_topic_0108275308_p49990086164128"><a name="zh-cn_topic_0108275308_p49990086164128"></a><a name="zh-cn_topic_0108275308_p49990086164128"></a>如果选择界面没有待选择的表，请确认表是否已经创建，或者对应连接里的帐号是否有元数据查询的权限。</p>
</td>
<td class="cellrowborder" valign="top" width="19.509999999999998%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275308_p41020337163953"><a name="zh-cn_topic_0108275308_p41020337163953"></a><a name="zh-cn_topic_0108275308_p41020337163953"></a>COLLECTION</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275308_row13417032753"><td class="cellrowborder" valign="top" width="15.61%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275308_p16417163215510"><a name="zh-cn_topic_0108275308_p16417163215510"></a><a name="zh-cn_topic_0108275308_p16417163215510"></a>查询筛选</p>
</td>
<td class="cellrowborder" valign="top" width="64.88000000000001%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108275308_p241710321259"><a name="zh-cn_topic_0108275308_p241710321259"></a><a name="zh-cn_topic_0108275308_p241710321259"></a>创建用于匹配文档的筛选条件，CDM只迁移符合条件的数据。例如：<a name="zh-cn_topic_0108275308_ol6793125415558"></a><a name="zh-cn_topic_0108275308_ol6793125415558"></a><ol id="zh-cn_topic_0108275308_ol6793125415558"><li>按表达式对象筛选：例如{'last_name': 'Smith'}，表示查找所有<span class="parmname" id="zh-cn_topic_0108275308_parmname0657201595916"><a name="zh-cn_topic_0108275308_parmname0657201595916"></a><a name="zh-cn_topic_0108275308_parmname0657201595916"></a>“last_name”</span>属性值为<span class="parmvalue" id="zh-cn_topic_0108275308_parmvalue21701627155916"><a name="zh-cn_topic_0108275308_parmvalue21701627155916"></a><a name="zh-cn_topic_0108275308_parmvalue21701627155916"></a>“Smith”</span>的文档。</li><li>按参数选项筛选：例如{ x : "john" }, { z : 1 }，表示查找x=john的所有z字段。</li><li>按条件筛选：例如{ "field" : { $gt: 5 } }，表示查找field字段中大于5的值。</li><li>按时间宏筛选：例如<p id="zh-cn_topic_0108275308_p1011414116580"><a name="zh-cn_topic_0108275308_p1011414116580"></a><a name="zh-cn_topic_0108275308_p1011414116580"></a>{"ts":{$gte:ISODate("${dateformat(yyyy-MM-dd'T'HH:mm:ss.SSS'Z',-1,HOUR)}")}}，表示查找ts字段中大于 时间宏转换后的值。</p>
</li></ol>
</div>
</td>
<td class="cellrowborder" valign="top" width="19.509999999999998%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275308_p18417203211519"><a name="zh-cn_topic_0108275308_p18417203211519"></a><a name="zh-cn_topic_0108275308_p18417203211519"></a>{'last_name': 'Smith'}</p>
</td>
</tr>
</tbody>
</table>

