# 配置Hive连接<a name="dayu_01_0026"></a>

目前CDM支持连接MRS的Hive，相关参数如[表1](#zh-cn_topic_0108618545_table6441152003419)所示。

>![](public_sys-resources/icon-note.gif) **说明：**   
>由于当前CDM Hive连接是从MRS HDFS组件获取core-site.xml配置信息，所以在MRS侧使用的是Hive over OBS场景时，在创建Hive连接前，需要用户在MRS管理界面的HDFS组件中配置OBS的AK，SK信息。  

**表 1**  Hive连接参数

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
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p1345602010341"><a name="zh-cn_topic_0108618545_p1345602010341"></a><a name="zh-cn_topic_0108618545_p1345602010341"></a>MRS Manager的IP地址，可以单击输入框后的<span class="uicontrol" id="zh-cn_topic_0108618545_zh-cn_topic_0108275286_uicontrol926725316310"><a name="zh-cn_topic_0108618545_zh-cn_topic_0108275286_uicontrol926725316310"></a><a name="zh-cn_topic_0108618545_zh-cn_topic_0108275286_uicontrol926725316310"></a>“选择”</span>来选定已创建的MRS集群，CDM会自动填充下面的鉴权参数。</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p13456420143418"><a name="zh-cn_topic_0108618545_p13456420143418"></a><a name="zh-cn_topic_0108618545_p13456420143418"></a>127.0.0.1</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row4332334184015"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p06421125396"><a name="zh-cn_topic_0108618545_p06421125396"></a><a name="zh-cn_topic_0108618545_p06421125396"></a>认证类型</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108618545_p3642111243916"><a name="zh-cn_topic_0108618545_p3642111243916"></a><a name="zh-cn_topic_0108618545_p3642111243916"></a>访问MRS的认证类型：<a name="zh-cn_topic_0108618545_zh-cn_topic_0108275286_ul552304715358"></a><a name="zh-cn_topic_0108618545_zh-cn_topic_0108275286_ul552304715358"></a><ul id="zh-cn_topic_0108618545_zh-cn_topic_0108275286_ul552304715358"><li>SIMPLE：非安全模式选择Simple鉴权。</li><li>KERBEROS：安全模式选择Kerberos鉴权。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p76428123396"><a name="zh-cn_topic_0108618545_p76428123396"></a><a name="zh-cn_topic_0108618545_p76428123396"></a>SIMPLE</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row16456152011347"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p94561620113420"><a name="zh-cn_topic_0108618545_p94561620113420"></a><a name="zh-cn_topic_0108618545_p94561620113420"></a>用户名</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p64738206349"><a name="zh-cn_topic_0108618545_p64738206349"></a><a name="zh-cn_topic_0108618545_p64738206349"></a>选择KERBEROS鉴权时，需要配置MRS Manager的用户名和密码。</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p3473020113416"><a name="zh-cn_topic_0108618545_p3473020113416"></a><a name="zh-cn_topic_0108618545_p3473020113416"></a>cdm</p>
</td>
</tr>
<tr id="zh-cn_topic_0108618545_row20456320123419"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p647322020346"><a name="zh-cn_topic_0108618545_p647322020346"></a><a name="zh-cn_topic_0108618545_p647322020346"></a>密码</p>
</td>
<td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p174737206340"><a name="zh-cn_topic_0108618545_p174737206340"></a><a name="zh-cn_topic_0108618545_p174737206340"></a>访问MRS Manager的用户密码。</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p204731920153414"><a name="zh-cn_topic_0108618545_p204731920153414"></a><a name="zh-cn_topic_0108618545_p204731920153414"></a>-</p>
</td>
</tr>
</tbody>
</table>

