# 转储至OBS<a name="dayu_01_0213"></a>

## 源数据类型JSON/BLOB/CSV==\>转储文件格式Text<a name="zh-cn_topic_0165739417_section5760185410392"></a>

**表 1**  转储Text格式文件的配置参数

<a name="zh-cn_topic_0165739417_table18468165816451"></a>
<table><thead align="left"><tr id="zh-cn_topic_0165739417_row15468165811456"><th class="cellrowborder" valign="top" width="21.08210821082108%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0165739417_p1746865813454"><a name="zh-cn_topic_0165739417_p1746865813454"></a><a name="zh-cn_topic_0165739417_p1746865813454"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="56.66566656665667%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0165739417_p1746811580453"><a name="zh-cn_topic_0165739417_p1746811580453"></a><a name="zh-cn_topic_0165739417_p1746811580453"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="22.252225222522252%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0165739417_p184682582458"><a name="zh-cn_topic_0165739417_p184682582458"></a><a name="zh-cn_topic_0165739417_p184682582458"></a>取值</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0165739417_row846805820453"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739417_p4468195810455"><a name="zh-cn_topic_0165739417_p4468195810455"></a><a name="zh-cn_topic_0165739417_p4468195810455"></a>任务名称</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p15371132211357"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p15371132211357"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p15371132211357"></a>用户创建转储任务时，需要指定转储任务名称，同一通道的转储任务名称不可重复。任务名称由<span id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_text2371822163519"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_text2371822163519"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_text2371822163519"></a>英文字母、数字、中划线和下划线组成。</span>长度为1～64个字符。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p9371522113518"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p9371522113518"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p9371522113518"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739417_row346865813454"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739417_p114692058184513"><a name="zh-cn_topic_0165739417_p114692058184513"></a><a name="zh-cn_topic_0165739417_p114692058184513"></a>数据转储地址</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p737182214358"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p737182214358"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p737182214358"></a>存储该通道数据的OBS桶名称。桶名称在“对象存储服务”中“创建桶”时创建。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p93712225357"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p93712225357"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p93712225357"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739417_row174699584459"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739417_p1046914582454"><a name="zh-cn_topic_0165739417_p1046914582454"></a><a name="zh-cn_topic_0165739417_p1046914582454"></a>转储文件目录</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p73711822193518"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p73711822193518"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p73711822193518"></a>在OBS中存储通道文件的自定义目录，多级目录可用“/”进行分隔，不能以“/”开头。</p>
<p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p203713226352"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p203713226352"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p203713226352"></a>取值范围：0~50个字符。</p>
<p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p437115221351"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p437115221351"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p437115221351"></a>默认配置为空。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p183712022113519"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p183712022113519"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p183712022113519"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739417_row446965814453"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739417_p17469058144516"><a name="zh-cn_topic_0165739417_p17469058144516"></a><a name="zh-cn_topic_0165739417_p17469058144516"></a>时间目录格式</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p1643163722112"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p1643163722112"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p1643163722112"></a>数据将存储在OBS桶中转储文件目录下，按时间格式作为层级的目录中。</p>
<p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p11371122113511"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p11371122113511"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p11371122113511"></a>当选择的时间目录格式精确到日时，存储目录为“桶名称/转储文件目录/年/月/日”。</p>
<div class="p" id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p103711522163519"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p103711522163519"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p103711522163519"></a>取值范围：<a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_ul33711722133517"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_ul33711722133517"></a><ul id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_ul33711722133517"><li>N/A：置空，不使用日期时间目录。</li><li>yyyy：年</li><li>yyyy/MM：年/月</li><li>yyyy/MM/dd：年/月/日</li><li>yyyy/MM/dd/HH：年/月/日/时</li><li>yyyy/MM/dd/HH/mm：年/月/日/时/分</li></ul>
</div>
<p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p103719228358"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p103719228358"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p103719228358"></a>此配置项仅支持选择，不可手动输入。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p1371322123511"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p1371322123511"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p1371322123511"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739417_row246955812451"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739417_p646917583450"><a name="zh-cn_topic_0165739417_p646917583450"></a><a name="zh-cn_topic_0165739417_p646917583450"></a>记录分隔符</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p037115226353"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p037115226353"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p037115226353"></a>进行OBS转储时，分隔不同转储记录的分隔符。</p>
<div class="p" id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p538714226359"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p538714226359"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p538714226359"></a>取值范围：<a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_ul4387722103510"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_ul4387722103510"></a><ul id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_ul4387722103510"><li>逗号 ","</li><li>分号 ";"</li><li>竖线 "|"</li><li>换行符 "\n"</li><li>NULL</li></ul>
</div>
<p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p103874223358"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p103874223358"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p103874223358"></a>此配置项仅支持选择，不可手动输入。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p43872227359"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p43872227359"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p43872227359"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739417_row154692588456"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739417_p846916586453"><a name="zh-cn_topic_0165739417_p846916586453"></a><a name="zh-cn_topic_0165739417_p846916586453"></a>偏移量</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_ul19387202217353"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_ul19387202217353"></a><ul id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_ul19387202217353"><li>最新：最大偏移量，即获取最新的有效数据。</li><li>最早：最小偏移量，即读取最早的有效数据。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p1838772218354"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p1838772218354"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p1838772218354"></a>最新</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739417_row14351951154713"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739417_p535285110473"><a name="zh-cn_topic_0165739417_p535285110473"></a><a name="zh-cn_topic_0165739417_p535285110473"></a>数据转储周期</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p4387172214359"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p4387172214359"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p4387172214359"></a>根据用户配置的时间，周期性的将数据导入目的地（OBS，MRS，DLI，DWS，CloudTable），若某个时间段内无数据，则此时间段不会生成打包文件。</p>
<p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p1938732213352"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p1938732213352"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p1938732213352"></a>取值范围：30～900。</p>
<p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p173876227356"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p173876227356"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p173876227356"></a>单位：秒。</p>
<p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p138716221355"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p138716221355"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p138716221355"></a>默认配置为300秒。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p1338782293511"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p1338782293511"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p1338782293511"></a>-</p>
</td>
</tr>
</tbody>
</table>

