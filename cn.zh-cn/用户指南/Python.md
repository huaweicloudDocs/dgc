# Python<a name="dgc_01_4504"></a>

## 功能<a name="section1329216425362"></a>

通过Python节点执行Python语句。

## 参数<a name="section7394398377"></a>

用户可以参考[表1](#zh-cn_topic_0113842761_table3764823994826)和[表2](#table1396374719116)配置Python节点的参数。

**表 1**  属性参数

<a name="zh-cn_topic_0113842761_table3764823994826"></a>
<table><thead align="left"><tr id="zh-cn_topic_0113842761_row3170822394826"><th class="cellrowborder" valign="top" width="21.42%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0113842761_p2984581994826"><a name="zh-cn_topic_0113842761_p2984581994826"></a><a name="zh-cn_topic_0113842761_p2984581994826"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="10.13%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0113842761_p159227094826"><a name="zh-cn_topic_0113842761_p159227094826"></a><a name="zh-cn_topic_0113842761_p159227094826"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="68.45%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0113842761_p6186505494826"><a name="zh-cn_topic_0113842761_p6186505494826"></a><a name="zh-cn_topic_0113842761_p6186505494826"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0113842761_row3614415394826"><td class="cellrowborder" valign="top" width="21.42%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0113842761_p1225314550306"><a name="zh-cn_topic_0113842761_p1225314550306"></a><a name="zh-cn_topic_0113842761_p1225314550306"></a>SQL或脚本</p>
</td>
<td class="cellrowborder" valign="top" width="10.13%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0113842761_p4617707494826"><a name="zh-cn_topic_0113842761_p4617707494826"></a><a name="zh-cn_topic_0113842761_p4617707494826"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="68.45%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0113842761_p61023369712"><a name="zh-cn_topic_0113842761_p61023369712"></a><a name="zh-cn_topic_0113842761_p61023369712"></a>可以选择SQL语句或SQL脚本。</p>
<a name="zh-cn_topic_0113842761_ul1857020154912"></a><a name="zh-cn_topic_0113842761_ul1857020154912"></a><ul id="zh-cn_topic_0113842761_ul1857020154912"><li>SQL语句<p id="zh-cn_topic_0113842761_p74181856897"><a name="zh-cn_topic_0113842761_p74181856897"></a><a name="zh-cn_topic_0113842761_p74181856897"></a>单击<span class="parmname" id="zh-cn_topic_0113842761_parmname116422231331"><a name="zh-cn_topic_0113842761_parmname116422231331"></a><a name="zh-cn_topic_0113842761_parmname116422231331"></a>“SQL语句”</span>参数下的文本框，在<span class="wintitle" id="zh-cn_topic_0113842761_wintitle28741019181110"><a name="zh-cn_topic_0113842761_wintitle28741019181110"></a><a name="zh-cn_topic_0113842761_wintitle28741019181110"></a>“SQL语句”</span>页面输入需要执行的SQL语句。</p>
</li><li>SQL脚本<p id="zh-cn_topic_0113842761_p310193912912"><a name="zh-cn_topic_0113842761_p310193912912"></a><a name="zh-cn_topic_0113842761_p310193912912"></a>在<span class="parmname" id="zh-cn_topic_0113842761_parmname18319357534"><a name="zh-cn_topic_0113842761_parmname18319357534"></a><a name="zh-cn_topic_0113842761_parmname18319357534"></a>“脚本路径”</span>参数后选择需要执行的脚本。如果脚本未创建，请参考<a href="新建脚本.md">新建脚本</a>和<a href="开发SQL脚本.md">开发SQL脚本</a>先创建和开发脚本。</p>
<div class="note" id="zh-cn_topic_0113842761_note15529154994813"><a name="zh-cn_topic_0113842761_note15529154994813"></a><a name="zh-cn_topic_0113842761_note15529154994813"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0113842761_p18530849164811"><a name="zh-cn_topic_0113842761_p18530849164811"></a><a name="zh-cn_topic_0113842761_p18530849164811"></a>若选择SQL语句方式，数据开发模块将无法解析您输入SQL语句中携带的参数。</p>
</div></div>
</li></ul>
</td>
</tr>
<tr id="row16123141615518"><td class="cellrowborder" valign="top" width="21.42%" headers="mcps1.2.4.1.1 "><p id="p123762216510"><a name="p123762216510"></a><a name="p123762216510"></a>主机连接</p>
</td>
<td class="cellrowborder" valign="top" width="10.13%" headers="mcps1.2.4.1.2 "><p id="p212441612515"><a name="p212441612515"></a><a name="p212441612515"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="68.45%" headers="mcps1.2.4.1.3 "><p id="p1124716052"><a name="p1124716052"></a><a name="p1124716052"></a>选择执行Python语句的主机。</p>
</td>
</tr>
<tr id="row1246614521252"><td class="cellrowborder" valign="top" width="21.42%" headers="mcps1.2.4.1.1 "><p id="p154660528513"><a name="p154660528513"></a><a name="p154660528513"></a>参数</p>
</td>
<td class="cellrowborder" valign="top" width="10.13%" headers="mcps1.2.4.1.2 "><p id="p1846610521056"><a name="p1846610521056"></a><a name="p1846610521056"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="68.45%" headers="mcps1.2.4.1.3 "><p id="p1846645219518"><a name="p1846645219518"></a><a name="p1846645219518"></a>填写执行Python语句时，向语句传递的参数，参数之间使用空格分隔，例如：a b c。此处的“参数”需要在Python语句中引用，否则配置无效。</p>
</td>
</tr>
<tr id="row63090551455"><td class="cellrowborder" valign="top" width="21.42%" headers="mcps1.2.4.1.1 "><p id="p1419619411610"><a name="p1419619411610"></a><a name="p1419619411610"></a>交互式输入</p>
</td>
<td class="cellrowborder" valign="top" width="10.13%" headers="mcps1.2.4.1.2 "><p id="p73092556515"><a name="p73092556515"></a><a name="p73092556515"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="68.45%" headers="mcps1.2.4.1.3 "><p id="p1030919551653"><a name="p1030919551653"></a><a name="p1030919551653"></a>填写交互式参数，即执行Python语句的过程中，需要用户输入的交互式信息（例如密码）。交互式参数之间以回车符分隔，Python语句根据交互情况按顺序读取参数值。</p>
</td>
</tr>
<tr id="zh-cn_topic_0113842761_row173916552814"><td class="cellrowborder" valign="top" width="21.42%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0113842761_p246794194826"><a name="zh-cn_topic_0113842761_p246794194826"></a><a name="zh-cn_topic_0113842761_p246794194826"></a>节点名称</p>
</td>
<td class="cellrowborder" valign="top" width="10.13%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0113842761_p6568554794826"><a name="zh-cn_topic_0113842761_p6568554794826"></a><a name="zh-cn_topic_0113842761_p6568554794826"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="68.45%" headers="mcps1.2.4.1.3 "><p id="p14740112265412"><a name="p14740112265412"></a><a name="p14740112265412"></a>节点名称，只能包含英文字母、数字、中文字符、中划线、下划线、/、&lt;&gt;和点号，且长度小于等于128个字符。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  高级参数

<a name="table1396374719116"></a>
<table><thead align="left"><tr id="row1796319476113"><th class="cellrowborder" valign="top" width="21.25212521252125%" id="mcps1.2.4.1.1"><p id="p840010520115"><a name="p840010520115"></a><a name="p840010520115"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="10.21102110211021%" id="mcps1.2.4.1.2"><p id="p0138205521115"><a name="p0138205521115"></a><a name="p0138205521115"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="68.53685368536854%" id="mcps1.2.4.1.3"><p id="p936835951120"><a name="p936835951120"></a><a name="p936835951120"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row129636473111"><td class="cellrowborder" valign="top" width="21.25212521252125%" headers="mcps1.2.4.1.1 "><p id="p18560332181218"><a name="p18560332181218"></a><a name="p18560332181218"></a>节点状态轮询时间（秒）</p>
</td>
<td class="cellrowborder" valign="top" width="10.21102110211021%" headers="mcps1.2.4.1.2 "><p id="p15605324129"><a name="p15605324129"></a><a name="p15605324129"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="68.53685368536854%" headers="mcps1.2.4.1.3 "><p id="p1456020328128"><a name="p1456020328128"></a><a name="p1456020328128"></a>设置轮询时间（1~60秒），每隔x秒查询一次节点是否执行完成。</p>
</td>
</tr>
<tr id="row119631347191118"><td class="cellrowborder" valign="top" width="21.25212521252125%" headers="mcps1.2.4.1.1 "><p id="p1256014328127"><a name="p1256014328127"></a><a name="p1256014328127"></a>节点执行的最长时间</p>
</td>
<td class="cellrowborder" valign="top" width="10.21102110211021%" headers="mcps1.2.4.1.2 "><p id="p16560153213122"><a name="p16560153213122"></a><a name="p16560153213122"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="68.53685368536854%" headers="mcps1.2.4.1.3 "><p id="p1556013321125"><a name="p1556013321125"></a><a name="p1556013321125"></a>设置节点执行的超时时间，如果节点配置了重试，在超时时间内未执行完成，该节点将不会再重试，直接置为失败状态。</p>
</td>
</tr>
<tr id="row14782172511219"><td class="cellrowborder" valign="top" width="21.25212521252125%" headers="mcps1.2.4.1.1 "><p id="p1956019328128"><a name="p1956019328128"></a><a name="p1956019328128"></a>失败重试</p>
</td>
<td class="cellrowborder" valign="top" width="10.21102110211021%" headers="mcps1.2.4.1.2 "><p id="p25603327128"><a name="p25603327128"></a><a name="p25603327128"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="68.53685368536854%" headers="mcps1.2.4.1.3 "><p id="p856020329128"><a name="p856020329128"></a><a name="p856020329128"></a>节点执行失败后，是否重新执行节点。</p>
<a name="ul18560193271216"></a><a name="ul18560193271216"></a><ul id="ul18560193271216"><li>是：重新执行节点，请配置以下参数。<a name="ul35605321129"></a><a name="ul35605321129"></a><ul id="ul35605321129"><li>最大重试次数</li><li>重试间隔时间（秒）</li></ul>
</li><li>否：默认值，不重新执行节点。</li></ul>
<div class="note" id="note163026610143"><a name="note163026610143"></a><a name="note163026610143"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p1302196121412"><a name="p1302196121412"></a><a name="p1302196121412"></a>如果作业节点配置了重试，并且配置了超时时间，该节点执行超时后将不会再重试，直接置为失败状态。</p>
</div></div>
</td>
</tr>
<tr id="row4328328131210"><td class="cellrowborder" valign="top" width="21.25212521252125%" headers="mcps1.2.4.1.1 "><p id="p195601532191219"><a name="p195601532191219"></a><a name="p195601532191219"></a>失败策略</p>
</td>
<td class="cellrowborder" valign="top" width="10.21102110211021%" headers="mcps1.2.4.1.2 "><p id="p6560732101218"><a name="p6560732101218"></a><a name="p6560732101218"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="68.53685368536854%" headers="mcps1.2.4.1.3 "><p id="p35601432161212"><a name="p35601432161212"></a><a name="p35601432161212"></a>节点执行失败后的操作：</p>
<a name="ul145601832131210"></a><a name="ul145601832131210"></a><ul id="ul145601832131210"><li>终止当前作业执行计划</li><li>继续执行下一作业</li><li>挂起当前作业执行计划</li><li>终止后续节点执行计划</li></ul>
</td>
</tr>
</tbody>
</table>

