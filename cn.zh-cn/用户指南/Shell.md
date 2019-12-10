# Shell<a name="dayu_01_0459"></a>

## 功能<a name="zh-cn_topic_0113842761_section44280035173841"></a>

通过Shell节点执行用户指定的Shell脚本。

>![](public_sys-resources/icon-note.gif) **说明：**   
>Shell节点的后续节点可以通过EL表达式**\#\{Job.getNodeOutput\(\)\}**，获取Shell脚本最后4000字符的标准输出。  
>使用示例：  
>获取某个Shell脚本（脚本名称为shell\_job1）输出值包含“<name\>jack<name1\>”的内容，EL表达式如下所示：  
>```  
>#{StringUtil.substringBetween(Job.getNodeOutput("shell_job1"),"<name>","<name1>")}  
>```  

## 参数<a name="zh-cn_topic_0113842761_section1685263812380"></a>

用户可以参考[表1](#zh-cn_topic_0113842761_table3764823994826)和[表2](#zh-cn_topic_0113842761_table58040457102411)配置Shell节点的参数。

**表 1**  属性参数

<a name="zh-cn_topic_0113842761_table3764823994826"></a>
<table><thead align="left"><tr id="zh-cn_topic_0113842761_row3170822394826"><th class="cellrowborder" valign="top" width="28.07%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0113842761_p2984581994826"><a name="zh-cn_topic_0113842761_p2984581994826"></a><a name="zh-cn_topic_0113842761_p2984581994826"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="15.659999999999998%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0113842761_p159227094826"><a name="zh-cn_topic_0113842761_p159227094826"></a><a name="zh-cn_topic_0113842761_p159227094826"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="56.269999999999996%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0113842761_p6186505494826"><a name="zh-cn_topic_0113842761_p6186505494826"></a><a name="zh-cn_topic_0113842761_p6186505494826"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0113842761_row3614415394826"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0113842761_p1225314550306"><a name="zh-cn_topic_0113842761_p1225314550306"></a><a name="zh-cn_topic_0113842761_p1225314550306"></a>SQL或脚本</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0113842761_p4617707494826"><a name="zh-cn_topic_0113842761_p4617707494826"></a><a name="zh-cn_topic_0113842761_p4617707494826"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0113842761_p61023369712"><a name="zh-cn_topic_0113842761_p61023369712"></a><a name="zh-cn_topic_0113842761_p61023369712"></a>可以选择SQL语句或SQL脚本。</p>
<a name="zh-cn_topic_0113842761_ul1857020154912"></a><a name="zh-cn_topic_0113842761_ul1857020154912"></a><ul id="zh-cn_topic_0113842761_ul1857020154912"><li>SQL语句<p id="zh-cn_topic_0113842761_p74181856897"><a name="zh-cn_topic_0113842761_p74181856897"></a><a name="zh-cn_topic_0113842761_p74181856897"></a>单击<span class="parmname" id="zh-cn_topic_0113842761_parmname116422231331"><a name="zh-cn_topic_0113842761_parmname116422231331"></a><a name="zh-cn_topic_0113842761_parmname116422231331"></a>“SQL语句”</span>参数下的文本框，在<span class="wintitle" id="zh-cn_topic_0113842761_wintitle28741019181110"><a name="zh-cn_topic_0113842761_wintitle28741019181110"></a><a name="zh-cn_topic_0113842761_wintitle28741019181110"></a>“SQL语句”</span>页面输入需要执行的SQL语句。</p>
</li><li>SQL脚本<p id="zh-cn_topic_0113842761_p310193912912"><a name="zh-cn_topic_0113842761_p310193912912"></a><a name="zh-cn_topic_0113842761_p310193912912"></a>在<span class="parmname" id="zh-cn_topic_0113842761_parmname18319357534"><a name="zh-cn_topic_0113842761_parmname18319357534"></a><a name="zh-cn_topic_0113842761_parmname18319357534"></a>“脚本路径”</span>参数后选择需要执行的脚本。如果脚本未创建，请参考<a href="新建脚本.md">新建脚本</a>和<a href="开发SQL脚本.md">开发SQL脚本</a>先创建和开发脚本。</p>
<div class="note" id="zh-cn_topic_0113842761_note15529154994813"><a name="zh-cn_topic_0113842761_note15529154994813"></a><a name="zh-cn_topic_0113842761_note15529154994813"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0113842761_p18530849164811"><a name="zh-cn_topic_0113842761_p18530849164811"></a><a name="zh-cn_topic_0113842761_p18530849164811"></a>若选择SQL语句方式，DLF将无法解析您输入SQL语句中携带的参数。</p>
</div></div>
</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0113842761_row5244434102217"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0113842761_p19439198113719"><a name="zh-cn_topic_0113842761_p19439198113719"></a><a name="zh-cn_topic_0113842761_p19439198113719"></a>主机连接</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0113842761_p154390813712"><a name="zh-cn_topic_0113842761_p154390813712"></a><a name="zh-cn_topic_0113842761_p154390813712"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0113842761_p943913843711"><a name="zh-cn_topic_0113842761_p943913843711"></a><a name="zh-cn_topic_0113842761_p943913843711"></a>选择执行Shell脚本的主机。</p>
</td>
</tr>
<tr id="zh-cn_topic_0113842761_row46298121478"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0113842761_p96301112154711"><a name="zh-cn_topic_0113842761_p96301112154711"></a><a name="zh-cn_topic_0113842761_p96301112154711"></a>参数</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0113842761_p146303127471"><a name="zh-cn_topic_0113842761_p146303127471"></a><a name="zh-cn_topic_0113842761_p146303127471"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0113842761_p7630111294718"><a name="zh-cn_topic_0113842761_p7630111294718"></a><a name="zh-cn_topic_0113842761_p7630111294718"></a>填写执行Shell脚本时，向脚本传递的参数，参数之间使用空格分隔，例如：a b c。此处的<span class="parmname" id="zh-cn_topic_0113842761_zh-cn_topic_0114018164_parmname135345411556"><a name="zh-cn_topic_0113842761_zh-cn_topic_0114018164_parmname135345411556"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0114018164_parmname135345411556"></a>“参数”</span>需要在Shell脚本中引用，否则配置无效。</p>
</td>
</tr>
<tr id="zh-cn_topic_0113842761_row47451655172218"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0113842761_p197452556220"><a name="zh-cn_topic_0113842761_p197452556220"></a><a name="zh-cn_topic_0113842761_p197452556220"></a>交互式输入</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0113842761_p574595572218"><a name="zh-cn_topic_0113842761_p574595572218"></a><a name="zh-cn_topic_0113842761_p574595572218"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0113842761_p13745175515228"><a name="zh-cn_topic_0113842761_p13745175515228"></a><a name="zh-cn_topic_0113842761_p13745175515228"></a>填写交互式参数，即执行Shell脚本的过程中，需要用户输入的交互式信息（例如密码）。交互式参数之间以回车符分隔，Shell脚本根据交互情况按顺序读取参数值。</p>
</td>
</tr>
<tr id="zh-cn_topic_0113842761_row173916552814"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0113842761_p246794194826"><a name="zh-cn_topic_0113842761_p246794194826"></a><a name="zh-cn_topic_0113842761_p246794194826"></a>节点名称</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0113842761_p6568554794826"><a name="zh-cn_topic_0113842761_p6568554794826"></a><a name="zh-cn_topic_0113842761_p6568554794826"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0113842761_p1892909794826"><a name="zh-cn_topic_0113842761_p1892909794826"></a><a name="zh-cn_topic_0113842761_p1892909794826"></a><span id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_text44323307153939"><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_text44323307153939"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_text44323307153939"></a>节点</span>名称，可以包含中文、英文字母、数字、<span class="parmvalue" id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a>“_”</span>、<span class="parmvalue" id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a>“-”</span>、<span class="parmvalue" id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_parmvalue3773104413412"><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_parmvalue3773104413412"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_parmvalue3773104413412"></a>“/”</span>、<span class="parmvalue" id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a>“&lt;”</span>、<span class="parmvalue" id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a>“&gt;”</span>等各类特殊字符，长度为1～128个字符。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  高级参数

<a name="zh-cn_topic_0113842761_table58040457102411"></a>
<table><thead align="left"><tr id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_row27216578102411"><th class="cellrowborder" valign="top" width="28.07%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p57059205102411"><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p57059205102411"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p57059205102411"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="15.659999999999998%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p58392901102411"><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p58392901102411"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p58392901102411"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="56.269999999999996%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p32204521102411"><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p32204521102411"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p32204521102411"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_row51612113175"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p416115112178"><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p416115112178"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p416115112178"></a>节点状态轮询时间（秒）</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p101615110176"><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p101615110176"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p101615110176"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p4161191101716"><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p4161191101716"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p4161191101716"></a>设置轮询时间（1~60秒），每隔x秒查询一次<span id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_text1526241235118"><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_text1526241235118"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_text1526241235118"></a>节点</span>是否执行完成。</p>
</td>
</tr>
<tr id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_row5101045193916"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p147314419397"><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p147314419397"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p147314419397"></a>节点执行的最长时间</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p610124511390"><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p610124511390"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p610124511390"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p11011456393"><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p11011456393"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p11011456393"></a>设置<span id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_text380131541112"><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_text380131541112"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_text380131541112"></a>节点</span>执行的超时时间，如果<span id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_text1944213322118"><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_text1944213322118"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_text1944213322118"></a>节点</span>配置了重试，在超时时间内未执行完成，该节点将不会再重试，直接置为失败状态。</p>
</td>
</tr>
<tr id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_row58429402102411"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p5533912102858"><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p5533912102858"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p5533912102858"></a>失败重试</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p45593742102858"><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p45593742102858"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p45593742102858"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p2105628102858"><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p2105628102858"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p2105628102858"></a><span id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_text29185571161243"><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_text29185571161243"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_text29185571161243"></a>节点</span>执行失败后，是否重新执行<span id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_text58583828161245"><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_text58583828161245"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_text58583828161245"></a>节点</span>。</p>
<a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_ul18950660102858"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_ul18950660102858"></a><ul id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_ul18950660102858"><li>是：重新执行<span id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_text19139245161248"><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_text19139245161248"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_text19139245161248"></a>节点</span>，请配置以下参数。<a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_ul58608523102858"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_ul58608523102858"></a><ul id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_ul58608523102858"><li>最大重试次数</li><li>重试间隔时间（秒）</li></ul>
</li><li>否：默认值，不重新执行<span id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_text1328324161254"><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_text1328324161254"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_text1328324161254"></a>节点</span>。</li></ul>
<div class="note" id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_note69071033105815"><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_note69071033105815"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_note69071033105815"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p1590733314581"><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p1590733314581"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p1590733314581"></a>如果作业节点配置了重试，并且配置了超时时间，该节点执行超时后将不会再重试，直接置为失败状态。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_row29541959102411"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p13154928102858"><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p13154928102858"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p13154928102858"></a>失败策略</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p58916261102858"><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p58916261102858"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p58916261102858"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p7487822102858"><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p7487822102858"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_p7487822102858"></a><span id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_text5371194616130"><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_text5371194616130"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_text5371194616130"></a>节点</span>执行失败后的操作：</p>
<a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_ul281538102858"></a><a name="zh-cn_topic_0113842761_zh-cn_topic_0099822521_ul281538102858"></a><ul id="zh-cn_topic_0113842761_zh-cn_topic_0099822521_ul281538102858"><li>终止当前作业执行计划</li><li>继续执行下一作业</li><li>挂起当前作业执行计划</li></ul>
</td>
</tr>
</tbody>
</table>

