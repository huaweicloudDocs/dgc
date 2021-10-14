# Sub Job<a name="dgc_01_0467"></a>

## 功能<a name="zh-cn_topic_0157404961_section19542113151719"></a>

通过Sub Job节点可以调用另外一个批处理作业。

## 参数<a name="zh-cn_topic_0157404961_section55641359184"></a>

用户可参考[表1](#zh-cn_topic_0157404961_table3764823994826)和[表2](#zh-cn_topic_0157404961_table58040457102411)配置Sub Job节点的参数。

**表 1**  属性参数

<a name="zh-cn_topic_0157404961_table3764823994826"></a>
<table><thead align="left"><tr id="zh-cn_topic_0157404961_row3170822394826"><th class="cellrowborder" valign="top" width="21.86%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0157404961_p2984581994826"><a name="zh-cn_topic_0157404961_p2984581994826"></a><a name="zh-cn_topic_0157404961_p2984581994826"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="10.040000000000001%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0157404961_p159227094826"><a name="zh-cn_topic_0157404961_p159227094826"></a><a name="zh-cn_topic_0157404961_p159227094826"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="68.10000000000001%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0157404961_p6186505494826"><a name="zh-cn_topic_0157404961_p6186505494826"></a><a name="zh-cn_topic_0157404961_p6186505494826"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0157404961_row1991457694826"><td class="cellrowborder" valign="top" width="21.86%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0157404961_p246794194826"><a name="zh-cn_topic_0157404961_p246794194826"></a><a name="zh-cn_topic_0157404961_p246794194826"></a>节点名称</p>
</td>
<td class="cellrowborder" valign="top" width="10.040000000000001%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0157404961_p6568554794826"><a name="zh-cn_topic_0157404961_p6568554794826"></a><a name="zh-cn_topic_0157404961_p6568554794826"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="68.10000000000001%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0157404961_p1892909794826"><a name="zh-cn_topic_0157404961_p1892909794826"></a><a name="zh-cn_topic_0157404961_p1892909794826"></a><span id="zh-cn_topic_0099822521_text44323307153939"><a name="zh-cn_topic_0099822521_text44323307153939"></a><a name="zh-cn_topic_0099822521_text44323307153939"></a>节点</span>名称，可以包含中文、英文字母、数字、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a>“_”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a>“-”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_parmvalue3773104413412"><a name="zh-cn_topic_0099822521_parmvalue3773104413412"></a><a name="zh-cn_topic_0099822521_parmvalue3773104413412"></a>“/”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a>“&lt;”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a>“&gt;”</span>等各类特殊字符，长度为1～128个字符。</p>
</td>
</tr>
<tr id="zh-cn_topic_0157404961_row824216571514"><td class="cellrowborder" valign="top" width="21.86%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0157404961_p1143912012225"><a name="zh-cn_topic_0157404961_p1143912012225"></a><a name="zh-cn_topic_0157404961_p1143912012225"></a>子作业名称</p>
</td>
<td class="cellrowborder" valign="top" width="10.040000000000001%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0157404961_p9438150152210"><a name="zh-cn_topic_0157404961_p9438150152210"></a><a name="zh-cn_topic_0157404961_p9438150152210"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="68.10000000000001%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0157404961_p9437901223"><a name="zh-cn_topic_0157404961_p9437901223"></a><a name="zh-cn_topic_0157404961_p9437901223"></a>选择需要调用的子作业名称。</p>
<div class="note" id="zh-cn_topic_0157404961_note1524524523816"><a name="zh-cn_topic_0157404961_note1524524523816"></a><a name="zh-cn_topic_0157404961_note1524524523816"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0157404961_p1024511457386"><a name="zh-cn_topic_0157404961_p1024511457386"></a><a name="zh-cn_topic_0157404961_p1024511457386"></a>您只能选择已存在的批处理作业名称，此批处理作业不能为作业本身，并且该批处理作业为不包含Sub Job节点的作业。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0157404961_row19710715192314"><td class="cellrowborder" valign="top" width="21.86%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0157404961_p67111615142312"><a name="zh-cn_topic_0157404961_p67111615142312"></a><a name="zh-cn_topic_0157404961_p67111615142312"></a>子作业参数名称</p>
</td>
<td class="cellrowborder" valign="top" width="10.040000000000001%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0157404961_p471171592313"><a name="zh-cn_topic_0157404961_p471171592313"></a><a name="zh-cn_topic_0157404961_p471171592313"></a>是/否</p>
</td>
<td class="cellrowborder" valign="top" width="68.10000000000001%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0157404961_ul1619814105495"></a><a name="zh-cn_topic_0157404961_ul1619814105495"></a><ul id="zh-cn_topic_0157404961_ul1619814105495"><li>当节点属性中子作业参数配置为空时，子作业使用自身参数变量执行。父作业的<span class="parmname" id="zh-cn_topic_0157404961_parmname2952112184912"><a name="zh-cn_topic_0157404961_parmname2952112184912"></a><a name="zh-cn_topic_0157404961_parmname2952112184912"></a>“子作业参数名称”</span>不显现。</li><li>当节点属性中子作业参数配置了数据时，子作业将使用配置参数变量执行。此时父作业的<span class="parmname" id="zh-cn_topic_0157404961_parmname1838619044919"><a name="zh-cn_topic_0157404961_parmname1838619044919"></a><a name="zh-cn_topic_0157404961_parmname1838619044919"></a>“子作业参数名称”</span>显现，并且节点属性中子作业参数配置的数据或者EL表达式，将根据父作业的环境变量读取替换。</li></ul>
</td>
</tr>
</tbody>
</table>

**表 2**  高级参数

<a name="zh-cn_topic_0157404961_table58040457102411"></a>
<table><thead align="left"><tr id="zh-cn_topic_0099822521_row27216578102411"><th class="cellrowborder" valign="top" width="21.58%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0099822521_p57059205102411"><a name="zh-cn_topic_0099822521_p57059205102411"></a><a name="zh-cn_topic_0099822521_p57059205102411"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="10.14%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0099822521_p58392901102411"><a name="zh-cn_topic_0099822521_p58392901102411"></a><a name="zh-cn_topic_0099822521_p58392901102411"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="68.28%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0099822521_p32204521102411"><a name="zh-cn_topic_0099822521_p32204521102411"></a><a name="zh-cn_topic_0099822521_p32204521102411"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0099822521_row51612113175"><td class="cellrowborder" valign="top" width="21.58%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0099822521_p416115112178"><a name="zh-cn_topic_0099822521_p416115112178"></a><a name="zh-cn_topic_0099822521_p416115112178"></a>节点状态轮询时间（秒）</p>
</td>
<td class="cellrowborder" valign="top" width="10.14%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0099822521_p101615110176"><a name="zh-cn_topic_0099822521_p101615110176"></a><a name="zh-cn_topic_0099822521_p101615110176"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="68.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0099822521_p4161191101716"><a name="zh-cn_topic_0099822521_p4161191101716"></a><a name="zh-cn_topic_0099822521_p4161191101716"></a>设置轮询时间（1~60秒），每隔x秒查询一次<span id="zh-cn_topic_0099822521_text1526241235118"><a name="zh-cn_topic_0099822521_text1526241235118"></a><a name="zh-cn_topic_0099822521_text1526241235118"></a>节点</span>是否执行完成。</p>
</td>
</tr>
<tr id="zh-cn_topic_0099822521_row5101045193916"><td class="cellrowborder" valign="top" width="21.58%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0099822521_p147314419397"><a name="zh-cn_topic_0099822521_p147314419397"></a><a name="zh-cn_topic_0099822521_p147314419397"></a>节点执行的最长时间</p>
</td>
<td class="cellrowborder" valign="top" width="10.14%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0099822521_p610124511390"><a name="zh-cn_topic_0099822521_p610124511390"></a><a name="zh-cn_topic_0099822521_p610124511390"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="68.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0099822521_p11011456393"><a name="zh-cn_topic_0099822521_p11011456393"></a><a name="zh-cn_topic_0099822521_p11011456393"></a>设置<span id="zh-cn_topic_0099822521_text380131541112"><a name="zh-cn_topic_0099822521_text380131541112"></a><a name="zh-cn_topic_0099822521_text380131541112"></a>节点</span>执行的超时时间，如果<span id="zh-cn_topic_0099822521_text1944213322118"><a name="zh-cn_topic_0099822521_text1944213322118"></a><a name="zh-cn_topic_0099822521_text1944213322118"></a>节点</span>配置了重试，在超时时间内未执行完成，该节点将不会再重试，直接置为失败状态。</p>
</td>
</tr>
<tr id="zh-cn_topic_0099822521_row58429402102411"><td class="cellrowborder" valign="top" width="21.58%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0099822521_p5533912102858"><a name="zh-cn_topic_0099822521_p5533912102858"></a><a name="zh-cn_topic_0099822521_p5533912102858"></a>失败重试</p>
</td>
<td class="cellrowborder" valign="top" width="10.14%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0099822521_p45593742102858"><a name="zh-cn_topic_0099822521_p45593742102858"></a><a name="zh-cn_topic_0099822521_p45593742102858"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="68.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0099822521_p2105628102858"><a name="zh-cn_topic_0099822521_p2105628102858"></a><a name="zh-cn_topic_0099822521_p2105628102858"></a><span id="zh-cn_topic_0099822521_text29185571161243"><a name="zh-cn_topic_0099822521_text29185571161243"></a><a name="zh-cn_topic_0099822521_text29185571161243"></a>节点</span>执行失败后，是否重新执行<span id="zh-cn_topic_0099822521_text58583828161245"><a name="zh-cn_topic_0099822521_text58583828161245"></a><a name="zh-cn_topic_0099822521_text58583828161245"></a>节点</span>。</p>
<a name="zh-cn_topic_0099822521_ul18950660102858"></a><a name="zh-cn_topic_0099822521_ul18950660102858"></a><ul id="zh-cn_topic_0099822521_ul18950660102858"><li>是：重新执行<span id="zh-cn_topic_0099822521_text19139245161248"><a name="zh-cn_topic_0099822521_text19139245161248"></a><a name="zh-cn_topic_0099822521_text19139245161248"></a>节点</span>，请配置以下参数。<a name="zh-cn_topic_0099822521_ul58608523102858"></a><a name="zh-cn_topic_0099822521_ul58608523102858"></a><ul id="zh-cn_topic_0099822521_ul58608523102858"><li>最大重试次数</li><li>重试间隔时间（秒）</li></ul>
</li><li>否：默认值，不重新执行<span id="zh-cn_topic_0099822521_text1328324161254"><a name="zh-cn_topic_0099822521_text1328324161254"></a><a name="zh-cn_topic_0099822521_text1328324161254"></a>节点</span>。</li></ul>
<div class="note" id="zh-cn_topic_0099822521_note69071033105815"><a name="zh-cn_topic_0099822521_note69071033105815"></a><a name="zh-cn_topic_0099822521_note69071033105815"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0099822521_p1590733314581"><a name="zh-cn_topic_0099822521_p1590733314581"></a><a name="zh-cn_topic_0099822521_p1590733314581"></a>如果作业节点配置了重试，并且配置了超时时间，该节点执行超时后将不会再重试，直接置为失败状态。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0099822521_row29541959102411"><td class="cellrowborder" valign="top" width="21.58%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0099822521_p13154928102858"><a name="zh-cn_topic_0099822521_p13154928102858"></a><a name="zh-cn_topic_0099822521_p13154928102858"></a>失败策略</p>
</td>
<td class="cellrowborder" valign="top" width="10.14%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0099822521_p58916261102858"><a name="zh-cn_topic_0099822521_p58916261102858"></a><a name="zh-cn_topic_0099822521_p58916261102858"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="68.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0099822521_p7487822102858"><a name="zh-cn_topic_0099822521_p7487822102858"></a><a name="zh-cn_topic_0099822521_p7487822102858"></a><span id="zh-cn_topic_0099822521_text5371194616130"><a name="zh-cn_topic_0099822521_text5371194616130"></a><a name="zh-cn_topic_0099822521_text5371194616130"></a>节点</span>执行失败后的操作：</p>
<a name="zh-cn_topic_0099822521_ul281538102858"></a><a name="zh-cn_topic_0099822521_ul281538102858"></a><ul id="zh-cn_topic_0099822521_ul281538102858"><li>终止当前作业执行计划</li><li>继续执行下一节点</li><li>挂起当前作业执行计划</li><li>终止后续节点执行计划</li></ul>
</td>
</tr>
</tbody>
</table>

