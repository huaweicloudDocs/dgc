# 配置Kafka连接<a name="dgc_01_0033"></a>

## MRS Kafka<a name="zh-cn_topic_0108275385_section8886729122818"></a>

连接MRS上的Kafka数据源时，相关参数如[表1](#zh-cn_topic_0108275385_table3104110173020)所示。

**表 1**  MRS Kafka连接参数

<a name="zh-cn_topic_0108275385_table3104110173020"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108275385_row9104908308"><th class="cellrowborder" valign="top" width="18.95%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108275385_p5104190113020"><a name="zh-cn_topic_0108275385_p5104190113020"></a><a name="zh-cn_topic_0108275385_p5104190113020"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="61.42999999999999%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108275385_p181045015309"><a name="zh-cn_topic_0108275385_p181045015309"></a><a name="zh-cn_topic_0108275385_p181045015309"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="19.62%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108275385_p810450163019"><a name="zh-cn_topic_0108275385_p810450163019"></a><a name="zh-cn_topic_0108275385_p810450163019"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108275385_row1110420173014"><td class="cellrowborder" valign="top" width="18.95%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275385_p1510415063017"><a name="zh-cn_topic_0108275385_p1510415063017"></a><a name="zh-cn_topic_0108275385_p1510415063017"></a>名称</p>
</td>
<td class="cellrowborder" valign="top" width="61.42999999999999%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275385_p71047053018"><a name="zh-cn_topic_0108275385_p71047053018"></a><a name="zh-cn_topic_0108275385_p71047053018"></a>连接的名称，根据连接的数据源类型，用户可自定义便于记忆、区分的连接名。</p>
</td>
<td class="cellrowborder" valign="top" width="19.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275385_p91041304307"><a name="zh-cn_topic_0108275385_p91041304307"></a><a name="zh-cn_topic_0108275385_p91041304307"></a>kafka_link</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275385_row11045013017"><td class="cellrowborder" valign="top" width="18.95%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275385_p121041208302"><a name="zh-cn_topic_0108275385_p121041208302"></a><a name="zh-cn_topic_0108275385_p121041208302"></a>Manager IP</p>
</td>
<td class="cellrowborder" valign="top" width="61.42999999999999%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275385_p6104305303"><a name="zh-cn_topic_0108275385_p6104305303"></a><a name="zh-cn_topic_0108275385_p6104305303"></a>MRS Manager的浮动IP地址，可以单击输入框后的<span class="uicontrol" id="zh-cn_topic_0108275385_zh-cn_topic_0108275286_uicontrol926725316310"><a name="zh-cn_topic_0108275385_zh-cn_topic_0108275286_uicontrol926725316310"></a><a name="zh-cn_topic_0108275385_zh-cn_topic_0108275286_uicontrol926725316310"></a>“选择”</span>来选定已创建的MRS集群，CDM会自动填充下面的鉴权参数。</p>
</td>
<td class="cellrowborder" valign="top" width="19.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275385_p1210414014308"><a name="zh-cn_topic_0108275385_p1210414014308"></a><a name="zh-cn_topic_0108275385_p1210414014308"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275385_row1110417013011"><td class="cellrowborder" valign="top" width="18.95%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275385_p16104120163017"><a name="zh-cn_topic_0108275385_p16104120163017"></a><a name="zh-cn_topic_0108275385_p16104120163017"></a>用户名</p>
</td>
<td class="cellrowborder" valign="top" width="61.42999999999999%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275385_p141051706305"><a name="zh-cn_topic_0108275385_p141051706305"></a><a name="zh-cn_topic_0108275385_p141051706305"></a>需要配置MRS Manager的用户名和密码。</p>
<div class="p" id="zh-cn_topic_0108275385_p194519141759"><a name="zh-cn_topic_0108275385_p194519141759"></a><a name="zh-cn_topic_0108275385_p194519141759"></a>如果要创建MRS安全集群的数据连接，不能使用admin用户。因为admin用户是默认的管理页面用户，这个用户无法作为安全集群的认证用户来使用。您可以创建一个新的MRS用户，然后在创建MRS数据连接时，<span class="parmname" id="zh-cn_topic_0108275385_zh-cn_topic_0108618545_dgc_01_0009_parmname3468191262313"><a name="zh-cn_topic_0108275385_zh-cn_topic_0108618545_dgc_01_0009_parmname3468191262313"></a><a name="zh-cn_topic_0108275385_zh-cn_topic_0108618545_dgc_01_0009_parmname3468191262313"></a>“用户名”</span>和<span class="parmname" id="zh-cn_topic_0108275385_zh-cn_topic_0108618545_dgc_01_0009_parmname64683124231"><a name="zh-cn_topic_0108275385_zh-cn_topic_0108618545_dgc_01_0009_parmname64683124231"></a><a name="zh-cn_topic_0108275385_zh-cn_topic_0108618545_dgc_01_0009_parmname64683124231"></a>“密码”</span>填写为新建的MRS用户及其密码。<div class="note" id="zh-cn_topic_0108275385_zh-cn_topic_0108618545_note15451659151217"><a name="zh-cn_topic_0108275385_zh-cn_topic_0108618545_note15451659151217"></a><a name="zh-cn_topic_0108275385_zh-cn_topic_0108618545_note15451659151217"></a><span class="notetitle"> 说明： </span><div class="notebody"><a name="zh-cn_topic_0108275385_zh-cn_topic_0108618545_ul17715141011134"></a><a name="zh-cn_topic_0108275385_zh-cn_topic_0108618545_ul17715141011134"></a><ul id="zh-cn_topic_0108275385_zh-cn_topic_0108618545_ul17715141011134"><li>如果CDM集群为2.9.0版本及之后版本，且MRS集群为3.1.0及之后版本，则所创建的用户至少需具备Manager_viewer的角色权限才能在CDM创建连接；如果需要对应组件的进行库、表、数据的操作，还需要添加对应组件的用户组权限。</li><li>如果CDM集群为2.9.0之前的版本，或MRS集群为3.1.0之前的版本，则所创建的用户需要具备Manager_administrator或System_administrator权限，才能在CDM创建连接。</li><li>仅具备Manager_tenant或Manager_auditor权限，无法创建连接。</li></ul>
</div></div>
</div>
</td>
<td class="cellrowborder" valign="top" width="19.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275385_p710517023010"><a name="zh-cn_topic_0108275385_p710517023010"></a><a name="zh-cn_topic_0108275385_p710517023010"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275385_row3105201309"><td class="cellrowborder" valign="top" width="18.95%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275385_p18105507306"><a name="zh-cn_topic_0108275385_p18105507306"></a><a name="zh-cn_topic_0108275385_p18105507306"></a>密码</p>
</td>
<td class="cellrowborder" valign="top" width="61.42999999999999%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275385_p71054011307"><a name="zh-cn_topic_0108275385_p71054011307"></a><a name="zh-cn_topic_0108275385_p71054011307"></a>访问MRS Manager的用户密码。</p>
</td>
<td class="cellrowborder" valign="top" width="19.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275385_p191051703302"><a name="zh-cn_topic_0108275385_p191051703302"></a><a name="zh-cn_topic_0108275385_p191051703302"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275385_row177699297305"><td class="cellrowborder" valign="top" width="18.95%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275385_p310410043015"><a name="zh-cn_topic_0108275385_p310410043015"></a><a name="zh-cn_topic_0108275385_p310410043015"></a>认证类型</p>
</td>
<td class="cellrowborder" valign="top" width="61.42999999999999%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108275385_p171048073013"><a name="zh-cn_topic_0108275385_p171048073013"></a><a name="zh-cn_topic_0108275385_p171048073013"></a>访问MRS的认证类型：<a name="zh-cn_topic_0108275385_ul17104806309"></a><a name="zh-cn_topic_0108275385_ul17104806309"></a><ul id="zh-cn_topic_0108275385_ul17104806309"><li>SIMPLE：非安全模式选择Simple鉴权。</li><li>KERBEROS：安全模式选择Kerberos鉴权。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="19.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275385_p191042018308"><a name="zh-cn_topic_0108275385_p191042018308"></a><a name="zh-cn_topic_0108275385_p191042018308"></a>是</p>
</td>
</tr>
</tbody>
</table>

单击“显示高级属性“，然后单击“添加“，您可以添加客户端的配置属性。所添加的每个属性需配置属性名称和值。对于不再需要的属性，可单击属性后的“删除“按钮进行删除。

## Apache Kafka<a name="zh-cn_topic_0108275385_section13645174115297"></a>

Apache Kafka连接适用于用户在本地数据中心或ECS上自建的第三方Kafka，其中本地数据中心的Kafka需通过专线连接。

连接Apache Hadoop上的Kafka数据源时，相关参数如[表2](#zh-cn_topic_0108275385_table1990636915212)所示。

**表 2**  Apache Kafka连接参数

<a name="zh-cn_topic_0108275385_table1990636915212"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108275385_row4257242215212"><th class="cellrowborder" valign="top" width="18.95%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108275385_p3100089215212"><a name="zh-cn_topic_0108275385_p3100089215212"></a><a name="zh-cn_topic_0108275385_p3100089215212"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="61.42999999999999%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108275385_p2804435515212"><a name="zh-cn_topic_0108275385_p2804435515212"></a><a name="zh-cn_topic_0108275385_p2804435515212"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="19.62%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108275385_p5700024515212"><a name="zh-cn_topic_0108275385_p5700024515212"></a><a name="zh-cn_topic_0108275385_p5700024515212"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108275385_row845118401045"><td class="cellrowborder" valign="top" width="18.95%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275385_p645116401542"><a name="zh-cn_topic_0108275385_p645116401542"></a><a name="zh-cn_topic_0108275385_p645116401542"></a>名称</p>
</td>
<td class="cellrowborder" valign="top" width="61.42999999999999%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275385_p1369564463813"><a name="zh-cn_topic_0108275385_p1369564463813"></a><a name="zh-cn_topic_0108275385_p1369564463813"></a>连接的名称，根据连接的数据源类型，用户可自定义便于记忆、区分的连接名。</p>
</td>
<td class="cellrowborder" valign="top" width="19.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275385_p7451104018412"><a name="zh-cn_topic_0108275385_p7451104018412"></a><a name="zh-cn_topic_0108275385_p7451104018412"></a>kafka_link</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275385_row4324016315212"><td class="cellrowborder" valign="top" width="18.95%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275385_p1279229115212"><a name="zh-cn_topic_0108275385_p1279229115212"></a><a name="zh-cn_topic_0108275385_p1279229115212"></a>Kafka broker</p>
</td>
<td class="cellrowborder" valign="top" width="61.42999999999999%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275385_p36793163165241"><a name="zh-cn_topic_0108275385_p36793163165241"></a><a name="zh-cn_topic_0108275385_p36793163165241"></a>Kafka broker的IP地址和端口。</p>
</td>
<td class="cellrowborder" valign="top" width="19.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275385_p7230798165241"><a name="zh-cn_topic_0108275385_p7230798165241"></a><a name="zh-cn_topic_0108275385_p7230798165241"></a>192.168.1.1:9092</p>
</td>
</tr>
</tbody>
</table>

单击“显示高级属性“，然后单击“添加“，您可以添加客户端的配置属性。所添加的每个属性需配置属性名称和值。对于不再需要的属性，可单击属性后的“删除“按钮进行删除。

