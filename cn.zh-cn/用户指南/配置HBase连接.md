# 配置HBase连接<a name="dayu_01_0039"></a>

目前CDM支持连接的HBase数据源有以下几种：

-   [MRS HBase](#zh-cn_topic_0108604188_section127371747103314)
-   [FusionInsight HBase](#zh-cn_topic_0108604188_section1851831133416)
-   [Apache HBase](#zh-cn_topic_0108604188_section690499173512)

## MRS HBase<a name="zh-cn_topic_0108604188_section127371747103314"></a>

连接MRS上的HBase数据源时，相关参数如[表1](#zh-cn_topic_0108604188_table6441152003419)所示。

**表 1**  MRS上的HBase连接参数

<a name="zh-cn_topic_0108604188_table6441152003419"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108604188_row15441220123417"><th class="cellrowborder" valign="top" width="21.520000000000003%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108604188_p18441202093413"><a name="zh-cn_topic_0108604188_p18441202093413"></a><a name="zh-cn_topic_0108604188_p18441202093413"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="59.20000000000001%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108604188_p1544152053412"><a name="zh-cn_topic_0108604188_p1544152053412"></a><a name="zh-cn_topic_0108604188_p1544152053412"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="19.28%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108604188_p4441112010341"><a name="zh-cn_topic_0108604188_p4441112010341"></a><a name="zh-cn_topic_0108604188_p4441112010341"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108604188_row11441182012346"><td class="cellrowborder" valign="top" width="21.520000000000003%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108604188_p4456620113417"><a name="zh-cn_topic_0108604188_p4456620113417"></a><a name="zh-cn_topic_0108604188_p4456620113417"></a>名称</p>
</td>
<td class="cellrowborder" valign="top" width="59.20000000000001%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108604188_p6456820183418"><a name="zh-cn_topic_0108604188_p6456820183418"></a><a name="zh-cn_topic_0108604188_p6456820183418"></a>连接的名称，根据连接的数据源类型，用户可自定义便于记忆、区分的连接名。</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108604188_p13456112023418"><a name="zh-cn_topic_0108604188_p13456112023418"></a><a name="zh-cn_topic_0108604188_p13456112023418"></a>mrs_hbase_link</p>
</td>
</tr>
<tr id="zh-cn_topic_0108604188_row2456122053415"><td class="cellrowborder" valign="top" width="21.520000000000003%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108604188_p13456172019344"><a name="zh-cn_topic_0108604188_p13456172019344"></a><a name="zh-cn_topic_0108604188_p13456172019344"></a>Manager IP</p>
</td>
<td class="cellrowborder" valign="top" width="59.20000000000001%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108604188_p1345602010341"><a name="zh-cn_topic_0108604188_p1345602010341"></a><a name="zh-cn_topic_0108604188_p1345602010341"></a>MRS Manager的IP地址，可以单击输入框后的<span class="uicontrol" id="zh-cn_topic_0108604188_zh-cn_topic_0108275286_uicontrol926725316310"><a name="zh-cn_topic_0108604188_zh-cn_topic_0108275286_uicontrol926725316310"></a><a name="zh-cn_topic_0108604188_zh-cn_topic_0108275286_uicontrol926725316310"></a>“选择”</span>来选定已创建的MRS集群，CDM会自动填充下面的鉴权参数。</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108604188_p13456420143418"><a name="zh-cn_topic_0108604188_p13456420143418"></a><a name="zh-cn_topic_0108604188_p13456420143418"></a>127.0.0.1</p>
</td>
</tr>
<tr id="zh-cn_topic_0108604188_row1639225920384"><td class="cellrowborder" valign="top" width="21.520000000000003%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108604188_p06421125396"><a name="zh-cn_topic_0108604188_p06421125396"></a><a name="zh-cn_topic_0108604188_p06421125396"></a>认证类型</p>
</td>
<td class="cellrowborder" valign="top" width="59.20000000000001%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108604188_p3642111243916"><a name="zh-cn_topic_0108604188_p3642111243916"></a><a name="zh-cn_topic_0108604188_p3642111243916"></a>访问MRS的认证类型：<a name="zh-cn_topic_0108604188_zh-cn_topic_0108275286_ul552304715358"></a><a name="zh-cn_topic_0108604188_zh-cn_topic_0108275286_ul552304715358"></a><ul id="zh-cn_topic_0108604188_zh-cn_topic_0108275286_ul552304715358"><li>SIMPLE：非安全模式选择Simple鉴权。</li><li>KERBEROS：安全模式选择Kerberos鉴权。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108604188_p76428123396"><a name="zh-cn_topic_0108604188_p76428123396"></a><a name="zh-cn_topic_0108604188_p76428123396"></a>SIMPLE</p>
</td>
</tr>
<tr id="zh-cn_topic_0108604188_row16456152011347"><td class="cellrowborder" valign="top" width="21.520000000000003%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108604188_p94561620113420"><a name="zh-cn_topic_0108604188_p94561620113420"></a><a name="zh-cn_topic_0108604188_p94561620113420"></a>用户名</p>
</td>
<td class="cellrowborder" valign="top" width="59.20000000000001%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108604188_p64738206349"><a name="zh-cn_topic_0108604188_p64738206349"></a><a name="zh-cn_topic_0108604188_p64738206349"></a>选择KERBEROS鉴权时，需要配置MRS Manager的用户名和密码。</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108604188_p3473020113416"><a name="zh-cn_topic_0108604188_p3473020113416"></a><a name="zh-cn_topic_0108604188_p3473020113416"></a>admin</p>
</td>
</tr>
<tr id="zh-cn_topic_0108604188_row20456320123419"><td class="cellrowborder" valign="top" width="21.520000000000003%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108604188_p647322020346"><a name="zh-cn_topic_0108604188_p647322020346"></a><a name="zh-cn_topic_0108604188_p647322020346"></a>密码</p>
</td>
<td class="cellrowborder" valign="top" width="59.20000000000001%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108604188_p174737206340"><a name="zh-cn_topic_0108604188_p174737206340"></a><a name="zh-cn_topic_0108604188_p174737206340"></a>访问MRS Manager的用户密码。</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108604188_p204731920153414"><a name="zh-cn_topic_0108604188_p204731920153414"></a><a name="zh-cn_topic_0108604188_p204731920153414"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0108604188_row9388103019455"><td class="cellrowborder" valign="top" width="21.520000000000003%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108604188_p12388183016457"><a name="zh-cn_topic_0108604188_p12388183016457"></a><a name="zh-cn_topic_0108604188_p12388183016457"></a>运行模式</p>
</td>
<td class="cellrowborder" valign="top" width="59.20000000000001%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108604188_p121733311504"><a name="zh-cn_topic_0108604188_p121733311504"></a><a name="zh-cn_topic_0108604188_p121733311504"></a>选择HBase连接的运行模式：</p>
<a name="zh-cn_topic_0108604188_ul192118325256"></a><a name="zh-cn_topic_0108604188_ul192118325256"></a><ul id="zh-cn_topic_0108604188_ul192118325256"><li>EMBEDDED：连接实例与CDM运行在一起，该模式性能较好。</li><li>STANDALONE：连接实例运行在独立进程。如果CDM需要对接多个Hadoop数据源（MRS、Hadoop或CloudTable），并且既有KERBEROS认证模式又有SIMPLE认证模式，只能使用STANDALONE模式或者配置不同的Agent。</li><li>Agent：连接实例运行在Agent上。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108604188_p1838813010450"><a name="zh-cn_topic_0108604188_p1838813010450"></a><a name="zh-cn_topic_0108604188_p1838813010450"></a>STANDALONE</p>
</td>
</tr>
</tbody>
</table>

## FusionInsight HBase<a name="zh-cn_topic_0108604188_section1851831133416"></a>

连接FusionInsight HD上的HBase数据源时，相关参数如[表2](#zh-cn_topic_0108604188_table34037531171418)所示。

**表 2**  FusionInsight HBase连接参数

<a name="zh-cn_topic_0108604188_table34037531171418"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108604188_row56630393171418"><th class="cellrowborder" valign="top" width="21.740000000000002%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108604188_p23659124171418"><a name="zh-cn_topic_0108604188_p23659124171418"></a><a name="zh-cn_topic_0108604188_p23659124171418"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="59.64%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108604188_p37340867171418"><a name="zh-cn_topic_0108604188_p37340867171418"></a><a name="zh-cn_topic_0108604188_p37340867171418"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="18.62%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108604188_p4711375171418"><a name="zh-cn_topic_0108604188_p4711375171418"></a><a name="zh-cn_topic_0108604188_p4711375171418"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108604188_row46077055171418"><td class="cellrowborder" valign="top" width="21.740000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108604188_p41253947171418"><a name="zh-cn_topic_0108604188_p41253947171418"></a><a name="zh-cn_topic_0108604188_p41253947171418"></a>名称</p>
</td>
<td class="cellrowborder" valign="top" width="59.64%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108604188_p6573133312010"><a name="zh-cn_topic_0108604188_p6573133312010"></a><a name="zh-cn_topic_0108604188_p6573133312010"></a>连接的名称，根据连接的数据源类型，用户可自定义便于记忆、区分的连接名。</p>
</td>
<td class="cellrowborder" valign="top" width="18.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108604188_p2330994016248"><a name="zh-cn_topic_0108604188_p2330994016248"></a><a name="zh-cn_topic_0108604188_p2330994016248"></a>FI_hbase_link</p>
</td>
</tr>
<tr id="zh-cn_topic_0108604188_row12661410173510"><td class="cellrowborder" valign="top" width="21.740000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108604188_p13662121012355"><a name="zh-cn_topic_0108604188_p13662121012355"></a><a name="zh-cn_topic_0108604188_p13662121012355"></a>Manager IP</p>
</td>
<td class="cellrowborder" valign="top" width="59.64%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108604188_p06633101352"><a name="zh-cn_topic_0108604188_p06633101352"></a><a name="zh-cn_topic_0108604188_p06633101352"></a>FusionInsight Manager平台的地址。</p>
</td>
<td class="cellrowborder" valign="top" width="18.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108604188_p10663131016353"><a name="zh-cn_topic_0108604188_p10663131016353"></a><a name="zh-cn_topic_0108604188_p10663131016353"></a>127.0.0.1</p>
</td>
</tr>
<tr id="zh-cn_topic_0108604188_row291371115352"><td class="cellrowborder" valign="top" width="21.740000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108604188_p9913311193516"><a name="zh-cn_topic_0108604188_p9913311193516"></a><a name="zh-cn_topic_0108604188_p9913311193516"></a>Manager端口</p>
</td>
<td class="cellrowborder" valign="top" width="59.64%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108604188_p3913811183515"><a name="zh-cn_topic_0108604188_p3913811183515"></a><a name="zh-cn_topic_0108604188_p3913811183515"></a>FusionInsight Manager平台的端口。</p>
</td>
<td class="cellrowborder" valign="top" width="18.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108604188_p491310118354"><a name="zh-cn_topic_0108604188_p491310118354"></a><a name="zh-cn_topic_0108604188_p491310118354"></a>28443</p>
</td>
</tr>
<tr id="zh-cn_topic_0108604188_row7625141843512"><td class="cellrowborder" valign="top" width="21.740000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108604188_p0625201813356"><a name="zh-cn_topic_0108604188_p0625201813356"></a><a name="zh-cn_topic_0108604188_p0625201813356"></a>CAS Server端口</p>
</td>
<td class="cellrowborder" valign="top" width="59.64%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108604188_p186251918103513"><a name="zh-cn_topic_0108604188_p186251918103513"></a><a name="zh-cn_topic_0108604188_p186251918103513"></a>与FusionInsight对接的CAS Server的端口。</p>
</td>
<td class="cellrowborder" valign="top" width="18.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108604188_p4625131883518"><a name="zh-cn_topic_0108604188_p4625131883518"></a><a name="zh-cn_topic_0108604188_p4625131883518"></a>20009</p>
</td>
</tr>
<tr id="zh-cn_topic_0108604188_row10481934205911"><td class="cellrowborder" valign="top" width="21.740000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108604188_p1648133485913"><a name="zh-cn_topic_0108604188_p1648133485913"></a><a name="zh-cn_topic_0108604188_p1648133485913"></a>用户名</p>
</td>
<td class="cellrowborder" valign="top" width="59.64%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108604188_p15481183410599"><a name="zh-cn_topic_0108604188_p15481183410599"></a><a name="zh-cn_topic_0108604188_p15481183410599"></a>登录FusionInsight Manager平台的用户名。</p>
</td>
<td class="cellrowborder" valign="top" width="18.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108604188_p548163420594"><a name="zh-cn_topic_0108604188_p548163420594"></a><a name="zh-cn_topic_0108604188_p548163420594"></a>cdm</p>
</td>
</tr>
<tr id="zh-cn_topic_0108604188_row4905133519593"><td class="cellrowborder" valign="top" width="21.740000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108604188_p16905153517591"><a name="zh-cn_topic_0108604188_p16905153517591"></a><a name="zh-cn_topic_0108604188_p16905153517591"></a>密码</p>
</td>
<td class="cellrowborder" valign="top" width="59.64%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108604188_p199057357597"><a name="zh-cn_topic_0108604188_p199057357597"></a><a name="zh-cn_topic_0108604188_p199057357597"></a>FusionInsight Manager平台的密码。</p>
</td>
<td class="cellrowborder" valign="top" width="18.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108604188_p189057358594"><a name="zh-cn_topic_0108604188_p189057358594"></a><a name="zh-cn_topic_0108604188_p189057358594"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0108604188_row15485153518397"><td class="cellrowborder" valign="top" width="21.740000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108604188_p1562410194013"><a name="zh-cn_topic_0108604188_p1562410194013"></a><a name="zh-cn_topic_0108604188_p1562410194013"></a>认证类型</p>
</td>
<td class="cellrowborder" valign="top" width="59.64%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108604188_p1962419018404"><a name="zh-cn_topic_0108604188_p1962419018404"></a><a name="zh-cn_topic_0108604188_p1962419018404"></a>访问FusionInsight HD的认证类型。<a name="zh-cn_topic_0108604188_zh-cn_topic_0108275286_ul36245017400"></a><a name="zh-cn_topic_0108604188_zh-cn_topic_0108275286_ul36245017400"></a><ul id="zh-cn_topic_0108604188_zh-cn_topic_0108275286_ul36245017400"><li>SIMPLE：非安全模式选择Simple鉴权。</li><li>KERBEROS：安全模式选择Kerberos鉴权。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="18.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108604188_p106241018407"><a name="zh-cn_topic_0108604188_p106241018407"></a><a name="zh-cn_topic_0108604188_p106241018407"></a>KERBEROS</p>
</td>
</tr>
<tr id="zh-cn_topic_0108604188_row1589194554614"><td class="cellrowborder" valign="top" width="21.740000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108604188_p35787478463"><a name="zh-cn_topic_0108604188_p35787478463"></a><a name="zh-cn_topic_0108604188_p35787478463"></a>运行模式</p>
</td>
<td class="cellrowborder" valign="top" width="59.64%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108604188_p357864774616"><a name="zh-cn_topic_0108604188_p357864774616"></a><a name="zh-cn_topic_0108604188_p357864774616"></a>选择HBase连接的运行模式：</p>
<a name="zh-cn_topic_0108604188_ul2077619371261"></a><a name="zh-cn_topic_0108604188_ul2077619371261"></a><ul id="zh-cn_topic_0108604188_ul2077619371261"><li>EMBEDDED：连接实例与CDM运行在一起，该模式性能较好。</li><li>STANDALONE：连接实例运行在独立进程。如果CDM需要对接多个Hadoop数据源（MRS、Hadoop或CloudTable），并且既有KERBEROS认证模式又有SIMPLE认证模式，只能使用STANDALONE模式或者配置不同的Agent。</li><li>Agent：连接实例运行在Agent上。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="18.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108604188_p659412476461"><a name="zh-cn_topic_0108604188_p659412476461"></a><a name="zh-cn_topic_0108604188_p659412476461"></a>STANDALONE</p>
</td>
</tr>
</tbody>
</table>

## Apache HBase<a name="zh-cn_topic_0108604188_section690499173512"></a>

连接Apache Hadoop上的HBase数据源时，相关参数如[表3](#zh-cn_topic_0108604188_table49051917359)所示。

**表 3**  Apache HBase连接参数

<a name="zh-cn_topic_0108604188_table49051917359"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108604188_row1990717913513"><th class="cellrowborder" valign="top" width="20.4%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108604188_p1390869143515"><a name="zh-cn_topic_0108604188_p1390869143515"></a><a name="zh-cn_topic_0108604188_p1390869143515"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="56.86%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108604188_p7909149183510"><a name="zh-cn_topic_0108604188_p7909149183510"></a><a name="zh-cn_topic_0108604188_p7909149183510"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="22.74%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108604188_p591059133516"><a name="zh-cn_topic_0108604188_p591059133516"></a><a name="zh-cn_topic_0108604188_p591059133516"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108604188_row1391259163511"><td class="cellrowborder" valign="top" width="20.4%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108604188_p0913139163519"><a name="zh-cn_topic_0108604188_p0913139163519"></a><a name="zh-cn_topic_0108604188_p0913139163519"></a>名称</p>
</td>
<td class="cellrowborder" valign="top" width="56.86%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108604188_p1369564463813"><a name="zh-cn_topic_0108604188_p1369564463813"></a><a name="zh-cn_topic_0108604188_p1369564463813"></a>连接的名称，根据连接的数据源类型，用户可自定义便于记忆、区分的连接名。</p>
</td>
<td class="cellrowborder" valign="top" width="22.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108604188_p5919292355"><a name="zh-cn_topic_0108604188_p5919292355"></a><a name="zh-cn_topic_0108604188_p5919292355"></a>hadoop_hbase_link</p>
</td>
</tr>
<tr id="zh-cn_topic_0108604188_row1191969203511"><td class="cellrowborder" valign="top" width="20.4%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108604188_p29204953520"><a name="zh-cn_topic_0108604188_p29204953520"></a><a name="zh-cn_topic_0108604188_p29204953520"></a>URI</p>
</td>
<td class="cellrowborder" valign="top" width="56.86%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108604188_p13924149173517"><a name="zh-cn_topic_0108604188_p13924149173517"></a><a name="zh-cn_topic_0108604188_p13924149173517"></a>表示NameNode URI地址。</p>
</td>
<td class="cellrowborder" valign="top" width="22.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108604188_p15245145210401"><a name="zh-cn_topic_0108604188_p15245145210401"></a><a name="zh-cn_topic_0108604188_p15245145210401"></a>hdfs://nn1.example.com/</p>
</td>
</tr>
<tr id="zh-cn_topic_0108604188_row49250918352"><td class="cellrowborder" valign="top" width="20.4%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108604188_p189268910357"><a name="zh-cn_topic_0108604188_p189268910357"></a><a name="zh-cn_topic_0108604188_p189268910357"></a>认证类型</p>
</td>
<td class="cellrowborder" valign="top" width="56.86%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108604188_p18927139153518"><a name="zh-cn_topic_0108604188_p18927139153518"></a><a name="zh-cn_topic_0108604188_p18927139153518"></a>访问Hadoop的认证类型。<a name="zh-cn_topic_0108604188_zh-cn_topic_0108275286_ul119271496357"></a><a name="zh-cn_topic_0108604188_zh-cn_topic_0108275286_ul119271496357"></a><ul id="zh-cn_topic_0108604188_zh-cn_topic_0108275286_ul119271496357"><li>SIMPLE：非安全模式Hadoop选择Simple鉴权。</li><li>KERBEROS：安全模式Hadoop选择Kerberos鉴权，通过获取客户端的principal和keytab文件在应用程序中进行认证。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="22.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108604188_p109305910356"><a name="zh-cn_topic_0108604188_p109305910356"></a><a name="zh-cn_topic_0108604188_p109305910356"></a>KERBEROS</p>
</td>
</tr>
<tr id="zh-cn_topic_0108604188_row1893111911354"><td class="cellrowborder" valign="top" width="20.4%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108604188_p59321897351"><a name="zh-cn_topic_0108604188_p59321897351"></a><a name="zh-cn_topic_0108604188_p59321897351"></a>Principal</p>
</td>
<td class="cellrowborder" valign="top" width="56.86%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108604188_p8933492358"><a name="zh-cn_topic_0108604188_p8933492358"></a><a name="zh-cn_topic_0108604188_p8933492358"></a>选择Kerberos鉴权时，用于认证的帐号Principal，您可以联系Hadoop管理员获取此帐号。</p>
</td>
<td class="cellrowborder" valign="top" width="22.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108604188_p159349920353"><a name="zh-cn_topic_0108604188_p159349920353"></a><a name="zh-cn_topic_0108604188_p159349920353"></a>USER@YOUR-REALM.COM</p>
</td>
</tr>
<tr id="zh-cn_topic_0108604188_row179341997352"><td class="cellrowborder" valign="top" width="20.4%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108604188_p1193512917358"><a name="zh-cn_topic_0108604188_p1193512917358"></a><a name="zh-cn_topic_0108604188_p1193512917358"></a>Keytab文件</p>
</td>
<td class="cellrowborder" valign="top" width="56.86%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108604188_p2935189143517"><a name="zh-cn_topic_0108604188_p2935189143517"></a><a name="zh-cn_topic_0108604188_p2935189143517"></a>选择Kerberos鉴权时，用于认证的Keytab文件，您可以联系Hadoop管理员获取此文件。</p>
</td>
<td class="cellrowborder" valign="top" width="22.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108604188_p135421727850"><a name="zh-cn_topic_0108604188_p135421727850"></a><a name="zh-cn_topic_0108604188_p135421727850"></a>/opt/user.keytab</p>
</td>
</tr>
<tr id="zh-cn_topic_0108604188_row399825032313"><td class="cellrowborder" valign="top" width="20.4%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108604188_p8915181018541"><a name="zh-cn_topic_0108604188_p8915181018541"></a><a name="zh-cn_topic_0108604188_p8915181018541"></a>IP与主机名映射</p>
</td>
<td class="cellrowborder" valign="top" width="56.86%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108604188_p791561045418"><a name="zh-cn_topic_0108604188_p791561045418"></a><a name="zh-cn_topic_0108604188_p791561045418"></a>如果配置文件使用主机名，需要配置IP与主机的映射。格式：IP与主机名之间使用空格分隔，多对映射使用分号或回车换行分隔。</p>
</td>
<td class="cellrowborder" valign="top" width="22.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108604188_p17915181012548"><a name="zh-cn_topic_0108604188_p17915181012548"></a><a name="zh-cn_topic_0108604188_p17915181012548"></a>10.3.6.9 hostname01</p>
<p id="zh-cn_topic_0108604188_p2011684813202"><a name="zh-cn_topic_0108604188_p2011684813202"></a><a name="zh-cn_topic_0108604188_p2011684813202"></a>10.4.7.9 hostname02</p>
</td>
</tr>
<tr id="zh-cn_topic_0108604188_row71073549237"><td class="cellrowborder" valign="top" width="20.4%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108604188_p174517362557"><a name="zh-cn_topic_0108604188_p174517362557"></a><a name="zh-cn_topic_0108604188_p174517362557"></a>运行模式</p>
</td>
<td class="cellrowborder" valign="top" width="56.86%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108604188_p693111135543"><a name="zh-cn_topic_0108604188_p693111135543"></a><a name="zh-cn_topic_0108604188_p693111135543"></a>选择HBase连接的运行模式：</p>
<a name="zh-cn_topic_0108604188_ul17131159112611"></a><a name="zh-cn_topic_0108604188_ul17131159112611"></a><ul id="zh-cn_topic_0108604188_ul17131159112611"><li>EMBEDDED：连接实例与CDM运行在一起，该模式性能较好。</li><li>STANDALONE：连接实例运行在独立进程。如果CDM需要对接多个Hadoop数据源（MRS、Hadoop或CloudTable），并且既有KERBEROS认证模式又有SIMPLE认证模式，只能使用STANDALONE模式或者配置不同的Agent。</li><li>Agent：连接实例运行在Agent上。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="22.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108604188_p15931141318544"><a name="zh-cn_topic_0108604188_p15931141318544"></a><a name="zh-cn_topic_0108604188_p15931141318544"></a>STANDALONE</p>
</td>
</tr>
</tbody>
</table>

