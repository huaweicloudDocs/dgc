# 转储至DWS<a name="dayu_01_0215"></a>

## 源数据类型JSON/CSV<a name="zh-cn_topic_0165739420_section5760185410392"></a>

**表 1**  转储相关配置参数

<a name="zh-cn_topic_0165739420_table18468165816451"></a>
<table><thead align="left"><tr id="zh-cn_topic_0165739420_row15468165811456"><th class="cellrowborder" valign="top" width="21.08210821082108%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0165739420_p1746865813454"><a name="zh-cn_topic_0165739420_p1746865813454"></a><a name="zh-cn_topic_0165739420_p1746865813454"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="56.66566656665667%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0165739420_p1746811580453"><a name="zh-cn_topic_0165739420_p1746811580453"></a><a name="zh-cn_topic_0165739420_p1746811580453"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="22.252225222522252%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0165739420_p184682582458"><a name="zh-cn_topic_0165739420_p184682582458"></a><a name="zh-cn_topic_0165739420_p184682582458"></a>取值</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0165739420_row846805820453"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739420_p4468195810455"><a name="zh-cn_topic_0165739420_p4468195810455"></a><a name="zh-cn_topic_0165739420_p4468195810455"></a>任务名称</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p15371132211357"><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p15371132211357"></a><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p15371132211357"></a>用户创建转储任务时，需要指定转储任务名称，同一通道的转储任务名称不可重复。任务名称由<span id="zh-cn_topic_0165739420_zh-cn_topic_0120206045_text2371822163519"><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_text2371822163519"></a><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_text2371822163519"></a>英文字母、数字、中划线和下划线组成。</span>长度为1～64个字符。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p9371522113518"><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p9371522113518"></a><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p9371522113518"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739420_row346865813454"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739420_p9610175415438"><a name="zh-cn_topic_0165739420_p9610175415438"></a><a name="zh-cn_topic_0165739420_p9610175415438"></a>DWS集群</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p11387132216352"><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p11387132216352"></a><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p11387132216352"></a>存储该通道数据的DWS集群名称。</p>
<p id="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p1387102214353"><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p1387102214353"></a><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p1387102214353"></a>单击<span class="wintitle" id="zh-cn_topic_0165739420_zh-cn_topic_0120206045_wintitle6387102253512"><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_wintitle6387102253512"></a><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_wintitle6387102253512"></a>“选择”</span>，在<span class="wintitle" id="zh-cn_topic_0165739420_zh-cn_topic_0120206045_wintitle738792233518"><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_wintitle738792233518"></a><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_wintitle738792233518"></a>“选择DWS集群”</span>窗口选择一个集群。</p>
<p id="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p12387132283514"><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p12387132283514"></a><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p12387132283514"></a>此配置项仅支持选择，不可手动输入。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739420_p206071954134312"><a name="zh-cn_topic_0165739420_p206071954134312"></a><a name="zh-cn_topic_0165739420_p206071954134312"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739420_row17888513010"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739420_p1460565410436"><a name="zh-cn_topic_0165739420_p1460565410436"></a><a name="zh-cn_topic_0165739420_p1460565410436"></a>DWS数据库</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p17387922123516"><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p17387922123516"></a><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p17387922123516"></a>存储该通道数据的DWS数据库名称。</p>
<p id="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p6387322153515"><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p6387322153515"></a><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p6387322153515"></a>手动输入，不可配置为空。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739420_p16601185434319"><a name="zh-cn_topic_0165739420_p16601185434319"></a><a name="zh-cn_topic_0165739420_p16601185434319"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739420_row2023713124411"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739420_p12351318441"><a name="zh-cn_topic_0165739420_p12351318441"></a><a name="zh-cn_topic_0165739420_p12351318441"></a>数据库模式</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739420_p152317133443"><a name="zh-cn_topic_0165739420_p152317133443"></a><a name="zh-cn_topic_0165739420_p152317133443"></a>一个数据库包含一个或多个命名的模式，模式又包含表。模式还包含其他命名的对象，包括数据类型、函数，以及操作符。同一个对象名可以在不同的模式里使用而不会导致冲突。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739420_p1223101316444"><a name="zh-cn_topic_0165739420_p1223101316444"></a><a name="zh-cn_topic_0165739420_p1223101316444"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739420_row8930102219444"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739420_p793011225443"><a name="zh-cn_topic_0165739420_p793011225443"></a><a name="zh-cn_topic_0165739420_p793011225443"></a>DWS数据表</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p10387152213356"><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p10387152213356"></a><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p10387152213356"></a>存储该通道数据的DWS数据库模式下的数据表。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739420_p209301522104413"><a name="zh-cn_topic_0165739420_p209301522104413"></a><a name="zh-cn_topic_0165739420_p209301522104413"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739420_row144394614444"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739420_p13441846114412"><a name="zh-cn_topic_0165739420_p13441846114412"></a><a name="zh-cn_topic_0165739420_p13441846114412"></a>数据分隔符</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p238792212357"><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p238792212357"></a><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p238792212357"></a>用户数据的字段分隔符，根据此分隔符分隔用户数据插入DWS数据表的相应列。</p>
<p id="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p13387142217350"><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p13387142217350"></a><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p13387142217350"></a>取值范围：不可为空</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739420_p344646134411"><a name="zh-cn_topic_0165739420_p344646134411"></a><a name="zh-cn_topic_0165739420_p344646134411"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739420_row154692588456"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739420_p846916586453"><a name="zh-cn_topic_0165739420_p846916586453"></a><a name="zh-cn_topic_0165739420_p846916586453"></a>偏移量</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_ul19387202217353"></a><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_ul19387202217353"></a><ul id="zh-cn_topic_0165739420_zh-cn_topic_0120206045_ul19387202217353"><li>最新：最大偏移量，即获取最新的有效数据。</li><li>最早：最小偏移量，即读取最早的有效数据。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p1838772218354"><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p1838772218354"></a><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p1838772218354"></a>最新</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739420_row14351951154713"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739420_p535285110473"><a name="zh-cn_topic_0165739420_p535285110473"></a><a name="zh-cn_topic_0165739420_p535285110473"></a>数据转储周期</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p4387172214359"><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p4387172214359"></a><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p4387172214359"></a>根据用户配置的时间，周期性的将数据导入目的地（OBS，MRS，DLI，DWS，CloudTable），若某个时间段内无数据，则此时间段不会生成打包文件。</p>
<p id="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p1938732213352"><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p1938732213352"></a><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p1938732213352"></a>取值范围：30～900。</p>
<p id="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p173876227356"><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p173876227356"></a><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p173876227356"></a>单位：秒。</p>
<p id="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p138716221355"><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p138716221355"></a><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p138716221355"></a>默认配置为300秒。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p1338782293511"><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p1338782293511"></a><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p1338782293511"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739420_row6716317114511"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739420_p1771601714458"><a name="zh-cn_topic_0165739420_p1771601714458"></a><a name="zh-cn_topic_0165739420_p1771601714458"></a>用户名</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p2387522103515"><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p2387522103515"></a><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p2387522103515"></a>DWS集群的用户名。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739420_p271681710458"><a name="zh-cn_topic_0165739420_p271681710458"></a><a name="zh-cn_topic_0165739420_p271681710458"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739420_row11573102412459"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739420_p19574192464514"><a name="zh-cn_topic_0165739420_p19574192464514"></a><a name="zh-cn_topic_0165739420_p19574192464514"></a>密码</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p1538715222354"><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p1538715222354"></a><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p1538715222354"></a>DWS集群的密码。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739420_p4574122484519"><a name="zh-cn_topic_0165739420_p4574122484519"></a><a name="zh-cn_topic_0165739420_p4574122484519"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739420_row11556734184515"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739420_p155610349457"><a name="zh-cn_topic_0165739420_p155610349457"></a><a name="zh-cn_topic_0165739420_p155610349457"></a>KMS密钥</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p16387112219354"><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p16387112219354"></a><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p16387112219354"></a>集群的数据库加密密钥。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739420_p35568346453"><a name="zh-cn_topic_0165739420_p35568346453"></a><a name="zh-cn_topic_0165739420_p35568346453"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739420_row7508810153116"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739420_p1508111043117"><a name="zh-cn_topic_0165739420_p1508111043117"></a><a name="zh-cn_topic_0165739420_p1508111043117"></a>数据临时桶</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p1238742213359"><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p1238742213359"></a><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p1238742213359"></a>用户数据先临时存储在OBS桶中，再转储到指定的转储服务，转储完成后临时桶中的数据会被清除。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p838762214358"><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p838762214358"></a><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p838762214358"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739420_row119451913118"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739420_p1895121953117"><a name="zh-cn_topic_0165739420_p1895121953117"></a><a name="zh-cn_topic_0165739420_p1895121953117"></a>数据临时目录</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p15387172211357"><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p15387172211357"></a><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p15387172211357"></a>需要转储的数据临时存储在OBS桶下此配置项配置的目录中，转储完成后临时目录中的数据会被清除。</p>
<p id="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p1838712222353"><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p1838712222353"></a><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p1838712222353"></a>配置为空时，数据直接存储在OBS桶内。</p>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p3387142219355"><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p3387142219355"></a><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p3387142219355"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0165739420_row96691584616"><td class="cellrowborder" valign="top" width="21.08210821082108%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0165739420_p466945144613"><a name="zh-cn_topic_0165739420_p466945144613"></a><a name="zh-cn_topic_0165739420_p466945144613"></a>容错选项</p>
</td>
<td class="cellrowborder" valign="top" width="56.66566656665667%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p109384485447"><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p109384485447"></a><a name="zh-cn_topic_0165739420_zh-cn_topic_0120206045_p109384485447"></a>通过单击<a name="image12311203415811"></a><a name="image12311203415811"></a><span><img id="image12311203415811" src="figures/icon-dayu-enable-HEC.png"></span>或<a name="image167641642115811"></a><a name="image167641642115811"></a><span><img id="image167641642115811" src="figures/icon-dayu-disable-HEC.png"></span>来关闭或开启容错选项开关。<a name="zh-cn_topic_0165739420_ul6169182011536"></a><a name="zh-cn_topic_0165739420_ul6169182011536"></a><ul id="zh-cn_topic_0165739420_ul6169182011536"><li>fill_missing_fields<p id="zh-cn_topic_0165739420_p379819383532"><a name="zh-cn_topic_0165739420_p379819383532"></a><a name="zh-cn_topic_0165739420_p379819383532"></a>当数据导入时，若数据源文件中一行的最后一个字段缺失的处理方式。</p>
<p id="zh-cn_topic_0165739420_p1887613329531"><a name="zh-cn_topic_0165739420_p1887613329531"></a><a name="zh-cn_topic_0165739420_p1887613329531"></a>取值范围：true/on，false/off。缺省值为false/off。</p>
<a name="zh-cn_topic_0165739420_ul2063194585320"></a><a name="zh-cn_topic_0165739420_ul2063194585320"></a><ul id="zh-cn_topic_0165739420_ul2063194585320"><li>参数为true/on，当数据导入时，若数据源文件中一行数据的最后一个字段缺失，则把最后一个字段的值设置为NULL，不报错。</li></ul>
<a name="zh-cn_topic_0165739420_ul735619055417"></a><a name="zh-cn_topic_0165739420_ul735619055417"></a><ul id="zh-cn_topic_0165739420_ul735619055417"><li>参数为false/off，如果最后一个字段缺失会显示如下错误信息。<pre class="screen" id="zh-cn_topic_0165739420_screen12356100125410"><a name="zh-cn_topic_0165739420_screen12356100125410"></a><a name="zh-cn_topic_0165739420_screen12356100125410"></a>missing data for column "tt"</pre>
</li></ul>
</li><li>ignore_extra_data<p id="zh-cn_topic_0165739420_p229103385410"><a name="zh-cn_topic_0165739420_p229103385410"></a><a name="zh-cn_topic_0165739420_p229103385410"></a>数据源文件中的字段比外表定义列数多时，是否忽略多出的列。该参数只在数据导入过程中使用。</p>
<p id="zh-cn_topic_0165739420_p121991431155416"><a name="zh-cn_topic_0165739420_p121991431155416"></a><a name="zh-cn_topic_0165739420_p121991431155416"></a>取值范围：true/on，false/off。缺省值为false/off。</p>
<a name="zh-cn_topic_0165739420_ul4802113825420"></a><a name="zh-cn_topic_0165739420_ul4802113825420"></a><ul id="zh-cn_topic_0165739420_ul4802113825420"><li>参数为true/on，若数据源文件比外表定义列数多，则忽略行尾多出来的列。</li></ul>
<a name="zh-cn_topic_0165739420_ul1755015435410"></a><a name="zh-cn_topic_0165739420_ul1755015435410"></a><ul id="zh-cn_topic_0165739420_ul1755015435410"><li>参数为false/off，若数据源文件比外表定义列数多，会显示如下错误信息。<pre class="screen" id="zh-cn_topic_0165739420_screen10550105495418"><a name="zh-cn_topic_0165739420_screen10550105495418"></a><a name="zh-cn_topic_0165739420_screen10550105495418"></a>extra data after last expected column</pre>
<div class="note" id="zh-cn_topic_0165739420_note01272024125514"><a name="zh-cn_topic_0165739420_note01272024125514"></a><a name="zh-cn_topic_0165739420_note01272024125514"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0165739420_p1818218398555"><a name="zh-cn_topic_0165739420_p1818218398555"></a><a name="zh-cn_topic_0165739420_p1818218398555"></a>如果行尾换行符丢失，使两行变成一行时，设置此参数为true将导致后一行数据被忽略掉。</p>
</div></div>
</li></ul>
</li><li>compatible_illegal_chars<p id="zh-cn_topic_0165739420_p1345116205587"><a name="zh-cn_topic_0165739420_p1345116205587"></a><a name="zh-cn_topic_0165739420_p1345116205587"></a>导入非法字符容错参数。此语法仅对READ ONLY的外表有效。</p>
<p id="zh-cn_topic_0165739420_p6996152265716"><a name="zh-cn_topic_0165739420_p6996152265716"></a><a name="zh-cn_topic_0165739420_p6996152265716"></a>取值范围：true/on，false/off。缺省值为false/off。</p>
<a name="zh-cn_topic_0165739420_ul39961022145717"></a><a name="zh-cn_topic_0165739420_ul39961022145717"></a><ul id="zh-cn_topic_0165739420_ul39961022145717"><li>参数为true/on，则导入时遇到非法字符进行容错处理，非法字符转换后入库，不报错，不中断导入。</li><li>参数为false/off，导入时遇到非法字符进行报错，中断导入。<div class="notice" id="zh-cn_topic_0165739420_note373118296577"><a name="zh-cn_topic_0165739420_note373118296577"></a><a name="zh-cn_topic_0165739420_note373118296577"></a><span class="noticetitle"> 须知： </span><div class="noticebody"><p id="zh-cn_topic_0165739420_p5189103912571"><a name="zh-cn_topic_0165739420_p5189103912571"></a><a name="zh-cn_topic_0165739420_p5189103912571"></a>Windows平台下OBS若按照文本格式读取数据文件，遇到0x1A会作为EOF符号结束数据读入造成解析错误，这是Windows平台的实现约束。由于OBS不支持BINARY形式读取，可将相应数据文件交由Linux平台下的OBS读取。</p>
</div></div>
</li></ul>
<div class="p" id="zh-cn_topic_0165739420_p1662117105813"><a name="zh-cn_topic_0165739420_p1662117105813"></a><a name="zh-cn_topic_0165739420_p1662117105813"></a><div class="note" id="zh-cn_topic_0165739420_note1433134311571"><a name="zh-cn_topic_0165739420_note1433134311571"></a><a name="zh-cn_topic_0165739420_note1433134311571"></a><span class="notetitle"> 说明： </span><div class="notebody"><a name="zh-cn_topic_0165739420_ul12292449165713"></a><a name="zh-cn_topic_0165739420_ul12292449165713"></a><ul id="zh-cn_topic_0165739420_ul12292449165713"><li>导入非法字符容错规则如下：<p id="zh-cn_topic_0165739420_p2292174919577"><a name="zh-cn_topic_0165739420_p2292174919577"></a><a name="zh-cn_topic_0165739420_p2292174919577"></a>（1）对于'\0'，容错后转换为空格；</p>
<p id="zh-cn_topic_0165739420_p329218499575"><a name="zh-cn_topic_0165739420_p329218499575"></a><a name="zh-cn_topic_0165739420_p329218499575"></a>（2）对于其他非法字符，容错后转换为问号；</p>
<p id="zh-cn_topic_0165739420_p102921649135712"><a name="zh-cn_topic_0165739420_p102921649135712"></a><a name="zh-cn_topic_0165739420_p102921649135712"></a>（3）若compatible_illegal_chars为true/on标识导入时对于非法字符进行容错处理，则若NULL、DELIMITER、QUOTE、ESCAPE设置为空格或问号则会通过如"illegal chars conversion may confuse COPY escape 0x20"等报错信息提示用户修改可能引起混淆的参数以避免导入错误。</p>
</li></ul>
</div></div>
</div>
</li><li><strong id="zh-cn_topic_0165739420_b12041043811"><a name="zh-cn_topic_0165739420_b12041043811"></a><a name="zh-cn_topic_0165739420_b12041043811"></a>PER NODE REJECT LIMIT 'value'</strong><p id="zh-cn_topic_0165739420_p1220413431711"><a name="zh-cn_topic_0165739420_p1220413431711"></a><a name="zh-cn_topic_0165739420_p1220413431711"></a>指定本次数据导入过程中每个DN实例上允许出现的数据格式错误的数量，如果有一个DN实例上的错误数量大于设定值，本次导入失败，报错退出。</p>
<div class="p" id="zh-cn_topic_0165739420_p5312105712216"><a name="zh-cn_topic_0165739420_p5312105712216"></a><a name="zh-cn_topic_0165739420_p5312105712216"></a>取值范围：整型值，unlimited（无限），缺省值为0，有错误信息立即返回。<div class="note" id="zh-cn_topic_0165739420_note42593594115"><a name="zh-cn_topic_0165739420_note42593594115"></a><a name="zh-cn_topic_0165739420_note42593594115"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0165739420_p11425151925"><a name="zh-cn_topic_0165739420_p11425151925"></a><a name="zh-cn_topic_0165739420_p11425151925"></a>此语法指定的是单个节点的错误容忍度。</p>
<p id="zh-cn_topic_0165739420_p1396812321217"><a name="zh-cn_topic_0165739420_p1396812321217"></a><a name="zh-cn_topic_0165739420_p1396812321217"></a>数据格式错误是指缺少或者多出字段值，数据类型错误或者编码错误。对于非数据格式错误，一旦发生就将导致整个数据扫描失败。</p>
</div></div>
</div>
</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="22.252225222522252%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0165739420_p14669135174611"><a name="zh-cn_topic_0165739420_p14669135174611"></a><a name="zh-cn_topic_0165739420_p14669135174611"></a>-</p>
</td>
</tr>
</tbody>
</table>

