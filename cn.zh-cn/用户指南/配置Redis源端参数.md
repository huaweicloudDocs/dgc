# 配置Redis源端参数<a name="dgc_01_0056"></a>

由于分布式缓存服务（DCS）限制了获取所有Key的命令，CDM无法支持DCS作为源端，但可以作为迁移目的端，第三方云的Redis服务也无法支持作为源端。如果是用户在本地数据中心或ECS上自行搭建的Redis支持作为源端或目的端。

从本地Redis导出数据时，源端作业参数如[表1](#zh-cn_topic_0108275313_table31823995163953)所示。

**表 1**  Redis作为源端时的作业参数

<a name="zh-cn_topic_0108275313_table31823995163953"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108275313_row18653487163953"><th class="cellrowborder" valign="top" width="15.379999999999999%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108275313_p15314298163953"><a name="zh-cn_topic_0108275313_p15314298163953"></a><a name="zh-cn_topic_0108275313_p15314298163953"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="65.44%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108275313_p32498630163953"><a name="zh-cn_topic_0108275313_p32498630163953"></a><a name="zh-cn_topic_0108275313_p32498630163953"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="19.18%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108275313_p15143370163953"><a name="zh-cn_topic_0108275313_p15143370163953"></a><a name="zh-cn_topic_0108275313_p15143370163953"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108275313_row34313000163953"><td class="cellrowborder" valign="top" width="15.379999999999999%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275313_p17037287203413"><a name="zh-cn_topic_0108275313_p17037287203413"></a><a name="zh-cn_topic_0108275313_p17037287203413"></a>Redis键前缀</p>
</td>
<td class="cellrowborder" valign="top" width="65.44%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275313_p46074171163953"><a name="zh-cn_topic_0108275313_p46074171163953"></a><a name="zh-cn_topic_0108275313_p46074171163953"></a>键的前缀，类似关系型数据库的表名。</p>
</td>
<td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275313_p41020337163953"><a name="zh-cn_topic_0108275313_p41020337163953"></a><a name="zh-cn_topic_0108275313_p41020337163953"></a>TABLE</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275313_row1928353163953"><td class="cellrowborder" valign="top" width="15.379999999999999%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275313_p5690285203418"><a name="zh-cn_topic_0108275313_p5690285203418"></a><a name="zh-cn_topic_0108275313_p5690285203418"></a>值存储类型</p>
</td>
<td class="cellrowborder" valign="top" width="65.44%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108275313_p152812281737"><a name="zh-cn_topic_0108275313_p152812281737"></a><a name="zh-cn_topic_0108275313_p152812281737"></a>仅支持以下数据格式：<a name="zh-cn_topic_0108275313_ul2053492417310"></a><a name="zh-cn_topic_0108275313_ul2053492417310"></a><ul id="zh-cn_topic_0108275313_ul2053492417310"><li>STRING：不带列名，如<span class="uicontrol" id="zh-cn_topic_0108275313_uicontrol2441804217642"><a name="zh-cn_topic_0108275313_uicontrol2441804217642"></a><a name="zh-cn_topic_0108275313_uicontrol2441804217642"></a>“值1，值2”</span>形式。</li><li>HASH：带列名，如<span class="uicontrol" id="zh-cn_topic_0108275313_uicontrol1152225917626"><a name="zh-cn_topic_0108275313_uicontrol1152225917626"></a><a name="zh-cn_topic_0108275313_uicontrol1152225917626"></a>“列名1=值1，列名2=值2”</span>的形式。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275313_p64647157163953"><a name="zh-cn_topic_0108275313_p64647157163953"></a><a name="zh-cn_topic_0108275313_p64647157163953"></a>STRING</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275313_row11687830163953"><td class="cellrowborder" valign="top" width="15.379999999999999%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275313_p63014384203424"><a name="zh-cn_topic_0108275313_p63014384203424"></a><a name="zh-cn_topic_0108275313_p63014384203424"></a>键分隔符</p>
</td>
<td class="cellrowborder" valign="top" width="65.44%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275313_p63592058163953"><a name="zh-cn_topic_0108275313_p63592058163953"></a><a name="zh-cn_topic_0108275313_p63592058163953"></a>用来分隔关系型数据库的表和列名。</p>
</td>
<td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275313_p50683068163953"><a name="zh-cn_topic_0108275313_p50683068163953"></a><a name="zh-cn_topic_0108275313_p50683068163953"></a>_</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275313_row43070736163953"><td class="cellrowborder" valign="top" width="15.379999999999999%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275313_p31419000203428"><a name="zh-cn_topic_0108275313_p31419000203428"></a><a name="zh-cn_topic_0108275313_p31419000203428"></a>值分隔符</p>
</td>
<td class="cellrowborder" valign="top" width="65.44%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275313_p64711742163953"><a name="zh-cn_topic_0108275313_p64711742163953"></a><a name="zh-cn_topic_0108275313_p64711742163953"></a>以STRING方式存储时，列之间的分隔符。</p>
</td>
<td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275313_p7159773163953"><a name="zh-cn_topic_0108275313_p7159773163953"></a><a name="zh-cn_topic_0108275313_p7159773163953"></a>;</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275313_row1730917444432"><td class="cellrowborder" valign="top" width="15.379999999999999%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275313_p37989497431"><a name="zh-cn_topic_0108275313_p37989497431"></a><a name="zh-cn_topic_0108275313_p37989497431"></a>字段相同</p>
</td>
<td class="cellrowborder" valign="top" width="65.44%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275313_p20577941164418"><a name="zh-cn_topic_0108275313_p20577941164418"></a><a name="zh-cn_topic_0108275313_p20577941164418"></a><span class="parmname" id="zh-cn_topic_0108275313_parmname227751014458"><a name="zh-cn_topic_0108275313_parmname227751014458"></a><a name="zh-cn_topic_0108275313_parmname227751014458"></a>“值存储类型”</span>参数值为<span class="parmvalue" id="zh-cn_topic_0108275313_parmvalue568531310451"><a name="zh-cn_topic_0108275313_parmvalue568531310451"></a><a name="zh-cn_topic_0108275313_parmvalue568531310451"></a>“HASH”</span>显示该参数。</p>
<p id="zh-cn_topic_0108275313_p1075812614441"><a name="zh-cn_topic_0108275313_p1075812614441"></a><a name="zh-cn_topic_0108275313_p1075812614441"></a>哈希键内有相同的字段。</p>
</td>
<td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275313_p1231024444316"><a name="zh-cn_topic_0108275313_p1231024444316"></a><a name="zh-cn_topic_0108275313_p1231024444316"></a>是</p>
</td>
</tr>
</tbody>
</table>

