# SMN<a name="dgc_01_0468"></a>

## 功能<a name="zh-cn_topic_0121505665_section44280035173841"></a>

通过SMN节点向用户发送通知消息。

## 参数<a name="zh-cn_topic_0121505665_section6331447317395"></a>

用户可参考[表1](#zh-cn_topic_0121505665_table3764823994826)和[表2](#zh-cn_topic_0121505665_table58040457102411)配置SMN节点的参数。

**表 1**  属性参数

<a name="zh-cn_topic_0121505665_table3764823994826"></a>
<table><thead align="left"><tr id="zh-cn_topic_0121505665_row3170822394826"><th class="cellrowborder" valign="top" width="21.740000000000002%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0121505665_p2984581994826"><a name="zh-cn_topic_0121505665_p2984581994826"></a><a name="zh-cn_topic_0121505665_p2984581994826"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="9.92%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0121505665_p159227094826"><a name="zh-cn_topic_0121505665_p159227094826"></a><a name="zh-cn_topic_0121505665_p159227094826"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="68.34%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0121505665_p6186505494826"><a name="zh-cn_topic_0121505665_p6186505494826"></a><a name="zh-cn_topic_0121505665_p6186505494826"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0121505665_row1991457694826"><td class="cellrowborder" valign="top" width="21.740000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0121505665_p246794194826"><a name="zh-cn_topic_0121505665_p246794194826"></a><a name="zh-cn_topic_0121505665_p246794194826"></a>节点名称</p>
</td>
<td class="cellrowborder" valign="top" width="9.92%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0121505665_p6568554794826"><a name="zh-cn_topic_0121505665_p6568554794826"></a><a name="zh-cn_topic_0121505665_p6568554794826"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="68.34%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0121505665_p1892909794826"><a name="zh-cn_topic_0121505665_p1892909794826"></a><a name="zh-cn_topic_0121505665_p1892909794826"></a><span id="zh-cn_topic_0099822521_text44323307153939"><a name="zh-cn_topic_0099822521_text44323307153939"></a><a name="zh-cn_topic_0099822521_text44323307153939"></a>节点</span>名称，可以包含中文、英文字母、数字、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a>“_”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a>“-”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_parmvalue3773104413412"><a name="zh-cn_topic_0099822521_parmvalue3773104413412"></a><a name="zh-cn_topic_0099822521_parmvalue3773104413412"></a>“/”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a>“&lt;”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a>“&gt;”</span>等各类特殊字符，长度为1～128个字符。</p>
</td>
</tr>
<tr id="zh-cn_topic_0121505665_row3614415394826"><td class="cellrowborder" valign="top" width="21.740000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0121505665_p4898925756"><a name="zh-cn_topic_0121505665_p4898925756"></a><a name="zh-cn_topic_0121505665_p4898925756"></a>主题名称</p>
</td>
<td class="cellrowborder" valign="top" width="9.92%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0121505665_p4617707494826"><a name="zh-cn_topic_0121505665_p4617707494826"></a><a name="zh-cn_topic_0121505665_p4617707494826"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="68.34%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0121505665_p4935552994826"><a name="zh-cn_topic_0121505665_p4935552994826"></a><a name="zh-cn_topic_0121505665_p4935552994826"></a>选择消息的主题，该主题已在SMN服务中创建好。</p>
</td>
</tr>
<tr id="zh-cn_topic_0121505665_row4154658494826"><td class="cellrowborder" valign="top" width="21.740000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0121505665_p983015394826"><a name="zh-cn_topic_0121505665_p983015394826"></a><a name="zh-cn_topic_0121505665_p983015394826"></a>消息标题</p>
</td>
<td class="cellrowborder" valign="top" width="9.92%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0121505665_p5804493094826"><a name="zh-cn_topic_0121505665_p5804493094826"></a><a name="zh-cn_topic_0121505665_p5804493094826"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="68.34%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0121505665_p401892494826"><a name="zh-cn_topic_0121505665_p401892494826"></a><a name="zh-cn_topic_0121505665_p401892494826"></a>自定义消息的标题，长度必须少于512个字符。</p>
</td>
</tr>
<tr id="zh-cn_topic_0121505665_row824216571514"><td class="cellrowborder" valign="top" width="21.740000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0121505665_p102421575510"><a name="zh-cn_topic_0121505665_p102421575510"></a><a name="zh-cn_topic_0121505665_p102421575510"></a>消息类型</p>
</td>
<td class="cellrowborder" valign="top" width="9.92%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0121505665_p32421357353"><a name="zh-cn_topic_0121505665_p32421357353"></a><a name="zh-cn_topic_0121505665_p32421357353"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="68.34%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0121505665_p324255714511"><a name="zh-cn_topic_0121505665_p324255714511"></a><a name="zh-cn_topic_0121505665_p324255714511"></a>选择消息的发送格式。</p>
<a name="zh-cn_topic_0121505665_ul894915486811"></a><a name="zh-cn_topic_0121505665_ul894915486811"></a><ul id="zh-cn_topic_0121505665_ul894915486811"><li>文本消息：按文本格式发送的消息。</li><li>JSON消息：按JSON格式发送的消息，用户可对不同的订阅者类型发送不同的消息。<a name="zh-cn_topic_0121505665_ul108611718201819"></a><a name="zh-cn_topic_0121505665_ul108611718201819"></a><ul id="zh-cn_topic_0121505665_ul108611718201819"><li>手动输入JSON格式的消息：在<span class="parmname" id="zh-cn_topic_0121505665_parmname11694522111920"><a name="zh-cn_topic_0121505665_parmname11694522111920"></a><a name="zh-cn_topic_0121505665_parmname11694522111920"></a>“消息内容”</span>直接输入。</li><li>通过工具自动生成JSON格式的消息：单击<span class="uicontrol" id="zh-cn_topic_0121505665_uicontrol496442094816"><a name="zh-cn_topic_0121505665_uicontrol496442094816"></a><a name="zh-cn_topic_0121505665_uicontrol496442094816"></a>“生成JSON消息”</span>，在弹出的对话框中填写<span class="parmname" id="zh-cn_topic_0121505665_parmname18859639162018"><a name="zh-cn_topic_0121505665_parmname18859639162018"></a><a name="zh-cn_topic_0121505665_parmname18859639162018"></a>“消息”</span>和选择<span class="parmname" id="zh-cn_topic_0121505665_parmname33748489208"><a name="zh-cn_topic_0121505665_parmname33748489208"></a><a name="zh-cn_topic_0121505665_parmname33748489208"></a>“协议”</span>。</li></ul>
</li><li>模板消息：按模板格式发送的消息，即固定格式的消息，可以通过tag的方式来处理变量的部分。<a name="zh-cn_topic_0121505665_ul5156162214236"></a><a name="zh-cn_topic_0121505665_ul5156162214236"></a><ul id="zh-cn_topic_0121505665_ul5156162214236"><li>手动输入模板格式的消息：在<span class="parmname" id="zh-cn_topic_0121505665_parmname9391225244"><a name="zh-cn_topic_0121505665_parmname9391225244"></a><a name="zh-cn_topic_0121505665_parmname9391225244"></a>“消息内容”</span>直接输入。</li><li>通过工具自动生成模板格式的消息：单击<span class="uicontrol" id="zh-cn_topic_0121505665_uicontrol119214173504"><a name="zh-cn_topic_0121505665_uicontrol119214173504"></a><a name="zh-cn_topic_0121505665_uicontrol119214173504"></a>“生成模板消息”</span>，在弹出的对话框中，选择<span class="parmname" id="zh-cn_topic_0121505665_parmname16903133312256"><a name="zh-cn_topic_0121505665_parmname16903133312256"></a><a name="zh-cn_topic_0121505665_parmname16903133312256"></a>“模板名称”</span>，并设置{tag}的值。</li></ul>
</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0121505665_row86829521857"><td class="cellrowborder" valign="top" width="21.740000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0121505665_p168315219518"><a name="zh-cn_topic_0121505665_p168315219518"></a><a name="zh-cn_topic_0121505665_p168315219518"></a>消息内容</p>
</td>
<td class="cellrowborder" valign="top" width="9.92%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0121505665_p668310521753"><a name="zh-cn_topic_0121505665_p668310521753"></a><a name="zh-cn_topic_0121505665_p668310521753"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="68.34%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0121505665_p176838521510"><a name="zh-cn_topic_0121505665_p176838521510"></a><a name="zh-cn_topic_0121505665_p176838521510"></a>填写消息的内容，不同消息类型的填写要求如下：</p>
<a name="zh-cn_topic_0121505665_ul12110204962819"></a><a name="zh-cn_topic_0121505665_ul12110204962819"></a><ul id="zh-cn_topic_0121505665_ul12110204962819"><li>文本消息：大小不超过10KB。</li><li>JSON消息：JSON消息中必须有Default协议，大小不超过10KB。<p id="zh-cn_topic_0121505665_p3357911183013"><a name="zh-cn_topic_0121505665_p3357911183013"></a><a name="zh-cn_topic_0121505665_p3357911183013"></a>示例如下：</p>
<pre class="screen" id="zh-cn_topic_0121505665_screen1111832917339"><a name="zh-cn_topic_0121505665_screen1111832917339"></a><a name="zh-cn_topic_0121505665_screen1111832917339"></a>{
  "default": "Dear Sir or Madam, this is a default message.",
  "email": "Dear Sir or Madam, this is an email message.",
  "http": "{'message':'Dear Sir or Madam, this is an HTTP message.'}",
  "https": "{'message':'Dear Sir or Madam, this is an HTTPS message.'}",
  "sms": "This is an SMS message."
    }</pre>
</li><li>模板消息：大小不超过10KB。<p id="zh-cn_topic_0121505665_p14393627193819"><a name="zh-cn_topic_0121505665_p14393627193819"></a><a name="zh-cn_topic_0121505665_p14393627193819"></a>示例如下：</p>
<pre class="screen" id="zh-cn_topic_0121505665_screen1768623311385"><a name="zh-cn_topic_0121505665_screen1768623311385"></a><a name="zh-cn_topic_0121505665_screen1768623311385"></a>"message_template_name":"confirm_message",
"tags":{
    "topic_urn":"urn:smn:regionId:xxxx:SMN_01"
     }</pre>
<p id="zh-cn_topic_0121505665_p261631719454"><a name="zh-cn_topic_0121505665_p261631719454"></a><a name="zh-cn_topic_0121505665_p261631719454"></a>其中，<span class="parmname" id="zh-cn_topic_0121505665_parmname133914315451"><a name="zh-cn_topic_0121505665_parmname133914315451"></a><a name="zh-cn_topic_0121505665_parmname133914315451"></a>“message_template_name”</span>为模板名称，<span class="parmname" id="zh-cn_topic_0121505665_parmname10694132754611"><a name="zh-cn_topic_0121505665_parmname10694132754611"></a><a name="zh-cn_topic_0121505665_parmname10694132754611"></a>“tags”</span>为模板中所有的tag标签。</p>
</li></ul>
<p id="zh-cn_topic_0121505665_p1847153271012"><a name="zh-cn_topic_0121505665_p1847153271012"></a><a name="zh-cn_topic_0121505665_p1847153271012"></a>如需了解更多SMN的配置说明，请参见<span id="zh-cn_topic_0121505665_cite270151510116"><a name="zh-cn_topic_0121505665_cite270151510116"></a><a name="zh-cn_topic_0121505665_cite270151510116"></a>《消息通知服务用户指南》</span>的<a href="https://support.huaweicloud.com/usermanual-smn/zh-cn_topic_0044170758.html" target="_blank" rel="noopener noreferrer">发布主题消息简介</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  高级参数

<a name="zh-cn_topic_0121505665_table58040457102411"></a>
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

