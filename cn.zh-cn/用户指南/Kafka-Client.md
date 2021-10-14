# Kafka Client<a name="dgc_01_0538"></a>

## 功能<a name="zh-cn_topic_0235670394_section44280035173841"></a>

通过Kafka Client向Kafka的Topic中发送数据。

## 参数<a name="zh-cn_topic_0235670394_section5516152714271"></a>

用户可参考[表1](#zh-cn_topic_0235670394_table3764823994826)配置Kafka Client节点的参数。

**表 1**  属性参数

<a name="zh-cn_topic_0235670394_table3764823994826"></a>
<table><thead align="left"><tr id="zh-cn_topic_0235670394_row3170822394826"><th class="cellrowborder" valign="top" width="21.740000000000002%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0235670394_p2984581994826"><a name="zh-cn_topic_0235670394_p2984581994826"></a><a name="zh-cn_topic_0235670394_p2984581994826"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="10.27%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0235670394_p159227094826"><a name="zh-cn_topic_0235670394_p159227094826"></a><a name="zh-cn_topic_0235670394_p159227094826"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="67.99%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0235670394_p6186505494826"><a name="zh-cn_topic_0235670394_p6186505494826"></a><a name="zh-cn_topic_0235670394_p6186505494826"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0235670394_row13745168174815"><td class="cellrowborder" valign="top" width="21.740000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0235670394_p77451280481"><a name="zh-cn_topic_0235670394_p77451280481"></a><a name="zh-cn_topic_0235670394_p77451280481"></a>数据连接</p>
</td>
<td class="cellrowborder" valign="top" width="10.27%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0235670394_p1274618815488"><a name="zh-cn_topic_0235670394_p1274618815488"></a><a name="zh-cn_topic_0235670394_p1274618815488"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="67.99%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0235670394_p13746281480"><a name="zh-cn_topic_0235670394_p13746281480"></a><a name="zh-cn_topic_0235670394_p13746281480"></a>选择管理中心中已创建的MRS Kafka连接。</p>
</td>
</tr>
<tr id="zh-cn_topic_0235670394_row1669516214485"><td class="cellrowborder" valign="top" width="21.740000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0235670394_p1169572112481"><a name="zh-cn_topic_0235670394_p1169572112481"></a><a name="zh-cn_topic_0235670394_p1169572112481"></a>Topic名称</p>
</td>
<td class="cellrowborder" valign="top" width="10.27%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0235670394_p5695172113486"><a name="zh-cn_topic_0235670394_p5695172113486"></a><a name="zh-cn_topic_0235670394_p5695172113486"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="67.99%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0235670394_p146951721144811"><a name="zh-cn_topic_0235670394_p146951721144811"></a><a name="zh-cn_topic_0235670394_p146951721144811"></a>选择需要上传数据的Topic，如果有多个partition，默认发送到partition 0。</p>
</td>
</tr>
<tr id="zh-cn_topic_0235670394_row1991457694826"><td class="cellrowborder" valign="top" width="21.740000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0235670394_p246794194826"><a name="zh-cn_topic_0235670394_p246794194826"></a><a name="zh-cn_topic_0235670394_p246794194826"></a>节点名称</p>
</td>
<td class="cellrowborder" valign="top" width="10.27%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0235670394_p6568554794826"><a name="zh-cn_topic_0235670394_p6568554794826"></a><a name="zh-cn_topic_0235670394_p6568554794826"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="67.99%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0235670394_p1892909794826"><a name="zh-cn_topic_0235670394_p1892909794826"></a><a name="zh-cn_topic_0235670394_p1892909794826"></a><span id="zh-cn_topic_0099822521_text44323307153939"><a name="zh-cn_topic_0099822521_text44323307153939"></a><a name="zh-cn_topic_0099822521_text44323307153939"></a>节点</span>名称，可以包含中文、英文字母、数字、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a>“_”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a>“-”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_parmvalue3773104413412"><a name="zh-cn_topic_0099822521_parmvalue3773104413412"></a><a name="zh-cn_topic_0099822521_parmvalue3773104413412"></a>“/”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a>“&lt;”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a>“&gt;”</span>等各类特殊字符，长度为1～128个字符。</p>
</td>
</tr>
<tr id="zh-cn_topic_0235670394_row303485991116"><td class="cellrowborder" valign="top" width="21.740000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0235670394_p47481414237"><a name="zh-cn_topic_0235670394_p47481414237"></a><a name="zh-cn_topic_0235670394_p47481414237"></a>发送数据</p>
</td>
<td class="cellrowborder" valign="top" width="10.27%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0235670394_p51613311116"><a name="zh-cn_topic_0235670394_p51613311116"></a><a name="zh-cn_topic_0235670394_p51613311116"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="67.99%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0235670394_p2602055553"><a name="zh-cn_topic_0235670394_p2602055553"></a><a name="zh-cn_topic_0235670394_p2602055553"></a>发送到Kafka的文本内容。可以直接输入文本或单击<a name="zh-cn_topic_0235670394_image176782036121314"></a><a name="zh-cn_topic_0235670394_image176782036121314"></a><span><img id="zh-cn_topic_0235670394_image176782036121314" src="figures/zh-cn_image_0000001102082720.png"></span>使用EL表达式编辑。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  高级参数

<a name="zh-cn_topic_0235670394_table16592383540"></a>
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

