# DIS Dump<a name="dayu_01_0445"></a>

## 功能<a name="zh-cn_topic_0121253875_section44280035173841"></a>

通过DIS Dump节点配置DIS的数据转储任务。

## 参数<a name="zh-cn_topic_0121253875_section6331447317395"></a>

用户可参考[表1](#zh-cn_topic_0121253875_table3764823994826)和[表2](#zh-cn_topic_0121253875_table58040457102411)配置DIS Dump节点的参数。

**表 1**  属性参数

<a name="zh-cn_topic_0121253875_table3764823994826"></a>
<table><thead align="left"><tr id="zh-cn_topic_0121253875_row3170822394826"><th class="cellrowborder" valign="top" width="28.07%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0121253875_p2984581994826"><a name="zh-cn_topic_0121253875_p2984581994826"></a><a name="zh-cn_topic_0121253875_p2984581994826"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="15.659999999999998%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0121253875_p159227094826"><a name="zh-cn_topic_0121253875_p159227094826"></a><a name="zh-cn_topic_0121253875_p159227094826"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="56.269999999999996%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0121253875_p6186505494826"><a name="zh-cn_topic_0121253875_p6186505494826"></a><a name="zh-cn_topic_0121253875_p6186505494826"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0121253875_row1991457694826"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0121253875_p246794194826"><a name="zh-cn_topic_0121253875_p246794194826"></a><a name="zh-cn_topic_0121253875_p246794194826"></a>节点名称</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0121253875_p6568554794826"><a name="zh-cn_topic_0121253875_p6568554794826"></a><a name="zh-cn_topic_0121253875_p6568554794826"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0121253875_p1892909794826"><a name="zh-cn_topic_0121253875_p1892909794826"></a><a name="zh-cn_topic_0121253875_p1892909794826"></a><span id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_text44323307153939"><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_text44323307153939"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_text44323307153939"></a>节点</span>名称，可以包含中文、英文字母、数字、<span class="parmvalue" id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a>“_”</span>、<span class="parmvalue" id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a>“-”</span>、<span class="parmvalue" id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_parmvalue3773104413412"><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_parmvalue3773104413412"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_parmvalue3773104413412"></a>“/”</span>、<span class="parmvalue" id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a>“&lt;”</span>、<span class="parmvalue" id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a>“&gt;”</span>等各类特殊字符，长度为1～128个字符。</p>
</td>
</tr>
<tr id="zh-cn_topic_0121253875_row3614415394826"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0121253875_p4199531294826"><a name="zh-cn_topic_0121253875_p4199531294826"></a><a name="zh-cn_topic_0121253875_p4199531294826"></a>通道名称</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0121253875_p4617707494826"><a name="zh-cn_topic_0121253875_p4617707494826"></a><a name="zh-cn_topic_0121253875_p4617707494826"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0121253875_p4935552994826"><a name="zh-cn_topic_0121253875_p4935552994826"></a><a name="zh-cn_topic_0121253875_p4935552994826"></a>选择或输入待配置的DIS通道，输入通道名称时支持引用作业参数和使用EL表达式（参见<a href="表达式概述.md#dayu_01_0494">表达式概述</a>）。</p>
<div class="p" id="zh-cn_topic_0121253875_p95346593"><a name="zh-cn_topic_0121253875_p95346593"></a><a name="zh-cn_topic_0121253875_p95346593"></a>如需新建DIS通道，请参考以下方法：<a name="zh-cn_topic_0121253875_zh-cn_topic_0118184395_zh-cn_topic_0099822521_ul46080727105259"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0118184395_zh-cn_topic_0099822521_ul46080727105259"></a><ul id="zh-cn_topic_0121253875_zh-cn_topic_0118184395_zh-cn_topic_0099822521_ul46080727105259"><li>单击<a name="zh-cn_topic_0121253875_zh-cn_topic_0118184395_image274717447175"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0118184395_image274717447175"></a><span><img id="zh-cn_topic_0121253875_zh-cn_topic_0118184395_image274717447175" src="figures/view.png"></span>，前往<span id="zh-cn_topic_0121253875_zh-cn_topic_0118184395_text193286818514"><a name="zh-cn_topic_0121253875_zh-cn_topic_0118184395_text193286818514"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0118184395_text193286818514"></a>DLF</span>的<span class="menucascade" id="zh-cn_topic_0121253875_zh-cn_topic_0118184395_menucascade1534810181012"><a name="zh-cn_topic_0121253875_zh-cn_topic_0118184395_menucascade1534810181012"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0118184395_menucascade1534810181012"></a>“<span class="uicontrol" id="zh-cn_topic_0121253875_zh-cn_topic_0118184395_uicontrol1821923716"><a name="zh-cn_topic_0121253875_zh-cn_topic_0118184395_uicontrol1821923716"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0118184395_uicontrol1821923716"></a><span id="zh-cn_topic_0121253875_zh-cn_topic_0118184395_text1795713398114"><a name="zh-cn_topic_0121253875_zh-cn_topic_0118184395_text1795713398114"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0118184395_text1795713398114"></a>数据集成</span></span> &gt; <span class="uicontrol" id="zh-cn_topic_0121253875_zh-cn_topic_0118184395_uicontrol183957281017"><a name="zh-cn_topic_0121253875_zh-cn_topic_0118184395_uicontrol183957281017"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0118184395_uicontrol183957281017"></a><span id="zh-cn_topic_0121253875_zh-cn_topic_0118184395_text63331510212"><a name="zh-cn_topic_0121253875_zh-cn_topic_0118184395_text63331510212"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0118184395_text63331510212"></a>DIS通道管理</span></span>”</span>页面新建DIS通道。</li><li>前往DIS管理控制台进行新建。</li></ul>
</div>
</td>
</tr>
<tr id="zh-cn_topic_0121253875_row14291718181712"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0121253875_p10291131819173"><a name="zh-cn_topic_0121253875_p10291131819173"></a><a name="zh-cn_topic_0121253875_p10291131819173"></a>转储任务重名策略</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0121253875_p529118186177"><a name="zh-cn_topic_0121253875_p529118186177"></a><a name="zh-cn_topic_0121253875_p529118186177"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0121253875_p132911518151713"><a name="zh-cn_topic_0121253875_p132911518151713"></a><a name="zh-cn_topic_0121253875_p132911518151713"></a>选择重名策略。当<span class="parmname" id="zh-cn_topic_0121253875_parmname1646103304920"><a name="zh-cn_topic_0121253875_parmname1646103304920"></a><a name="zh-cn_topic_0121253875_parmname1646103304920"></a>“转储服务类型”</span>配置的转储任务名称出现重名时，<span id="zh-cn_topic_0121253875_text149948227530"><a name="zh-cn_topic_0121253875_text149948227530"></a><a name="zh-cn_topic_0121253875_text149948227530"></a>DIS Dump</span>将根据重名策略进行下一步操作。</p>
<a name="zh-cn_topic_0121253875_ul11938101612190"></a><a name="zh-cn_topic_0121253875_ul11938101612190"></a><ul id="zh-cn_topic_0121253875_ul11938101612190"><li>忽略：不添加转储任务，并退出<span id="zh-cn_topic_0121253875_text109311327231"><a name="zh-cn_topic_0121253875_text109311327231"></a><a name="zh-cn_topic_0121253875_text109311327231"></a>DIS Dump</span>，<span id="zh-cn_topic_0121253875_text7969335101619"><a name="zh-cn_topic_0121253875_text7969335101619"></a><a name="zh-cn_topic_0121253875_text7969335101619"></a>DIS Dump</span>的状态为<span class="parmvalue" id="zh-cn_topic_0121253875_parmvalue4262185210167"><a name="zh-cn_topic_0121253875_parmvalue4262185210167"></a><a name="zh-cn_topic_0121253875_parmvalue4262185210167"></a>“成功”</span>。</li><li>覆盖：继续添加转储任务，覆盖已存在的重名转储任务。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0121253875_row4273161092410"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0121253875_p20275510172415"><a name="zh-cn_topic_0121253875_p20275510172415"></a><a name="zh-cn_topic_0121253875_p20275510172415"></a>转储服务类型</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0121253875_p1127591032414"><a name="zh-cn_topic_0121253875_p1127591032414"></a><a name="zh-cn_topic_0121253875_p1127591032414"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0121253875_ol168716015365"></a><a name="zh-cn_topic_0121253875_ol168716015365"></a><ol id="zh-cn_topic_0121253875_ol168716015365"><li>选择转储服务类型，目前支持转储至：<a name="zh-cn_topic_0121253875_ul7848154215135"></a><a name="zh-cn_topic_0121253875_ul7848154215135"></a><ul id="zh-cn_topic_0121253875_ul7848154215135"><li>CloudTable：通道里的流式数据存储在DIS中，并实时导入表格存储服务Cloudtable集群的HBase/OpenTSDB表。</li><li>OBS：通道里的流式数据存储在DIS中，并周期性导入对象存储服务OBS；通道里的实时文件数据传输完成后，导入OBS。</li></ul>
<div class="note" id="zh-cn_topic_0121253875_note13681207140"><a name="zh-cn_topic_0121253875_note13681207140"></a><a name="zh-cn_topic_0121253875_note13681207140"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0121253875_p66826031418"><a name="zh-cn_topic_0121253875_p66826031418"></a><a name="zh-cn_topic_0121253875_p66826031418"></a>转储至CloudTable，仅华北-北京一区域支持。</p>
</div></div>
</li><li>单击<a name="zh-cn_topic_0121253875_image1184814309555"></a><a name="zh-cn_topic_0121253875_image1184814309555"></a><span><img id="zh-cn_topic_0121253875_image1184814309555" src="figures/node_config.png"></span>，在弹出的对话框中配置转储任务的参数（参数说明请见<span id="zh-cn_topic_0121253875_cite887170123617"><a name="zh-cn_topic_0121253875_cite887170123617"></a><a name="zh-cn_topic_0121253875_cite887170123617"></a>《数据接入服务用户指南》</span>的<a href="https://support.huaweicloud.com/usermanual-dis/dis_01_0047.html" target="_blank" rel="noopener noreferrer">管理转储任务</a>）。</li></ol>
</td>
</tr>
</tbody>
</table>

**表 2**  高级参数

<a name="zh-cn_topic_0121253875_table58040457102411"></a>
<table><thead align="left"><tr id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_row27216578102411"><th class="cellrowborder" valign="top" width="28.07%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p57059205102411"><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p57059205102411"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p57059205102411"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="15.659999999999998%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p58392901102411"><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p58392901102411"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p58392901102411"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="56.269999999999996%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p32204521102411"><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p32204521102411"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p32204521102411"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_row51612113175"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p416115112178"><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p416115112178"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p416115112178"></a>节点状态轮询时间（秒）</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p101615110176"><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p101615110176"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p101615110176"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p4161191101716"><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p4161191101716"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p4161191101716"></a>设置轮询时间（1~60秒），每隔x秒查询一次<span id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_text1526241235118"><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_text1526241235118"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_text1526241235118"></a>节点</span>是否执行完成。</p>
</td>
</tr>
<tr id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_row5101045193916"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p147314419397"><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p147314419397"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p147314419397"></a>节点执行的最长时间</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p610124511390"><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p610124511390"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p610124511390"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p11011456393"><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p11011456393"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p11011456393"></a>设置<span id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_text380131541112"><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_text380131541112"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_text380131541112"></a>节点</span>执行的超时时间，如果<span id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_text1944213322118"><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_text1944213322118"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_text1944213322118"></a>节点</span>配置了重试，在超时时间内未执行完成，该节点将不会再重试，直接置为失败状态。</p>
</td>
</tr>
<tr id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_row58429402102411"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p5533912102858"><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p5533912102858"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p5533912102858"></a>失败重试</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p45593742102858"><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p45593742102858"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p45593742102858"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p2105628102858"><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p2105628102858"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p2105628102858"></a><span id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_text29185571161243"><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_text29185571161243"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_text29185571161243"></a>节点</span>执行失败后，是否重新执行<span id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_text58583828161245"><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_text58583828161245"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_text58583828161245"></a>节点</span>。</p>
<a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_ul18950660102858"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_ul18950660102858"></a><ul id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_ul18950660102858"><li>是：重新执行<span id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_text19139245161248"><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_text19139245161248"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_text19139245161248"></a>节点</span>，请配置以下参数。<a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_ul58608523102858"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_ul58608523102858"></a><ul id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_ul58608523102858"><li>最大重试次数</li><li>重试间隔时间（秒）</li></ul>
</li><li>否：默认值，不重新执行<span id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_text1328324161254"><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_text1328324161254"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_text1328324161254"></a>节点</span>。</li></ul>
<div class="note" id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_note69071033105815"><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_note69071033105815"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_note69071033105815"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p1590733314581"><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p1590733314581"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p1590733314581"></a>如果作业节点配置了重试，并且配置了超时时间，该节点执行超时后将不会再重试，直接置为失败状态。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_row29541959102411"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p13154928102858"><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p13154928102858"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p13154928102858"></a>失败策略</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p58916261102858"><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p58916261102858"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p58916261102858"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p7487822102858"><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p7487822102858"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_p7487822102858"></a><span id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_text5371194616130"><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_text5371194616130"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_text5371194616130"></a>节点</span>执行失败后的操作：</p>
<a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_ul281538102858"></a><a name="zh-cn_topic_0121253875_zh-cn_topic_0099822521_ul281538102858"></a><ul id="zh-cn_topic_0121253875_zh-cn_topic_0099822521_ul281538102858"><li>终止当前作业执行计划</li><li>继续执行下一作业</li><li>挂起当前作业执行计划</li></ul>
</td>
</tr>
</tbody>
</table>

