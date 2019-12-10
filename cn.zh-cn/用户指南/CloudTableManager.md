# CloudTableManager<a name="dayu_01_0466"></a>

## 功能<a name="zh-cn_topic_0135911440_section44280035173841"></a>

通过CloudTableManager节点新建或删除一个CloudTable表。

## 参数<a name="zh-cn_topic_0135911440_section6331447317395"></a>

用户可参考[表1](#zh-cn_topic_0135911440_table3764823994826)和[表2](#zh-cn_topic_0135911440_table58040457102411)配置CloudTableManager节点的参数。

**表 1**  属性参数

<a name="zh-cn_topic_0135911440_table3764823994826"></a>
<table><thead align="left"><tr id="zh-cn_topic_0135911440_row3170822394826"><th class="cellrowborder" valign="top" width="28.07%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0135911440_p2984581994826"><a name="zh-cn_topic_0135911440_p2984581994826"></a><a name="zh-cn_topic_0135911440_p2984581994826"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="15.659999999999998%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0135911440_p159227094826"><a name="zh-cn_topic_0135911440_p159227094826"></a><a name="zh-cn_topic_0135911440_p159227094826"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="56.269999999999996%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0135911440_p6186505494826"><a name="zh-cn_topic_0135911440_p6186505494826"></a><a name="zh-cn_topic_0135911440_p6186505494826"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0135911440_row2453112011566"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0135911440_p246794194826"><a name="zh-cn_topic_0135911440_p246794194826"></a><a name="zh-cn_topic_0135911440_p246794194826"></a>节点名称</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0135911440_p6568554794826"><a name="zh-cn_topic_0135911440_p6568554794826"></a><a name="zh-cn_topic_0135911440_p6568554794826"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0135911440_p1892909794826"><a name="zh-cn_topic_0135911440_p1892909794826"></a><a name="zh-cn_topic_0135911440_p1892909794826"></a><span id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_text44323307153939"><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_text44323307153939"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_text44323307153939"></a>节点</span>名称，可以包含中文、英文字母、数字、<span class="parmvalue" id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a>“_”</span>、<span class="parmvalue" id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a>“-”</span>、<span class="parmvalue" id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_parmvalue3773104413412"><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_parmvalue3773104413412"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_parmvalue3773104413412"></a>“/”</span>、<span class="parmvalue" id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a>“&lt;”</span>、<span class="parmvalue" id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a>“&gt;”</span>等各类特殊字符，长度为1～128个字符。</p>
</td>
</tr>
<tr id="zh-cn_topic_0135911440_row047514818260"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0135911440_p34751148142615"><a name="zh-cn_topic_0135911440_p34751148142615"></a><a name="zh-cn_topic_0135911440_p34751148142615"></a>CloudTable集群名</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0135911440_p1947504832610"><a name="zh-cn_topic_0135911440_p1947504832610"></a><a name="zh-cn_topic_0135911440_p1947504832610"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0135911440_p947534862619"><a name="zh-cn_topic_0135911440_p947534862619"></a><a name="zh-cn_topic_0135911440_p947534862619"></a>选择或输入CloudTable集群，输入集群名称时支持引用作业参数和使用EL表达式（参见<a href="表达式概述.md#dayu_01_0494">表达式概述</a>）。</p>
</td>
</tr>
<tr id="zh-cn_topic_0135911440_row6435347490"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0135911440_p19431134104910"><a name="zh-cn_topic_0135911440_p19431134104910"></a><a name="zh-cn_topic_0135911440_p19431134104910"></a>命名空间</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0135911440_p243193418494"><a name="zh-cn_topic_0135911440_p243193418494"></a><a name="zh-cn_topic_0135911440_p243193418494"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0135911440_p743173444910"><a name="zh-cn_topic_0135911440_p743173444910"></a><a name="zh-cn_topic_0135911440_p743173444910"></a>选择或输入命名空间，输入命名空间名称时支持引用作业参数和使用EL表达式（参见<a href="表达式概述.md#dayu_01_0494">表达式概述</a>）。</p>
</td>
</tr>
<tr id="zh-cn_topic_0135911440_row690273114917"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0135911440_p199021731154914"><a name="zh-cn_topic_0135911440_p199021731154914"></a><a name="zh-cn_topic_0135911440_p199021731154914"></a>表操作</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0135911440_p1902173110492"><a name="zh-cn_topic_0135911440_p1902173110492"></a><a name="zh-cn_topic_0135911440_p1902173110492"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0135911440_p199022312496"><a name="zh-cn_topic_0135911440_p199022312496"></a><a name="zh-cn_topic_0135911440_p199022312496"></a>选择新建或删除数据表：</p>
<a name="zh-cn_topic_0135911440_ul156601100511"></a><a name="zh-cn_topic_0135911440_ul156601100511"></a><ul id="zh-cn_topic_0135911440_ul156601100511"><li>CREATE</li><li>DELETE</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0135911440_row946511292492"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0135911440_p13465929194910"><a name="zh-cn_topic_0135911440_p13465929194910"></a><a name="zh-cn_topic_0135911440_p13465929194910"></a>表名</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0135911440_p146542924914"><a name="zh-cn_topic_0135911440_p146542924914"></a><a name="zh-cn_topic_0135911440_p146542924914"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0135911440_p646572944920"><a name="zh-cn_topic_0135911440_p646572944920"></a><a name="zh-cn_topic_0135911440_p646572944920"></a>输入数据表的名称。</p>
</td>
</tr>
<tr id="zh-cn_topic_0135911440_row1041882354915"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0135911440_p1741818232498"><a name="zh-cn_topic_0135911440_p1741818232498"></a><a name="zh-cn_topic_0135911440_p1741818232498"></a>列族名</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0135911440_p741818230492"><a name="zh-cn_topic_0135911440_p741818230492"></a><a name="zh-cn_topic_0135911440_p741818230492"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0135911440_p12418122311491"><a name="zh-cn_topic_0135911440_p12418122311491"></a><a name="zh-cn_topic_0135911440_p12418122311491"></a>输入列族名称，多个列族之间使用英文逗号（,）间隔。当<span class="parmname" id="zh-cn_topic_0135911440_parmname991165195313"><a name="zh-cn_topic_0135911440_parmname991165195313"></a><a name="zh-cn_topic_0135911440_parmname991165195313"></a>“表操作”</span>选择<span class="parmvalue" id="zh-cn_topic_0135911440_parmvalue62161910535"><a name="zh-cn_topic_0135911440_parmvalue62161910535"></a><a name="zh-cn_topic_0135911440_parmvalue62161910535"></a>“CREATE”</span>时，显示该配置项。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  高级参数

<a name="zh-cn_topic_0135911440_table58040457102411"></a>
<table><thead align="left"><tr id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_row27216578102411"><th class="cellrowborder" valign="top" width="28.07%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p57059205102411"><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p57059205102411"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p57059205102411"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="15.659999999999998%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p58392901102411"><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p58392901102411"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p58392901102411"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="56.269999999999996%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p32204521102411"><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p32204521102411"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p32204521102411"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_row51612113175"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p416115112178"><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p416115112178"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p416115112178"></a>节点状态轮询时间（秒）</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p101615110176"><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p101615110176"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p101615110176"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p4161191101716"><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p4161191101716"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p4161191101716"></a>设置轮询时间（1~60秒），每隔x秒查询一次<span id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_text1526241235118"><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_text1526241235118"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_text1526241235118"></a>节点</span>是否执行完成。</p>
</td>
</tr>
<tr id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_row5101045193916"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p147314419397"><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p147314419397"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p147314419397"></a>节点执行的最长时间</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p610124511390"><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p610124511390"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p610124511390"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p11011456393"><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p11011456393"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p11011456393"></a>设置<span id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_text380131541112"><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_text380131541112"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_text380131541112"></a>节点</span>执行的超时时间，如果<span id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_text1944213322118"><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_text1944213322118"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_text1944213322118"></a>节点</span>配置了重试，在超时时间内未执行完成，该节点将不会再重试，直接置为失败状态。</p>
</td>
</tr>
<tr id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_row58429402102411"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p5533912102858"><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p5533912102858"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p5533912102858"></a>失败重试</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p45593742102858"><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p45593742102858"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p45593742102858"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p2105628102858"><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p2105628102858"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p2105628102858"></a><span id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_text29185571161243"><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_text29185571161243"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_text29185571161243"></a>节点</span>执行失败后，是否重新执行<span id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_text58583828161245"><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_text58583828161245"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_text58583828161245"></a>节点</span>。</p>
<a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_ul18950660102858"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_ul18950660102858"></a><ul id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_ul18950660102858"><li>是：重新执行<span id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_text19139245161248"><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_text19139245161248"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_text19139245161248"></a>节点</span>，请配置以下参数。<a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_ul58608523102858"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_ul58608523102858"></a><ul id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_ul58608523102858"><li>最大重试次数</li><li>重试间隔时间（秒）</li></ul>
</li><li>否：默认值，不重新执行<span id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_text1328324161254"><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_text1328324161254"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_text1328324161254"></a>节点</span>。</li></ul>
<div class="note" id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_note69071033105815"><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_note69071033105815"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_note69071033105815"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p1590733314581"><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p1590733314581"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p1590733314581"></a>如果作业节点配置了重试，并且配置了超时时间，该节点执行超时后将不会再重试，直接置为失败状态。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_row29541959102411"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p13154928102858"><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p13154928102858"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p13154928102858"></a>失败策略</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p58916261102858"><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p58916261102858"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p58916261102858"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p7487822102858"><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p7487822102858"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_p7487822102858"></a><span id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_text5371194616130"><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_text5371194616130"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_text5371194616130"></a>节点</span>执行失败后的操作：</p>
<a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_ul281538102858"></a><a name="zh-cn_topic_0135911440_zh-cn_topic_0099822521_ul281538102858"></a><ul id="zh-cn_topic_0135911440_zh-cn_topic_0099822521_ul281538102858"><li>终止当前作业执行计划</li><li>继续执行下一作业</li><li>挂起当前作业执行计划</li></ul>
</td>
</tr>
</tbody>
</table>

