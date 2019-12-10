# Import GES<a name="dayu_01_0448"></a>

## 功能<a name="zh-cn_topic_0156398630_section884953485719"></a>

通过Import GES节点可以将OBS桶中的文件导入到GES的图中。

## 参数<a name="zh-cn_topic_0156398630_section1370012116332"></a>

用户可参考[表1](#zh-cn_topic_0156398630_table3764823994826)和[表2](#zh-cn_topic_0156398630_table58040457102411)配置Import GES节点的参数。

**表 1**  属性参数

<a name="zh-cn_topic_0156398630_table3764823994826"></a>
<table><thead align="left"><tr id="zh-cn_topic_0156398630_row3170822394826"><th class="cellrowborder" valign="top" width="28.07%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0156398630_p2984581994826"><a name="zh-cn_topic_0156398630_p2984581994826"></a><a name="zh-cn_topic_0156398630_p2984581994826"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="15.659999999999998%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0156398630_p159227094826"><a name="zh-cn_topic_0156398630_p159227094826"></a><a name="zh-cn_topic_0156398630_p159227094826"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="56.269999999999996%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0156398630_p6186505494826"><a name="zh-cn_topic_0156398630_p6186505494826"></a><a name="zh-cn_topic_0156398630_p6186505494826"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0156398630_row1991457694826"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0156398630_p246794194826"><a name="zh-cn_topic_0156398630_p246794194826"></a><a name="zh-cn_topic_0156398630_p246794194826"></a>节点名称</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0156398630_p6568554794826"><a name="zh-cn_topic_0156398630_p6568554794826"></a><a name="zh-cn_topic_0156398630_p6568554794826"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0156398630_p6428596455"><a name="zh-cn_topic_0156398630_p6428596455"></a><a name="zh-cn_topic_0156398630_p6428596455"></a><span id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_text44323307153939"><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_text44323307153939"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_text44323307153939"></a>节点</span>名称，可以包含中文、英文字母、数字、<span class="parmvalue" id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a>“_”</span>、<span class="parmvalue" id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a>“-”</span>、<span class="parmvalue" id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_parmvalue3773104413412"><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_parmvalue3773104413412"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_parmvalue3773104413412"></a>“/”</span>、<span class="parmvalue" id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a>“&lt;”</span>、<span class="parmvalue" id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a>“&gt;”</span>等各类特殊字符，长度为1～128个字符。</p>
</td>
</tr>
<tr id="zh-cn_topic_0156398630_row655815348539"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0156398630_p3559143410532"><a name="zh-cn_topic_0156398630_p3559143410532"></a><a name="zh-cn_topic_0156398630_p3559143410532"></a>图名称</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0156398630_p7559634155312"><a name="zh-cn_topic_0156398630_p7559634155312"></a><a name="zh-cn_topic_0156398630_p7559634155312"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0156398630_p9254133612259"><a name="zh-cn_topic_0156398630_p9254133612259"></a><a name="zh-cn_topic_0156398630_p9254133612259"></a>选择需要导入的图。</p>
<p id="zh-cn_topic_0156398630_p525483642519"><a name="zh-cn_topic_0156398630_p525483642519"></a><a name="zh-cn_topic_0156398630_p525483642519"></a>如需新建GES图，请前往GES管理控制台进行新建。</p>
</td>
</tr>
<tr id="zh-cn_topic_0156398630_row19689172419555"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0156398630_p1268932475513"><a name="zh-cn_topic_0156398630_p1268932475513"></a><a name="zh-cn_topic_0156398630_p1268932475513"></a>元数据</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0156398630_p16893248553"><a name="zh-cn_topic_0156398630_p16893248553"></a><a name="zh-cn_topic_0156398630_p16893248553"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0156398630_p176899243554"><a name="zh-cn_topic_0156398630_p176899243554"></a><a name="zh-cn_topic_0156398630_p176899243554"></a>选择对应的元数据。</p>
</td>
</tr>
<tr id="zh-cn_topic_0156398630_row86371351124313"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0156398630_p7637451144318"><a name="zh-cn_topic_0156398630_p7637451144318"></a><a name="zh-cn_topic_0156398630_p7637451144318"></a>边数据集</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0156398630_p36374516432"><a name="zh-cn_topic_0156398630_p36374516432"></a><a name="zh-cn_topic_0156398630_p36374516432"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0156398630_p1963755134320"><a name="zh-cn_topic_0156398630_p1963755134320"></a><a name="zh-cn_topic_0156398630_p1963755134320"></a>选择对应的边数据集。</p>
</td>
</tr>
<tr id="zh-cn_topic_0156398630_row1133144918432"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0156398630_p413354954311"><a name="zh-cn_topic_0156398630_p413354954311"></a><a name="zh-cn_topic_0156398630_p413354954311"></a>点数据集</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0156398630_p3133749164316"><a name="zh-cn_topic_0156398630_p3133749164316"></a><a name="zh-cn_topic_0156398630_p3133749164316"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0156398630_p16133049104311"><a name="zh-cn_topic_0156398630_p16133049104311"></a><a name="zh-cn_topic_0156398630_p16133049104311"></a>选择对应的点数据集。若不选择，则以边数据集中的点作为点数据集来源。</p>
</td>
</tr>
<tr id="zh-cn_topic_0156398630_row55943612550"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0156398630_p25917362557"><a name="zh-cn_topic_0156398630_p25917362557"></a><a name="zh-cn_topic_0156398630_p25917362557"></a>边处理</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0156398630_p145918369552"><a name="zh-cn_topic_0156398630_p145918369552"></a><a name="zh-cn_topic_0156398630_p145918369552"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0156398630_p5343856184817"><a name="zh-cn_topic_0156398630_p5343856184817"></a><a name="zh-cn_topic_0156398630_p5343856184817"></a>边处理支持如下几种方式：</p>
<a name="zh-cn_topic_0156398630_ul19567959125310"></a><a name="zh-cn_topic_0156398630_ul19567959125310"></a><ul id="zh-cn_topic_0156398630_ul19567959125310"><li>允许重复边</li><li>不允许重复，忽略之后的重复边</li><li>不允许重复，覆盖之前的重复边</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0156398630_row162541038123818"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0156398630_p625618385388"><a name="zh-cn_topic_0156398630_p625618385388"></a><a name="zh-cn_topic_0156398630_p625618385388"></a>重复边忽略Lable</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0156398630_p425610384382"><a name="zh-cn_topic_0156398630_p425610384382"></a><a name="zh-cn_topic_0156398630_p425610384382"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0156398630_p1491516165442"><a name="zh-cn_topic_0156398630_p1491516165442"></a><a name="zh-cn_topic_0156398630_p1491516165442"></a>重复边的定义，是否忽略Label。取值为true或者false，默认取true。</p>
<a name="zh-cn_topic_0156398630_ul29151016144416"></a><a name="zh-cn_topic_0156398630_ul29151016144416"></a><ul id="zh-cn_topic_0156398630_ul29151016144416"><li>true 表示重复边定义不包含Label，即用&lt;源点，终点&gt;标记一条边，不包含Label。</li><li>false 表示重复边定义包含Label，即用&lt;源点，终点，Label&gt;标记一条边。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0156398630_row1047074117386"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0156398630_p54701941113818"><a name="zh-cn_topic_0156398630_p54701941113818"></a><a name="zh-cn_topic_0156398630_p54701941113818"></a>日志存储路径</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0156398630_p1470741103820"><a name="zh-cn_topic_0156398630_p1470741103820"></a><a name="zh-cn_topic_0156398630_p1470741103820"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0156398630_p1647054115384"><a name="zh-cn_topic_0156398630_p1647054115384"></a><a name="zh-cn_topic_0156398630_p1647054115384"></a>用于存储导入图过程中不符合元数据定义的点、边数据集和详细日志。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  高级参数

<a name="zh-cn_topic_0156398630_table58040457102411"></a>
<table><thead align="left"><tr id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_row27216578102411"><th class="cellrowborder" valign="top" width="28.07%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p57059205102411"><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p57059205102411"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p57059205102411"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="15.659999999999998%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p58392901102411"><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p58392901102411"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p58392901102411"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="56.269999999999996%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p32204521102411"><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p32204521102411"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p32204521102411"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_row51612113175"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p416115112178"><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p416115112178"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p416115112178"></a>节点状态轮询时间（秒）</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p101615110176"><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p101615110176"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p101615110176"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p4161191101716"><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p4161191101716"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p4161191101716"></a>设置轮询时间（1~60秒），每隔x秒查询一次<span id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_text1526241235118"><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_text1526241235118"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_text1526241235118"></a>节点</span>是否执行完成。</p>
</td>
</tr>
<tr id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_row5101045193916"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p147314419397"><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p147314419397"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p147314419397"></a>节点执行的最长时间</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p610124511390"><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p610124511390"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p610124511390"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p11011456393"><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p11011456393"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p11011456393"></a>设置<span id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_text380131541112"><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_text380131541112"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_text380131541112"></a>节点</span>执行的超时时间，如果<span id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_text1944213322118"><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_text1944213322118"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_text1944213322118"></a>节点</span>配置了重试，在超时时间内未执行完成，该节点将不会再重试，直接置为失败状态。</p>
</td>
</tr>
<tr id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_row58429402102411"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p5533912102858"><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p5533912102858"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p5533912102858"></a>失败重试</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p45593742102858"><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p45593742102858"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p45593742102858"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p2105628102858"><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p2105628102858"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p2105628102858"></a><span id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_text29185571161243"><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_text29185571161243"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_text29185571161243"></a>节点</span>执行失败后，是否重新执行<span id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_text58583828161245"><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_text58583828161245"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_text58583828161245"></a>节点</span>。</p>
<a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_ul18950660102858"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_ul18950660102858"></a><ul id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_ul18950660102858"><li>是：重新执行<span id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_text19139245161248"><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_text19139245161248"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_text19139245161248"></a>节点</span>，请配置以下参数。<a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_ul58608523102858"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_ul58608523102858"></a><ul id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_ul58608523102858"><li>最大重试次数</li><li>重试间隔时间（秒）</li></ul>
</li><li>否：默认值，不重新执行<span id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_text1328324161254"><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_text1328324161254"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_text1328324161254"></a>节点</span>。</li></ul>
<div class="note" id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_note69071033105815"><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_note69071033105815"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_note69071033105815"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p1590733314581"><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p1590733314581"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p1590733314581"></a>如果作业节点配置了重试，并且配置了超时时间，该节点执行超时后将不会再重试，直接置为失败状态。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_row29541959102411"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p13154928102858"><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p13154928102858"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p13154928102858"></a>失败策略</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p58916261102858"><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p58916261102858"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p58916261102858"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p7487822102858"><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p7487822102858"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_p7487822102858"></a><span id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_text5371194616130"><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_text5371194616130"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_text5371194616130"></a>节点</span>执行失败后的操作：</p>
<a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_ul281538102858"></a><a name="zh-cn_topic_0156398630_zh-cn_topic_0099822521_ul281538102858"></a><ul id="zh-cn_topic_0156398630_zh-cn_topic_0099822521_ul281538102858"><li>终止当前作业执行计划</li><li>继续执行下一作业</li><li>挂起当前作业执行计划</li></ul>
</td>
</tr>
</tbody>
</table>