## 源数据类型JSON==\>转储文件格式CSV<a name="section83387312148"></a>

**表 2**  转储csv格式文件的配置参数

<a name="table6338163110141"></a>
<table><thead align="left"><tr id="row633823191412"><th class="cellrowborder" valign="top" width="21.08210821082108%" id="mcps1.2.4.1.1"><p id="p15338631141413"><a name="p15338631141413"></a><a name="p15338631141413"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="56.66566656665667%" id="mcps1.2.4.1.2"><p id="p20338203117141"><a name="p20338203117141"></a><a name="p20338203117141"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="22.252225222522252%" id="mcps1.2.4.1.3"><p id="p18338183111414"><a name="p18338183111414"></a><a name="p18338183111414"></a>取值</p>
</th>
</tr>
</thead>
<tbody><tr id="row2033833110142"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="p6339123161417"><a name="p6339123161417"></a><a name="p6339123161417"></a>任务名称</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="p933910317145"><a name="p933910317145"></a><a name="p933910317145"></a>用户创建转储任务时，需要指定转储任务名称，同一通道的转储任务名称不可重复。任务名称由<span id="text15339123111416"><a name="text15339123111416"></a><a name="text15339123111416"></a>英文字母、数字、中划线和下划线组成。</span>长度为1～64个字符。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="p533953117146"><a name="p533953117146"></a><a name="p533953117146"></a>-</p>
</td>
</tr>
<tr id="row10339431111410"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="p12339431151416"><a name="p12339431151416"></a><a name="p12339431151416"></a>数据转储地址</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="p18339131201418"><a name="p18339131201418"></a><a name="p18339131201418"></a>存储该通道数据的OBS桶名称。桶名称在“对象存储服务”中“创建桶”时创建。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="p73391831191417"><a name="p73391831191417"></a><a name="p73391831191417"></a>-</p>
</td>
</tr>
<tr id="row12339193115148"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="p14339133161412"><a name="p14339133161412"></a><a name="p14339133161412"></a>转储文件目录</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="p19339173121416"><a name="p19339173121416"></a><a name="p19339173121416"></a>在OBS中存储通道文件的自定义目录，多级目录可用“/”进行分隔，不能以“/”开头。</p>
<p id="p1133943116141"><a name="p1133943116141"></a><a name="p1133943116141"></a>取值范围：0~50个字符。</p>
<p id="p13391311141"><a name="p13391311141"></a><a name="p13391311141"></a>默认配置为空。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="p633913114143"><a name="p633913114143"></a><a name="p633913114143"></a>-</p>
</td>
</tr>
<tr id="row1833918318144"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="p16339143191419"><a name="p16339143191419"></a><a name="p16339143191419"></a>时间目录格式</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="p6339931141412"><a name="p6339931141412"></a><a name="p6339931141412"></a>数据将存储在OBS桶中转储文件目录下，按时间格式作为层级的目录中。</p>
<p id="p1733913316143"><a name="p1733913316143"></a><a name="p1733913316143"></a>当选择的时间目录格式精确到日时，存储目录为“桶名称/转储文件目录/年/月/日”。</p>
<div class="p" id="p1033914319144"><a name="p1033914319144"></a><a name="p1033914319144"></a>取值范围：<a name="ul1433915315140"></a><a name="ul1433915315140"></a><ul id="ul1433915315140"><li>N/A：置空，不使用日期时间目录。</li><li>yyyy：年</li><li>yyyy/MM：年/月</li><li>yyyy/MM/dd：年/月/日</li><li>yyyy/MM/dd/HH：年/月/日/时</li><li>yyyy/MM/dd/HH/mm：年/月/日/时/分</li></ul>
</div>
<p id="p133392031161414"><a name="p133392031161414"></a><a name="p133392031161414"></a>此配置项仅支持选择，不可手动输入。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="p333915314145"><a name="p333915314145"></a><a name="p333915314145"></a>-</p>
</td>
</tr>
<tr id="row19340103116141"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="p33401131171419"><a name="p33401131171419"></a><a name="p33401131171419"></a>偏移量</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><a name="ul1634013121419"></a><a name="ul1634013121419"></a><ul id="ul1634013121419"><li>最新：最大偏移量，即获取最新的有效数据。</li><li>最早：最小偏移量，即读取最早的有效数据。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="p134018313147"><a name="p134018313147"></a><a name="p134018313147"></a>最新</p>
</td>
</tr>
<tr id="row434073181418"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="p14340123116146"><a name="p14340123116146"></a><a name="p14340123116146"></a>数据转储周期</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="p6340123111418"><a name="p6340123111418"></a><a name="p6340123111418"></a>根据用户配置的时间，周期性的将数据导入目的地，若某个时间段内无数据，则此时间段不会生成打包文件。</p>
<p id="p15340163115146"><a name="p15340163115146"></a><a name="p15340163115146"></a>取值范围：30～900。</p>
<p id="p03401631191415"><a name="p03401631191415"></a><a name="p03401631191415"></a>单位：秒。</p>
<p id="p1134023101415"><a name="p1134023101415"></a><a name="p1134023101415"></a>默认配置为300秒。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="p12340173181414"><a name="p12340173181414"></a><a name="p12340173181414"></a>-</p>
</td>
</tr>
</tbody>
</table>

