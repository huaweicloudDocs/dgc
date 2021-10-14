# Create OBS<a name="dgc_01_0462"></a>

## 约束限制<a name="section571015184916"></a>

该功能依赖于OBS服务。

## 功能<a name="zh-cn_topic_0102588984_section44280035173841"></a>

通过Create OBS节点在OBS服务中创建桶和目录。

## 参数<a name="zh-cn_topic_0102588984_section1791764173933"></a>

用户可参考[表1](#zh-cn_topic_0102588984_table3764823994826)和[表2](#zh-cn_topic_0102588984_table58040457102411)配置Create OBS节点的参数。

**表 1**  属性参数

<a name="zh-cn_topic_0102588984_table3764823994826"></a>
<table><thead align="left"><tr id="zh-cn_topic_0102588984_row3170822394826"><th class="cellrowborder" valign="top" width="21.86%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0102588984_p2984581994826"><a name="zh-cn_topic_0102588984_p2984581994826"></a><a name="zh-cn_topic_0102588984_p2984581994826"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="10.16%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0102588984_p159227094826"><a name="zh-cn_topic_0102588984_p159227094826"></a><a name="zh-cn_topic_0102588984_p159227094826"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="67.97999999999999%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0102588984_p6186505494826"><a name="zh-cn_topic_0102588984_p6186505494826"></a><a name="zh-cn_topic_0102588984_p6186505494826"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0102588984_row1991457694826"><td class="cellrowborder" valign="top" width="21.86%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0102588984_p246794194826"><a name="zh-cn_topic_0102588984_p246794194826"></a><a name="zh-cn_topic_0102588984_p246794194826"></a>节点名称</p>
</td>
<td class="cellrowborder" valign="top" width="10.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0102588984_p6568554794826"><a name="zh-cn_topic_0102588984_p6568554794826"></a><a name="zh-cn_topic_0102588984_p6568554794826"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="67.97999999999999%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0102588984_p1892909794826"><a name="zh-cn_topic_0102588984_p1892909794826"></a><a name="zh-cn_topic_0102588984_p1892909794826"></a><span id="zh-cn_topic_0099822521_text44323307153939"><a name="zh-cn_topic_0099822521_text44323307153939"></a><a name="zh-cn_topic_0099822521_text44323307153939"></a>节点</span>名称，可以包含中文、英文字母、数字、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a>“_”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a>“-”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_parmvalue3773104413412"><a name="zh-cn_topic_0099822521_parmvalue3773104413412"></a><a name="zh-cn_topic_0099822521_parmvalue3773104413412"></a>“/”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a>“&lt;”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a>“&gt;”</span>等各类特殊字符，长度为1～128个字符。</p>
</td>
</tr>
<tr id="zh-cn_topic_0102588984_row3614415394826"><td class="cellrowborder" valign="top" width="21.86%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0102588984_p4199531294826"><a name="zh-cn_topic_0102588984_p4199531294826"></a><a name="zh-cn_topic_0102588984_p4199531294826"></a>OBS路径</p>
</td>
<td class="cellrowborder" valign="top" width="10.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0102588984_p4617707494826"><a name="zh-cn_topic_0102588984_p4617707494826"></a><a name="zh-cn_topic_0102588984_p4617707494826"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="67.97999999999999%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0102588984_p1101101916208"><a name="zh-cn_topic_0102588984_p1101101916208"></a><a name="zh-cn_topic_0102588984_p1101101916208"></a>创建OBS桶或目录的路径。</p>
<a name="zh-cn_topic_0102588984_ul9303034162011"></a><a name="zh-cn_topic_0102588984_ul9303034162011"></a><ul id="zh-cn_topic_0102588984_ul9303034162011"><li>创建桶：在<span class="parmname" id="zh-cn_topic_0102588984_parmname23939002162047"><a name="zh-cn_topic_0102588984_parmname23939002162047"></a><a name="zh-cn_topic_0102588984_parmname23939002162047"></a>“//”</span>后输入OBS桶名称，OBS桶名称不允许重名。</li><li>创建OBS目录：选择需要创建目录的路径，在路径后输入<span class="parmvalue" id="zh-cn_topic_0102588984_parmvalue3274342162723"><a name="zh-cn_topic_0102588984_parmvalue3274342162723"></a><a name="zh-cn_topic_0102588984_parmvalue3274342162723"></a>“/目录名”</span>，目录名不允许重名。</li></ul>
</td>
</tr>
</tbody>
</table>

**表 2**  高级参数

<a name="zh-cn_topic_0102588984_table58040457102411"></a>
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

