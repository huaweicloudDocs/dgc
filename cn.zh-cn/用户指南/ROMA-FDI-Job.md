# ROMA FDI Job<a name="dgc_01_1098"></a>

## 功能<a name="zh-cn_topic_0226206976_section17228524131210"></a>

通过ROMA FDI Job节点执行一个预先定义的ROMA Connect数据集成任务，实现源端到目标端的数据集成转换。

## 原理<a name="zh-cn_topic_0226206976_section07401729201213"></a>

该节点方便用户启动或者查询FDI任务是否正在运行。

## 参数<a name="section1656161955"></a>

ROMA FDI Job的参数配置，请参考以下内容：

**表 1**  属性参数

<a name="zh-cn_topic_0226206976_table647011333413"></a>
<table><thead align="left"><tr id="zh-cn_topic_0226206976_row34705331412"><th class="cellrowborder" valign="top" width="24.88%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0226206976_p54708331840"><a name="zh-cn_topic_0226206976_p54708331840"></a><a name="zh-cn_topic_0226206976_p54708331840"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="10.38%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0226206976_p747011337414"><a name="zh-cn_topic_0226206976_p747011337414"></a><a name="zh-cn_topic_0226206976_p747011337414"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="64.74%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0226206976_p14470203313410"><a name="zh-cn_topic_0226206976_p14470203313410"></a><a name="zh-cn_topic_0226206976_p14470203313410"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0226206976_row647013331646"><td class="cellrowborder" valign="top" width="24.88%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226206976_p2047013331042"><a name="zh-cn_topic_0226206976_p2047013331042"></a><a name="zh-cn_topic_0226206976_p2047013331042"></a>ROMA实例</p>
</td>
<td class="cellrowborder" valign="top" width="10.38%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226206976_p1470103313411"><a name="zh-cn_topic_0226206976_p1470103313411"></a><a name="zh-cn_topic_0226206976_p1470103313411"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="64.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226206976_p1547011332412"><a name="zh-cn_topic_0226206976_p1547011332412"></a><a name="zh-cn_topic_0226206976_p1547011332412"></a>选择一个已存在的ROMA实例。</p>
</td>
</tr>
<tr id="zh-cn_topic_0226206976_row2470163315410"><td class="cellrowborder" valign="top" width="24.88%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226206976_p104702331748"><a name="zh-cn_topic_0226206976_p104702331748"></a><a name="zh-cn_topic_0226206976_p104702331748"></a>FDI任务</p>
</td>
<td class="cellrowborder" valign="top" width="10.38%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226206976_p64706331749"><a name="zh-cn_topic_0226206976_p64706331749"></a><a name="zh-cn_topic_0226206976_p64706331749"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="64.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226206976_p8470183320416"><a name="zh-cn_topic_0226206976_p8470183320416"></a><a name="zh-cn_topic_0226206976_p8470183320416"></a>选择一个已存在的ROMA FDI任务。</p>
</td>
</tr>
<tr id="zh-cn_topic_0226206976_row14706331041"><td class="cellrowborder" valign="top" width="24.88%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226206976_p1470103314418"><a name="zh-cn_topic_0226206976_p1470103314418"></a><a name="zh-cn_topic_0226206976_p1470103314418"></a>节点名称</p>
</td>
<td class="cellrowborder" valign="top" width="10.38%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226206976_p1647020331146"><a name="zh-cn_topic_0226206976_p1647020331146"></a><a name="zh-cn_topic_0226206976_p1647020331146"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="64.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226206976_p1346974112913"><a name="zh-cn_topic_0226206976_p1346974112913"></a><a name="zh-cn_topic_0226206976_p1346974112913"></a><span id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_text44323307153939"><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_text44323307153939"></a><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_text44323307153939"></a>节点</span>名称，可以包含中文、英文字母、数字、<span class="parmvalue" id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a>“_”</span>、<span class="parmvalue" id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a>“-”</span>、<span class="parmvalue" id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_parmvalue3773104413412"><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_parmvalue3773104413412"></a><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_parmvalue3773104413412"></a>“/”</span>、<span class="parmvalue" id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a>“&lt;”</span>、<span class="parmvalue" id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a>“&gt;”</span>等各类特殊字符，长度为1～128个字符。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  高级参数