## 源数据类型JSON/CSV==\>转储文件格式Parquet<a name="zh-cn_topic_0165739417_section51282162613"></a>

>![](public_sys-resources/icon-note.gif) **说明：**   
>[表3](#zh-cn_topic_0165739417_table1068705245510)罗列了源数据类型为JSON，CSV，转储至OBS（对应转储文件格式Parquet）时需要配置的差异化参数，共性参数的配置请参见[表1](#zh-cn_topic_0165739417_table18468165816451)。  

**表 3**  转储Parquet格式文件的配置参数

<a name="zh-cn_topic_0165739417_table1068705245510"></a>
<table><thead align="left"><tr id="zh-cn_topic_0165739417_row1668710524553"><th class="cellrowborder" valign="top" width="23.262326232623263%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0165739417_p0305164555620"><a name="zh-cn_topic_0165739417_p0305164555620"></a><a name="zh-cn_topic_0165739417_p0305164555620"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="43.28432843284328%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0165739417_p13051045165612"><a name="zh-cn_topic_0165739417_p13051045165612"></a><a name="zh-cn_topic_0165739417_p13051045165612"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="33.45334533453346%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0165739417_p1230517459563"><a name="zh-cn_topic_0165739417_p1230517459563"></a><a name="zh-cn_topic_0165739417_p1230517459563"></a>取值</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0165739417_row2097131155910"><td class="cellrowborder" valign="top" width="23.262326232623263%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739417_p11971131155914"><a name="zh-cn_topic_0165739417_p11971131155914"></a><a name="zh-cn_topic_0165739417_p11971131155914"></a>源数据Schema</p>
</td>
<td class="cellrowborder" valign="top" width="43.28432843284328%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739417_p5969122711441"><a name="zh-cn_topic_0165739417_p5969122711441"></a><a name="zh-cn_topic_0165739417_p5969122711441"></a>用户的JSON或CSV数据样例，用于描述JSON或CSV数据格式。DIS可以根据此JSON或CSV数据样例生成Avro schema, 将通道内上传的JSON或CSV数据转换为Parquet格式。</p>
</td>
<td class="cellrowborder" valign="top" width="33.45334533453346%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739417_p20976314593"><a name="zh-cn_topic_0165739417_p20976314593"></a><a name="zh-cn_topic_0165739417_p20976314593"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739417_row68418359262"><td class="cellrowborder" valign="top" width="23.262326232623263%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739417_p3882143762614"><a name="zh-cn_topic_0165739417_p3882143762614"></a><a name="zh-cn_topic_0165739417_p3882143762614"></a>转储文件目录</p>
</td>
<td class="cellrowborder" valign="top" width="43.28432843284328%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739417_p118822377268"><a name="zh-cn_topic_0165739417_p118822377268"></a><a name="zh-cn_topic_0165739417_p118822377268"></a>在OBS中存储通道文件的自定义目录，多级目录可用“/”进行分隔，不能以“/”开头。</p>
<p id="zh-cn_topic_0165739417_p6882837182610"><a name="zh-cn_topic_0165739417_p6882837182610"></a><a name="zh-cn_topic_0165739417_p6882837182610"></a>取值范围：0~100个字符。</p>
<p id="zh-cn_topic_0165739417_p6882037162617"><a name="zh-cn_topic_0165739417_p6882037162617"></a><a name="zh-cn_topic_0165739417_p6882037162617"></a>默认配置为空。</p>
<div class="note" id="zh-cn_topic_0165739417_note152371748185117"><a name="zh-cn_topic_0165739417_note152371748185117"></a><a name="zh-cn_topic_0165739417_note152371748185117"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0165739417_p18237184865114"><a name="zh-cn_topic_0165739417_p18237184865114"></a><a name="zh-cn_topic_0165739417_p18237184865114"></a>源数据类型为JSON时，支持EL表达式和内置函数。</p>
</div></div>
</td>
<td class="cellrowborder" valign="top" width="33.45334533453346%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0165739417_ul12405153214567"></a><a name="zh-cn_topic_0165739417_ul12405153214567"></a><ul id="zh-cn_topic_0165739417_ul12405153214567"><li><strong id="zh-cn_topic_0165739417_b1191055610118"><a name="zh-cn_topic_0165739417_b1191055610118"></a><a name="zh-cn_topic_0165739417_b1191055610118"></a>EL表达式示例：</strong></li></ul>
<p id="zh-cn_topic_0165739417_p1370156192917"><a name="zh-cn_topic_0165739417_p1370156192917"></a><a name="zh-cn_topic_0165739417_p1370156192917"></a>源数据：</p>
<p id="zh-cn_topic_0165739417_p14657946172115"><a name="zh-cn_topic_0165739417_p14657946172115"></a><a name="zh-cn_topic_0165739417_p14657946172115"></a>{"name":"Andy","city":"","time":1556323141582}</p>
<p id="zh-cn_topic_0165739417_p184065431802"><a name="zh-cn_topic_0165739417_p184065431802"></a><a name="zh-cn_topic_0165739417_p184065431802"></a>转储文件目录配置如下：</p>
<p id="zh-cn_topic_0165739417_p18736108614"><a name="zh-cn_topic_0165739417_p18736108614"></a><a name="zh-cn_topic_0165739417_p18736108614"></a>dis/basePath/app_key_p=${name}</p>
<p id="zh-cn_topic_0165739417_p5821132410113"><a name="zh-cn_topic_0165739417_p5821132410113"></a><a name="zh-cn_topic_0165739417_p5821132410113"></a>则数据的最终存储目录结构为：</p>
<p id="zh-cn_topic_0165739417_p1545320591712"><a name="zh-cn_topic_0165739417_p1545320591712"></a><a name="zh-cn_topic_0165739417_p1545320591712"></a>{$桶名称}/dis/basePath/app_key_p=Andy</p>
<a name="zh-cn_topic_0165739417_ul37751538165612"></a><a name="zh-cn_topic_0165739417_ul37751538165612"></a><ul id="zh-cn_topic_0165739417_ul37751538165612"><li><strong id="zh-cn_topic_0165739417_b77011016215"><a name="zh-cn_topic_0165739417_b77011016215"></a><a name="zh-cn_topic_0165739417_b77011016215"></a>内置函数示例：</strong></li></ul>
<p id="zh-cn_topic_0165739417_p152893720316"><a name="zh-cn_topic_0165739417_p152893720316"></a><a name="zh-cn_topic_0165739417_p152893720316"></a>源数据：</p>
<p id="zh-cn_topic_0165739417_p195281837834"><a name="zh-cn_topic_0165739417_p195281837834"></a><a name="zh-cn_topic_0165739417_p195281837834"></a>{"name":"Andy","city":"","time":1556323141582}</p>
<p id="zh-cn_topic_0165739417_p152817379319"><a name="zh-cn_topic_0165739417_p152817379319"></a><a name="zh-cn_topic_0165739417_p152817379319"></a>转储文件目录配置如下：</p>
<p id="zh-cn_topic_0165739417_p9219193515719"><a name="zh-cn_topic_0165739417_p9219193515719"></a><a name="zh-cn_topic_0165739417_p9219193515719"></a>dis/basePath/date_p=toDate(${time}, "yyMMdd")</p>
<p id="zh-cn_topic_0165739417_p19528193717319"><a name="zh-cn_topic_0165739417_p19528193717319"></a><a name="zh-cn_topic_0165739417_p19528193717319"></a>则数据的最终存储目录结构为：</p>
<p id="zh-cn_topic_0165739417_p552815372320"><a name="zh-cn_topic_0165739417_p552815372320"></a><a name="zh-cn_topic_0165739417_p552815372320"></a>{$桶名称}/dis-basePath/date_p=20190427</p>
<p id="zh-cn_topic_0165739417_p14891125510526"><a name="zh-cn_topic_0165739417_p14891125510526"></a><a name="zh-cn_topic_0165739417_p14891125510526"></a><strong id="zh-cn_topic_0165739417_b7855251736"><a name="zh-cn_topic_0165739417_b7855251736"></a><a name="zh-cn_topic_0165739417_b7855251736"></a>支持的内置函数列表：</strong></p>
<p id="zh-cn_topic_0165739417_p15567115295612"><a name="zh-cn_topic_0165739417_p15567115295612"></a><a name="zh-cn_topic_0165739417_p15567115295612"></a>toDate(timestamp,format)：将时间戳转化为指定的时间格式，例如：toDate(1556323141582,'yymmdd')</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739417_row201713565599"><td class="cellrowborder" valign="top" width="23.262326232623263%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739417_p8171135618592"><a name="zh-cn_topic_0165739417_p8171135618592"></a><a name="zh-cn_topic_0165739417_p8171135618592"></a>自定义时间目录</p>
</td>
<td class="cellrowborder" valign="top" width="43.28432843284328%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p109384485447"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p109384485447"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p109384485447"></a>通过单击<a name="image937611339519"></a><a name="image937611339519"></a><span><img id="image937611339519" src="figures/icon-dayu-enable-HEC.png"></span>或<a name="image1962172914531"></a><a name="image1962172914531"></a><span><img id="image1962172914531" src="figures/icon-dayu-disable-HEC.png"></span>来关闭或开启自定义时间戳开关。</p>
<a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_ul758115401126"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_ul758115401126"></a><ul id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_ul758115401126"><li>关闭自定义时间戳开关，则写到OBS的Object文件所在的目录层次结构，将使用转储文件的生成时间。<p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p183381534162120"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p183381534162120"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p183381534162120"></a>例如系统在2018年10月16日生成转储文件，选择<span class="parmname" id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmname984917893018"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmname984917893018"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmname984917893018"></a>“时间目录格式”</span>精确到日，则数据转储成功后，在OBS的存储目录为“桶名称/转储文件目录/2018/10/16”。</p>
</li><li>开启自定义时间戳开关，则写到OBS的Object文件所在的目录层次结构，将使用源数据中定义的时间。<p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p1181145635618"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p1181145635618"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p1181145635618"></a>例如您在2018年10月16日创建某转储任务，选择<span class="parmname" id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmname16606426911"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmname16606426911"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmname16606426911"></a>“时间目录格式”</span>精确到日，待上传的源数据中已定义时间字段"2017/09/08 11:01:01"，则数据转储成功后，在OBS的存储目录为“桶名称/转储文件目录/2017/09/08”。存储目录按照源数据中定义的时间字段进行定义，而不是转储文件的生成时间。</p>
</li></ul>
</td>
<td class="cellrowborder" rowspan="2" valign="top" width="33.45334533453346%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_ul242514794915"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_ul242514794915"></a><ul id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_ul242514794915"><li>示例1：转储简单的Json数据。</li></ul>
<p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p13799581689"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p13799581689"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p13799581689"></a>源数据：</p>
<p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p246581516453"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p246581516453"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p246581516453"></a>{    "id":"1",    "date":"2018/10/16 11:00:05"}</p>
<p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p1697333419410"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p1697333419410"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p1697333419410"></a>配置如下：</p>
<p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p8515191715313"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p8515191715313"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p8515191715313"></a>根据待转储的源数据类型，分别设置<span class="parmname" id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmname15738130195615"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmname15738130195615"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmname15738130195615"></a>“时间戳属性名”</span>为<span class="parmvalue" id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmvalue3567143616569"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmvalue3567143616569"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmvalue3567143616569"></a>“date”</span>，数据类型为<span class="parmvalue" id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmvalue151311555155611"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmvalue151311555155611"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmvalue151311555155611"></a>“String”</span>，时间戳格式为<span class="parmvalue" id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmvalue0100137105712"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmvalue0100137105712"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmvalue0100137105712"></a>“yyyy/MM/dd HH:mm:ss”</span>。</p>
<p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p185217221581"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p185217221581"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p185217221581"></a>因数据转储成功后，存储的目录结构取决于源数据的时间戳和时间目录格式定义的年月日层级。本示例中，时间目录格式精确到日，所以数据最终存储目录结构为“桶名称/转储文件目录/2018/10/16”。</p>
<a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_ul8297195613349"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_ul8297195613349"></a><ul id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_ul8297195613349"><li>示例2：转储多层嵌套的Json数据。<p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p49712221082"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p49712221082"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p49712221082"></a>源数据：</p>
<p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p1047182223517"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p1047182223517"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p1047182223517"></a>{    "id":"1",    "detail":{        "detID":"05790110000000000103#567fd3cb13a4493eaa43076953253eed",        "endTime":"2018/10/07 13:26:35"    }}</p>
</li></ul>
<p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p23133562349"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p23133562349"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p23133562349"></a>配置如下：</p>
<p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p14329756133413"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p14329756133413"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p14329756133413"></a>根据待转储的源数据类型，分别设置<span class="parmname" id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmname63291756203412"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmname63291756203412"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmname63291756203412"></a>“时间戳属性名”</span>为<span class="parmvalue" id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmvalue123291567342"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmvalue123291567342"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmvalue123291567342"></a>“detail.endTime”</span>，数据类型为<span class="parmvalue" id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmvalue8343256153412"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmvalue8343256153412"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmvalue8343256153412"></a>“String”</span>，时间戳格式为<span class="parmvalue" id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmvalue4343125633414"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmvalue4343125633414"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmvalue4343125633414"></a>“yyyy/MM/dd HH:mm:ss”</span>。</p>
<p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p163435562349"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p163435562349"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p163435562349"></a>因数据转储成功后，存储的目录结构取决于源数据的时间戳和时间目录格式定义的年月日层级。本示例中，时间目录格式精确到日，所以数据最终存储目录结构为“桶名称/转储文件目录/2018/10/07”。</p>
<a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_ul9507111915371"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_ul9507111915371"></a><ul id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_ul9507111915371"><li>示例3：转储CSV格式的数据。</li></ul>
<p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p1744223114816"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p1744223114816"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p1744223114816"></a>源数据：</p>
<p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p18531396133"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p18531396133"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p18531396133"></a>a,2010-10-12 11:00:00,b,2011-10-12 11:00:10</p>
<p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p5441125010817"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p5441125010817"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p5441125010817"></a>配置如下：</p>
<p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p144412050281"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p144412050281"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p144412050281"></a>根据待转储的源数据，选定时间戳“2010-10-12 11:00:00”，经DIS转换为Parquet格式后，对应的属性字段名称为field_1。则创建转储任务时分别设置<span class="parmname" id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmname1644110501085"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmname1644110501085"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmname1644110501085"></a>“时间戳属性名”</span>为<span class="parmvalue" id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmvalue11457195016819"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmvalue11457195016819"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmvalue11457195016819"></a>“field_1”</span>，数据类型为<span class="parmvalue" id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmvalue2457250584"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmvalue2457250584"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmvalue2457250584"></a>“String”</span>，时间戳格式为<span class="parmvalue" id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmvalue94574501286"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmvalue94574501286"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_parmvalue94574501286"></a>“yyyy/MM/dd HH:mm:ss”</span>。</p>
<p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p1045714501089"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p1045714501089"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p1045714501089"></a>因数据转储成功后，存储的目录结构取决于源数据的时间戳和时间目录格式定义的年月日层级。本示例中，时间目录格式精确到日，所以数据最终存储目录结构为“桶名称/转储文件目录/2010/10/12”。</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739417_row1390112278010"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739417_p69021327305"><a name="zh-cn_topic_0165739417_p69021327305"></a><a name="zh-cn_topic_0165739417_p69021327305"></a>源数据时间戳</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_ul2686128153"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_ul2686128153"></a><ul id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_ul2686128153"><li>时间戳的属性名。<div class="note" id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_note847092512169"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_note847092512169"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_note847092512169"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p747012513166"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p747012513166"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p747012513166"></a>请输入您待上传的源数据中定义的时间戳对应的字段名称。</p>
</div></div>
</li><li>时间戳的格式，从下拉框中选择。<p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p770215219156"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p770215219156"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p770215219156"></a>yyyy/MM/dd HH:mm:ss</p>
<p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p07177218156"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p07177218156"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p07177218156"></a>MM/dd/yyyy HH:mm:ss</p>
<p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p171718291517"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p171718291517"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p171718291517"></a>dd/MM/yyyy HH:mm:ss</p>
<p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p9717625156"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p9717625156"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p9717625156"></a>yyyy-MM-dd HH:mm:ss</p>
<p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p147171261517"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p147171261517"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p147171261517"></a>MM-dd-yyyy HH:mm:ss</p>
<p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p5733529159"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p5733529159"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p5733529159"></a>dd-MM-yyyy HH:mm:ss</p>
</li><li>数据类型，从下拉框中选择。<a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_ul274962171520"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_ul274962171520"></a><ul id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_ul274962171520"><li>String</li><li>Timestamp<div class="note" id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_note1624112537265"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_note1624112537265"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_note1624112537265"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p18241185310265"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p18241185310265"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p18241185310265"></a>当您待上传的源数据类型为Timestamp，请精确到毫秒级。</p>
</div></div>
</li></ul>
</li></ul>
</td>
</tr>
</tbody>
</table>

## 源数据类型JSON/CSV==\>转储文件格式CarbonData<a name="zh-cn_topic_0165739417_section167738422917"></a>

>![](public_sys-resources/icon-note.gif) **说明：**   
>[表4](#zh-cn_topic_0165739417_table1977324211913)罗列了源数据类型为JSON，CSV，转储至OBS（对应转储文件格式CarbonData）时需要配置的差异化参数，共性参数的配置请参见[表1](#zh-cn_topic_0165739417_table18468165816451)。  

**表 4**  转储CarbonData格式文件的配置参数

<a name="zh-cn_topic_0165739417_table1977324211913"></a>
<table><thead align="left"><tr id="zh-cn_topic_0165739417_row157732421993"><th class="cellrowborder" valign="top" width="23.262326232623263%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0165739417_p3773114212919"><a name="zh-cn_topic_0165739417_p3773114212919"></a><a name="zh-cn_topic_0165739417_p3773114212919"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="43.404340434043405%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0165739417_p10773164215912"><a name="zh-cn_topic_0165739417_p10773164215912"></a><a name="zh-cn_topic_0165739417_p10773164215912"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0165739417_p1577311424915"><a name="zh-cn_topic_0165739417_p1577311424915"></a><a name="zh-cn_topic_0165739417_p1577311424915"></a>取值</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0165739417_row17775184215917"><td class="cellrowborder" valign="top" width="23.262326232623263%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739417_p1277511423913"><a name="zh-cn_topic_0165739417_p1277511423913"></a><a name="zh-cn_topic_0165739417_p1277511423913"></a>源数据Schema</p>
</td>
<td class="cellrowborder" valign="top" width="43.404340434043405%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739417_p14317210417"><a name="zh-cn_topic_0165739417_p14317210417"></a><a name="zh-cn_topic_0165739417_p14317210417"></a>用户的JSON或CSV数据样例，用于描述JSON或CSV数据格式。DIS可以根据此JSON或CSV数据样例生成Avro schema, 将通道内上传的JSON或CSV数据转换为CarbonData格式。</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739417_p877511422092"><a name="zh-cn_topic_0165739417_p877511422092"></a><a name="zh-cn_topic_0165739417_p877511422092"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739417_row7775842990"><td class="cellrowborder" valign="top" width="23.262326232623263%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739417_p6159105319119"><a name="zh-cn_topic_0165739417_p6159105319119"></a><a name="zh-cn_topic_0165739417_p6159105319119"></a>CarbonData检索属性</p>
</td>
<td class="cellrowborder" valign="top" width="43.404340434043405%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p19391102713416"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p19391102713416"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p19391102713416"></a>carbon表属性，用于创建carbon writer。</p>
<p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p19478201112210"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p19478201112210"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p19478201112210"></a>支持的Key如下：</p>
<a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_ul126024616213"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_ul126024616213"></a><ul id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_ul126024616213"><li>table_blocksize：表的block大小，取值范围是1~2048MB，默认值是1024MB。</li><li>table_blocklet_size：文件内的Blocklet大小，默认值是64MB。</li><li>local_dictionary_threshold</li><li>local_dictionary_enable：配置为true或者false，默认值是false。</li><li>sort_columns：指定索引列，多级索引列用“，”分隔。</li><li>sort_scope：加载时，数据排序的范围。目前支持如下几种：<a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_ul19249218407"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_ul19249218407"></a><ul id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_ul19249218407"><li>local_sort：默认值，表示在一个node下做数据排序；</li><li>no_sort：即不排序，在需要快速入库时使用，可以在入库后系统闲时通过Compaction命令再建立索引；</li><li>batch_sort：表示在一个node下，内存排序后直接生成CarbonData文件，不再进行node下的全排序；使用该配置，可以提升加载速度，但查询性能不如LOCAL_SORT；</li></ul>
</li><li>long_string_columns</li></ul>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p42571613476"><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p42571613476"></a><a name="zh-cn_topic_0165739417_zh-cn_topic_0120206045_p42571613476"></a>-</p>
</td>
</tr>
</tbody>
</table>

