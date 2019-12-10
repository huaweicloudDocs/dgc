# MRS Hive SQL<a name="dayu_01_0454"></a>

## 功能<a name="zh-cn_topic_0101095440_section44280035173841"></a>

通过MRS Hive SQL节点执行DLF中预先定义的Hive SQL脚本。

## 参数<a name="zh-cn_topic_0101095440_section1791764173933"></a>

用户可参考[表1](#zh-cn_topic_0101095440_table3764823994826)和[表2](#zh-cn_topic_0101095440_table58040457102411)配置MRS Hive SQL节点的参数。

**表 1**  属性参数

<a name="zh-cn_topic_0101095440_table3764823994826"></a>
<table><thead align="left"><tr id="zh-cn_topic_0101095440_row3170822394826"><th class="cellrowborder" valign="top" width="28.000000000000004%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0101095440_p2984581994826"><a name="zh-cn_topic_0101095440_p2984581994826"></a><a name="zh-cn_topic_0101095440_p2984581994826"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="16%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0101095440_p159227094826"><a name="zh-cn_topic_0101095440_p159227094826"></a><a name="zh-cn_topic_0101095440_p159227094826"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="56.00000000000001%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0101095440_p6186505494826"><a name="zh-cn_topic_0101095440_p6186505494826"></a><a name="zh-cn_topic_0101095440_p6186505494826"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0101095440_row303485991116"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0101095440_p65876130143546"><a name="zh-cn_topic_0101095440_p65876130143546"></a><a name="zh-cn_topic_0101095440_p65876130143546"></a>SQL脚本</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0101095440_p51613311116"><a name="zh-cn_topic_0101095440_p51613311116"></a><a name="zh-cn_topic_0101095440_p51613311116"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.00000000000001%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0101095440_p154146861116"><a name="zh-cn_topic_0101095440_p154146861116"></a><a name="zh-cn_topic_0101095440_p154146861116"></a>选择需要执行的脚本。如果脚本未创建，请参考<a href="新建脚本.md">新建脚本</a>和<a href="开发SQL脚本.md">开发SQL脚本</a>先创建和开发脚本。</p>
</td>
</tr>
<tr id="zh-cn_topic_0101095440_row553016425357"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0101095440_p983015394826"><a name="zh-cn_topic_0101095440_p983015394826"></a><a name="zh-cn_topic_0101095440_p983015394826"></a>数据连接</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0101095440_p5804493094826"><a name="zh-cn_topic_0101095440_p5804493094826"></a><a name="zh-cn_topic_0101095440_p5804493094826"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.00000000000001%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0101095440_p20781413102414"><a name="zh-cn_topic_0101095440_p20781413102414"></a><a name="zh-cn_topic_0101095440_p20781413102414"></a>默认选择SQL脚本中设置的数据连接，支持修改。</p>
</td>
</tr>
<tr id="zh-cn_topic_0101095440_row4695054111155"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0101095440_p4489744011155"><a name="zh-cn_topic_0101095440_p4489744011155"></a><a name="zh-cn_topic_0101095440_p4489744011155"></a>数据库</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0101095440_p1281406111155"><a name="zh-cn_topic_0101095440_p1281406111155"></a><a name="zh-cn_topic_0101095440_p1281406111155"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.00000000000001%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0101095440_p7610111714256"><a name="zh-cn_topic_0101095440_p7610111714256"></a><a name="zh-cn_topic_0101095440_p7610111714256"></a>默认选择SQL脚本中设置的数据库，支持修改。</p>
</td>
</tr>
<tr id="zh-cn_topic_0101095440_row959892418618"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0101095440_p55987241761"><a name="zh-cn_topic_0101095440_p55987241761"></a><a name="zh-cn_topic_0101095440_p55987241761"></a>脚本参数</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0101095440_p1259817247611"><a name="zh-cn_topic_0101095440_p1259817247611"></a><a name="zh-cn_topic_0101095440_p1259817247611"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="56.00000000000001%" headers="mcps1.2.4.1.3 "><p id="p1968518451852"><a name="p1968518451852"></a><a name="p1968518451852"></a>关联的SQL脚本如果使用了参数，此处显示参数名称，请在参数名称后的输入框配置参数值。参数值支持使用<a href="函数概述.md#dayu_01_0471">内置函数</a>和<a href="表达式概述.md#dayu_01_0494">EL表达式</a>。</p>
<p id="zh-cn_topic_0101095440_p1053415211393"><a name="zh-cn_topic_0101095440_p1053415211393"></a><a name="zh-cn_topic_0101095440_p1053415211393"></a>若关联的SQL脚本，脚本参数发生变化，可单击刷新按钮<a name="zh-cn_topic_0101095440_zh-cn_topic_0102588983_image83361028443"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0102588983_image83361028443"></a><span><img id="zh-cn_topic_0101095440_zh-cn_topic_0102588983_image83361028443" src="figures/zh-cn_image_0171784900.png"></span>同步。</p>
</td>
</tr>
<tr id="zh-cn_topic_0101095440_row184721543611"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0101095440_p246794194826"><a name="zh-cn_topic_0101095440_p246794194826"></a><a name="zh-cn_topic_0101095440_p246794194826"></a>节点名称</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0101095440_p6568554794826"><a name="zh-cn_topic_0101095440_p6568554794826"></a><a name="zh-cn_topic_0101095440_p6568554794826"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.00000000000001%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0101095440_p1780513175216"><a name="zh-cn_topic_0101095440_p1780513175216"></a><a name="zh-cn_topic_0101095440_p1780513175216"></a>默认显示为SQL脚本的名称，支持修改。规则如下：</p>
<p id="zh-cn_topic_0101095440_p1892909794826"><a name="zh-cn_topic_0101095440_p1892909794826"></a><a name="zh-cn_topic_0101095440_p1892909794826"></a><span id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_text44323307153939"><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_text44323307153939"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_text44323307153939"></a>节点</span>名称，可以包含中文、英文字母、数字、<span class="parmvalue" id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a>“_”</span>、<span class="parmvalue" id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a>“-”</span>、<span class="parmvalue" id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_parmvalue3773104413412"><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_parmvalue3773104413412"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_parmvalue3773104413412"></a>“/”</span>、<span class="parmvalue" id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a>“&lt;”</span>、<span class="parmvalue" id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a>“&gt;”</span>等各类特殊字符，长度为1～128个字符。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  高级参数

<a name="zh-cn_topic_0101095440_table58040457102411"></a>
<table><thead align="left"><tr id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_row27216578102411"><th class="cellrowborder" valign="top" width="28.07%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p57059205102411"><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p57059205102411"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p57059205102411"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="15.659999999999998%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p58392901102411"><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p58392901102411"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p58392901102411"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="56.269999999999996%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p32204521102411"><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p32204521102411"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p32204521102411"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_row51612113175"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p416115112178"><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p416115112178"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p416115112178"></a>节点状态轮询时间（秒）</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p101615110176"><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p101615110176"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p101615110176"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p4161191101716"><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p4161191101716"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p4161191101716"></a>设置轮询时间（1~60秒），每隔x秒查询一次<span id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_text1526241235118"><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_text1526241235118"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_text1526241235118"></a>节点</span>是否执行完成。</p>
</td>
</tr>
<tr id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_row5101045193916"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p147314419397"><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p147314419397"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p147314419397"></a>节点执行的最长时间</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p610124511390"><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p610124511390"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p610124511390"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p11011456393"><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p11011456393"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p11011456393"></a>设置<span id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_text380131541112"><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_text380131541112"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_text380131541112"></a>节点</span>执行的超时时间，如果<span id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_text1944213322118"><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_text1944213322118"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_text1944213322118"></a>节点</span>配置了重试，在超时时间内未执行完成，该节点将不会再重试，直接置为失败状态。</p>
</td>
</tr>
<tr id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_row58429402102411"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p5533912102858"><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p5533912102858"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p5533912102858"></a>失败重试</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p45593742102858"><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p45593742102858"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p45593742102858"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p2105628102858"><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p2105628102858"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p2105628102858"></a><span id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_text29185571161243"><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_text29185571161243"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_text29185571161243"></a>节点</span>执行失败后，是否重新执行<span id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_text58583828161245"><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_text58583828161245"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_text58583828161245"></a>节点</span>。</p>
<a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_ul18950660102858"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_ul18950660102858"></a><ul id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_ul18950660102858"><li>是：重新执行<span id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_text19139245161248"><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_text19139245161248"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_text19139245161248"></a>节点</span>，请配置以下参数。<a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_ul58608523102858"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_ul58608523102858"></a><ul id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_ul58608523102858"><li>最大重试次数</li><li>重试间隔时间（秒）</li></ul>
</li><li>否：默认值，不重新执行<span id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_text1328324161254"><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_text1328324161254"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_text1328324161254"></a>节点</span>。</li></ul>
<div class="note" id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_note69071033105815"><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_note69071033105815"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_note69071033105815"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p1590733314581"><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p1590733314581"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p1590733314581"></a>如果作业节点配置了重试，并且配置了超时时间，该节点执行超时后将不会再重试，直接置为失败状态。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_row29541959102411"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p13154928102858"><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p13154928102858"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p13154928102858"></a>失败策略</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p58916261102858"><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p58916261102858"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p58916261102858"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p7487822102858"><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p7487822102858"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_p7487822102858"></a><span id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_text5371194616130"><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_text5371194616130"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_text5371194616130"></a>节点</span>执行失败后的操作：</p>
<a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_ul281538102858"></a><a name="zh-cn_topic_0101095440_zh-cn_topic_0099822521_ul281538102858"></a><ul id="zh-cn_topic_0101095440_zh-cn_topic_0099822521_ul281538102858"><li>终止当前作业执行计划</li><li>继续执行下一作业</li><li>挂起当前作业执行计划</li></ul>
</td>
</tr>
</tbody>
</table>

