# 转储至MRS<a name="dayu_01_0216"></a>

## 源数据类型JSON/BLOB/CSV==\>转储文件格式Text<a name="zh-cn_topic_0165739418_section5760185410392"></a>

**表 1**  转储Text格式文件的配置参数

<a name="zh-cn_topic_0165739418_table18468165816451"></a>
<table><thead align="left"><tr id="zh-cn_topic_0165739418_row15468165811456"><th class="cellrowborder" valign="top" width="21.08210821082108%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0165739418_p1746865813454"><a name="zh-cn_topic_0165739418_p1746865813454"></a><a name="zh-cn_topic_0165739418_p1746865813454"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="56.66566656665667%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0165739418_p1746811580453"><a name="zh-cn_topic_0165739418_p1746811580453"></a><a name="zh-cn_topic_0165739418_p1746811580453"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="22.252225222522252%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0165739418_p184682582458"><a name="zh-cn_topic_0165739418_p184682582458"></a><a name="zh-cn_topic_0165739418_p184682582458"></a>取值</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0165739418_row846805820453"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739418_p4468195810455"><a name="zh-cn_topic_0165739418_p4468195810455"></a><a name="zh-cn_topic_0165739418_p4468195810455"></a>任务名称</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p15371132211357"><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p15371132211357"></a><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p15371132211357"></a>用户创建转储任务时，需要指定转储任务名称，同一通道的转储任务名称不可重复。任务名称由<span id="zh-cn_topic_0165739418_zh-cn_topic_0120206045_text2371822163519"><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_text2371822163519"></a><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_text2371822163519"></a>英文字母、数字、中划线和下划线组成。</span>长度为1～64个字符。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p9371522113518"><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p9371522113518"></a><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p9371522113518"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739418_row346865813454"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739418_p061319534299"><a name="zh-cn_topic_0165739418_p061319534299"></a><a name="zh-cn_topic_0165739418_p061319534299"></a>MRS集群</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p1738710229352"><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p1738710229352"></a><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p1738710229352"></a>单击“选择”，在“选择集群”窗口选择一个MRS集群。仅支持转储至非Kerberos认证的MRS集群。</p>
<p id="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p1738722219356"><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p1738722219356"></a><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p1738722219356"></a>此配置项仅支持选择，不可手动输入。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p83870226357"><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p83870226357"></a><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p83870226357"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739418_row17888513010"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739418_p17886573017"><a name="zh-cn_topic_0165739418_p17886573017"></a><a name="zh-cn_topic_0165739418_p17886573017"></a>HDFS路径</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p18387622203515"><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p18387622203515"></a><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p18387622203515"></a>单击“选择”，在“选择HDFS文件路径”窗口按层级选择所需HDFS文件所在路径。</p>
<p id="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p53875225355"><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p53875225355"></a><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p53875225355"></a>此处路径仅支持选择，不可手动输入。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p538792220357"><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p538792220357"></a><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p538792220357"></a>配置此项必须已配置“MRS集群”。</p>
<p id="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p10387182219359"><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p10387182219359"></a><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p10387182219359"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739418_row174699584459"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739418_p1046914582454"><a name="zh-cn_topic_0165739418_p1046914582454"></a><a name="zh-cn_topic_0165739418_p1046914582454"></a>转储文件目录</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p73711822193518"><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p73711822193518"></a><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p73711822193518"></a>在MRS中存储通道文件的自定义目录，多级目录可用“/”进行分隔，不能以“/”开头。</p>
<p id="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p203713226352"><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p203713226352"></a><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p203713226352"></a>取值范围：0~50个字符。</p>
<p id="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p437115221351"><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p437115221351"></a><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p437115221351"></a>默认配置为空。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p183712022113519"><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p183712022113519"></a><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p183712022113519"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739418_row154692588456"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739418_p846916586453"><a name="zh-cn_topic_0165739418_p846916586453"></a><a name="zh-cn_topic_0165739418_p846916586453"></a>偏移量</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_ul19387202217353"></a><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_ul19387202217353"></a><ul id="zh-cn_topic_0165739418_zh-cn_topic_0120206045_ul19387202217353"><li>最新：最大偏移量，即获取最新的有效数据。</li><li>最早：最小偏移量，即读取最早的有效数据。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p1838772218354"><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p1838772218354"></a><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p1838772218354"></a>最新</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739418_row14351951154713"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739418_p535285110473"><a name="zh-cn_topic_0165739418_p535285110473"></a><a name="zh-cn_topic_0165739418_p535285110473"></a>数据转储周期</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p4387172214359"><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p4387172214359"></a><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p4387172214359"></a>根据用户配置的时间，周期性的将数据导入目的地（OBS，MRS，DLI，DWS，CloudTable），若某个时间段内无数据，则此时间段不会生成打包文件。</p>
<p id="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p1938732213352"><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p1938732213352"></a><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p1938732213352"></a>取值范围：30～900。</p>
<p id="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p173876227356"><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p173876227356"></a><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p173876227356"></a>单位：秒。</p>
<p id="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p138716221355"><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p138716221355"></a><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p138716221355"></a>默认配置为300秒。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p1338782293511"><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p1338782293511"></a><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p1338782293511"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739418_row7508810153116"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739418_p1508111043117"><a name="zh-cn_topic_0165739418_p1508111043117"></a><a name="zh-cn_topic_0165739418_p1508111043117"></a>数据临时桶</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p1238742213359"><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p1238742213359"></a><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p1238742213359"></a>用户数据先临时存储在OBS桶中，再转储到指定的转储服务，转储完成后临时桶中的数据会被清除。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p838762214358"><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p838762214358"></a><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p838762214358"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739418_row119451913118"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739418_p1895121953117"><a name="zh-cn_topic_0165739418_p1895121953117"></a><a name="zh-cn_topic_0165739418_p1895121953117"></a>数据临时目录</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p15387172211357"><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p15387172211357"></a><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p15387172211357"></a>需要转储的数据临时存储在OBS桶下此配置项配置的目录中，转储完成后临时目录中的数据会被清除。</p>
<p id="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p1838712222353"><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p1838712222353"></a><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p1838712222353"></a>配置为空时，数据直接存储在OBS桶内。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p3387142219355"><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p3387142219355"></a><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p3387142219355"></a>-</p>
</td>
</tr>
</tbody>
</table>

