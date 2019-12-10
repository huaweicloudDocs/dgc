# DLI Spark<a name="dayu_01_0451"></a>

## 功能<a name="zh-cn_topic_0118184397_section44280035173841"></a>

通过DLI Spark节点执行一个预先定义的Spark作业。

## 参数<a name="zh-cn_topic_0118184397_section6331447317395"></a>

用户可参考[表1](#zh-cn_topic_0118184397_table3764823994826)和[表2](#zh-cn_topic_0118184397_table58040457102411)配置DLI Spark节点的参数。

**表 1**  属性参数

<a name="zh-cn_topic_0118184397_table3764823994826"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118184397_row3170822394826"><th class="cellrowborder" valign="top" width="28.07%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118184397_p2984581994826"><a name="zh-cn_topic_0118184397_p2984581994826"></a><a name="zh-cn_topic_0118184397_p2984581994826"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="15.659999999999998%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118184397_p159227094826"><a name="zh-cn_topic_0118184397_p159227094826"></a><a name="zh-cn_topic_0118184397_p159227094826"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="56.269999999999996%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118184397_p6186505494826"><a name="zh-cn_topic_0118184397_p6186505494826"></a><a name="zh-cn_topic_0118184397_p6186505494826"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118184397_row1991457694826"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184397_p246794194826"><a name="zh-cn_topic_0118184397_p246794194826"></a><a name="zh-cn_topic_0118184397_p246794194826"></a>节点名称</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184397_p6568554794826"><a name="zh-cn_topic_0118184397_p6568554794826"></a><a name="zh-cn_topic_0118184397_p6568554794826"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184397_p1892909794826"><a name="zh-cn_topic_0118184397_p1892909794826"></a><a name="zh-cn_topic_0118184397_p1892909794826"></a><span id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_text44323307153939"><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_text44323307153939"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_text44323307153939"></a>节点</span>名称，可以包含中文、英文字母、数字、<span class="parmvalue" id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a>“_”</span>、<span class="parmvalue" id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a>“-”</span>、<span class="parmvalue" id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_parmvalue3773104413412"><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_parmvalue3773104413412"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_parmvalue3773104413412"></a>“/”</span>、<span class="parmvalue" id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a>“&lt;”</span>、<span class="parmvalue" id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a>“&gt;”</span>等各类特殊字符，长度为1～128个字符。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184397_row3614415394826"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184397_p4199531294826"><a name="zh-cn_topic_0118184397_p4199531294826"></a><a name="zh-cn_topic_0118184397_p4199531294826"></a><span id="zh-cn_topic_0118184397_text99702162243"><a name="zh-cn_topic_0118184397_text99702162243"></a><a name="zh-cn_topic_0118184397_text99702162243"></a>DLI</span>集群名称</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184397_p4617707494826"><a name="zh-cn_topic_0118184397_p4617707494826"></a><a name="zh-cn_topic_0118184397_p4617707494826"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184397_p4935552994826"><a name="zh-cn_topic_0118184397_p4935552994826"></a><a name="zh-cn_topic_0118184397_p4935552994826"></a>选择<span id="zh-cn_topic_0118184397_text35566305815"><a name="zh-cn_topic_0118184397_text35566305815"></a><a name="zh-cn_topic_0118184397_text35566305815"></a>DLI</span>集群。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184397_row8143124232413"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184397_p1214314216245"><a name="zh-cn_topic_0118184397_p1214314216245"></a><a name="zh-cn_topic_0118184397_p1214314216245"></a>作业名称</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184397_p1714384282417"><a name="zh-cn_topic_0118184397_p1714384282417"></a><a name="zh-cn_topic_0118184397_p1714384282417"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184397_p814364216242"><a name="zh-cn_topic_0118184397_p814364216242"></a><a name="zh-cn_topic_0118184397_p814364216242"></a>填写<span id="zh-cn_topic_0118184397_text1613494515915"><a name="zh-cn_topic_0118184397_text1613494515915"></a><a name="zh-cn_topic_0118184397_text1613494515915"></a>DLI</span> Spark作业的名称，只能包含英文字母、数字、<span class="parmvalue" id="zh-cn_topic_0118184397_parmvalue73435113313"><a name="zh-cn_topic_0118184397_parmvalue73435113313"></a><a name="zh-cn_topic_0118184397_parmvalue73435113313"></a>“_”</span>，且长度为1~64个字符。默认与节点的名称一致。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184397_row224716257545"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184397_p99625062412"><a name="zh-cn_topic_0118184397_p99625062412"></a><a name="zh-cn_topic_0118184397_p99625062412"></a>作业运行资源</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184397_p596195011249"><a name="zh-cn_topic_0118184397_p596195011249"></a><a name="zh-cn_topic_0118184397_p596195011249"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184397_p149614505248"><a name="zh-cn_topic_0118184397_p149614505248"></a><a name="zh-cn_topic_0118184397_p149614505248"></a>选择作业运行的资源规格：</p>
<a name="zh-cn_topic_0118184397_ul192438361317"></a><a name="zh-cn_topic_0118184397_ul192438361317"></a><ul id="zh-cn_topic_0118184397_ul192438361317"><li>8核32G内存</li><li>16核64G内存</li><li>32核128G内存</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0118184397_row139701456248"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184397_p097024592410"><a name="zh-cn_topic_0118184397_p097024592410"></a><a name="zh-cn_topic_0118184397_p097024592410"></a>作业主类</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184397_p2097054592413"><a name="zh-cn_topic_0118184397_p2097054592413"></a><a name="zh-cn_topic_0118184397_p2097054592413"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184397_p16970174519242"><a name="zh-cn_topic_0118184397_p16970174519242"></a><a name="zh-cn_topic_0118184397_p16970174519242"></a>填写Spark作业的主类，即Jar包的主类。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184397_row12916917152512"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184397_p13916717132512"><a name="zh-cn_topic_0118184397_p13916717132512"></a><a name="zh-cn_topic_0118184397_p13916717132512"></a>Jar包资源</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184397_p4916181713257"><a name="zh-cn_topic_0118184397_p4916181713257"></a><a name="zh-cn_topic_0118184397_p4916181713257"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184397_p1191671719259"><a name="zh-cn_topic_0118184397_p1191671719259"></a><a name="zh-cn_topic_0118184397_p1191671719259"></a>选择Jar包，该Jar已上传至<a href="资源管理.md">资源管理</a>列表。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184397_row136501714122512"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184397_p56508140251"><a name="zh-cn_topic_0118184397_p56508140251"></a><a name="zh-cn_topic_0118184397_p56508140251"></a>主类入口参数</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184397_p1466513148250"><a name="zh-cn_topic_0118184397_p1466513148250"></a><a name="zh-cn_topic_0118184397_p1466513148250"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184397_p14665101482520"><a name="zh-cn_topic_0118184397_p14665101482520"></a><a name="zh-cn_topic_0118184397_p14665101482520"></a>填写程序的入口参数，参数之间使用Enter键分隔。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184397_row141411753202517"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184397_p7141195316258"><a name="zh-cn_topic_0118184397_p7141195316258"></a><a name="zh-cn_topic_0118184397_p7141195316258"></a>Spark作业运行参数</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184397_p1214195332511"><a name="zh-cn_topic_0118184397_p1214195332511"></a><a name="zh-cn_topic_0118184397_p1214195332511"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184397_p15141175310257"><a name="zh-cn_topic_0118184397_p15141175310257"></a><a name="zh-cn_topic_0118184397_p15141175310257"></a>填写Spark作业运行环境参数。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  高级参数

<a name="zh-cn_topic_0118184397_table58040457102411"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_row27216578102411"><th class="cellrowborder" valign="top" width="28.07%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p57059205102411"><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p57059205102411"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p57059205102411"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="15.659999999999998%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p58392901102411"><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p58392901102411"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p58392901102411"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="56.269999999999996%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p32204521102411"><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p32204521102411"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p32204521102411"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_row51612113175"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p416115112178"><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p416115112178"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p416115112178"></a>节点状态轮询时间（秒）</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p101615110176"><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p101615110176"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p101615110176"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p4161191101716"><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p4161191101716"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p4161191101716"></a>设置轮询时间（1~60秒），每隔x秒查询一次<span id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_text1526241235118"><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_text1526241235118"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_text1526241235118"></a>节点</span>是否执行完成。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_row5101045193916"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p147314419397"><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p147314419397"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p147314419397"></a>节点执行的最长时间</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p610124511390"><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p610124511390"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p610124511390"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p11011456393"><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p11011456393"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p11011456393"></a>设置<span id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_text380131541112"><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_text380131541112"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_text380131541112"></a>节点</span>执行的超时时间，如果<span id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_text1944213322118"><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_text1944213322118"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_text1944213322118"></a>节点</span>配置了重试，在超时时间内未执行完成，该节点将不会再重试，直接置为失败状态。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_row58429402102411"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p5533912102858"><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p5533912102858"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p5533912102858"></a>失败重试</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p45593742102858"><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p45593742102858"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p45593742102858"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p2105628102858"><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p2105628102858"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p2105628102858"></a><span id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_text29185571161243"><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_text29185571161243"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_text29185571161243"></a>节点</span>执行失败后，是否重新执行<span id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_text58583828161245"><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_text58583828161245"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_text58583828161245"></a>节点</span>。</p>
<a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_ul18950660102858"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_ul18950660102858"></a><ul id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_ul18950660102858"><li>是：重新执行<span id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_text19139245161248"><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_text19139245161248"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_text19139245161248"></a>节点</span>，请配置以下参数。<a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_ul58608523102858"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_ul58608523102858"></a><ul id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_ul58608523102858"><li>最大重试次数</li><li>重试间隔时间（秒）</li></ul>
</li><li>否：默认值，不重新执行<span id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_text1328324161254"><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_text1328324161254"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_text1328324161254"></a>节点</span>。</li></ul>
<div class="note" id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_note69071033105815"><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_note69071033105815"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_note69071033105815"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p1590733314581"><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p1590733314581"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p1590733314581"></a>如果作业节点配置了重试，并且配置了超时时间，该节点执行超时后将不会再重试，直接置为失败状态。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_row29541959102411"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p13154928102858"><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p13154928102858"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p13154928102858"></a>失败策略</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p58916261102858"><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p58916261102858"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p58916261102858"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p7487822102858"><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p7487822102858"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_p7487822102858"></a><span id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_text5371194616130"><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_text5371194616130"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_text5371194616130"></a>节点</span>执行失败后的操作：</p>
<a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_ul281538102858"></a><a name="zh-cn_topic_0118184397_zh-cn_topic_0099822521_ul281538102858"></a><ul id="zh-cn_topic_0118184397_zh-cn_topic_0099822521_ul281538102858"><li>终止当前作业执行计划</li><li>继续执行下一作业</li><li>挂起当前作业执行计划</li></ul>
</td>
</tr>
</tbody>
</table>