<a name="zh-cn_topic_0226206976_table58040457102411"></a>
<table><thead align="left"><tr id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_row27216578102411"><th class="cellrowborder" valign="top" width="24.88%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p57059205102411"><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p57059205102411"></a><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p57059205102411"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="10.14%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p58392901102411"><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p58392901102411"></a><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p58392901102411"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="64.98%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p32204521102411"><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p32204521102411"></a><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p32204521102411"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_row5101045193916"><td class="cellrowborder" valign="top" width="24.88%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p147314419397"><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p147314419397"></a><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p147314419397"></a>节点执行的最长时间</p>
</td>
<td class="cellrowborder" valign="top" width="10.14%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p610124511390"><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p610124511390"></a><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p610124511390"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="64.98%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p11011456393"><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p11011456393"></a><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p11011456393"></a>设置<span id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_text380131541112"><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_text380131541112"></a><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_text380131541112"></a>节点</span>执行的超时时间，如果<span id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_text1944213322118"><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_text1944213322118"></a><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_text1944213322118"></a>节点</span>配置了重试，在超时时间内未执行完成，该节点将不会再重试，直接置为失败状态。</p>
</td>
</tr>
<tr id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_row58429402102411"><td class="cellrowborder" valign="top" width="24.88%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p5533912102858"><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p5533912102858"></a><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p5533912102858"></a>失败重试</p>
</td>
<td class="cellrowborder" valign="top" width="10.14%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p45593742102858"><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p45593742102858"></a><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p45593742102858"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="64.98%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p2105628102858"><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p2105628102858"></a><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p2105628102858"></a><span id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_text29185571161243"><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_text29185571161243"></a><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_text29185571161243"></a>节点</span>执行失败后，是否重新执行<span id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_text58583828161245"><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_text58583828161245"></a><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_text58583828161245"></a>节点</span>。</p>
<a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_ul18950660102858"></a><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_ul18950660102858"></a><ul id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_ul18950660102858"><li>是：重新执行<span id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_text19139245161248"><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_text19139245161248"></a><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_text19139245161248"></a>节点</span>，请配置以下参数。<a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_ul58608523102858"></a><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_ul58608523102858"></a><ul id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_ul58608523102858"><li>最大重试次数</li><li>重试间隔时间（秒）</li></ul>
</li><li>否：默认值，不重新执行<span id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_text1328324161254"><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_text1328324161254"></a><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_text1328324161254"></a>节点</span>。</li></ul>
<div class="note" id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_note69071033105815"><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_note69071033105815"></a><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_note69071033105815"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p1590733314581"><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p1590733314581"></a><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p1590733314581"></a>如果作业节点配置了重试，并且配置了超时时间，该节点执行超时后将不会再重试，直接置为失败状态。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_row29541959102411"><td class="cellrowborder" valign="top" width="24.88%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p13154928102858"><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p13154928102858"></a><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p13154928102858"></a>失败策略</p>
</td>
<td class="cellrowborder" valign="top" width="10.14%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p58916261102858"><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p58916261102858"></a><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p58916261102858"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="64.98%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p7487822102858"><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p7487822102858"></a><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_p7487822102858"></a><span id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_text5371194616130"><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_text5371194616130"></a><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_text5371194616130"></a>节点</span>执行失败后的操作：</p>
<a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_ul281538102858"></a><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_ul281538102858"></a><ul id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_ul281538102858"><li>终止后续节点执行计划</li><li>终止当前作业执行计划</li><li>继续执行下一作业</li><li>挂起当前作业执行计划</li></ul>
</td>
</tr>
</tbody>
</table>

