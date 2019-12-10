# MRS Spark Python<a name="dayu_01_0456"></a>

## 功能<a name="zh-cn_topic_0177038589_section44280035173841"></a>

通过MRS Spark Python节点实现在MRS中执行预先定义的Spark Python作业。

## 参数<a name="zh-cn_topic_0177038589_section1791764173933"></a>

用户可参考[表1](#zh-cn_topic_0177038589_table3764823994826)和[表2](#zh-cn_topic_0177038589_table7463135744918)配置MRS Spark Python节点的参数。

**表 1**  属性参数

<a name="zh-cn_topic_0177038589_table3764823994826"></a>
<table><thead align="left"><tr id="zh-cn_topic_0177038589_row3170822394826"><th class="cellrowborder" valign="top" width="28.07%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0177038589_p2984581994826"><a name="zh-cn_topic_0177038589_p2984581994826"></a><a name="zh-cn_topic_0177038589_p2984581994826"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="15.659999999999998%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0177038589_p159227094826"><a name="zh-cn_topic_0177038589_p159227094826"></a><a name="zh-cn_topic_0177038589_p159227094826"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="56.269999999999996%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0177038589_p6186505494826"><a name="zh-cn_topic_0177038589_p6186505494826"></a><a name="zh-cn_topic_0177038589_p6186505494826"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0177038589_row1991457694826"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0177038589_p246794194826"><a name="zh-cn_topic_0177038589_p246794194826"></a><a name="zh-cn_topic_0177038589_p246794194826"></a>节点名称</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0177038589_p6568554794826"><a name="zh-cn_topic_0177038589_p6568554794826"></a><a name="zh-cn_topic_0177038589_p6568554794826"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0177038589_p1892909794826"><a name="zh-cn_topic_0177038589_p1892909794826"></a><a name="zh-cn_topic_0177038589_p1892909794826"></a><span id="zh-cn_topic_0177038589_zh-cn_topic_0099822521_text44323307153939"><a name="zh-cn_topic_0177038589_zh-cn_topic_0099822521_text44323307153939"></a><a name="zh-cn_topic_0177038589_zh-cn_topic_0099822521_text44323307153939"></a>节点</span>名称，可以包含中文、英文字母、数字、<span class="parmvalue" id="zh-cn_topic_0177038589_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"><a name="zh-cn_topic_0177038589_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a><a name="zh-cn_topic_0177038589_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a>“_”</span>、<span class="parmvalue" id="zh-cn_topic_0177038589_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"><a name="zh-cn_topic_0177038589_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a><a name="zh-cn_topic_0177038589_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a>“-”</span>、<span class="parmvalue" id="zh-cn_topic_0177038589_zh-cn_topic_0099822521_parmvalue3773104413412"><a name="zh-cn_topic_0177038589_zh-cn_topic_0099822521_parmvalue3773104413412"></a><a name="zh-cn_topic_0177038589_zh-cn_topic_0099822521_parmvalue3773104413412"></a>“/”</span>、<span class="parmvalue" id="zh-cn_topic_0177038589_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"><a name="zh-cn_topic_0177038589_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a><a name="zh-cn_topic_0177038589_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a>“&lt;”</span>、<span class="parmvalue" id="zh-cn_topic_0177038589_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"><a name="zh-cn_topic_0177038589_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a><a name="zh-cn_topic_0177038589_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a>“&gt;”</span>等各类特殊字符，长度为1～128个字符。</p>
</td>
</tr>
<tr id="zh-cn_topic_0177038589_row3614415394826"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0177038589_p4199531294826"><a name="zh-cn_topic_0177038589_p4199531294826"></a><a name="zh-cn_topic_0177038589_p4199531294826"></a>MRS集群名</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0177038589_p4617707494826"><a name="zh-cn_topic_0177038589_p4617707494826"></a><a name="zh-cn_topic_0177038589_p4617707494826"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0177038589_p17967492105259"><a name="zh-cn_topic_0177038589_p17967492105259"></a><a name="zh-cn_topic_0177038589_p17967492105259"></a>选择支持spark python的mrs集群。MRS只有特定版本支持spark python的集群，请先测试运行，保证集群支持。</p>
<div class="p" id="zh-cn_topic_0177038589_p27489702105259"><a name="zh-cn_topic_0177038589_p27489702105259"></a><a name="zh-cn_topic_0177038589_p27489702105259"></a>如需新建集群，请参考以下方法：<a name="zh-cn_topic_0177038589_zh-cn_topic_0101095234_zh-cn_topic_0099822521_ul46080727105259"></a><a name="zh-cn_topic_0177038589_zh-cn_topic_0101095234_zh-cn_topic_0099822521_ul46080727105259"></a><ul id="zh-cn_topic_0177038589_zh-cn_topic_0101095234_zh-cn_topic_0099822521_ul46080727105259"><li>单击<a name="zh-cn_topic_0177038589_zh-cn_topic_0101095234_image898618712510"></a><a name="zh-cn_topic_0177038589_zh-cn_topic_0101095234_image898618712510"></a><span><img id="zh-cn_topic_0177038589_zh-cn_topic_0101095234_image898618712510" src="figures/view-9.png"></span>，进入<span class="wintitle" id="zh-cn_topic_0177038589_zh-cn_topic_0101095234_wintitle3126196153112"><a name="zh-cn_topic_0177038589_zh-cn_topic_0101095234_wintitle3126196153112"></a><a name="zh-cn_topic_0177038589_zh-cn_topic_0101095234_wintitle3126196153112"></a>“集群列表”</span>页面新建MRS集群。</li><li>前往MRS管理控制台进行新建。</li></ul>
</div>
<p id="zh-cn_topic_0177038589_p186181620284"><a name="zh-cn_topic_0177038589_p186181620284"></a><a name="zh-cn_topic_0177038589_p186181620284"></a>如何新建集群，请参见<span id="zh-cn_topic_0177038589_cite042911197588"><a name="zh-cn_topic_0177038589_cite042911197588"></a><a name="zh-cn_topic_0177038589_cite042911197588"></a>《MapReduce服务用户指南》</span>的<a href="https://support.huaweicloud.com/usermanual-mrs/zh-cn_topic_0013363945.html" target="_blank" rel="noopener noreferrer">创建集群</a>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0177038589_row4154658494826"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0177038589_p983015394826"><a name="zh-cn_topic_0177038589_p983015394826"></a><a name="zh-cn_topic_0177038589_p983015394826"></a>作业名称</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0177038589_p5804493094826"><a name="zh-cn_topic_0177038589_p5804493094826"></a><a name="zh-cn_topic_0177038589_p5804493094826"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0177038589_p15602016115115"><a name="zh-cn_topic_0177038589_p15602016115115"></a><a name="zh-cn_topic_0177038589_p15602016115115"></a>输入MRS Spark Python作业名称，只能包含英文字母、数字、<span class="parmvalue" id="zh-cn_topic_0177038589_parmvalue1999072575115"><a name="zh-cn_topic_0177038589_parmvalue1999072575115"></a><a name="zh-cn_topic_0177038589_parmvalue1999072575115"></a>“_”</span>，且长度为1~64个字符。</p>
</td>
</tr>
<tr id="zh-cn_topic_0177038589_row1949012674611"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0177038589_p154913613464"><a name="zh-cn_topic_0177038589_p154913613464"></a><a name="zh-cn_topic_0177038589_p154913613464"></a>参数</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0177038589_p1749110664620"><a name="zh-cn_topic_0177038589_p1749110664620"></a><a name="zh-cn_topic_0177038589_p1749110664620"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0177038589_p649136154615"><a name="zh-cn_topic_0177038589_p649136154615"></a><a name="zh-cn_topic_0177038589_p649136154615"></a>输入MRS的执行程序参数，多个参数间使用Enter键分隔。</p>
</td>
</tr>
<tr id="zh-cn_topic_0177038589_row10153101910469"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0177038589_p101533199468"><a name="zh-cn_topic_0177038589_p101533199468"></a><a name="zh-cn_topic_0177038589_p101533199468"></a>属性</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0177038589_p10153519154612"><a name="zh-cn_topic_0177038589_p10153519154612"></a><a name="zh-cn_topic_0177038589_p10153519154612"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0177038589_p91531719134620"><a name="zh-cn_topic_0177038589_p91531719134620"></a><a name="zh-cn_topic_0177038589_p91531719134620"></a>输入key=value格式的参数，多个参数间使用Enter键分割。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  高级参数

<a name="zh-cn_topic_0177038589_table7463135744918"></a>
<table><thead align="left"><tr id="zh-cn_topic_0177038589_row12463155714915"><th class="cellrowborder" valign="top" width="27.862786278627865%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0177038589_p201064619506"><a name="zh-cn_topic_0177038589_p201064619506"></a><a name="zh-cn_topic_0177038589_p201064619506"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="16.711671167116712%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0177038589_p8106176145018"><a name="zh-cn_topic_0177038589_p8106176145018"></a><a name="zh-cn_topic_0177038589_p8106176145018"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="55.42554255425542%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0177038589_p171062625015"><a name="zh-cn_topic_0177038589_p171062625015"></a><a name="zh-cn_topic_0177038589_p171062625015"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0177038589_row1546465711493"><td class="cellrowborder" valign="top" width="27.862786278627865%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0177038589_p1157215345539"><a name="zh-cn_topic_0177038589_p1157215345539"></a><a name="zh-cn_topic_0177038589_p1157215345539"></a>节点执行的最长时间</p>
</td>
<td class="cellrowborder" valign="top" width="16.711671167116712%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0177038589_p1957217349530"><a name="zh-cn_topic_0177038589_p1957217349530"></a><a name="zh-cn_topic_0177038589_p1957217349530"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="55.42554255425542%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0177038589_p10572534175315"><a name="zh-cn_topic_0177038589_p10572534175315"></a><a name="zh-cn_topic_0177038589_p10572534175315"></a>设置<span id="zh-cn_topic_0177038589_text857263415310"><a name="zh-cn_topic_0177038589_text857263415310"></a><a name="zh-cn_topic_0177038589_text857263415310"></a>节点</span>执行的超时时间，如果<span id="zh-cn_topic_0177038589_text4572434205312"><a name="zh-cn_topic_0177038589_text4572434205312"></a><a name="zh-cn_topic_0177038589_text4572434205312"></a>节点</span>配置了重试，在超时时间内未执行完成，该节点将不会再重试，直接置为失败状态。</p>
</td>
</tr>
<tr id="zh-cn_topic_0177038589_row154300427537"><td class="cellrowborder" valign="top" width="27.862786278627865%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0177038589_p66221849165318"><a name="zh-cn_topic_0177038589_p66221849165318"></a><a name="zh-cn_topic_0177038589_p66221849165318"></a>失败重试</p>
</td>
<td class="cellrowborder" valign="top" width="16.711671167116712%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0177038589_p7623149145314"><a name="zh-cn_topic_0177038589_p7623149145314"></a><a name="zh-cn_topic_0177038589_p7623149145314"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="55.42554255425542%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0177038589_p9623949125317"><a name="zh-cn_topic_0177038589_p9623949125317"></a><a name="zh-cn_topic_0177038589_p9623949125317"></a><span id="zh-cn_topic_0177038589_text18623164945317"><a name="zh-cn_topic_0177038589_text18623164945317"></a><a name="zh-cn_topic_0177038589_text18623164945317"></a>节点</span>执行失败后，是否重新执行<span id="zh-cn_topic_0177038589_text7623194945315"><a name="zh-cn_topic_0177038589_text7623194945315"></a><a name="zh-cn_topic_0177038589_text7623194945315"></a>节点</span>。</p>
<a name="zh-cn_topic_0177038589_ul10623194916530"></a><a name="zh-cn_topic_0177038589_ul10623194916530"></a><ul id="zh-cn_topic_0177038589_ul10623194916530"><li>是：重新执行<span id="zh-cn_topic_0177038589_text1623114925317"><a name="zh-cn_topic_0177038589_text1623114925317"></a><a name="zh-cn_topic_0177038589_text1623114925317"></a>节点</span>，请配置以下参数。<a name="zh-cn_topic_0177038589_ul5623184915313"></a><a name="zh-cn_topic_0177038589_ul5623184915313"></a><ul id="zh-cn_topic_0177038589_ul5623184915313"><li>最大重试次数</li><li>重试间隔时间（秒）</li></ul>
</li><li>否：默认值，不重新执行<span id="zh-cn_topic_0177038589_text36231649115312"><a name="zh-cn_topic_0177038589_text36231649115312"></a><a name="zh-cn_topic_0177038589_text36231649115312"></a>节点</span>。</li></ul>
<div class="note" id="zh-cn_topic_0177038589_note2623164925318"><a name="zh-cn_topic_0177038589_note2623164925318"></a><a name="zh-cn_topic_0177038589_note2623164925318"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0177038589_p162364913535"><a name="zh-cn_topic_0177038589_p162364913535"></a><a name="zh-cn_topic_0177038589_p162364913535"></a>如果作业节点配置了重试，并且配置了超时时间，该节点执行超时后将不会再重试，直接置为失败状态。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0177038589_row3791655185313"><td class="cellrowborder" valign="top" width="27.862786278627865%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0177038589_p174990595418"><a name="zh-cn_topic_0177038589_p174990595418"></a><a name="zh-cn_topic_0177038589_p174990595418"></a>失败策略</p>
</td>
<td class="cellrowborder" valign="top" width="16.711671167116712%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0177038589_p1849914535418"><a name="zh-cn_topic_0177038589_p1849914535418"></a><a name="zh-cn_topic_0177038589_p1849914535418"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="55.42554255425542%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0177038589_p13500165175414"><a name="zh-cn_topic_0177038589_p13500165175414"></a><a name="zh-cn_topic_0177038589_p13500165175414"></a><span id="zh-cn_topic_0177038589_text1150045205417"><a name="zh-cn_topic_0177038589_text1150045205417"></a><a name="zh-cn_topic_0177038589_text1150045205417"></a>节点</span>执行失败后的操作：</p>
<a name="zh-cn_topic_0177038589_ul3500145135413"></a><a name="zh-cn_topic_0177038589_ul3500145135413"></a><ul id="zh-cn_topic_0177038589_ul3500145135413"><li>终止当前作业执行计划</li><li>继续执行下一作业</li><li>挂起当前作业执行计划</li></ul>
</td>
</tr>
</tbody>
</table>

