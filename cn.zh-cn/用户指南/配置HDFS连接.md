# 配置HDFS连接<a name="dayu_01_0040"></a>

目前CDM支持连接的HDFS数据源有以下几种：

-   [MRS HDFS](#zh-cn_topic_0108275286_section127371747103314)
-   [FusionInsight HDFS](#zh-cn_topic_0108275286_section1851831133416)
-   [Apache HDFS](#zh-cn_topic_0108275286_section690499173512)

## MRS HDFS<a name="zh-cn_topic_0108275286_section127371747103314"></a>

连接MRS上的HDFS数据源时，相关参数如[表1](#zh-cn_topic_0108275286_table6441152003419)所示。

**表 1**  MRS上的HDFS连接参数

<a name="zh-cn_topic_0108275286_table6441152003419"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108275286_row15441220123417"><th class="cellrowborder" valign="top" width="20.51%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108275286_p18441202093413"><a name="zh-cn_topic_0108275286_p18441202093413"></a><a name="zh-cn_topic_0108275286_p18441202093413"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="57.720000000000006%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108275286_p1544152053412"><a name="zh-cn_topic_0108275286_p1544152053412"></a><a name="zh-cn_topic_0108275286_p1544152053412"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="21.77%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108275286_p4441112010341"><a name="zh-cn_topic_0108275286_p4441112010341"></a><a name="zh-cn_topic_0108275286_p4441112010341"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108275286_row11441182012346"><td class="cellrowborder" valign="top" width="20.51%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p4456620113417"><a name="zh-cn_topic_0108275286_p4456620113417"></a><a name="zh-cn_topic_0108275286_p4456620113417"></a>名称</p>
</td>
<td class="cellrowborder" valign="top" width="57.720000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p6456820183418"><a name="zh-cn_topic_0108275286_p6456820183418"></a><a name="zh-cn_topic_0108275286_p6456820183418"></a>连接的名称，根据连接的数据源类型，用户可自定义便于记忆、区分的连接名。</p>
</td>
<td class="cellrowborder" valign="top" width="21.77%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p13456112023418"><a name="zh-cn_topic_0108275286_p13456112023418"></a><a name="zh-cn_topic_0108275286_p13456112023418"></a>mrs_hdfs_link</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row2456122053415"><td class="cellrowborder" valign="top" width="20.51%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p13456172019344"><a name="zh-cn_topic_0108275286_p13456172019344"></a><a name="zh-cn_topic_0108275286_p13456172019344"></a>Manager IP</p>
</td>
<td class="cellrowborder" valign="top" width="57.720000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p1345602010341"><a name="zh-cn_topic_0108275286_p1345602010341"></a><a name="zh-cn_topic_0108275286_p1345602010341"></a>MRS Manager的IP地址，可以单击输入框后的<span class="uicontrol" id="zh-cn_topic_0108275286_uicontrol926725316310"><a name="zh-cn_topic_0108275286_uicontrol926725316310"></a><a name="zh-cn_topic_0108275286_uicontrol926725316310"></a>“选择”</span>来选定已创建的MRS集群，CDM会自动填充下面的鉴权参数。</p>
</td>
<td class="cellrowborder" valign="top" width="21.77%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p13456420143418"><a name="zh-cn_topic_0108275286_p13456420143418"></a><a name="zh-cn_topic_0108275286_p13456420143418"></a>127.0.0.1</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row35701836203511"><td class="cellrowborder" valign="top" width="20.51%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p1752314773514"><a name="zh-cn_topic_0108275286_p1752314773514"></a><a name="zh-cn_topic_0108275286_p1752314773514"></a>认证类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.720000000000006%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108275286_p12523147173511"><a name="zh-cn_topic_0108275286_p12523147173511"></a><a name="zh-cn_topic_0108275286_p12523147173511"></a>访问MRS的认证类型：<a name="zh-cn_topic_0108275286_ul552304715358"></a><a name="zh-cn_topic_0108275286_ul552304715358"></a><ul id="zh-cn_topic_0108275286_ul552304715358"><li>SIMPLE：非安全模式选择Simple鉴权。</li><li>KERBEROS：安全模式选择Kerberos鉴权。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="21.77%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p252324712357"><a name="zh-cn_topic_0108275286_p252324712357"></a><a name="zh-cn_topic_0108275286_p252324712357"></a>SIMPLE</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row16456152011347"><td class="cellrowborder" valign="top" width="20.51%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p94561620113420"><a name="zh-cn_topic_0108275286_p94561620113420"></a><a name="zh-cn_topic_0108275286_p94561620113420"></a>用户名</p>
</td>
<td class="cellrowborder" valign="top" width="57.720000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p64738206349"><a name="zh-cn_topic_0108275286_p64738206349"></a><a name="zh-cn_topic_0108275286_p64738206349"></a>选择KERBEROS鉴权时，需要配置MRS Manager的用户名和密码。</p>
<p id="zh-cn_topic_0108275286_p44304453301"><a name="zh-cn_topic_0108275286_p44304453301"></a><a name="zh-cn_topic_0108275286_p44304453301"></a>从HDFS导出目录时，如果需要创建快照，这里配置的用户需要HDFS系统的管理员权限。</p>
</td>
<td class="cellrowborder" valign="top" width="21.77%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p3473020113416"><a name="zh-cn_topic_0108275286_p3473020113416"></a><a name="zh-cn_topic_0108275286_p3473020113416"></a>cdm</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row20456320123419"><td class="cellrowborder" valign="top" width="20.51%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p647322020346"><a name="zh-cn_topic_0108275286_p647322020346"></a><a name="zh-cn_topic_0108275286_p647322020346"></a>密码</p>
</td>
<td class="cellrowborder" valign="top" width="57.720000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p174737206340"><a name="zh-cn_topic_0108275286_p174737206340"></a><a name="zh-cn_topic_0108275286_p174737206340"></a>访问MRS Manager的用户密码。</p>
</td>
<td class="cellrowborder" valign="top" width="21.77%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p204731920153414"><a name="zh-cn_topic_0108275286_p204731920153414"></a><a name="zh-cn_topic_0108275286_p204731920153414"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row10211145833913"><td class="cellrowborder" valign="top" width="20.51%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p721185823920"><a name="zh-cn_topic_0108275286_p721185823920"></a><a name="zh-cn_topic_0108275286_p721185823920"></a>运行模式</p>
</td>
<td class="cellrowborder" valign="top" width="57.720000000000006%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108275286_p206752056145718"><a name="zh-cn_topic_0108275286_p206752056145718"></a><a name="zh-cn_topic_0108275286_p206752056145718"></a>选择HDFS连接的运行模式：<a name="zh-cn_topic_0108275286_ul1747017597574"></a><a name="zh-cn_topic_0108275286_ul1747017597574"></a><ul id="zh-cn_topic_0108275286_ul1747017597574"><li>EMBEDDED：连接实例与CDM运行在一起，该模式性能较好。</li><li>STANDALONE：连接实例运行在独立进程。如果CDM需要对接多个Hadoop数据源（MRS、Hadoop或CloudTable），并且既有KERBEROS认证模式又有SIMPLE认证模式，只能使用STANDALONE模式或者配置不同的Agent。</li><li>Agent：连接实例运行在Agent上。</li></ul>
</div>
<p id="zh-cn_topic_0108275286_p5211105873913"><a name="zh-cn_topic_0108275286_p5211105873913"></a><a name="zh-cn_topic_0108275286_p5211105873913"></a>选择STANDALONE模式时，CDM支持在多个MRS集群的HDFS之间迁移数据。</p>
</td>
<td class="cellrowborder" valign="top" width="21.77%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p1021155811394"><a name="zh-cn_topic_0108275286_p1021155811394"></a><a name="zh-cn_topic_0108275286_p1021155811394"></a>STANDALONE</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row1946581311414"><td class="cellrowborder" valign="top" width="20.51%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p1999031319386"><a name="zh-cn_topic_0108275286_p1999031319386"></a><a name="zh-cn_topic_0108275286_p1999031319386"></a>Agent</p>
</td>
<td class="cellrowborder" valign="top" width="57.720000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p5412193413515"><a name="zh-cn_topic_0108275286_p5412193413515"></a><a name="zh-cn_topic_0108275286_p5412193413515"></a>单击<span class="uicontrol" id="zh-cn_topic_0108275286_uicontrol7592322128"><a name="zh-cn_topic_0108275286_uicontrol7592322128"></a><a name="zh-cn_topic_0108275286_uicontrol7592322128"></a>“选择”</span>，选择<a href="Agent管理.md">Agent管理</a>中已创建的Agent。</p>
</td>
<td class="cellrowborder" valign="top" width="21.77%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p1499013137381"><a name="zh-cn_topic_0108275286_p1499013137381"></a><a name="zh-cn_topic_0108275286_p1499013137381"></a>-</p>
</td>
</tr>
</tbody>
</table>

## FusionInsight HDFS<a name="zh-cn_topic_0108275286_section1851831133416"></a>

连接FusionInsight HD上的HDFS数据源时，相关参数如[表2](#zh-cn_topic_0108275286_table34037531171418)所示。

**表 2**  FusionInsight HDFS连接参数

<a name="zh-cn_topic_0108275286_table34037531171418"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108275286_row56630393171418"><th class="cellrowborder" valign="top" width="20.74%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108275286_p23659124171418"><a name="zh-cn_topic_0108275286_p23659124171418"></a><a name="zh-cn_topic_0108275286_p23659124171418"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="57.97%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108275286_p37340867171418"><a name="zh-cn_topic_0108275286_p37340867171418"></a><a name="zh-cn_topic_0108275286_p37340867171418"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="21.29%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108275286_p4711375171418"><a name="zh-cn_topic_0108275286_p4711375171418"></a><a name="zh-cn_topic_0108275286_p4711375171418"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108275286_row46077055171418"><td class="cellrowborder" valign="top" width="20.74%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p41253947171418"><a name="zh-cn_topic_0108275286_p41253947171418"></a><a name="zh-cn_topic_0108275286_p41253947171418"></a>名称</p>
</td>
<td class="cellrowborder" valign="top" width="57.97%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p6573133312010"><a name="zh-cn_topic_0108275286_p6573133312010"></a><a name="zh-cn_topic_0108275286_p6573133312010"></a>连接的名称，根据连接的数据源类型，用户可自定义便于记忆、区分的连接名。</p>
</td>
<td class="cellrowborder" valign="top" width="21.29%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p2330994016248"><a name="zh-cn_topic_0108275286_p2330994016248"></a><a name="zh-cn_topic_0108275286_p2330994016248"></a>FI_hdfs_link</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row12661410173510"><td class="cellrowborder" valign="top" width="20.74%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p13662121012355"><a name="zh-cn_topic_0108275286_p13662121012355"></a><a name="zh-cn_topic_0108275286_p13662121012355"></a>Manager IP</p>
</td>
<td class="cellrowborder" valign="top" width="57.97%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p06633101352"><a name="zh-cn_topic_0108275286_p06633101352"></a><a name="zh-cn_topic_0108275286_p06633101352"></a>FusionInsight Manager平台的地址。</p>
</td>
<td class="cellrowborder" valign="top" width="21.29%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p10663131016353"><a name="zh-cn_topic_0108275286_p10663131016353"></a><a name="zh-cn_topic_0108275286_p10663131016353"></a>127.0.0.1</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row291371115352"><td class="cellrowborder" valign="top" width="20.74%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p9913311193516"><a name="zh-cn_topic_0108275286_p9913311193516"></a><a name="zh-cn_topic_0108275286_p9913311193516"></a>Manager端口</p>
</td>
<td class="cellrowborder" valign="top" width="57.97%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p3913811183515"><a name="zh-cn_topic_0108275286_p3913811183515"></a><a name="zh-cn_topic_0108275286_p3913811183515"></a>FusionInsight Manager平台的端口。</p>
</td>
<td class="cellrowborder" valign="top" width="21.29%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p491310118354"><a name="zh-cn_topic_0108275286_p491310118354"></a><a name="zh-cn_topic_0108275286_p491310118354"></a>28443</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row7625141843512"><td class="cellrowborder" valign="top" width="20.74%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p0625201813356"><a name="zh-cn_topic_0108275286_p0625201813356"></a><a name="zh-cn_topic_0108275286_p0625201813356"></a>CAS Server端口</p>
</td>
<td class="cellrowborder" valign="top" width="57.97%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p186251918103513"><a name="zh-cn_topic_0108275286_p186251918103513"></a><a name="zh-cn_topic_0108275286_p186251918103513"></a>与FusionInsight对接的CAS Server的端口。</p>
</td>
<td class="cellrowborder" valign="top" width="21.29%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p4625131883518"><a name="zh-cn_topic_0108275286_p4625131883518"></a><a name="zh-cn_topic_0108275286_p4625131883518"></a>20009</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row10481934205911"><td class="cellrowborder" valign="top" width="20.74%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p1648133485913"><a name="zh-cn_topic_0108275286_p1648133485913"></a><a name="zh-cn_topic_0108275286_p1648133485913"></a>用户名</p>
</td>
<td class="cellrowborder" valign="top" width="57.97%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p15481183410599"><a name="zh-cn_topic_0108275286_p15481183410599"></a><a name="zh-cn_topic_0108275286_p15481183410599"></a>登录FusionInsight Manager平台的用户名。</p>
<p id="zh-cn_topic_0108275286_p15879213349"><a name="zh-cn_topic_0108275286_p15879213349"></a><a name="zh-cn_topic_0108275286_p15879213349"></a>从HDFS导出目录时，如果需要创建快照，这里配置的用户需要HDFS系统的管理员权限。</p>
</td>
<td class="cellrowborder" valign="top" width="21.29%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p548163420594"><a name="zh-cn_topic_0108275286_p548163420594"></a><a name="zh-cn_topic_0108275286_p548163420594"></a>cdm</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row4905133519593"><td class="cellrowborder" valign="top" width="20.74%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p16905153517591"><a name="zh-cn_topic_0108275286_p16905153517591"></a><a name="zh-cn_topic_0108275286_p16905153517591"></a>密码</p>
</td>
<td class="cellrowborder" valign="top" width="57.97%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p199057357597"><a name="zh-cn_topic_0108275286_p199057357597"></a><a name="zh-cn_topic_0108275286_p199057357597"></a>FusionInsight Manager平台的密码。</p>
</td>
<td class="cellrowborder" valign="top" width="21.29%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p189057358594"><a name="zh-cn_topic_0108275286_p189057358594"></a><a name="zh-cn_topic_0108275286_p189057358594"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row15485153518397"><td class="cellrowborder" valign="top" width="20.74%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p1562410194013"><a name="zh-cn_topic_0108275286_p1562410194013"></a><a name="zh-cn_topic_0108275286_p1562410194013"></a>认证类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.97%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108275286_p1962419018404"><a name="zh-cn_topic_0108275286_p1962419018404"></a><a name="zh-cn_topic_0108275286_p1962419018404"></a>访问FusionInsight HD的认证类型。<a name="zh-cn_topic_0108275286_ul36245017400"></a><a name="zh-cn_topic_0108275286_ul36245017400"></a><ul id="zh-cn_topic_0108275286_ul36245017400"><li>SIMPLE：非安全模式选择Simple鉴权。</li><li>KERBEROS：安全模式选择Kerberos鉴权。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="21.29%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p106241018407"><a name="zh-cn_topic_0108275286_p106241018407"></a><a name="zh-cn_topic_0108275286_p106241018407"></a>KERBEROS</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row129026915554"><td class="cellrowborder" valign="top" width="20.74%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p1418522311554"><a name="zh-cn_topic_0108275286_p1418522311554"></a><a name="zh-cn_topic_0108275286_p1418522311554"></a>运行模式</p>
</td>
<td class="cellrowborder" valign="top" width="57.97%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108275286_p1990239195518"><a name="zh-cn_topic_0108275286_p1990239195518"></a><a name="zh-cn_topic_0108275286_p1990239195518"></a>选择HDFS连接的运行模式：<a name="zh-cn_topic_0108275286_zh-cn_topic_0108275286_ul1747017597574"></a><a name="zh-cn_topic_0108275286_zh-cn_topic_0108275286_ul1747017597574"></a><ul id="zh-cn_topic_0108275286_zh-cn_topic_0108275286_ul1747017597574"><li>EMBEDDED：连接实例与CDM运行在一起，该模式性能较好。</li><li>STANDALONE：连接实例运行在独立进程。如果CDM需要对接多个Hadoop数据源（MRS、Hadoop或CloudTable），并且既有KERBEROS认证模式又有SIMPLE认证模式，只能使用STANDALONE模式或者配置不同的Agent。</li><li>Agent：连接实例运行在Agent上。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="21.29%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p18902892555"><a name="zh-cn_topic_0108275286_p18902892555"></a><a name="zh-cn_topic_0108275286_p18902892555"></a>STANDALONE</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row5249204817429"><td class="cellrowborder" valign="top" width="20.74%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p10250104844219"><a name="zh-cn_topic_0108275286_p10250104844219"></a><a name="zh-cn_topic_0108275286_p10250104844219"></a>Agent</p>
</td>
<td class="cellrowborder" valign="top" width="57.97%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p1425064819422"><a name="zh-cn_topic_0108275286_p1425064819422"></a><a name="zh-cn_topic_0108275286_p1425064819422"></a>单击<span class="uicontrol" id="zh-cn_topic_0108275286_zh-cn_topic_0108275286_uicontrol7592322128"><a name="zh-cn_topic_0108275286_zh-cn_topic_0108275286_uicontrol7592322128"></a><a name="zh-cn_topic_0108275286_zh-cn_topic_0108275286_uicontrol7592322128"></a>“选择”</span>，选择<a href="Agent管理.md">Agent管理</a>中已创建的Agent。</p>
</td>
<td class="cellrowborder" valign="top" width="21.29%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p13250648124212"><a name="zh-cn_topic_0108275286_p13250648124212"></a><a name="zh-cn_topic_0108275286_p13250648124212"></a>-</p>
</td>
</tr>
</tbody>
</table>

## Apache HDFS<a name="zh-cn_topic_0108275286_section690499173512"></a>

连接Apache Hadoop上的HDFS数据源时，相关参数如[表3](#zh-cn_topic_0108275286_table49051917359)所示。

**表 3**  Apache HDFS连接参数

<a name="zh-cn_topic_0108275286_table49051917359"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108275286_row1990717913513"><th class="cellrowborder" valign="top" width="20.96%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108275286_p1390869143515"><a name="zh-cn_topic_0108275286_p1390869143515"></a><a name="zh-cn_topic_0108275286_p1390869143515"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="58.08%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108275286_p7909149183510"><a name="zh-cn_topic_0108275286_p7909149183510"></a><a name="zh-cn_topic_0108275286_p7909149183510"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="20.96%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108275286_p591059133516"><a name="zh-cn_topic_0108275286_p591059133516"></a><a name="zh-cn_topic_0108275286_p591059133516"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108275286_row1391259163511"><td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p0913139163519"><a name="zh-cn_topic_0108275286_p0913139163519"></a><a name="zh-cn_topic_0108275286_p0913139163519"></a>名称</p>
</td>
<td class="cellrowborder" valign="top" width="58.08%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p1369564463813"><a name="zh-cn_topic_0108275286_p1369564463813"></a><a name="zh-cn_topic_0108275286_p1369564463813"></a>连接的名称，根据连接的数据源类型，用户可自定义便于记忆、区分的连接名。</p>
</td>
<td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p5919292355"><a name="zh-cn_topic_0108275286_p5919292355"></a><a name="zh-cn_topic_0108275286_p5919292355"></a>hadoop_hdfs_link</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row1191969203511"><td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p29204953520"><a name="zh-cn_topic_0108275286_p29204953520"></a><a name="zh-cn_topic_0108275286_p29204953520"></a>URI</p>
</td>
<td class="cellrowborder" valign="top" width="58.08%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p13924149173517"><a name="zh-cn_topic_0108275286_p13924149173517"></a><a name="zh-cn_topic_0108275286_p13924149173517"></a>表示NameNode URI地址。</p>
</td>
<td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p15245145210401"><a name="zh-cn_topic_0108275286_p15245145210401"></a><a name="zh-cn_topic_0108275286_p15245145210401"></a>hdfs://nn1.example.com/</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row49250918352"><td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p189268910357"><a name="zh-cn_topic_0108275286_p189268910357"></a><a name="zh-cn_topic_0108275286_p189268910357"></a>认证类型</p>
</td>
<td class="cellrowborder" valign="top" width="58.08%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108275286_p18927139153518"><a name="zh-cn_topic_0108275286_p18927139153518"></a><a name="zh-cn_topic_0108275286_p18927139153518"></a>访问Hadoop的认证类型。<a name="zh-cn_topic_0108275286_ul119271496357"></a><a name="zh-cn_topic_0108275286_ul119271496357"></a><ul id="zh-cn_topic_0108275286_ul119271496357"><li>SIMPLE：非安全模式Hadoop选择Simple鉴权。</li><li>KERBEROS：安全模式Hadoop选择Kerberos鉴权，通过获取客户端的principal和keytab文件在应用程序中进行认证。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p109305910356"><a name="zh-cn_topic_0108275286_p109305910356"></a><a name="zh-cn_topic_0108275286_p109305910356"></a>KERBEROS</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row1893111911354"><td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p59321897351"><a name="zh-cn_topic_0108275286_p59321897351"></a><a name="zh-cn_topic_0108275286_p59321897351"></a>Principal</p>
</td>
<td class="cellrowborder" valign="top" width="58.08%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p8933492358"><a name="zh-cn_topic_0108275286_p8933492358"></a><a name="zh-cn_topic_0108275286_p8933492358"></a>选择Kerberos鉴权时，用于认证的帐号Principal，您可以联系Hadoop管理员获取此帐号。</p>
</td>
<td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p159349920353"><a name="zh-cn_topic_0108275286_p159349920353"></a><a name="zh-cn_topic_0108275286_p159349920353"></a>USER@YOUR-REALM.COM</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row179341997352"><td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p1193512917358"><a name="zh-cn_topic_0108275286_p1193512917358"></a><a name="zh-cn_topic_0108275286_p1193512917358"></a>Keytab文件</p>
</td>
<td class="cellrowborder" valign="top" width="58.08%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p2935189143517"><a name="zh-cn_topic_0108275286_p2935189143517"></a><a name="zh-cn_topic_0108275286_p2935189143517"></a>选择Kerberos鉴权时，用于认证的Keytab文件，您可以联系Hadoop管理员获取此文件。</p>
</td>
<td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p135421727850"><a name="zh-cn_topic_0108275286_p135421727850"></a><a name="zh-cn_topic_0108275286_p135421727850"></a>/opt/user.keytab</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row19155101546"><td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p8915181018541"><a name="zh-cn_topic_0108275286_p8915181018541"></a><a name="zh-cn_topic_0108275286_p8915181018541"></a>IP与主机名映射</p>
</td>
<td class="cellrowborder" valign="top" width="58.08%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p791561045418"><a name="zh-cn_topic_0108275286_p791561045418"></a><a name="zh-cn_topic_0108275286_p791561045418"></a>如果HDFS配置文件使用主机名，需要配置IP与主机的映射。格式：IP与主机名之间使用空格分隔，多对映射使用分号或回车换行分隔。</p>
</td>
<td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p17915181012548"><a name="zh-cn_topic_0108275286_p17915181012548"></a><a name="zh-cn_topic_0108275286_p17915181012548"></a>10.1.6.9 hostname01</p>
<p id="zh-cn_topic_0108275286_p2011684813202"><a name="zh-cn_topic_0108275286_p2011684813202"></a><a name="zh-cn_topic_0108275286_p2011684813202"></a>10.2.7.9 hostname02</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row693151312543"><td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p174517362557"><a name="zh-cn_topic_0108275286_p174517362557"></a><a name="zh-cn_topic_0108275286_p174517362557"></a>运行模式</p>
</td>
<td class="cellrowborder" valign="top" width="58.08%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108275286_p693111135543"><a name="zh-cn_topic_0108275286_p693111135543"></a><a name="zh-cn_topic_0108275286_p693111135543"></a>选择HDFS连接的运行模式：<a name="zh-cn_topic_0108275286_zh-cn_topic_0108275286_ul1747017597574_1"></a><a name="zh-cn_topic_0108275286_zh-cn_topic_0108275286_ul1747017597574_1"></a><ul id="zh-cn_topic_0108275286_zh-cn_topic_0108275286_ul1747017597574_1"><li>EMBEDDED：连接实例与CDM运行在一起，该模式性能较好。</li><li>STANDALONE：连接实例运行在独立进程。如果CDM需要对接多个Hadoop数据源（MRS、Hadoop或CloudTable），并且既有KERBEROS认证模式又有SIMPLE认证模式，只能使用STANDALONE模式或者配置不同的Agent。</li><li>Agent：连接实例运行在Agent上。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p15931141318544"><a name="zh-cn_topic_0108275286_p15931141318544"></a><a name="zh-cn_topic_0108275286_p15931141318544"></a>STANDALONE</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row13173134416"><td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p20303117444"><a name="zh-cn_topic_0108275286_p20303117444"></a><a name="zh-cn_topic_0108275286_p20303117444"></a>Agent</p>
</td>
<td class="cellrowborder" valign="top" width="58.08%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p461134915213"><a name="zh-cn_topic_0108275286_p461134915213"></a><a name="zh-cn_topic_0108275286_p461134915213"></a>单击<span class="uicontrol" id="zh-cn_topic_0108275286_zh-cn_topic_0108275286_uicontrol7592322128_1"><a name="zh-cn_topic_0108275286_zh-cn_topic_0108275286_uicontrol7592322128_1"></a><a name="zh-cn_topic_0108275286_zh-cn_topic_0108275286_uicontrol7592322128_1"></a>“选择”</span>，选择<a href="Agent管理.md">Agent管理</a>中已创建的Agent。</p>
</td>
<td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p123193116445"><a name="zh-cn_topic_0108275286_p123193116445"></a><a name="zh-cn_topic_0108275286_p123193116445"></a>-</p>
</td>
</tr>
</tbody>
</table>

