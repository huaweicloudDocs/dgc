# DIS Client<a name="dgc_01_0446"></a>

## 功能<a name="zh-cn_topic_0163990342_section44280035173841"></a>

通过DIS Client节点可以给DIS通道发送消息。

您可以参考[跨空间进行作业调度](https://support.huaweicloud.com/bestpractice-dgc/dgc_05_0101.html)和[获取Rest Client算子返回值教程](https://support.huaweicloud.com/bestpractice-dgc/dgc_05_0104.html)，获取DIS Client节点的使用案例。

## 参数<a name="zh-cn_topic_0163990342_section5516152714271"></a>

用户可参考[表1](#zh-cn_topic_0163990342_table3764823994826)配置DIS Client节点的参数。

**表 1**  属性参数

<a name="zh-cn_topic_0163990342_table3764823994826"></a>
<table><thead align="left"><tr id="zh-cn_topic_0163990342_row3170822394826"><th class="cellrowborder" valign="top" width="21.62%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0163990342_p2984581994826"><a name="zh-cn_topic_0163990342_p2984581994826"></a><a name="zh-cn_topic_0163990342_p2984581994826"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="10.16%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0163990342_p159227094826"><a name="zh-cn_topic_0163990342_p159227094826"></a><a name="zh-cn_topic_0163990342_p159227094826"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="68.22%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0163990342_p6186505494826"><a name="zh-cn_topic_0163990342_p6186505494826"></a><a name="zh-cn_topic_0163990342_p6186505494826"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0163990342_row14155105315184"><td class="cellrowborder" valign="top" width="21.62%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0163990342_p111579531187"><a name="zh-cn_topic_0163990342_p111579531187"></a><a name="zh-cn_topic_0163990342_p111579531187"></a>是否使用DIS数据通道连接</p>
</td>
<td class="cellrowborder" valign="top" width="10.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0163990342_p0157115321816"><a name="zh-cn_topic_0163990342_p0157115321816"></a><a name="zh-cn_topic_0163990342_p0157115321816"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="68.22%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0163990342_p1015813531186"><a name="zh-cn_topic_0163990342_p1015813531186"></a><a name="zh-cn_topic_0163990342_p1015813531186"></a>若使用数据通道连接, 可以向其他账号的DIS通道发送消息; 若不使用, 仅能给本账号下所有region的通道发送消息。</p>
</td>
</tr>
<tr id="zh-cn_topic_0163990342_row0502202411910"><td class="cellrowborder" valign="top" width="21.62%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0163990342_p45059246196"><a name="zh-cn_topic_0163990342_p45059246196"></a><a name="zh-cn_topic_0163990342_p45059246196"></a>数据通道连接名称</p>
</td>
<td class="cellrowborder" valign="top" width="10.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0163990342_p55051124161918"><a name="zh-cn_topic_0163990342_p55051124161918"></a><a name="zh-cn_topic_0163990342_p55051124161918"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="68.22%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0163990342_p35065246197"><a name="zh-cn_topic_0163990342_p35065246197"></a><a name="zh-cn_topic_0163990342_p35065246197"></a>选择“管理中心”中已创建的DIS连接名称。</p>
</td>
</tr>
<tr id="zh-cn_topic_0163990342_row1548312431194"><td class="cellrowborder" valign="top" width="21.62%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0163990342_p6484343161911"><a name="zh-cn_topic_0163990342_p6484343161911"></a><a name="zh-cn_topic_0163990342_p6484343161911"></a>通道所属Region</p>
</td>
<td class="cellrowborder" valign="top" width="10.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0163990342_p124863439197"><a name="zh-cn_topic_0163990342_p124863439197"></a><a name="zh-cn_topic_0163990342_p124863439197"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="68.22%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0163990342_p948611437198"><a name="zh-cn_topic_0163990342_p948611437198"></a><a name="zh-cn_topic_0163990342_p948611437198"></a>使用DIS Client节点发送消息至目标DIS通道时，目标通道所在的Region。</p>
</td>
</tr>
<tr id="zh-cn_topic_0163990342_row1991457694826"><td class="cellrowborder" valign="top" width="21.62%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0163990342_p246794194826"><a name="zh-cn_topic_0163990342_p246794194826"></a><a name="zh-cn_topic_0163990342_p246794194826"></a>节点名称</p>
</td>
<td class="cellrowborder" valign="top" width="10.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0163990342_p6568554794826"><a name="zh-cn_topic_0163990342_p6568554794826"></a><a name="zh-cn_topic_0163990342_p6568554794826"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="68.22%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0163990342_p1892909794826"><a name="zh-cn_topic_0163990342_p1892909794826"></a><a name="zh-cn_topic_0163990342_p1892909794826"></a><span id="zh-cn_topic_0099822521_text44323307153939"><a name="zh-cn_topic_0099822521_text44323307153939"></a><a name="zh-cn_topic_0099822521_text44323307153939"></a>节点</span>名称，可以包含中文、英文字母、数字、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a>“_”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a>“-”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_parmvalue3773104413412"><a name="zh-cn_topic_0099822521_parmvalue3773104413412"></a><a name="zh-cn_topic_0099822521_parmvalue3773104413412"></a>“/”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a>“&lt;”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a>“&gt;”</span>等各类特殊字符，长度为1～128个字符。</p>
</td>
</tr>
<tr id="zh-cn_topic_0163990342_row3614415394826"><td class="cellrowborder" valign="top" width="21.62%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0163990342_p685511219363"><a name="zh-cn_topic_0163990342_p685511219363"></a><a name="zh-cn_topic_0163990342_p685511219363"></a>通道名称</p>
</td>
<td class="cellrowborder" valign="top" width="10.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0163990342_p4617707494826"><a name="zh-cn_topic_0163990342_p4617707494826"></a><a name="zh-cn_topic_0163990342_p4617707494826"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="68.22%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0163990342_p56021545520"><a name="zh-cn_topic_0163990342_p56021545520"></a><a name="zh-cn_topic_0163990342_p56021545520"></a>需要发送消息的DIS通道。可以直接输入DIS通道地址或单击<a name="zh-cn_topic_0163990342_image7949832974"></a><a name="zh-cn_topic_0163990342_image7949832974"></a><span><img id="zh-cn_topic_0163990342_image7949832974" src="figures/zh-cn_image_0000001148602681.png"></span>选择DIS通道。</p>
</td>
</tr>
<tr id="zh-cn_topic_0163990342_row303485991116"><td class="cellrowborder" valign="top" width="21.62%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0163990342_p47481414237"><a name="zh-cn_topic_0163990342_p47481414237"></a><a name="zh-cn_topic_0163990342_p47481414237"></a>发送数据</p>
</td>
<td class="cellrowborder" valign="top" width="10.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0163990342_p51613311116"><a name="zh-cn_topic_0163990342_p51613311116"></a><a name="zh-cn_topic_0163990342_p51613311116"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="68.22%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0163990342_p2602055553"><a name="zh-cn_topic_0163990342_p2602055553"></a><a name="zh-cn_topic_0163990342_p2602055553"></a>发送到DIS通道的文本内容。可以直接输入文本或单击<a name="zh-cn_topic_0163990342_image176782036121314"></a><a name="zh-cn_topic_0163990342_image176782036121314"></a><span><img id="zh-cn_topic_0163990342_image176782036121314" src="figures/zh-cn_image_0000001101922744.png"></span>使用EL表达式编辑。</p>
</td>
</tr>
<tr id="zh-cn_topic_0163990342_row178956111811"><td class="cellrowborder" valign="top" width="21.62%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0163990342_p5900691812"><a name="zh-cn_topic_0163990342_p5900691812"></a><a name="zh-cn_topic_0163990342_p5900691812"></a>相关作业</p>
</td>
<td class="cellrowborder" valign="top" width="10.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0163990342_p290561186"><a name="zh-cn_topic_0163990342_p290561186"></a><a name="zh-cn_topic_0163990342_p290561186"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="68.22%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0163990342_p9903614187"><a name="zh-cn_topic_0163990342_p9903614187"></a><a name="zh-cn_topic_0163990342_p9903614187"></a>单击<a name="zh-cn_topic_0163990342_image758820305388"></a><a name="zh-cn_topic_0163990342_image758820305388"></a><span><img id="zh-cn_topic_0163990342_image758820305388" src="figures/zh-cn_image_0000001148722633.png"></span>选择相关作业，您可以选择批作业，也可以实时作业。</p>
<div class="note" id="zh-cn_topic_0163990342_note1753318552417"><a name="zh-cn_topic_0163990342_note1753318552417"></a><a name="zh-cn_topic_0163990342_note1753318552417"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0163990342_p16534855164110"><a name="zh-cn_topic_0163990342_p16534855164110"></a><a name="zh-cn_topic_0163990342_p16534855164110"></a>您最多只能选择10个作业。</p>
</div></div>
<p id="zh-cn_topic_0163990342_p1944157114513"><a name="zh-cn_topic_0163990342_p1944157114513"></a><a name="zh-cn_topic_0163990342_p1944157114513"></a>选择完相关作业，单击<span class="uicontrol" id="zh-cn_topic_0163990342_uicontrol18956923145216"><a name="zh-cn_topic_0163990342_uicontrol18956923145216"></a><a name="zh-cn_topic_0163990342_uicontrol18956923145216"></a>“前往监控”</span>在<span class="wintitle" id="zh-cn_topic_0163990342_wintitle11924171844612"><a name="zh-cn_topic_0163990342_wintitle11924171844612"></a><a name="zh-cn_topic_0163990342_wintitle11924171844612"></a>“作业监控”</span>页面选择<span id="zh-cn_topic_0163990342_text149191327194613"><a name="zh-cn_topic_0163990342_text149191327194613"></a><a name="zh-cn_topic_0163990342_text149191327194613"></a>DIS Client</span><span id="zh-cn_topic_0163990342_text891982734612"><a name="zh-cn_topic_0163990342_text891982734612"></a><a name="zh-cn_topic_0163990342_text891982734612"></a>节点</span>时，单击页面下方的<span class="uicontrol" id="zh-cn_topic_0163990342_uicontrol1593972234811"><a name="zh-cn_topic_0163990342_uicontrol1593972234811"></a><a name="zh-cn_topic_0163990342_uicontrol1593972234811"></a>“查看相关作业”</span>按钮可以查看相关作业。</p>
<p id="zh-cn_topic_0163990342_p7405191275510"><a name="zh-cn_topic_0163990342_p7405191275510"></a><a name="zh-cn_topic_0163990342_p7405191275510"></a>在<span class="wintitle" id="zh-cn_topic_0163990342_wintitle137021724125518"><a name="zh-cn_topic_0163990342_wintitle137021724125518"></a><a name="zh-cn_topic_0163990342_wintitle137021724125518"></a>“相关作业”</span>页面，单击<span class="parmname" id="zh-cn_topic_0163990342_parmname13990055612"><a name="zh-cn_topic_0163990342_parmname13990055612"></a><a name="zh-cn_topic_0163990342_parmname13990055612"></a>“查看”</span>能跳转到对应的作业。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  高级参数

<a name="zh-cn_topic_0163990342_table16592383540"></a>
<table><thead align="left"><tr id="zh-cn_topic_0099822521_row9846111555118"><th class="cellrowborder" valign="top" width="21.58%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0099822521_p2846515195115"><a name="zh-cn_topic_0099822521_p2846515195115"></a><a name="zh-cn_topic_0099822521_p2846515195115"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="10.14%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0099822521_p108461215185110"><a name="zh-cn_topic_0099822521_p108461215185110"></a><a name="zh-cn_topic_0099822521_p108461215185110"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="68.28%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0099822521_p1484719153511"><a name="zh-cn_topic_0099822521_p1484719153511"></a><a name="zh-cn_topic_0099822521_p1484719153511"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0099822521_row18847141515512"><td class="cellrowborder" valign="top" width="21.58%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0099822521_p2847181535113"><a name="zh-cn_topic_0099822521_p2847181535113"></a><a name="zh-cn_topic_0099822521_p2847181535113"></a>节点执行的最长时间</p>
</td>
<td class="cellrowborder" valign="top" width="10.14%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0099822521_p15847171511512"><a name="zh-cn_topic_0099822521_p15847171511512"></a><a name="zh-cn_topic_0099822521_p15847171511512"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="68.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0099822521_p1884761565119"><a name="zh-cn_topic_0099822521_p1884761565119"></a><a name="zh-cn_topic_0099822521_p1884761565119"></a>设置<span id="zh-cn_topic_0099822521_text17847191515114"><a name="zh-cn_topic_0099822521_text17847191515114"></a><a name="zh-cn_topic_0099822521_text17847191515114"></a>节点</span>执行的超时时间，如果<span id="zh-cn_topic_0099822521_text1847191595118"><a name="zh-cn_topic_0099822521_text1847191595118"></a><a name="zh-cn_topic_0099822521_text1847191595118"></a>节点</span>配置了重试，在超时时间内未执行完成，该节点将不会再重试，直接置为失败状态。</p>
</td>
</tr>
<tr id="zh-cn_topic_0099822521_row19847181555112"><td class="cellrowborder" valign="top" width="21.58%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0099822521_p12847815125117"><a name="zh-cn_topic_0099822521_p12847815125117"></a><a name="zh-cn_topic_0099822521_p12847815125117"></a>失败重试</p>
</td>
<td class="cellrowborder" valign="top" width="10.14%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0099822521_p8847161516511"><a name="zh-cn_topic_0099822521_p8847161516511"></a><a name="zh-cn_topic_0099822521_p8847161516511"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="68.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0099822521_p684761514516"><a name="zh-cn_topic_0099822521_p684761514516"></a><a name="zh-cn_topic_0099822521_p684761514516"></a><span id="zh-cn_topic_0099822521_text68471415185118"><a name="zh-cn_topic_0099822521_text68471415185118"></a><a name="zh-cn_topic_0099822521_text68471415185118"></a>节点</span>执行失败后，是否重新执行<span id="zh-cn_topic_0099822521_text784719150517"><a name="zh-cn_topic_0099822521_text784719150517"></a><a name="zh-cn_topic_0099822521_text784719150517"></a>节点</span>。</p>
<a name="zh-cn_topic_0099822521_ul18479151514"></a><a name="zh-cn_topic_0099822521_ul18479151514"></a><ul id="zh-cn_topic_0099822521_ul18479151514"><li>是：重新执行<span id="zh-cn_topic_0099822521_text184861512517"><a name="zh-cn_topic_0099822521_text184861512517"></a><a name="zh-cn_topic_0099822521_text184861512517"></a>节点</span>，请配置以下参数。<a name="zh-cn_topic_0099822521_ul284811151511"></a><a name="zh-cn_topic_0099822521_ul284811151511"></a><ul id="zh-cn_topic_0099822521_ul284811151511"><li>最大重试次数</li><li>重试间隔时间（秒）</li></ul>
</li><li>否：默认值，不重新执行<span id="zh-cn_topic_0099822521_text5848215145116"><a name="zh-cn_topic_0099822521_text5848215145116"></a><a name="zh-cn_topic_0099822521_text5848215145116"></a>节点</span>。</li></ul>
<div class="note" id="zh-cn_topic_0099822521_note6848101513516"><a name="zh-cn_topic_0099822521_note6848101513516"></a><a name="zh-cn_topic_0099822521_note6848101513516"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0099822521_p14848515185114"><a name="zh-cn_topic_0099822521_p14848515185114"></a><a name="zh-cn_topic_0099822521_p14848515185114"></a>如果作业节点配置了重试，并且配置了超时时间，该节点执行超时后将不会再重试，直接置为失败状态。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0099822521_row148481015115110"><td class="cellrowborder" valign="top" width="21.58%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0099822521_p168481315165110"><a name="zh-cn_topic_0099822521_p168481315165110"></a><a name="zh-cn_topic_0099822521_p168481315165110"></a>失败策略</p>
</td>
<td class="cellrowborder" valign="top" width="10.14%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0099822521_p7848181515114"><a name="zh-cn_topic_0099822521_p7848181515114"></a><a name="zh-cn_topic_0099822521_p7848181515114"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="68.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0099822521_p1848915165110"><a name="zh-cn_topic_0099822521_p1848915165110"></a><a name="zh-cn_topic_0099822521_p1848915165110"></a><span id="zh-cn_topic_0099822521_text184871517513"><a name="zh-cn_topic_0099822521_text184871517513"></a><a name="zh-cn_topic_0099822521_text184871517513"></a>节点</span>执行失败后的操作：</p>
<a name="zh-cn_topic_0099822521_ul684811155518"></a><a name="zh-cn_topic_0099822521_ul684811155518"></a><ul id="zh-cn_topic_0099822521_ul684811155518"><li>终止当前作业执行计划</li><li>继续执行下一节点</li><li>挂起当前作业执行计划</li><li>终止后续节点执行计划</li></ul>
</td>
</tr>
</tbody>
</table>