## 源数据类型JSON/CSV==\>转储文件格式Parquet<a name="zh-cn_topic_0165739418_section51282162613"></a>

>![](public_sys-resources/icon-note.gif) **说明：**   
>[表2](#zh-cn_topic_0165739418_table1068705245510)罗列了源数据类型为JSON，CSV，转储至MRS（对应转储文件格式Parquet）时需要配置的差异化参数，共性参数的配置请参见[表1](#zh-cn_topic_0165739418_table18468165816451)。  

**表 2**  转储Parquet格式文件的配置参数

<a name="zh-cn_topic_0165739418_table1068705245510"></a>
<table><thead align="left"><tr id="zh-cn_topic_0165739418_row1668710524553"><th class="cellrowborder" valign="top" width="23.262326232623263%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0165739418_p0305164555620"><a name="zh-cn_topic_0165739418_p0305164555620"></a><a name="zh-cn_topic_0165739418_p0305164555620"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="43.404340434043405%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0165739418_p13051045165612"><a name="zh-cn_topic_0165739418_p13051045165612"></a><a name="zh-cn_topic_0165739418_p13051045165612"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0165739418_p1230517459563"><a name="zh-cn_topic_0165739418_p1230517459563"></a><a name="zh-cn_topic_0165739418_p1230517459563"></a>取值</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0165739418_row2097131155910"><td class="cellrowborder" valign="top" width="23.262326232623263%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739418_p11971131155914"><a name="zh-cn_topic_0165739418_p11971131155914"></a><a name="zh-cn_topic_0165739418_p11971131155914"></a>源数据Schema</p>
</td>
<td class="cellrowborder" valign="top" width="43.404340434043405%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739418_p5969122711441"><a name="zh-cn_topic_0165739418_p5969122711441"></a><a name="zh-cn_topic_0165739418_p5969122711441"></a>用户的JSON或CSV数据样例，用于描述JSON或CSV数据格式。DIS可以根据此JSON或CSV数据样例生成Avro schema, 将通道内上传的JSON或CSV数据转换为Parquet格式。</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739418_p20976314593"><a name="zh-cn_topic_0165739418_p20976314593"></a><a name="zh-cn_topic_0165739418_p20976314593"></a>-</p>
</td>
</tr>
</tbody>
</table>

## 源数据类型JSON/CSV==\>转储文件格式CarbonData<a name="zh-cn_topic_0165739418_section167738422917"></a>

>![](public_sys-resources/icon-note.gif) **说明：**   
>[表3](#zh-cn_topic_0165739418_table1977324211913)罗列了源数据类型为JSON，CSV，转储至OBS（对应转储文件格式CarbonData）时需要配置的差异化参数，共性参数的配置请参见[表1](#zh-cn_topic_0165739418_table18468165816451)。  

**表 3**  转储CarbonData格式文件的配置参数

<a name="zh-cn_topic_0165739418_table1977324211913"></a>
<table><thead align="left"><tr id="zh-cn_topic_0165739418_row157732421993"><th class="cellrowborder" valign="top" width="23.262326232623263%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0165739418_p3773114212919"><a name="zh-cn_topic_0165739418_p3773114212919"></a><a name="zh-cn_topic_0165739418_p3773114212919"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="43.404340434043405%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0165739418_p10773164215912"><a name="zh-cn_topic_0165739418_p10773164215912"></a><a name="zh-cn_topic_0165739418_p10773164215912"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0165739418_p1577311424915"><a name="zh-cn_topic_0165739418_p1577311424915"></a><a name="zh-cn_topic_0165739418_p1577311424915"></a>取值</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0165739418_row17775184215917"><td class="cellrowborder" valign="top" width="23.262326232623263%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739418_p1277511423913"><a name="zh-cn_topic_0165739418_p1277511423913"></a><a name="zh-cn_topic_0165739418_p1277511423913"></a>源数据Schema</p>
</td>
<td class="cellrowborder" valign="top" width="43.404340434043405%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739418_p14317210417"><a name="zh-cn_topic_0165739418_p14317210417"></a><a name="zh-cn_topic_0165739418_p14317210417"></a>用户的JSON或CSV数据样例，用于描述JSON或CSV数据格式。DIS可以根据此JSON或CSV数据样例生成Avro schema, 将通道内上传的JSON或CSV数据转换为CarbonData格式。</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739418_p877511422092"><a name="zh-cn_topic_0165739418_p877511422092"></a><a name="zh-cn_topic_0165739418_p877511422092"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739418_row7775842990"><td class="cellrowborder" valign="top" width="23.262326232623263%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739418_p6159105319119"><a name="zh-cn_topic_0165739418_p6159105319119"></a><a name="zh-cn_topic_0165739418_p6159105319119"></a>CarbonData检索属性</p>
</td>
<td class="cellrowborder" valign="top" width="43.404340434043405%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p19391102713416"><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p19391102713416"></a><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p19391102713416"></a>carbon表属性，用于创建carbon writer。</p>
<p id="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p19478201112210"><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p19478201112210"></a><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p19478201112210"></a>支持的Key如下：</p>
<a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_ul126024616213"></a><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_ul126024616213"></a><ul id="zh-cn_topic_0165739418_zh-cn_topic_0120206045_ul126024616213"><li>table_blocksize：表的block大小，取值范围是1~2048MB，默认值是1024MB。</li><li>table_blocklet_size：文件内的Blocklet大小，默认值是64MB。</li><li>local_dictionary_threshold</li><li>local_dictionary_enable：配置为true或者false，默认值是false。</li><li>sort_columns：指定索引列，多级索引列用“，”分隔。</li><li>sort_scope：加载时，数据排序的范围。目前支持如下几种：<a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_ul19249218407"></a><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_ul19249218407"></a><ul id="zh-cn_topic_0165739418_zh-cn_topic_0120206045_ul19249218407"><li>local_sort：默认值，表示在一个node下做数据排序；</li><li>no_sort：即不排序，在需要快速入库时使用，可以在入库后系统闲时通过Compaction命令再建立索引；</li><li>batch_sort：表示在一个node下，内存排序后直接生成CarbonData文件，不再进行node下的全排序；使用该配置，可以提升加载速度，但查询性能不如LOCAL_SORT；</li></ul>
</li><li>long_string_columns</li></ul>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p42571613476"><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p42571613476"></a><a name="zh-cn_topic_0165739418_zh-cn_topic_0120206045_p42571613476"></a>-</p>
</td>
</tr>
</tbody>
</table>

