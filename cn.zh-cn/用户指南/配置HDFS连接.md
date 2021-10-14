# 配置HDFS连接<a name="dgc_01_0040"></a>

目前CDM支持连接的HDFS数据源有以下几种：

-   [MRS HDFS](#zh-cn_topic_0108275286_section127371747103314)
-   [FusionInsight HDFS](#zh-cn_topic_0108275286_section1851831133416)
-   [Apache HDFS](#zh-cn_topic_0108275286_section690499173512)

## MRS HDFS<a name="zh-cn_topic_0108275286_section127371747103314"></a>

连接MRS上的HDFS数据源时，相关参数如[表1](#zh-cn_topic_0108275286_table6441152003419)所示。

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   新建MRS连接前，需在MRS中添加一个kerberos认证用户并登录MRS管理页面更新其初始密码，然后使用该新建用户创建MRS连接。
>-   如需连接MRS 2.x版本的集群，请先创建2.x版本的CDM集群。CDM 1.8.x版本的集群无法连接MRS 2.x版本的集群。
>-   需确保MRS集群和DGC实例之间网络互通，网络互通需满足如下条件：
>-   DGC实例（指DGC实例中的批量数据迁移集群）与MRS集群处于不同区域的情况下，需要通过公网或者专线打通网络。
>-   DGC实例（指DGC实例中的批量数据迁移集群）与MRS集群同区域情况下，同虚拟私有云、同子网、同安全组的不同实例默认网络互通；如果同虚拟私有云但子网或安全组不同，还需配置路由规则及安全组规则，配置路由规则请参见[如何配置路由规则](https://support.huaweicloud.com/bestpractice-vpc/bestpractice_0009.html#bestpractice_0009__zh-cn_topic_0252060877_li16617547103419)章节，配置安全组规则请参见[如何配置安全组规则](https://support.huaweicloud.com/usermanual-ecs/zh-cn_topic_0140323152.html)章节。
>-   此外，还需确保该MRS集群与DGC工作空间所属的企业项目相同，如果不同，您需要修改工作空间的企业项目。

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
<td class="cellrowborder" valign="top" width="57.720000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p1345602010341"><a name="zh-cn_topic_0108275286_p1345602010341"></a><a name="zh-cn_topic_0108275286_p1345602010341"></a>MRS Manager的浮动IP地址，可以单击输入框后的<span class="uicontrol" id="zh-cn_topic_0108275286_uicontrol926725316310"><a name="zh-cn_topic_0108275286_uicontrol926725316310"></a><a name="zh-cn_topic_0108275286_uicontrol926725316310"></a>“选择”</span>来选定已创建的MRS集群，CDM会自动填充下面的鉴权参数。</p>
</td>
<td class="cellrowborder" valign="top" width="21.77%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p13456420143418"><a name="zh-cn_topic_0108275286_p13456420143418"></a><a name="zh-cn_topic_0108275286_p13456420143418"></a>127.0.0.1</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row16456152011347"><td class="cellrowborder" valign="top" width="20.51%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p94561620113420"><a name="zh-cn_topic_0108275286_p94561620113420"></a><a name="zh-cn_topic_0108275286_p94561620113420"></a>用户名</p>
</td>
<td class="cellrowborder" valign="top" width="57.720000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p64738206349"><a name="zh-cn_topic_0108275286_p64738206349"></a><a name="zh-cn_topic_0108275286_p64738206349"></a>选择KERBEROS鉴权时，需要配置MRS Manager的用户名和密码。从HDFS导出目录时，如果需要创建快照，这里配置的用户需要HDFS系统的管理员权限。</p>
<div class="p" id="zh-cn_topic_0108275286_p194519141759"><a name="zh-cn_topic_0108275286_p194519141759"></a><a name="zh-cn_topic_0108275286_p194519141759"></a>如果要创建MRS安全集群的数据连接，不能使用admin用户。因为admin用户是默认的管理页面用户，这个用户无法作为安全集群的认证用户来使用。您可以创建一个新的MRS用户，然后在创建MRS数据连接时，<span class="parmname" id="zh-cn_topic_0108275286_zh-cn_topic_0108618545_dgc_01_0009_parmname3468191262313"><a name="zh-cn_topic_0108275286_zh-cn_topic_0108618545_dgc_01_0009_parmname3468191262313"></a><a name="zh-cn_topic_0108275286_zh-cn_topic_0108618545_dgc_01_0009_parmname3468191262313"></a>“用户名”</span>和<span class="parmname" id="zh-cn_topic_0108275286_zh-cn_topic_0108618545_dgc_01_0009_parmname64683124231"><a name="zh-cn_topic_0108275286_zh-cn_topic_0108618545_dgc_01_0009_parmname64683124231"></a><a name="zh-cn_topic_0108275286_zh-cn_topic_0108618545_dgc_01_0009_parmname64683124231"></a>“密码”</span>填写为新建的MRS用户及其密码。<div class="note" id="zh-cn_topic_0108275286_zh-cn_topic_0108618545_note15451659151217"><a name="zh-cn_topic_0108275286_zh-cn_topic_0108618545_note15451659151217"></a><a name="zh-cn_topic_0108275286_zh-cn_topic_0108618545_note15451659151217"></a><span class="notetitle"> 说明： </span><div class="notebody"><a name="zh-cn_topic_0108275286_zh-cn_topic_0108618545_ul17715141011134"></a><a name="zh-cn_topic_0108275286_zh-cn_topic_0108618545_ul17715141011134"></a><ul id="zh-cn_topic_0108275286_zh-cn_topic_0108618545_ul17715141011134"><li>如果CDM集群为2.9.0版本及之后版本，且MRS集群为3.1.0及之后版本，则所创建的用户至少需具备Manager_viewer的角色权限才能在CDM创建连接；如果需要对应组件的进行库、表、数据的操作，还需要添加对应组件的用户组权限。</li><li>如果CDM集群为2.9.0之前的版本，或MRS集群为3.1.0之前的版本，则所创建的用户需要具备Manager_administrator或System_administrator权限，才能在CDM创建连接。</li><li>仅具备Manager_tenant或Manager_auditor权限，无法创建连接。</li></ul>
</div></div>
</div>
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
<tr id="zh-cn_topic_0108275286_row7856101034511"><td class="cellrowborder" valign="top" width="20.51%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p7622317114514"><a name="zh-cn_topic_0108275286_p7622317114514"></a><a name="zh-cn_topic_0108275286_p7622317114514"></a>认证类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.720000000000006%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108275286_p13355246182213"><a name="zh-cn_topic_0108275286_p13355246182213"></a><a name="zh-cn_topic_0108275286_p13355246182213"></a>访问MRS的认证类型：<a name="zh-cn_topic_0108275286_zh-cn_topic_0108618545_ul12623191718453"></a><a name="zh-cn_topic_0108275286_zh-cn_topic_0108618545_ul12623191718453"></a><ul id="zh-cn_topic_0108275286_zh-cn_topic_0108618545_ul12623191718453"><li>SIMPLE：非安全模式选择Simple鉴权。</li><li>KERBEROS：安全模式选择Kerberos鉴权。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="21.77%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p662311175459"><a name="zh-cn_topic_0108275286_p662311175459"></a><a name="zh-cn_topic_0108275286_p662311175459"></a>SIMPLE</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row10211145833913"><td class="cellrowborder" valign="top" width="20.51%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p721185823920"><a name="zh-cn_topic_0108275286_p721185823920"></a><a name="zh-cn_topic_0108275286_p721185823920"></a>运行模式</p>
</td>
<td class="cellrowborder" valign="top" width="57.720000000000006%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108275286_p206752056145718"><a name="zh-cn_topic_0108275286_p206752056145718"></a><a name="zh-cn_topic_0108275286_p206752056145718"></a>选择HDFS连接的运行模式：<a name="zh-cn_topic_0108275286_ul1747017597574"></a><a name="zh-cn_topic_0108275286_ul1747017597574"></a><ul id="zh-cn_topic_0108275286_ul1747017597574"><li>EMBEDDED：连接实例与CDM运行在一起，该模式性能较好。</li><li>STANDALONE：连接实例运行在独立进程。如果CDM需要对接多个Hadoop数据源（MRS、Hadoop或CloudTable），并且既有KERBEROS认证模式又有SIMPLE认证模式，只能使用STANDALONE模式或者配置不同的Agent。<p id="zh-cn_topic_0108275286_p8792217159"><a name="zh-cn_topic_0108275286_p8792217159"></a><a name="zh-cn_topic_0108275286_p8792217159"></a><strong id="zh-cn_topic_0108275286_b1446022218189"><a name="zh-cn_topic_0108275286_b1446022218189"></a><a name="zh-cn_topic_0108275286_b1446022218189"></a>说明</strong>：STANDALONE模式主要是用来解决版本冲突问题的运行模式。当同一种数据连接的源端或者目的端连接器的版本不一致时，存在jar包冲突的情况，这时需要将源端或目的端放在STANDALONE进程里，防止冲突导致迁移失败。</p>
</li><li>Agent：连接实例运行在Agent上。</li></ul>
</div>
<p id="zh-cn_topic_0108275286_p192253613346"><a name="zh-cn_topic_0108275286_p192253613346"></a><a name="zh-cn_topic_0108275286_p192253613346"></a>若不使用AGENT运行模式，且在一个CDM中同时连接两个及以上开启Kerberos认证且realm相同的集群，只能使用EMBEDDED运行模式连接其中一个集群，其余需使用STANDALONE。</p>
</td>
<td class="cellrowborder" valign="top" width="21.77%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p1021155811394"><a name="zh-cn_topic_0108275286_p1021155811394"></a><a name="zh-cn_topic_0108275286_p1021155811394"></a>STANDALONE</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row1946581311414"><td class="cellrowborder" valign="top" width="20.51%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p1999031319386"><a name="zh-cn_topic_0108275286_p1999031319386"></a><a name="zh-cn_topic_0108275286_p1999031319386"></a>Agent</p>
</td>
<td class="cellrowborder" valign="top" width="57.720000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p5412193413515"><a name="zh-cn_topic_0108275286_p5412193413515"></a><a name="zh-cn_topic_0108275286_p5412193413515"></a>单击<span class="uicontrol" id="zh-cn_topic_0108275286_uicontrol7592322128"><a name="zh-cn_topic_0108275286_uicontrol7592322128"></a><a name="zh-cn_topic_0108275286_uicontrol7592322128"></a>“选择”</span>，选择<a href="管理Agent.md#zh-cn_topic_0207402273_zh-cn_topic_0191978474_section1072083564713">连接Agent</a>中已创建的Agent。运行模式选择Agent时显示此参数。</p>
</td>
<td class="cellrowborder" valign="top" width="21.77%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p1499013137381"><a name="zh-cn_topic_0108275286_p1499013137381"></a><a name="zh-cn_topic_0108275286_p1499013137381"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row153901628202511"><td class="cellrowborder" valign="top" width="20.51%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p1205102763015"><a name="zh-cn_topic_0108275286_p1205102763015"></a><a name="zh-cn_topic_0108275286_p1205102763015"></a>是否使用集群配置</p>
</td>
<td class="cellrowborder" valign="top" width="57.720000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p3791105013307"><a name="zh-cn_topic_0108275286_p3791105013307"></a><a name="zh-cn_topic_0108275286_p3791105013307"></a>您可以通过使用集群配置，简化Hadoop连接参数配置。</p>
</td>
<td class="cellrowborder" valign="top" width="21.77%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p147705512305"><a name="zh-cn_topic_0108275286_p147705512305"></a><a name="zh-cn_topic_0108275286_p147705512305"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row19389228162513"><td class="cellrowborder" valign="top" width="20.51%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p1713125033015"><a name="zh-cn_topic_0108275286_p1713125033015"></a><a name="zh-cn_topic_0108275286_p1713125033015"></a>集群配置名</p>
</td>
<td class="cellrowborder" valign="top" width="57.720000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p1171175111302"><a name="zh-cn_topic_0108275286_p1171175111302"></a><a name="zh-cn_topic_0108275286_p1171175111302"></a>仅当“是否使用集群配置”为“是”时，此参数有效。此参数用于选择用户已经创建好的集群配置。</p>
<p id="zh-cn_topic_0108275286_p192211597367"><a name="zh-cn_topic_0108275286_p192211597367"></a><a name="zh-cn_topic_0108275286_p192211597367"></a>集群配置的创建方法请参见<a href="管理集群配置.md#dgc_01_1096">管理集群配置</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="21.77%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p0147252193019"><a name="zh-cn_topic_0108275286_p0147252193019"></a><a name="zh-cn_topic_0108275286_p0147252193019"></a>hdfs_01</p>
</td>
</tr>
</tbody>
</table>

单击“显示高级属性“，然后单击“添加“，您可以添加客户端的配置属性。所添加的每个属性需配置属性名称和值。对于不再需要的属性，可单击属性后的“删除“按钮进行删除。

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
<td class="cellrowborder" valign="top" width="57.97%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108275286_p12185184611567"><a name="zh-cn_topic_0108275286_p12185184611567"></a><a name="zh-cn_topic_0108275286_p12185184611567"></a>访问集群的认证类型：<a name="zh-cn_topic_0108275286_ul193521539183819"></a><a name="zh-cn_topic_0108275286_ul193521539183819"></a><ul id="zh-cn_topic_0108275286_ul193521539183819"><li>SIMPLE：非安全模式选择Simple鉴权。</li><li>KERBEROS：安全模式选择Kerberos鉴权。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="21.29%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p106241018407"><a name="zh-cn_topic_0108275286_p106241018407"></a><a name="zh-cn_topic_0108275286_p106241018407"></a>KERBEROS</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row129026915554"><td class="cellrowborder" valign="top" width="20.74%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p1418522311554"><a name="zh-cn_topic_0108275286_p1418522311554"></a><a name="zh-cn_topic_0108275286_p1418522311554"></a>运行模式</p>
</td>
<td class="cellrowborder" valign="top" width="57.97%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108275286_p1990239195518"><a name="zh-cn_topic_0108275286_p1990239195518"></a><a name="zh-cn_topic_0108275286_p1990239195518"></a>选择HDFS连接的运行模式：<a name="zh-cn_topic_0108275286_zh-cn_topic_0108275286_ul1747017597574"></a><a name="zh-cn_topic_0108275286_zh-cn_topic_0108275286_ul1747017597574"></a><ul id="zh-cn_topic_0108275286_zh-cn_topic_0108275286_ul1747017597574"><li>EMBEDDED：连接实例与CDM运行在一起，该模式性能较好。</li><li>STANDALONE：连接实例运行在独立进程。如果CDM需要对接多个Hadoop数据源（MRS、Hadoop或CloudTable），并且既有KERBEROS认证模式又有SIMPLE认证模式，只能使用STANDALONE模式或者配置不同的Agent。<p id="zh-cn_topic_0108275286_zh-cn_topic_0108275286_p8792217159"><a name="zh-cn_topic_0108275286_zh-cn_topic_0108275286_p8792217159"></a><a name="zh-cn_topic_0108275286_zh-cn_topic_0108275286_p8792217159"></a><strong id="zh-cn_topic_0108275286_zh-cn_topic_0108275286_b1446022218189"><a name="zh-cn_topic_0108275286_zh-cn_topic_0108275286_b1446022218189"></a><a name="zh-cn_topic_0108275286_zh-cn_topic_0108275286_b1446022218189"></a>说明</strong>：STANDALONE模式主要是用来解决版本冲突问题的运行模式。当同一种数据连接的源端或者目的端连接器的版本不一致时，存在jar包冲突的情况，这时需要将源端或目的端放在STANDALONE进程里，防止冲突导致迁移失败。</p>
</li><li>Agent：连接实例运行在Agent上。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="21.29%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p18902892555"><a name="zh-cn_topic_0108275286_p18902892555"></a><a name="zh-cn_topic_0108275286_p18902892555"></a>STANDALONE</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row5249204817429"><td class="cellrowborder" valign="top" width="20.74%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p10250104844219"><a name="zh-cn_topic_0108275286_p10250104844219"></a><a name="zh-cn_topic_0108275286_p10250104844219"></a>Agent</p>
</td>
<td class="cellrowborder" valign="top" width="57.97%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p1425064819422"><a name="zh-cn_topic_0108275286_p1425064819422"></a><a name="zh-cn_topic_0108275286_p1425064819422"></a>单击<span class="uicontrol" id="zh-cn_topic_0108275286_zh-cn_topic_0108275286_uicontrol7592322128"><a name="zh-cn_topic_0108275286_zh-cn_topic_0108275286_uicontrol7592322128"></a><a name="zh-cn_topic_0108275286_zh-cn_topic_0108275286_uicontrol7592322128"></a>“选择”</span>，选择<a href="管理Agent.md#zh-cn_topic_0207402273_zh-cn_topic_0191978474_section1072083564713">连接Agent</a>中已创建的Agent。运行模式选择Agent时显示此参数。</p>
</td>
<td class="cellrowborder" valign="top" width="21.29%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p13250648124212"><a name="zh-cn_topic_0108275286_p13250648124212"></a><a name="zh-cn_topic_0108275286_p13250648124212"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row566014278278"><td class="cellrowborder" valign="top" width="20.74%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p15646727112718"><a name="zh-cn_topic_0108275286_p15646727112718"></a><a name="zh-cn_topic_0108275286_p15646727112718"></a>是否使用集群配置</p>
</td>
<td class="cellrowborder" valign="top" width="57.97%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p1664652719273"><a name="zh-cn_topic_0108275286_p1664652719273"></a><a name="zh-cn_topic_0108275286_p1664652719273"></a>您可以通过使用集群配置，简化Hadoop连接参数配置。</p>
</td>
<td class="cellrowborder" valign="top" width="21.29%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p156469276274"><a name="zh-cn_topic_0108275286_p156469276274"></a><a name="zh-cn_topic_0108275286_p156469276274"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row12659162762719"><td class="cellrowborder" valign="top" width="20.74%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p1764662782719"><a name="zh-cn_topic_0108275286_p1764662782719"></a><a name="zh-cn_topic_0108275286_p1764662782719"></a>集群配置名</p>
</td>
<td class="cellrowborder" valign="top" width="57.97%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p16646142715274"><a name="zh-cn_topic_0108275286_p16646142715274"></a><a name="zh-cn_topic_0108275286_p16646142715274"></a>仅当“是否使用集群配置”为“是”时，此参数有效。此参数用于选择用户已经创建好的集群配置。</p>
<p id="zh-cn_topic_0108275286_p146461327142719"><a name="zh-cn_topic_0108275286_p146461327142719"></a><a name="zh-cn_topic_0108275286_p146461327142719"></a>集群配置的创建方法请参见<a href="管理集群配置.md#dgc_01_1096">管理集群配置</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="21.29%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p76468275271"><a name="zh-cn_topic_0108275286_p76468275271"></a><a name="zh-cn_topic_0108275286_p76468275271"></a>hdfs_01</p>
</td>
</tr>
</tbody>
</table>

单击“显示高级属性“，然后单击“添加“，您可以添加客户端的配置属性。所添加的每个属性需配置属性名称和值。对于不再需要的属性，可单击属性后的“删除“按钮进行删除。

## Apache HDFS<a name="zh-cn_topic_0108275286_section690499173512"></a>

连接Apache Hadoop上的HDFS数据源时，相关参数如[表3](#zh-cn_topic_0108275286_table49051917359)所示。

**表 3**  Apache HDFS连接参数

<a name="zh-cn_topic_0108275286_table49051917359"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108275286_row1990717913513"><th class="cellrowborder" valign="top" width="21.060000000000002%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108275286_p1390869143515"><a name="zh-cn_topic_0108275286_p1390869143515"></a><a name="zh-cn_topic_0108275286_p1390869143515"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="57.98%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108275286_p7909149183510"><a name="zh-cn_topic_0108275286_p7909149183510"></a><a name="zh-cn_topic_0108275286_p7909149183510"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="20.96%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108275286_p591059133516"><a name="zh-cn_topic_0108275286_p591059133516"></a><a name="zh-cn_topic_0108275286_p591059133516"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108275286_row1391259163511"><td class="cellrowborder" valign="top" width="21.060000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p0913139163519"><a name="zh-cn_topic_0108275286_p0913139163519"></a><a name="zh-cn_topic_0108275286_p0913139163519"></a>名称</p>
</td>
<td class="cellrowborder" valign="top" width="57.98%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p1369564463813"><a name="zh-cn_topic_0108275286_p1369564463813"></a><a name="zh-cn_topic_0108275286_p1369564463813"></a>连接的名称，根据连接的数据源类型，用户可自定义便于记忆、区分的连接名。</p>
</td>
<td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p5919292355"><a name="zh-cn_topic_0108275286_p5919292355"></a><a name="zh-cn_topic_0108275286_p5919292355"></a>hadoop_hdfs_link</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row1191969203511"><td class="cellrowborder" valign="top" width="21.060000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p29204953520"><a name="zh-cn_topic_0108275286_p29204953520"></a><a name="zh-cn_topic_0108275286_p29204953520"></a>URI</p>
</td>
<td class="cellrowborder" valign="top" width="57.98%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p13924149173517"><a name="zh-cn_topic_0108275286_p13924149173517"></a><a name="zh-cn_topic_0108275286_p13924149173517"></a>表示NameNode URI地址。</p>
</td>
<td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p15245145210401"><a name="zh-cn_topic_0108275286_p15245145210401"></a><a name="zh-cn_topic_0108275286_p15245145210401"></a>hdfs://nn1.example.com/</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row49250918352"><td class="cellrowborder" valign="top" width="21.060000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p189268910357"><a name="zh-cn_topic_0108275286_p189268910357"></a><a name="zh-cn_topic_0108275286_p189268910357"></a>认证类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.98%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108275286_p17606125316569"><a name="zh-cn_topic_0108275286_p17606125316569"></a><a name="zh-cn_topic_0108275286_p17606125316569"></a>访问集群的认证类型：<a name="zh-cn_topic_0108275286_zh-cn_topic_0108275286_ul193521539183819"></a><a name="zh-cn_topic_0108275286_zh-cn_topic_0108275286_ul193521539183819"></a><ul id="zh-cn_topic_0108275286_zh-cn_topic_0108275286_ul193521539183819"><li>SIMPLE：非安全模式选择Simple鉴权。</li><li>KERBEROS：安全模式选择Kerberos鉴权。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p109305910356"><a name="zh-cn_topic_0108275286_p109305910356"></a><a name="zh-cn_topic_0108275286_p109305910356"></a>KERBEROS</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row176991243103216"><td class="cellrowborder" valign="top" width="21.060000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p1754151515313"><a name="zh-cn_topic_0108275286_p1754151515313"></a><a name="zh-cn_topic_0108275286_p1754151515313"></a>Principal</p>
</td>
<td class="cellrowborder" valign="top" width="57.98%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p1224139143111"><a name="zh-cn_topic_0108275286_p1224139143111"></a><a name="zh-cn_topic_0108275286_p1224139143111"></a>认证类型为“KERBEROS”时，需要填写Principal。Principal即Kerberos安全模式下的用户名，可以联系Hadoop管理员获取。此处填写的Principal需要与Keytab文件保持一致。</p>
</td>
<td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p0483184663113"><a name="zh-cn_topic_0108275286_p0483184663113"></a><a name="zh-cn_topic_0108275286_p0483184663113"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row385893819326"><td class="cellrowborder" valign="top" width="21.060000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p1232143803114"><a name="zh-cn_topic_0108275286_p1232143803114"></a><a name="zh-cn_topic_0108275286_p1232143803114"></a>Keytab文件</p>
</td>
<td class="cellrowborder" valign="top" width="57.98%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p178963963114"><a name="zh-cn_topic_0108275286_p178963963114"></a><a name="zh-cn_topic_0108275286_p178963963114"></a>认证类型为“KERBEROS”时，需要上传Keytab文件。Keytab文件为认证凭据文件，可以联系Hadoop管理员获取。获取Keytab文件前，需要在集群上至少修改过一次此用户的密码，否则下载获取的keytab文件可能无法使用。另外，修改用户密码后，之前导出的keytab将失效，需要重新导出。</p>
</td>
<td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p578521710314"><a name="zh-cn_topic_0108275286_p578521710314"></a><a name="zh-cn_topic_0108275286_p578521710314"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row693151312543"><td class="cellrowborder" valign="top" width="21.060000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p174517362557"><a name="zh-cn_topic_0108275286_p174517362557"></a><a name="zh-cn_topic_0108275286_p174517362557"></a>运行模式</p>
</td>
<td class="cellrowborder" valign="top" width="57.98%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108275286_p693111135543"><a name="zh-cn_topic_0108275286_p693111135543"></a><a name="zh-cn_topic_0108275286_p693111135543"></a>选择HDFS连接的运行模式：<a name="zh-cn_topic_0108275286_zh-cn_topic_0108275286_ul1747017597574_1"></a><a name="zh-cn_topic_0108275286_zh-cn_topic_0108275286_ul1747017597574_1"></a><ul id="zh-cn_topic_0108275286_zh-cn_topic_0108275286_ul1747017597574_1"><li>EMBEDDED：连接实例与CDM运行在一起，该模式性能较好。</li><li>STANDALONE：连接实例运行在独立进程。如果CDM需要对接多个Hadoop数据源（MRS、Hadoop或CloudTable），并且既有KERBEROS认证模式又有SIMPLE认证模式，只能使用STANDALONE模式或者配置不同的Agent。<p id="zh-cn_topic_0108275286_zh-cn_topic_0108275286_p8792217159_1"><a name="zh-cn_topic_0108275286_zh-cn_topic_0108275286_p8792217159_1"></a><a name="zh-cn_topic_0108275286_zh-cn_topic_0108275286_p8792217159_1"></a><strong id="zh-cn_topic_0108275286_zh-cn_topic_0108275286_b1446022218189_1"><a name="zh-cn_topic_0108275286_zh-cn_topic_0108275286_b1446022218189_1"></a><a name="zh-cn_topic_0108275286_zh-cn_topic_0108275286_b1446022218189_1"></a>说明</strong>：STANDALONE模式主要是用来解决版本冲突问题的运行模式。当同一种数据连接的源端或者目的端连接器的版本不一致时，存在jar包冲突的情况，这时需要将源端或目的端放在STANDALONE进程里，防止冲突导致迁移失败。</p>
</li><li>Agent：连接实例运行在Agent上。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p15931141318544"><a name="zh-cn_topic_0108275286_p15931141318544"></a><a name="zh-cn_topic_0108275286_p15931141318544"></a>STANDALONE</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row94271058105817"><td class="cellrowborder" valign="top" width="21.060000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p1137218565914"><a name="zh-cn_topic_0108275286_p1137218565914"></a><a name="zh-cn_topic_0108275286_p1137218565914"></a>IP与主机名映射</p>
</td>
<td class="cellrowborder" valign="top" width="57.98%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p176403238592"><a name="zh-cn_topic_0108275286_p176403238592"></a><a name="zh-cn_topic_0108275286_p176403238592"></a>运行模式选择<span class="parmvalue" id="zh-cn_topic_0108275286_parmvalue13882955125917"><a name="zh-cn_topic_0108275286_parmvalue13882955125917"></a><a name="zh-cn_topic_0108275286_parmvalue13882955125917"></a>“EMBEDDED”</span>、<span class="parmvalue" id="zh-cn_topic_0108275286_parmvalue19890135714596"><a name="zh-cn_topic_0108275286_parmvalue19890135714596"></a><a name="zh-cn_topic_0108275286_parmvalue19890135714596"></a>“STANDALONE”</span>时，该参数有效。</p>
<p id="zh-cn_topic_0108275286_p113721555592"><a name="zh-cn_topic_0108275286_p113721555592"></a><a name="zh-cn_topic_0108275286_p113721555592"></a>如果HDFS配置文件使用主机名，需要配置IP与主机的映射。格式：IP与主机名之间使用空格分隔，多对映射使用分号或回车换行分隔。</p>
</td>
<td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p937211525914"><a name="zh-cn_topic_0108275286_p937211525914"></a><a name="zh-cn_topic_0108275286_p937211525914"></a>10.1.6.9 hostname01</p>
<p id="zh-cn_topic_0108275286_p143727565914"><a name="zh-cn_topic_0108275286_p143727565914"></a><a name="zh-cn_topic_0108275286_p143727565914"></a>10.2.7.9 hostname02</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row13173134416"><td class="cellrowborder" valign="top" width="21.060000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p20303117444"><a name="zh-cn_topic_0108275286_p20303117444"></a><a name="zh-cn_topic_0108275286_p20303117444"></a>Agent</p>
</td>
<td class="cellrowborder" valign="top" width="57.98%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p461134915213"><a name="zh-cn_topic_0108275286_p461134915213"></a><a name="zh-cn_topic_0108275286_p461134915213"></a>运行模式选择<span class="parmvalue" id="zh-cn_topic_0108275286_parmvalue028412299585"><a name="zh-cn_topic_0108275286_parmvalue028412299585"></a><a name="zh-cn_topic_0108275286_parmvalue028412299585"></a>“Agent”</span>时，单击<span class="uicontrol" id="zh-cn_topic_0108275286_zh-cn_topic_0108275286_uicontrol7592322128_1"><a name="zh-cn_topic_0108275286_zh-cn_topic_0108275286_uicontrol7592322128_1"></a><a name="zh-cn_topic_0108275286_zh-cn_topic_0108275286_uicontrol7592322128_1"></a>“选择”</span>，选择<a href="管理Agent.md#zh-cn_topic_0207402273_zh-cn_topic_0191978474_section1072083564713">连接Agent</a>中已创建的Agent。</p>
</td>
<td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p123193116445"><a name="zh-cn_topic_0108275286_p123193116445"></a><a name="zh-cn_topic_0108275286_p123193116445"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row3301111432916"><td class="cellrowborder" valign="top" width="21.060000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p2029911417295"><a name="zh-cn_topic_0108275286_p2029911417295"></a><a name="zh-cn_topic_0108275286_p2029911417295"></a>是否使用集群配置</p>
</td>
<td class="cellrowborder" valign="top" width="57.98%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p12991141296"><a name="zh-cn_topic_0108275286_p12991141296"></a><a name="zh-cn_topic_0108275286_p12991141296"></a>您可以通过使用集群配置，简化Hadoop连接参数配置。</p>
</td>
<td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p2029931402918"><a name="zh-cn_topic_0108275286_p2029931402918"></a><a name="zh-cn_topic_0108275286_p2029931402918"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275286_row9301151462916"><td class="cellrowborder" valign="top" width="21.060000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275286_p029911492914"><a name="zh-cn_topic_0108275286_p029911492914"></a><a name="zh-cn_topic_0108275286_p029911492914"></a>集群配置名</p>
</td>
<td class="cellrowborder" valign="top" width="57.98%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275286_p16299171492913"><a name="zh-cn_topic_0108275286_p16299171492913"></a><a name="zh-cn_topic_0108275286_p16299171492913"></a>仅当“是否使用集群配置”为“是”时，此参数有效。此参数用于选择用户已经创建好的集群配置。</p>
<p id="zh-cn_topic_0108275286_p20299121492914"><a name="zh-cn_topic_0108275286_p20299121492914"></a><a name="zh-cn_topic_0108275286_p20299121492914"></a>集群配置的创建方法请参见<a href="管理集群配置.md#dgc_01_1096">管理集群配置</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275286_p4299181416295"><a name="zh-cn_topic_0108275286_p4299181416295"></a><a name="zh-cn_topic_0108275286_p4299181416295"></a>hdfs_01</p>
</td>
</tr>
</tbody>
</table>

