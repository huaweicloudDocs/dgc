# 配置七牛云KODO/腾讯云COS连接<a name="dgc_01_0042"></a>

连接七牛云对象存储（KODO）或者腾讯云对象存储（COS）时，相关连接参数如[表1](#zh-cn_topic_0118889582_table56513226152843)所示。

-   对象存储服务之间的迁移，推荐使用对象存储迁移服务OMS。
-   使用CDM迁移其他对象存储数据时，仅支持迁移数据到OBS。

**表 1**  KODO/COS连接的参数

<a name="zh-cn_topic_0118889582_table56513226152843"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118889582_row51765490152843"><th class="cellrowborder" valign="top" width="24.04%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118889582_p25915791152843"><a name="zh-cn_topic_0118889582_p25915791152843"></a><a name="zh-cn_topic_0118889582_p25915791152843"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="47.599999999999994%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118889582_p38360350165510"><a name="zh-cn_topic_0118889582_p38360350165510"></a><a name="zh-cn_topic_0118889582_p38360350165510"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="28.360000000000003%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118889582_p64999942163911"><a name="zh-cn_topic_0118889582_p64999942163911"></a><a name="zh-cn_topic_0118889582_p64999942163911"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118889582_row172676953014"><td class="cellrowborder" valign="top" width="24.04%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118889582_p426714916301"><a name="zh-cn_topic_0118889582_p426714916301"></a><a name="zh-cn_topic_0118889582_p426714916301"></a>名称</p>
</td>
<td class="cellrowborder" valign="top" width="47.599999999999994%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118889582_p6573133312010"><a name="zh-cn_topic_0118889582_p6573133312010"></a><a name="zh-cn_topic_0118889582_p6573133312010"></a>连接的名称，根据连接的数据源类型，用户可自定义便于记忆、区分的连接名。</p>
</td>
<td class="cellrowborder" valign="top" width="28.360000000000003%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118889582_p1826719919305"><a name="zh-cn_topic_0118889582_p1826719919305"></a><a name="zh-cn_topic_0118889582_p1826719919305"></a>linkname</p>
</td>
</tr>
<tr id="zh-cn_topic_0118889582_row58346992152843"><td class="cellrowborder" valign="top" width="24.04%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118889582_p25657651152843"><a name="zh-cn_topic_0118889582_p25657651152843"></a><a name="zh-cn_topic_0118889582_p25657651152843"></a>存储区域</p>
</td>
<td class="cellrowborder" valign="top" width="47.599999999999994%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118889582_p66961515161910"><a name="zh-cn_topic_0118889582_p66961515161910"></a><a name="zh-cn_topic_0118889582_p66961515161910"></a>KODO/COS所属的区域。</p>
</td>
<td class="cellrowborder" valign="top" width="28.360000000000003%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118889582_p75588220114"><a name="zh-cn_topic_0118889582_p75588220114"></a><a name="zh-cn_topic_0118889582_p75588220114"></a>华东</p>
</td>
</tr>
<tr id="zh-cn_topic_0118889582_row55275051152843"><td class="cellrowborder" valign="top" width="24.04%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118889582_p3311745152843"><a name="zh-cn_topic_0118889582_p3311745152843"></a><a name="zh-cn_topic_0118889582_p3311745152843"></a>访问标识(Secretld)</p>
</td>
<td class="cellrowborder" valign="top" width="47.599999999999994%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118889582_p41664200165510"><a name="zh-cn_topic_0118889582_p41664200165510"></a><a name="zh-cn_topic_0118889582_p41664200165510"></a>KODO/COS的访问标识。</p>
</td>
<td class="cellrowborder" valign="top" width="28.360000000000003%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118889582_p28831327163911"><a name="zh-cn_topic_0118889582_p28831327163911"></a><a name="zh-cn_topic_0118889582_p28831327163911"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118889582_row3886299152843"><td class="cellrowborder" valign="top" width="24.04%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118889582_p63749320152843"><a name="zh-cn_topic_0118889582_p63749320152843"></a><a name="zh-cn_topic_0118889582_p63749320152843"></a>密钥(SK)</p>
</td>
<td class="cellrowborder" valign="top" width="47.599999999999994%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118889582_p39995786165510"><a name="zh-cn_topic_0118889582_p39995786165510"></a><a name="zh-cn_topic_0118889582_p39995786165510"></a>KODO/COS的访问密钥。</p>
</td>
<td class="cellrowborder" valign="top" width="28.360000000000003%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118889582_p12963499163911"><a name="zh-cn_topic_0118889582_p12963499163911"></a><a name="zh-cn_topic_0118889582_p12963499163911"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118889582_row1838723418115"><td class="cellrowborder" valign="top" width="24.04%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118889582_p4387143491118"><a name="zh-cn_topic_0118889582_p4387143491118"></a><a name="zh-cn_topic_0118889582_p4387143491118"></a>优先使用自定义域名下载对象</p>
</td>
<td class="cellrowborder" valign="top" width="47.599999999999994%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118889582_p886019518016"><a name="zh-cn_topic_0118889582_p886019518016"></a><a name="zh-cn_topic_0118889582_p886019518016"></a>高级属性参数，KODO连接才有该参数。</p>
<p id="zh-cn_topic_0118889582_p1538717341111"><a name="zh-cn_topic_0118889582_p1538717341111"></a><a name="zh-cn_topic_0118889582_p1538717341111"></a>如果对象存储的桶有CDN或者其它自定义域名，选择是否优先使用该自定义域名从桶中下载对象。</p>
</td>
<td class="cellrowborder" valign="top" width="28.360000000000003%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118889582_p1538717346117"><a name="zh-cn_topic_0118889582_p1538717346117"></a><a name="zh-cn_topic_0118889582_p1538717346117"></a>是</p>
</td>
</tr>
</tbody>
</table>

单击“显示高级属性“，您可以配置是否“优先使用自定义域名下载对象”。开启后，如果对象存储的桶有CDN或者其它自定义域名，优先使用该自定义域名从桶中下载对象。

