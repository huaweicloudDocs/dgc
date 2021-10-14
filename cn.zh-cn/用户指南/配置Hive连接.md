# 配置Hive连接<a name="dgc_01_0026"></a>

目前CDM支持连接的Hive数据源有以下几种：

-   [MRS Hive](#zh-cn_topic_0108618545_section6335145774617)
-   [FusionInsight Hive](#zh-cn_topic_0108618545_section999517914488)
-   [Apache Hive](#zh-cn_topic_0108618545_section9585729145218)

## MRS Hive<a name="zh-cn_topic_0108618545_section6335145774617"></a>

用户具有MRS Hive连接的表的访问权限时，才能在字段映射时看到表。

MRS Hive连接适用于华为云上的MapReduce服务。MRS Hive的连接参数如[表1](#zh-cn_topic_0108618545_table111803819501)所示。

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   新建MRS连接前，需在MRS中添加一个kerberos认证用户并登录MRS管理页面更新其初始密码，然后使用该新建用户创建MRS连接。
>-   如需连接MRS 2.x版本的集群，请先创建2.x版本的CDM集群。CDM 1.8.x版本的集群无法连接MRS 2.x版本的集群。
>-   由于当前CDM Hive连接是从MRS HDFS组件获取core-site.xml配置信息，所以在MRS侧使用的是Hive over OBS场景时，在创建Hive连接前，需要用户在MRS管理界面的HDFS组件中配置OBS的AK、SK信息。
>-   需确保MRS集群和DGC实例之间网络互通，网络互通需满足如下条件：
>-   DGC实例（指DGC实例中的批量数据迁移集群）与MRS集群处于不同区域的情况下，需要通过公网或者专线打通网络。
>-   DGC实例（指DGC实例中的批量数据迁移集群）与MRS集群同区域情况下，同虚拟私有云、同子网、同安全组的不同实例默认网络互通；如果同虚拟私有云但子网或安全组不同，还需配置路由规则及安全组规则，配置路由规则请参见[如何配置路由规则](https://support.huaweicloud.com/bestpractice-vpc/bestpractice_0009.html#bestpractice_0009__zh-cn_topic_0252060877_li16617547103419)章节，配置安全组规则请参见[如何配置安全组规则](https://support.huaweicloud.com/usermanual-ecs/zh-cn_topic_0140323152.html)章节。
>-   此外，还需确保该MRS集群与DGC工作空间所属的企业项目相同，如果不同，您需要修改工作空间的企业项目。

**表 1**  MRS Hive连接参数

<a name="zh-cn_topic_0108618545_table111803819501"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108618545_row918111835015"><th class="cellrowborder" valign="top" width="16.72%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108618545_p111816835015"><a name="zh-cn_topic_0108618545_p111816835015"></a><a name="zh-cn_topic_0108618545_p111816835015"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="62.1%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108618545_p171813845018"><a name="zh-cn_topic_0108618545_p171813845018"></a><a name="zh-cn_topic_0108618545_p171813845018"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="21.18%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108618545_p8181198115015"><a name="zh-cn_topic_0108618545_p8181198115015"></a><a name="zh-cn_topic_0108618545_p8181198115015"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108618545_row151817815505"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p218198205013"><a name="zh-cn_topic_0108618545_p218198205013"></a><a name="zh-cn_topic_0108618545_p218198205013"></a>名称</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p5181487501"><a name="zh-cn_topic_0108618545_p5181487501"></a><a name="zh-cn_topic_0108618545_p5181487501"></a>连接的名称，根据连接的数据源类型，用户可自定义便于记忆、区分的连接名。</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p10181138135017"><a name="zh-cn_topic_0108618545_p10181138135017"></a><a name="zh-cn_topic_0108618545_p10181138135017"></a>hivelink</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row16181208165013"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p21818818506"><a name="zh-cn_topic_0108618545_p21818818506"></a><a name="zh-cn_topic_0108618545_p21818818506"></a>Manager IP</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p218148165010"><a name="zh-cn_topic_0108618545_p218148165010"></a><a name="zh-cn_topic_0108618545_p218148165010"></a>MRS Manager的浮动IP地址，可以单击输入框后的<span class="uicontrol" id="zh-cn_topic_0108618545_zh-cn_topic_0108275286_uicontrol926725316310"><a name="zh-cn_topic_0108618545_zh-cn_topic_0108275286_uicontrol926725316310"></a><a name="zh-cn_topic_0108618545_zh-cn_topic_0108275286_uicontrol926725316310"></a>“选择”</span>来选定已创建的MRS集群，CDM会自动填充下面的鉴权参数。</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p718110815509"><a name="zh-cn_topic_0108618545_p718110815509"></a><a name="zh-cn_topic_0108618545_p718110815509"></a>127.0.0.1</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row7181168105018"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p141816885017"><a name="zh-cn_topic_0108618545_p141816885017"></a><a name="zh-cn_topic_0108618545_p141816885017"></a>认证类型</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108618545_p11181148185017"><a name="zh-cn_topic_0108618545_p11181148185017"></a><a name="zh-cn_topic_0108618545_p11181148185017"></a>访问MRS的认证类型：<a name="zh-cn_topic_0108618545_ul12623191718453"></a><a name="zh-cn_topic_0108618545_ul12623191718453"></a><ul id="zh-cn_topic_0108618545_ul12623191718453"><li>SIMPLE：非安全模式选择Simple鉴权。</li><li>KERBEROS：安全模式选择Kerberos鉴权。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p818111819508"><a name="zh-cn_topic_0108618545_p818111819508"></a><a name="zh-cn_topic_0108618545_p818111819508"></a>SIMPLE</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row6181138195013"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p51811188500"><a name="zh-cn_topic_0108618545_p51811188500"></a><a name="zh-cn_topic_0108618545_p51811188500"></a>Hive版本</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p111811682501"><a name="zh-cn_topic_0108618545_p111811682501"></a><a name="zh-cn_topic_0108618545_p111811682501"></a>Hive的版本。根据服务端Hive版本设置。</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p191811987501"><a name="zh-cn_topic_0108618545_p191811987501"></a><a name="zh-cn_topic_0108618545_p191811987501"></a>HIVE_3_X</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row818110813502"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p1818118185015"><a name="zh-cn_topic_0108618545_p1818118185015"></a><a name="zh-cn_topic_0108618545_p1818118185015"></a>用户名</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p1018178155019"><a name="zh-cn_topic_0108618545_p1018178155019"></a><a name="zh-cn_topic_0108618545_p1018178155019"></a>选择KERBEROS鉴权时，需要配置MRS Manager的用户名和密码。从HDFS导出目录时，如果需要创建快照，这里配置的用户需要HDFS系统的管理员权限。</p>
<div class="p" id="zh-cn_topic_0108618545_p129641211269"><a name="zh-cn_topic_0108618545_p129641211269"></a><a name="zh-cn_topic_0108618545_p129641211269"></a>如果要创建MRS安全集群的数据连接，不能使用admin用户。因为admin用户是默认的管理页面用户，这个用户无法作为安全集群的认证用户来使用。您可以创建一个新的MRS用户，然后在创建MRS数据连接时，<span class="parmname" id="zh-cn_topic_0108618545_dgc_01_0009_parmname3468191262313"><a name="zh-cn_topic_0108618545_dgc_01_0009_parmname3468191262313"></a><a name="zh-cn_topic_0108618545_dgc_01_0009_parmname3468191262313"></a>“用户名”</span>和<span class="parmname" id="zh-cn_topic_0108618545_dgc_01_0009_parmname64683124231"><a name="zh-cn_topic_0108618545_dgc_01_0009_parmname64683124231"></a><a name="zh-cn_topic_0108618545_dgc_01_0009_parmname64683124231"></a>“密码”</span>填写为新建的MRS用户及其密码。<div class="note" id="zh-cn_topic_0108618545_note15451659151217"><a name="zh-cn_topic_0108618545_note15451659151217"></a><a name="zh-cn_topic_0108618545_note15451659151217"></a><span class="notetitle"> 说明： </span><div class="notebody"><a name="zh-cn_topic_0108618545_ul17715141011134"></a><a name="zh-cn_topic_0108618545_ul17715141011134"></a><ul id="zh-cn_topic_0108618545_ul17715141011134"><li>如果CDM集群为2.9.0版本及之后版本，且MRS集群为3.1.0及之后版本，则所创建的用户至少需具备Manager_viewer的角色权限才能在CDM创建连接；如果需要对应组件的进行库、表、数据的操作，还需要添加对应组件的用户组权限。</li><li>如果CDM集群为2.9.0之前的版本，或MRS集群为3.1.0之前的版本，则所创建的用户需要具备Manager_administrator或System_administrator权限，才能在CDM创建连接。</li><li>仅具备Manager_tenant或Manager_auditor权限，无法创建连接。</li></ul>
</div></div>
</div>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p1318119865013"><a name="zh-cn_topic_0108618545_p1318119865013"></a><a name="zh-cn_topic_0108618545_p1318119865013"></a>cdm</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row8181188155013"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p12181583505"><a name="zh-cn_topic_0108618545_p12181583505"></a><a name="zh-cn_topic_0108618545_p12181583505"></a>密码</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p14181480502"><a name="zh-cn_topic_0108618545_p14181480502"></a><a name="zh-cn_topic_0108618545_p14181480502"></a>访问MRS Manager的用户密码。</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p6181689507"><a name="zh-cn_topic_0108618545_p6181689507"></a><a name="zh-cn_topic_0108618545_p6181689507"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row191817855019"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p718111875014"><a name="zh-cn_topic_0108618545_p718111875014"></a><a name="zh-cn_topic_0108618545_p718111875014"></a>OBS支持</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p15181783504"><a name="zh-cn_topic_0108618545_p15181783504"></a><a name="zh-cn_topic_0108618545_p15181783504"></a>需服务端支持OBS存储。在创建Hive表时，您可以指定将表存储在OBS中。</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p141818819501"><a name="zh-cn_topic_0108618545_p141818819501"></a><a name="zh-cn_topic_0108618545_p141818819501"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row218148115017"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p1718178205019"><a name="zh-cn_topic_0108618545_p1718178205019"></a><a name="zh-cn_topic_0108618545_p1718178205019"></a>运行模式</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108618545_p918188135016"><a name="zh-cn_topic_0108618545_p918188135016"></a><a name="zh-cn_topic_0108618545_p918188135016"></a><span class="parmvalue" id="zh-cn_topic_0108618545_parmvalue12272019556"><a name="zh-cn_topic_0108618545_parmvalue12272019556"></a><a name="zh-cn_topic_0108618545_parmvalue12272019556"></a>“HIVE_3_X”</span>版本支持该参数。支持以下模式：<a name="zh-cn_topic_0108618545_ul111811818502"></a><a name="zh-cn_topic_0108618545_ul111811818502"></a><ul id="zh-cn_topic_0108618545_ul111811818502"><li>EMBEDDED：连接实例与CDM运行在一起，该模式性能较好。</li><li>STANDALONE：连接实例运行在独立进程。如果CDM需要对接多个Hadoop数据源（MRS、Hadoop或CloudTable），并且既有KERBEROS认证模式又有SIMPLE认证模式，只能使用STANDALONE模式或者配置不同的Agent。<p id="zh-cn_topic_0108618545_p1184511312281"><a name="zh-cn_topic_0108618545_p1184511312281"></a><a name="zh-cn_topic_0108618545_p1184511312281"></a><strong id="zh-cn_topic_0108618545_b6845133152817"><a name="zh-cn_topic_0108618545_b6845133152817"></a><a name="zh-cn_topic_0108618545_b6845133152817"></a>说明</strong>：STANDALONE模式主要是用来解决版本冲突问题的运行模式。当同一种数据连接的源端或者目的端连接器的版本不一致时，存在jar包冲突的情况，这时需要将源端或目的端放在STANDALONE进程里，防止冲突导致迁移失败。</p>
</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p161817865014"><a name="zh-cn_topic_0108618545_p161817865014"></a><a name="zh-cn_topic_0108618545_p161817865014"></a>EMBEDDED</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row1574651145712"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p720517447382"><a name="zh-cn_topic_0108618545_p720517447382"></a><a name="zh-cn_topic_0108618545_p720517447382"></a>是否使用集群配置</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p15999193719436"><a name="zh-cn_topic_0108618545_p15999193719436"></a><a name="zh-cn_topic_0108618545_p15999193719436"></a>您可以通过使用集群配置，简化Hadoop连接参数配置。</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p1820544419380"><a name="zh-cn_topic_0108618545_p1820544419380"></a><a name="zh-cn_topic_0108618545_p1820544419380"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row25741451205711"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p71575599434"><a name="zh-cn_topic_0108618545_p71575599434"></a><a name="zh-cn_topic_0108618545_p71575599434"></a>集群配置名</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p16157155904317"><a name="zh-cn_topic_0108618545_p16157155904317"></a><a name="zh-cn_topic_0108618545_p16157155904317"></a>仅当“是否使用集群配置”为“是”时，此参数有效。此参数用于选择用户已经创建好的集群配置。</p>
<p id="zh-cn_topic_0108618545_p192441948154613"><a name="zh-cn_topic_0108618545_p192441948154613"></a><a name="zh-cn_topic_0108618545_p192441948154613"></a>集群配置的创建方法请参见<a href="管理集群配置.md#dgc_01_1096">管理集群配置</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p1115715591436"><a name="zh-cn_topic_0108618545_p1115715591436"></a><a name="zh-cn_topic_0108618545_p1115715591436"></a>hive_01</p>
</td>
</tr>
</tbody>
</table>

单击“显示高级属性“，然后单击“添加“，您可以添加客户端的配置属性。所添加的每个属性需配置属性名称和值。对于不再需要的属性，可单击属性后的“删除“按钮进行删除。

## FusionInsight Hive<a name="zh-cn_topic_0108618545_section999517914488"></a>

FusionInsight Hive连接适用于用户在本地数据中心自建的FusionInsight HD，需通过专线连接。

FusionInsight Hive的连接参数如[表2](#zh-cn_topic_0108618545_table6441152003419)所示。

**表 2**  FusionInsight Hive连接参数

<a name="zh-cn_topic_0108618545_table6441152003419"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108618545_row15441220123417"><th class="cellrowborder" valign="top" width="16.72%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108618545_p18441202093413"><a name="zh-cn_topic_0108618545_p18441202093413"></a><a name="zh-cn_topic_0108618545_p18441202093413"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="62.1%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108618545_p1544152053412"><a name="zh-cn_topic_0108618545_p1544152053412"></a><a name="zh-cn_topic_0108618545_p1544152053412"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="21.18%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108618545_p4441112010341"><a name="zh-cn_topic_0108618545_p4441112010341"></a><a name="zh-cn_topic_0108618545_p4441112010341"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108618545_row11441182012346"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p4456620113417"><a name="zh-cn_topic_0108618545_p4456620113417"></a><a name="zh-cn_topic_0108618545_p4456620113417"></a>名称</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p6456820183418"><a name="zh-cn_topic_0108618545_p6456820183418"></a><a name="zh-cn_topic_0108618545_p6456820183418"></a>连接的名称，根据连接的数据源类型，用户可自定义便于记忆、区分的连接名。</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p13456112023418"><a name="zh-cn_topic_0108618545_p13456112023418"></a><a name="zh-cn_topic_0108618545_p13456112023418"></a>hivelink</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row2456122053415"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p13456172019344"><a name="zh-cn_topic_0108618545_p13456172019344"></a><a name="zh-cn_topic_0108618545_p13456172019344"></a>Manager IP</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p06633101352"><a name="zh-cn_topic_0108618545_p06633101352"></a><a name="zh-cn_topic_0108618545_p06633101352"></a>FusionInsight Manager平台的地址。</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p13456420143418"><a name="zh-cn_topic_0108618545_p13456420143418"></a><a name="zh-cn_topic_0108618545_p13456420143418"></a>127.0.0.1</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row69818335447"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p1991533164412"><a name="zh-cn_topic_0108618545_p1991533164412"></a><a name="zh-cn_topic_0108618545_p1991533164412"></a>Manager端口</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p3913811183515"><a name="zh-cn_topic_0108618545_p3913811183515"></a><a name="zh-cn_topic_0108618545_p3913811183515"></a>FusionInsight Manager平台的端口。</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p10993333441"><a name="zh-cn_topic_0108618545_p10993333441"></a><a name="zh-cn_topic_0108618545_p10993333441"></a>28443</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row6130136184519"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p1813015361459"><a name="zh-cn_topic_0108618545_p1813015361459"></a><a name="zh-cn_topic_0108618545_p1813015361459"></a>CAS Server端口</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p186251918103513"><a name="zh-cn_topic_0108618545_p186251918103513"></a><a name="zh-cn_topic_0108618545_p186251918103513"></a>与FusionInsight对接的CAS Server的端口。</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p1813011362455"><a name="zh-cn_topic_0108618545_p1813011362455"></a><a name="zh-cn_topic_0108618545_p1813011362455"></a>20009</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row15511955415"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p18308035125414"><a name="zh-cn_topic_0108618545_p18308035125414"></a><a name="zh-cn_topic_0108618545_p18308035125414"></a>认证类型</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108618545_p13355246182213"><a name="zh-cn_topic_0108618545_p13355246182213"></a><a name="zh-cn_topic_0108618545_p13355246182213"></a>访问集群的认证类型：<a name="zh-cn_topic_0108618545_zh-cn_topic_0108275286_ul193521539183819"></a><a name="zh-cn_topic_0108618545_zh-cn_topic_0108275286_ul193521539183819"></a><ul id="zh-cn_topic_0108618545_zh-cn_topic_0108275286_ul193521539183819"><li>SIMPLE：非安全模式选择Simple鉴权。</li><li>KERBEROS：安全模式选择Kerberos鉴权。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p16308123510546"><a name="zh-cn_topic_0108618545_p16308123510546"></a><a name="zh-cn_topic_0108618545_p16308123510546"></a>SIMPLE</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row49732021195414"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p183081535195411"><a name="zh-cn_topic_0108618545_p183081535195411"></a><a name="zh-cn_topic_0108618545_p183081535195411"></a>Hive版本</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p123082350549"><a name="zh-cn_topic_0108618545_p123082350549"></a><a name="zh-cn_topic_0108618545_p123082350549"></a>Hive的版本。</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p33081535155414"><a name="zh-cn_topic_0108618545_p33081535155414"></a><a name="zh-cn_topic_0108618545_p33081535155414"></a>HIVE_3_X</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row16456152011347"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p94561620113420"><a name="zh-cn_topic_0108618545_p94561620113420"></a><a name="zh-cn_topic_0108618545_p94561620113420"></a>用户名</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p64738206349"><a name="zh-cn_topic_0108618545_p64738206349"></a><a name="zh-cn_topic_0108618545_p64738206349"></a>登录FusionInsight Manager平台的用户名。</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p3473020113416"><a name="zh-cn_topic_0108618545_p3473020113416"></a><a name="zh-cn_topic_0108618545_p3473020113416"></a>cdm</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row20456320123419"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p647322020346"><a name="zh-cn_topic_0108618545_p647322020346"></a><a name="zh-cn_topic_0108618545_p647322020346"></a>密码</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p174737206340"><a name="zh-cn_topic_0108618545_p174737206340"></a><a name="zh-cn_topic_0108618545_p174737206340"></a>FusionInsight Manager平台的密码。</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p204731920153414"><a name="zh-cn_topic_0108618545_p204731920153414"></a><a name="zh-cn_topic_0108618545_p204731920153414"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row138306469346"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p68311546193412"><a name="zh-cn_topic_0108618545_p68311546193412"></a><a name="zh-cn_topic_0108618545_p68311546193412"></a>OBS支持</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p148311546123415"><a name="zh-cn_topic_0108618545_p148311546123415"></a><a name="zh-cn_topic_0108618545_p148311546123415"></a>需服务端支持OBS存储。在创建Hive表时，您可以指定将表存储在OBS中。</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p15831114633413"><a name="zh-cn_topic_0108618545_p15831114633413"></a><a name="zh-cn_topic_0108618545_p15831114633413"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row4651550133414"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p116565033415"><a name="zh-cn_topic_0108618545_p116565033415"></a><a name="zh-cn_topic_0108618545_p116565033415"></a>运行模式</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p372035318271"><a name="zh-cn_topic_0108618545_p372035318271"></a><a name="zh-cn_topic_0108618545_p372035318271"></a><span class="parmvalue" id="zh-cn_topic_0108618545_parmvalue17202532276"><a name="zh-cn_topic_0108618545_parmvalue17202532276"></a><a name="zh-cn_topic_0108618545_parmvalue17202532276"></a>“HIVE_3_X”</span>版本支持该参数。支持以下模式：</p>
<a name="zh-cn_topic_0108618545_ul192118325256"></a><a name="zh-cn_topic_0108618545_ul192118325256"></a><ul id="zh-cn_topic_0108618545_ul192118325256"><li>EMBEDDED：连接实例与CDM运行在一起，该模式性能较好。</li><li>STANDALONE：连接实例运行在独立进程。如果CDM需要对接多个Hadoop数据源（MRS、Hadoop或CloudTable），并且既有KERBEROS认证模式又有SIMPLE认证模式，只能使用STANDALONE模式或者配置不同的Agent。<p id="zh-cn_topic_0108618545_zh-cn_topic_0108618545_p1184511312281"><a name="zh-cn_topic_0108618545_zh-cn_topic_0108618545_p1184511312281"></a><a name="zh-cn_topic_0108618545_zh-cn_topic_0108618545_p1184511312281"></a><strong id="zh-cn_topic_0108618545_zh-cn_topic_0108618545_b6845133152817"><a name="zh-cn_topic_0108618545_zh-cn_topic_0108618545_b6845133152817"></a><a name="zh-cn_topic_0108618545_zh-cn_topic_0108618545_b6845133152817"></a>说明</strong>：STANDALONE模式主要是用来解决版本冲突问题的运行模式。当同一种数据连接的源端或者目的端连接器的版本不一致时，存在jar包冲突的情况，这时需要将源端或目的端放在STANDALONE进程里，防止冲突导致迁移失败。</p>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p765250193414"><a name="zh-cn_topic_0108618545_p765250193414"></a><a name="zh-cn_topic_0108618545_p765250193414"></a>EMBEDDED</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row12050271302"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p1205102763015"><a name="zh-cn_topic_0108618545_p1205102763015"></a><a name="zh-cn_topic_0108618545_p1205102763015"></a>是否使用集群配置</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p3791105013307"><a name="zh-cn_topic_0108618545_p3791105013307"></a><a name="zh-cn_topic_0108618545_p3791105013307"></a>您可以通过使用集群配置，简化Hadoop连接参数配置。</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p147705512305"><a name="zh-cn_topic_0108618545_p147705512305"></a><a name="zh-cn_topic_0108618545_p147705512305"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row1710453013302"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p1713125033015"><a name="zh-cn_topic_0108618545_p1713125033015"></a><a name="zh-cn_topic_0108618545_p1713125033015"></a>集群配置名</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p1171175111302"><a name="zh-cn_topic_0108618545_p1171175111302"></a><a name="zh-cn_topic_0108618545_p1171175111302"></a>仅当“是否使用集群配置”为“是”时，此参数有效。此参数用于选择用户已经创建好的集群配置。</p>
<p id="zh-cn_topic_0108618545_p192211597367"><a name="zh-cn_topic_0108618545_p192211597367"></a><a name="zh-cn_topic_0108618545_p192211597367"></a>集群配置的创建方法请参见<a href="管理集群配置.md#dgc_01_1096">管理集群配置</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p0147252193019"><a name="zh-cn_topic_0108618545_p0147252193019"></a><a name="zh-cn_topic_0108618545_p0147252193019"></a>hive_01</p>
</td>
</tr>
</tbody>
</table>

单击“显示高级属性“，然后单击“添加“，您可以添加客户端的配置属性。所添加的每个属性需配置属性名称和值。对于不再需要的属性，可单击属性后的“删除“按钮进行删除。

## Apache Hive<a name="zh-cn_topic_0108618545_section9585729145218"></a>

Apache Hive连接适用于用户在本地数据中心或ECS上自建的第三方Hadoop，其中本地数据中心的Hadoop需通过专线连接。

Apache Hive的连接参数如[表3](#zh-cn_topic_0108618545_table3324121355313)所示。

**表 3**  Apache Hive连接参数

<a name="zh-cn_topic_0108618545_table3324121355313"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108618545_row19324151314536"><th class="cellrowborder" valign="top" width="16.72%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108618545_p1832481320534"><a name="zh-cn_topic_0108618545_p1832481320534"></a><a name="zh-cn_topic_0108618545_p1832481320534"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="62.1%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108618545_p832441312539"><a name="zh-cn_topic_0108618545_p832441312539"></a><a name="zh-cn_topic_0108618545_p832441312539"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="21.18%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108618545_p18324313165315"><a name="zh-cn_topic_0108618545_p18324313165315"></a><a name="zh-cn_topic_0108618545_p18324313165315"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108618545_row1432410135532"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p1324613145314"><a name="zh-cn_topic_0108618545_p1324613145314"></a><a name="zh-cn_topic_0108618545_p1324613145314"></a>名称</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p183241713175313"><a name="zh-cn_topic_0108618545_p183241713175313"></a><a name="zh-cn_topic_0108618545_p183241713175313"></a>连接的名称，根据连接的数据源类型，用户可自定义便于记忆、区分的连接名。</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p13241513105315"><a name="zh-cn_topic_0108618545_p13241513105315"></a><a name="zh-cn_topic_0108618545_p13241513105315"></a>hivelink</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row789444422317"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p1232413139535"><a name="zh-cn_topic_0108618545_p1232413139535"></a><a name="zh-cn_topic_0108618545_p1232413139535"></a>URI</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p7813915182410"><a name="zh-cn_topic_0108618545_p7813915182410"></a><a name="zh-cn_topic_0108618545_p7813915182410"></a>NameNode URI地址。</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p7324113145310"><a name="zh-cn_topic_0108618545_p7324113145310"></a><a name="zh-cn_topic_0108618545_p7324113145310"></a>hdfs://hacluster</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row7715132582410"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p12324313195314"><a name="zh-cn_topic_0108618545_p12324313195314"></a><a name="zh-cn_topic_0108618545_p12324313195314"></a>Hive元数据地址</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p262575310247"><a name="zh-cn_topic_0108618545_p262575310247"></a><a name="zh-cn_topic_0108618545_p262575310247"></a>设置Hive元数据地址，参考 hive.metastore.uris配置项。例如：thrift://host-192-168-1-212:9083</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p332521318536"><a name="zh-cn_topic_0108618545_p332521318536"></a><a name="zh-cn_topic_0108618545_p332521318536"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row43251713205314"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p632591345311"><a name="zh-cn_topic_0108618545_p632591345311"></a><a name="zh-cn_topic_0108618545_p632591345311"></a>认证类型</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><div class="p" id="p18155104792510"><a name="p18155104792510"></a><a name="p18155104792510"></a>访问集群的认证类型：<a name="zh-cn_topic_0108618545_zh-cn_topic_0108618545_zh-cn_topic_0108275286_ul193521539183819"></a><a name="zh-cn_topic_0108618545_zh-cn_topic_0108618545_zh-cn_topic_0108275286_ul193521539183819"></a><ul id="zh-cn_topic_0108618545_zh-cn_topic_0108618545_zh-cn_topic_0108275286_ul193521539183819"><li>SIMPLE：非安全模式选择Simple鉴权。</li><li>KERBEROS：安全模式选择Kerberos鉴权。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p133251139531"><a name="zh-cn_topic_0108618545_p133251139531"></a><a name="zh-cn_topic_0108618545_p133251139531"></a>SIMPLE</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row19325813125317"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p732501320534"><a name="zh-cn_topic_0108618545_p732501320534"></a><a name="zh-cn_topic_0108618545_p732501320534"></a>Hive版本</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p83251913155314"><a name="zh-cn_topic_0108618545_p83251913155314"></a><a name="zh-cn_topic_0108618545_p83251913155314"></a>Hive的版本。</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p133258138533"><a name="zh-cn_topic_0108618545_p133258138533"></a><a name="zh-cn_topic_0108618545_p133258138533"></a>HIVE_3_X</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row17231834182517"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p183251113105315"><a name="zh-cn_topic_0108618545_p183251113105315"></a><a name="zh-cn_topic_0108618545_p183251113105315"></a>IP与主机名映射</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p151061147264"><a name="zh-cn_topic_0108618545_p151061147264"></a><a name="zh-cn_topic_0108618545_p151061147264"></a>如果Hadoop配置文件使用主机名，需要配置IP与主机的映射。格式：IP与主机名之间使用空格分隔，多对映射使用分号或回车换行分隔。</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p16325191355312"><a name="zh-cn_topic_0108618545_p16325191355312"></a><a name="zh-cn_topic_0108618545_p16325191355312"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row1332551310534"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p2032514137536"><a name="zh-cn_topic_0108618545_p2032514137536"></a><a name="zh-cn_topic_0108618545_p2032514137536"></a>OBS支持</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p103251713145314"><a name="zh-cn_topic_0108618545_p103251713145314"></a><a name="zh-cn_topic_0108618545_p103251713145314"></a>需服务端支持OBS存储。在创建Hive表时，您可以指定将表存储在OBS中。</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p19325101312534"><a name="zh-cn_topic_0108618545_p19325101312534"></a><a name="zh-cn_topic_0108618545_p19325101312534"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row326875891919"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p152681058201918"><a name="zh-cn_topic_0108618545_p152681058201918"></a><a name="zh-cn_topic_0108618545_p152681058201918"></a>Principal</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p1826818583197"><a name="zh-cn_topic_0108618545_p1826818583197"></a><a name="zh-cn_topic_0108618545_p1826818583197"></a>认证类型为“KERBEROS”时，需要填写Principal。Principal即Kerberos安全模式下的用户名，可以联系Hadoop管理员获取。此处填写的Principal需要与Keytab文件保持一致。</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p026845851917"><a name="zh-cn_topic_0108618545_p026845851917"></a><a name="zh-cn_topic_0108618545_p026845851917"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row1667905206"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p136678013202"><a name="zh-cn_topic_0108618545_p136678013202"></a><a name="zh-cn_topic_0108618545_p136678013202"></a>Keytab文件</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p333954514271"><a name="zh-cn_topic_0108618545_p333954514271"></a><a name="zh-cn_topic_0108618545_p333954514271"></a>认证类型为“KERBEROS”时，需要上传Keytab文件。Keytab文件为认证凭据文件，可以联系Hadoop管理员获取。获取Keytab文件前，需要在集群上至少修改过一次此用户的密码，否则下载获取的keytab文件可能无法使用。另外，修改用户密码后，之前导出的keytab将失效，需要重新导出。</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p8667100112018"><a name="zh-cn_topic_0108618545_p8667100112018"></a><a name="zh-cn_topic_0108618545_p8667100112018"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row5325131312537"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p133251513195314"><a name="zh-cn_topic_0108618545_p133251513195314"></a><a name="zh-cn_topic_0108618545_p133251513195314"></a>运行模式</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p13251913175310"><a name="zh-cn_topic_0108618545_p13251913175310"></a><a name="zh-cn_topic_0108618545_p13251913175310"></a><span class="parmvalue" id="zh-cn_topic_0108618545_parmvalue1232515138535"><a name="zh-cn_topic_0108618545_parmvalue1232515138535"></a><a name="zh-cn_topic_0108618545_parmvalue1232515138535"></a>“HIVE_3_X”</span>版本支持该参数。支持以下模式：</p>
<a name="zh-cn_topic_0108618545_ul83512207444"></a><a name="zh-cn_topic_0108618545_ul83512207444"></a><ul id="zh-cn_topic_0108618545_ul83512207444"><li>EMBEDDED：连接实例与CDM运行在一起，该模式性能较好。</li><li>STANDALONE：连接实例运行在独立进程。如果CDM需要对接多个Hadoop数据源（MRS、Hadoop或CloudTable），并且既有KERBEROS认证模式又有SIMPLE认证模式，只能使用STANDALONE模式或者配置不同的Agent。<p id="zh-cn_topic_0108618545_zh-cn_topic_0108618545_p1184511312281_1"><a name="zh-cn_topic_0108618545_zh-cn_topic_0108618545_p1184511312281_1"></a><a name="zh-cn_topic_0108618545_zh-cn_topic_0108618545_p1184511312281_1"></a><strong id="zh-cn_topic_0108618545_zh-cn_topic_0108618545_b6845133152817_1"><a name="zh-cn_topic_0108618545_zh-cn_topic_0108618545_b6845133152817_1"></a><a name="zh-cn_topic_0108618545_zh-cn_topic_0108618545_b6845133152817_1"></a>说明</strong>：STANDALONE模式主要是用来解决版本冲突问题的运行模式。当同一种数据连接的源端或者目的端连接器的版本不一致时，存在jar包冲突的情况，这时需要将源端或目的端放在STANDALONE进程里，防止冲突导致迁移失败。</p>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p9325191316537"><a name="zh-cn_topic_0108618545_p9325191316537"></a><a name="zh-cn_topic_0108618545_p9325191316537"></a>EMBEDDED</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row155901217113910"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p8769519135519"><a name="zh-cn_topic_0108618545_p8769519135519"></a><a name="zh-cn_topic_0108618545_p8769519135519"></a>是否使用集群配置</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p1976991919558"><a name="zh-cn_topic_0108618545_p1976991919558"></a><a name="zh-cn_topic_0108618545_p1976991919558"></a>您可以通过使用集群配置，简化Hadoop连接参数配置。</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p1476914197553"><a name="zh-cn_topic_0108618545_p1476914197553"></a><a name="zh-cn_topic_0108618545_p1476914197553"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row558910177392"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p476991911553"><a name="zh-cn_topic_0108618545_p476991911553"></a><a name="zh-cn_topic_0108618545_p476991911553"></a>集群配置名</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p17691919185511"><a name="zh-cn_topic_0108618545_p17691919185511"></a><a name="zh-cn_topic_0108618545_p17691919185511"></a>仅当“是否使用集群配置”为“是”时，此参数有效。此参数用于选择用户已经创建好的集群配置。</p>
<p id="zh-cn_topic_0108618545_p27695198558"><a name="zh-cn_topic_0108618545_p27695198558"></a><a name="zh-cn_topic_0108618545_p27695198558"></a>集群配置的创建方法请参见<a href="管理集群配置.md#dgc_01_1096">管理集群配置</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p1676921975513"><a name="zh-cn_topic_0108618545_p1676921975513"></a><a name="zh-cn_topic_0108618545_p1676921975513"></a>hive_01</p>
</td>
</tr>
</tbody>
</table>

单击“显示高级属性“，然后单击“添加“，您可以添加客户端的配置属性。所添加的每个属性需配置属性名称和值。对于不再需要的属性，可单击属性后的“删除“按钮进行删除。

