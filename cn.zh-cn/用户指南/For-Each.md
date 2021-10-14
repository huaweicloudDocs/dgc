# For Each<a name="dgc_01_0535"></a>

## 功能<a name="zh-cn_topic_0226360828_section44280035173841"></a>

该节点可以指定一个子作业循环执行，并支持用一个数据集对子作业中的变量进行循环替换。

For Each算子的具体使用教程，请参见[For Each算子使用介绍](https://support.huaweicloud.com/bestpractice-dgc/dgc_05_0103.html)。

## 参数<a name="zh-cn_topic_0226360828_section5516152714271"></a>

用户可参考[表1](#zh-cn_topic_0226360828_table3764823994826)配置For Each节点的参数。

**表 1**  属性参数

<a name="zh-cn_topic_0226360828_table3764823994826"></a>
<table><thead align="left"><tr id="zh-cn_topic_0226360828_row3170822394826"><th class="cellrowborder" valign="top" width="21.62%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0226360828_p2984581994826"><a name="zh-cn_topic_0226360828_p2984581994826"></a><a name="zh-cn_topic_0226360828_p2984581994826"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="9.92%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0226360828_p159227094826"><a name="zh-cn_topic_0226360828_p159227094826"></a><a name="zh-cn_topic_0226360828_p159227094826"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="68.46%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0226360828_p6186505494826"><a name="zh-cn_topic_0226360828_p6186505494826"></a><a name="zh-cn_topic_0226360828_p6186505494826"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0226360828_row1991457694826"><td class="cellrowborder" valign="top" width="21.62%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226360828_p246794194826"><a name="zh-cn_topic_0226360828_p246794194826"></a><a name="zh-cn_topic_0226360828_p246794194826"></a>节点名称</p>
</td>
<td class="cellrowborder" valign="top" width="9.92%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226360828_p6568554794826"><a name="zh-cn_topic_0226360828_p6568554794826"></a><a name="zh-cn_topic_0226360828_p6568554794826"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="68.46%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226360828_p1892909794826"><a name="zh-cn_topic_0226360828_p1892909794826"></a><a name="zh-cn_topic_0226360828_p1892909794826"></a><span id="zh-cn_topic_0099822521_text44323307153939"><a name="zh-cn_topic_0099822521_text44323307153939"></a><a name="zh-cn_topic_0099822521_text44323307153939"></a>节点</span>名称，可以包含中文、英文字母、数字、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a>“_”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a>“-”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_parmvalue3773104413412"><a name="zh-cn_topic_0099822521_parmvalue3773104413412"></a><a name="zh-cn_topic_0099822521_parmvalue3773104413412"></a>“/”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a>“&lt;”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a>“&gt;”</span>等各类特殊字符，长度为1～128个字符。</p>
</td>
</tr>
<tr id="zh-cn_topic_0226360828_row3614415394826"><td class="cellrowborder" valign="top" width="21.62%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226360828_p691118102013"><a name="zh-cn_topic_0226360828_p691118102013"></a><a name="zh-cn_topic_0226360828_p691118102013"></a>循环执行的子作业</p>
</td>
<td class="cellrowborder" valign="top" width="9.92%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226360828_p19910710907"><a name="zh-cn_topic_0226360828_p19910710907"></a><a name="zh-cn_topic_0226360828_p19910710907"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="68.46%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226360828_p1490912101503"><a name="zh-cn_topic_0226360828_p1490912101503"></a><a name="zh-cn_topic_0226360828_p1490912101503"></a>选择需要循环执行的子作业。</p>
</td>
</tr>
<tr id="zh-cn_topic_0226360828_row303485991116"><td class="cellrowborder" valign="top" width="21.62%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226360828_p1290816101701"><a name="zh-cn_topic_0226360828_p1290816101701"></a><a name="zh-cn_topic_0226360828_p1290816101701"></a>数据集</p>
</td>
<td class="cellrowborder" valign="top" width="9.92%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226360828_p690881010014"><a name="zh-cn_topic_0226360828_p690881010014"></a><a name="zh-cn_topic_0226360828_p690881010014"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="68.46%" headers="mcps1.2.4.1.3 "><div class="p" id="p9311195617300"><a name="p9311195617300"></a><a name="p9311195617300"></a>For循环算子需要定义一个数据集，这个数据集用来循环替换子作业中的变量，数据集的一行数据会对应一个子作业实例。数据集的来源包括：<a name="ul989322513306"></a><a name="ul989322513306"></a><ul id="ul989322513306"><li>来自于上游节点的输出。例如DLI SQL、Hive SQL、Spark SQL的select语句，或者Shell节点的echo等。使用EL表达式为：#{Job.getNodeOutput('preNodeName')}，即前一个节点的输出值。</li><li>来自于给定的数组。如一维数组：[['001'],['002'],['003']] 。</li></ul>
</div>
</td>
</tr>
<tr id="zh-cn_topic_0226360828_row178956111811"><td class="cellrowborder" valign="top" width="21.62%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226360828_p990618101011"><a name="zh-cn_topic_0226360828_p990618101011"></a><a name="zh-cn_topic_0226360828_p990618101011"></a>子作业并发数</p>
</td>
<td class="cellrowborder" valign="top" width="9.92%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226360828_p890571010011"><a name="zh-cn_topic_0226360828_p890571010011"></a><a name="zh-cn_topic_0226360828_p890571010011"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="68.46%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226360828_p5348616409"><a name="zh-cn_topic_0226360828_p5348616409"></a><a name="zh-cn_topic_0226360828_p5348616409"></a>循环产生的子作业可以并发执行，您可设置并发数。</p>
</td>
</tr>
<tr id="zh-cn_topic_0226360828_row79412423017"><td class="cellrowborder" valign="top" width="21.62%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226360828_p0958421802"><a name="zh-cn_topic_0226360828_p0958421802"></a><a name="zh-cn_topic_0226360828_p0958421802"></a>子作业实例名称后缀</p>
</td>
<td class="cellrowborder" valign="top" width="9.92%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226360828_p09513421805"><a name="zh-cn_topic_0226360828_p09513421805"></a><a name="zh-cn_topic_0226360828_p09513421805"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="68.46%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226360828_p984119208427"><a name="zh-cn_topic_0226360828_p984119208427"></a><a name="zh-cn_topic_0226360828_p984119208427"></a>For循环生成的子任务名称：For循环节点名称 + 下划线 + 后缀。</p>
<p id="zh-cn_topic_0226360828_p11842122010424"><a name="zh-cn_topic_0226360828_p11842122010424"></a><a name="zh-cn_topic_0226360828_p11842122010424"></a>后缀可配置，如果不配置，则按照数字顺序依次递增。</p>
</td>
</tr>
<tr id="zh-cn_topic_0226360828_row74011147193917"><td class="cellrowborder" valign="top" width="21.62%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226360828_p13402204713396"><a name="zh-cn_topic_0226360828_p13402204713396"></a><a name="zh-cn_topic_0226360828_p13402204713396"></a>作业运行参数</p>
</td>
<td class="cellrowborder" valign="top" width="9.92%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226360828_p13402204712396"><a name="zh-cn_topic_0226360828_p13402204712396"></a><a name="zh-cn_topic_0226360828_p13402204712396"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="68.46%" headers="mcps1.2.4.1.3 "><div class="p" id="p729428193513"><a name="p729428193513"></a><a name="p729428193513"></a>仅当子作业配置作业参数后，出现该参数。<a name="ul144670159358"></a><a name="ul144670159358"></a><ul id="ul144670159358"><li>节点属性中子作业参数配置为空时，子作业使用自身参数变量执行。</li><li>节点属性中子作业参数配置后，将使用配置参数变量执行。节点属性中子作业参数配置的方法或者EL表达式，将根据父作业的环境变量读取替换。</li></ul>
</div>
</td>
</tr>
</tbody>
</table>

**表 2**  高级参数

<a name="zh-cn_topic_0226360828_table16592383540"></a>
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

