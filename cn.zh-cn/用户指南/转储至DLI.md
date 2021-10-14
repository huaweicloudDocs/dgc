# 转储至DLI<a name="dgc_01_0214"></a>

## 源数据类型JSON/CSV<a name="zh-cn_topic_0165739419_section5760185410392"></a>

**表 1**  转储相关配置参数

<a name="zh-cn_topic_0165739419_table18468165816451"></a>
<table><thead align="left"><tr id="zh-cn_topic_0165739419_row15468165811456"><th class="cellrowborder" valign="top" width="21.08210821082108%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0165739419_p1746865813454"><a name="zh-cn_topic_0165739419_p1746865813454"></a><a name="zh-cn_topic_0165739419_p1746865813454"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="56.66566656665667%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0165739419_p1746811580453"><a name="zh-cn_topic_0165739419_p1746811580453"></a><a name="zh-cn_topic_0165739419_p1746811580453"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="22.252225222522252%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0165739419_p184682582458"><a name="zh-cn_topic_0165739419_p184682582458"></a><a name="zh-cn_topic_0165739419_p184682582458"></a>取值</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0165739419_row846805820453"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739419_p4468195810455"><a name="zh-cn_topic_0165739419_p4468195810455"></a><a name="zh-cn_topic_0165739419_p4468195810455"></a>任务名称</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p15371132211357"><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p15371132211357"></a><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p15371132211357"></a>用户创建转储任务时，需要指定转储任务名称，同一通道的转储任务名称不可重复。任务名称由<span id="zh-cn_topic_0165739419_zh-cn_topic_0120206045_text2371822163519"><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_text2371822163519"></a><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_text2371822163519"></a>英文字母、数字、中划线和下划线组成。</span>长度为1～64个字符。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p9371522113518"><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p9371522113518"></a><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p9371522113518"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739419_row346865813454"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739419_p061319534299"><a name="zh-cn_topic_0165739419_p061319534299"></a><a name="zh-cn_topic_0165739419_p061319534299"></a>DLI数据库</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p5387172223510"><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p5387172223510"></a><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p5387172223510"></a>单击“选择”，在“选择DLI数据库”窗口选择一个数据库。</p>
<p id="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p14387922203512"><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p14387922203512"></a><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p14387922203512"></a>此配置项仅支持选择，不可手动输入。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739419_p2156151334018"><a name="zh-cn_topic_0165739419_p2156151334018"></a><a name="zh-cn_topic_0165739419_p2156151334018"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739419_row17888513010"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739419_p17886573017"><a name="zh-cn_topic_0165739419_p17886573017"></a><a name="zh-cn_topic_0165739419_p17886573017"></a>DLI数据表</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p1438782219355"><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p1438782219355"></a><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p1438782219355"></a>单击“选择”，在“选择DLI数据表”窗口选择一个数据表。仅支持数据位置为DLI类型的数据表，且用户需具有该表的插入权限。</p>
<p id="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p738722223516"><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p738722223516"></a><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p738722223516"></a>此配置项仅支持选择，不可手动输入。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p18387522153511"><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p18387522153511"></a><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p18387522153511"></a>配置此项必须已配置“DLI 数据库”。</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739419_row154692588456"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739419_p846916586453"><a name="zh-cn_topic_0165739419_p846916586453"></a><a name="zh-cn_topic_0165739419_p846916586453"></a>偏移量</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_ul19387202217353"></a><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_ul19387202217353"></a><ul id="zh-cn_topic_0165739419_zh-cn_topic_0120206045_ul19387202217353"><li>最新：最大偏移量，即获取最新的有效数据。</li><li>最早：最小偏移量，即读取最早的有效数据。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p1838772218354"><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p1838772218354"></a><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p1838772218354"></a>最新</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739419_row14351951154713"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739419_p535285110473"><a name="zh-cn_topic_0165739419_p535285110473"></a><a name="zh-cn_topic_0165739419_p535285110473"></a>数据转储周期</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p4387172214359"><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p4387172214359"></a><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p4387172214359"></a>根据用户配置的时间，周期性的将数据导入目的地（OBS，MRS，DLI，DWS，CloudTable），若某个时间段内无数据，则此时间段不会生成打包文件。</p>
<p id="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p1938732213352"><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p1938732213352"></a><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p1938732213352"></a>取值范围：30～900。</p>
<p id="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p173876227356"><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p173876227356"></a><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p173876227356"></a>单位：秒。</p>
<p id="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p138716221355"><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p138716221355"></a><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p138716221355"></a>默认配置为300秒。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p1338782293511"><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p1338782293511"></a><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p1338782293511"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739419_row7508810153116"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739419_p1508111043117"><a name="zh-cn_topic_0165739419_p1508111043117"></a><a name="zh-cn_topic_0165739419_p1508111043117"></a>数据临时桶</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p1238742213359"><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p1238742213359"></a><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p1238742213359"></a>用户数据先临时存储在OBS桶中，再转储到指定的转储服务，转储完成后临时桶中的数据会被清除。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p838762214358"><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p838762214358"></a><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p838762214358"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739419_row119451913118"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739419_p1895121953117"><a name="zh-cn_topic_0165739419_p1895121953117"></a><a name="zh-cn_topic_0165739419_p1895121953117"></a>数据临时目录</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p15387172211357"><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p15387172211357"></a><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p15387172211357"></a>需要转储的数据临时存储在OBS桶下此配置项配置的目录中，转储完成后临时目录中的数据会被清除。</p>
<p id="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p1838712222353"><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p1838712222353"></a><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p1838712222353"></a>配置为空时，数据直接存储在OBS桶内。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p3387142219355"><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p3387142219355"></a><a name="zh-cn_topic_0165739419_zh-cn_topic_0120206045_p3387142219355"></a>-</p>
</td>
</tr>
</tbody>
</table>

