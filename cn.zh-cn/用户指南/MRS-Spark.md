# MRS Spark<a name="dayu_01_0455"></a>

## 功能<a name="zh-cn_topic_0101095437_section44280035173841"></a>

通过MRS Spark节点实现在MRS中执行预先定义的Spark作业。

## 参数<a name="zh-cn_topic_0101095437_section1791764173933"></a>

用户可参考[表1](#zh-cn_topic_0101095437_table3764823994826)和[表2](#zh-cn_topic_0101095437_table58040457102411)配置MRS Spark节点的参数。

**表 1**  属性参数

<a name="zh-cn_topic_0101095437_table3764823994826"></a>
<table><thead align="left"><tr id="zh-cn_topic_0101095437_row3170822394826"><th class="cellrowborder" valign="top" width="28.07%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0101095437_p2984581994826"><a name="zh-cn_topic_0101095437_p2984581994826"></a><a name="zh-cn_topic_0101095437_p2984581994826"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="15.659999999999998%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0101095437_p159227094826"><a name="zh-cn_topic_0101095437_p159227094826"></a><a name="zh-cn_topic_0101095437_p159227094826"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="56.269999999999996%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0101095437_p6186505494826"><a name="zh-cn_topic_0101095437_p6186505494826"></a><a name="zh-cn_topic_0101095437_p6186505494826"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0101095437_row1991457694826"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0101095437_p246794194826"><a name="zh-cn_topic_0101095437_p246794194826"></a><a name="zh-cn_topic_0101095437_p246794194826"></a>节点名称</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0101095437_p6568554794826"><a name="zh-cn_topic_0101095437_p6568554794826"></a><a name="zh-cn_topic_0101095437_p6568554794826"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0101095437_p1892909794826"><a name="zh-cn_topic_0101095437_p1892909794826"></a><a name="zh-cn_topic_0101095437_p1892909794826"></a><span id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_text44323307153939"><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_text44323307153939"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_text44323307153939"></a>节点</span>名称，可以包含中文、英文字母、数字、<span class="parmvalue" id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a>“_”</span>、<span class="parmvalue" id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a>“-”</span>、<span class="parmvalue" id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_parmvalue3773104413412"><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_parmvalue3773104413412"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_parmvalue3773104413412"></a>“/”</span>、<span class="parmvalue" id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a>“&lt;”</span>、<span class="parmvalue" id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a>“&gt;”</span>等各类特殊字符，长度为1～128个字符。</p>
</td>
</tr>
<tr id="zh-cn_topic_0101095437_row3614415394826"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0101095437_p4199531294826"><a name="zh-cn_topic_0101095437_p4199531294826"></a><a name="zh-cn_topic_0101095437_p4199531294826"></a>MRS集群名</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0101095437_p4617707494826"><a name="zh-cn_topic_0101095437_p4617707494826"></a><a name="zh-cn_topic_0101095437_p4617707494826"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0101095437_p4935552994826"><a name="zh-cn_topic_0101095437_p4935552994826"></a><a name="zh-cn_topic_0101095437_p4935552994826"></a>选择MRS集群。</p>
<div class="p" id="zh-cn_topic_0101095437_p14106064105658"><a name="zh-cn_topic_0101095437_p14106064105658"></a><a name="zh-cn_topic_0101095437_p14106064105658"></a>如需新建集群，请参考以下方法：<a name="zh-cn_topic_0101095437_zh-cn_topic_0101095234_zh-cn_topic_0099822521_ul46080727105259"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0101095234_zh-cn_topic_0099822521_ul46080727105259"></a><ul id="zh-cn_topic_0101095437_zh-cn_topic_0101095234_zh-cn_topic_0099822521_ul46080727105259"><li>单击<a name="zh-cn_topic_0101095437_zh-cn_topic_0101095234_image898618712510"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0101095234_image898618712510"></a><span><img id="zh-cn_topic_0101095437_zh-cn_topic_0101095234_image898618712510" src="figures/view-9.png"></span>，进入<span class="wintitle" id="zh-cn_topic_0101095437_zh-cn_topic_0101095234_wintitle3126196153112"><a name="zh-cn_topic_0101095437_zh-cn_topic_0101095234_wintitle3126196153112"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0101095234_wintitle3126196153112"></a>“集群列表”</span>页面新建MRS集群。</li><li>前往MRS管理控制台进行新建。</li></ul>
</div>
</td>
</tr>
<tr id="zh-cn_topic_0101095437_row4154658494826"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0101095437_p983015394826"><a name="zh-cn_topic_0101095437_p983015394826"></a><a name="zh-cn_topic_0101095437_p983015394826"></a>Spark作业名称</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0101095437_p5804493094826"><a name="zh-cn_topic_0101095437_p5804493094826"></a><a name="zh-cn_topic_0101095437_p5804493094826"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0101095437_p401892494826"><a name="zh-cn_topic_0101095437_p401892494826"></a><a name="zh-cn_topic_0101095437_p401892494826"></a>MRS作业名称，只能包含英文字母、数字、<span class="parmvalue" id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_parmvalue49148214105927"><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_parmvalue49148214105927"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_parmvalue49148214105927"></a>“_”</span>，且长度为1~64个字符。</p>
</td>
</tr>
<tr id="zh-cn_topic_0101095437_row303485991116"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0101095437_p423174491116"><a name="zh-cn_topic_0101095437_p423174491116"></a><a name="zh-cn_topic_0101095437_p423174491116"></a>Jar包资源</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0101095437_p51613311116"><a name="zh-cn_topic_0101095437_p51613311116"></a><a name="zh-cn_topic_0101095437_p51613311116"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0101095437_p154146861116"><a name="zh-cn_topic_0101095437_p154146861116"></a><a name="zh-cn_topic_0101095437_p154146861116"></a>选择Jar包，该Jar已上传至<a href="资源管理.md">资源管理</a>列表。</p>
</td>
</tr>
<tr id="zh-cn_topic_0101095437_row430706211158"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0101095437_p1332771411158"><a name="zh-cn_topic_0101095437_p1332771411158"></a><a name="zh-cn_topic_0101095437_p1332771411158"></a>Jar包参数</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0101095437_p580307511158"><a name="zh-cn_topic_0101095437_p580307511158"></a><a name="zh-cn_topic_0101095437_p580307511158"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0101095437_p28710511158"><a name="zh-cn_topic_0101095437_p28710511158"></a><a name="zh-cn_topic_0101095437_p28710511158"></a>Jar包的参数。</p>
</td>
</tr>
<tr id="zh-cn_topic_0101095437_row838395916445"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0101095437_p14384185924410"><a name="zh-cn_topic_0101095437_p14384185924410"></a><a name="zh-cn_topic_0101095437_p14384185924410"></a>运行程序参数</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0101095437_p2038416595446"><a name="zh-cn_topic_0101095437_p2038416595446"></a><a name="zh-cn_topic_0101095437_p2038416595446"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0101095437_p33849599443"><a name="zh-cn_topic_0101095437_p33849599443"></a><a name="zh-cn_topic_0101095437_p33849599443"></a>为本次执行的作业配置相关优化参数（例如线程、内存、CPU核数等），用于优化资源使用效率，提升作业的执行性能。</p>
<div class="note" id="zh-cn_topic_0101095437_note2073561518462"><a name="zh-cn_topic_0101095437_note2073561518462"></a><a name="zh-cn_topic_0101095437_note2073561518462"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0101095437_p1226422124616"><a name="zh-cn_topic_0101095437_p1226422124616"></a><a name="zh-cn_topic_0101095437_p1226422124616"></a>若集群为MRS 1.8.7版本或MRS 2.0.1之后版本，需要配置此参数。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0101095437_row4695054111155"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0101095437_p4489744011155"><a name="zh-cn_topic_0101095437_p4489744011155"></a><a name="zh-cn_topic_0101095437_p4489744011155"></a>输入数据路径</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0101095437_p1281406111155"><a name="zh-cn_topic_0101095437_p1281406111155"></a><a name="zh-cn_topic_0101095437_p1281406111155"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0101095437_p3130601011155"><a name="zh-cn_topic_0101095437_p3130601011155"></a><a name="zh-cn_topic_0101095437_p3130601011155"></a>选择输入数据所在的路径。</p>
</td>
</tr>
<tr id="zh-cn_topic_0101095437_row633704411335"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0101095437_p4353855211335"><a name="zh-cn_topic_0101095437_p4353855211335"></a><a name="zh-cn_topic_0101095437_p4353855211335"></a>输出数据路径</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0101095437_p3696185311335"><a name="zh-cn_topic_0101095437_p3696185311335"></a><a name="zh-cn_topic_0101095437_p3696185311335"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0101095437_p4112013911335"><a name="zh-cn_topic_0101095437_p4112013911335"></a><a name="zh-cn_topic_0101095437_p4112013911335"></a>选择输出数据存储的路径。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  高级参数

<a name="zh-cn_topic_0101095437_table58040457102411"></a>
<table><thead align="left"><tr id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_row27216578102411"><th class="cellrowborder" valign="top" width="28.07%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p57059205102411"><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p57059205102411"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p57059205102411"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="15.659999999999998%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p58392901102411"><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p58392901102411"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p58392901102411"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="56.269999999999996%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p32204521102411"><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p32204521102411"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p32204521102411"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_row51612113175"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p416115112178"><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p416115112178"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p416115112178"></a>节点状态轮询时间（秒）</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p101615110176"><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p101615110176"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p101615110176"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p4161191101716"><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p4161191101716"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p4161191101716"></a>设置轮询时间（1~60秒），每隔x秒查询一次<span id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_text1526241235118"><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_text1526241235118"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_text1526241235118"></a>节点</span>是否执行完成。</p>
</td>
</tr>
<tr id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_row5101045193916"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p147314419397"><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p147314419397"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p147314419397"></a>节点执行的最长时间</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p610124511390"><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p610124511390"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p610124511390"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p11011456393"><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p11011456393"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p11011456393"></a>设置<span id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_text380131541112"><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_text380131541112"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_text380131541112"></a>节点</span>执行的超时时间，如果<span id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_text1944213322118"><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_text1944213322118"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_text1944213322118"></a>节点</span>配置了重试，在超时时间内未执行完成，该节点将不会再重试，直接置为失败状态。</p>
</td>
</tr>
<tr id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_row58429402102411"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p5533912102858"><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p5533912102858"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p5533912102858"></a>失败重试</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p45593742102858"><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p45593742102858"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p45593742102858"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p2105628102858"><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p2105628102858"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p2105628102858"></a><span id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_text29185571161243"><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_text29185571161243"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_text29185571161243"></a>节点</span>执行失败后，是否重新执行<span id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_text58583828161245"><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_text58583828161245"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_text58583828161245"></a>节点</span>。</p>
<a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_ul18950660102858"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_ul18950660102858"></a><ul id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_ul18950660102858"><li>是：重新执行<span id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_text19139245161248"><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_text19139245161248"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_text19139245161248"></a>节点</span>，请配置以下参数。<a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_ul58608523102858"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_ul58608523102858"></a><ul id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_ul58608523102858"><li>最大重试次数</li><li>重试间隔时间（秒）</li></ul>
</li><li>否：默认值，不重新执行<span id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_text1328324161254"><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_text1328324161254"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_text1328324161254"></a>节点</span>。</li></ul>
<div class="note" id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_note69071033105815"><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_note69071033105815"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_note69071033105815"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p1590733314581"><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p1590733314581"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p1590733314581"></a>如果作业节点配置了重试，并且配置了超时时间，该节点执行超时后将不会再重试，直接置为失败状态。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_row29541959102411"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p13154928102858"><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p13154928102858"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p13154928102858"></a>失败策略</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p58916261102858"><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p58916261102858"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p58916261102858"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p7487822102858"><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p7487822102858"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_p7487822102858"></a><span id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_text5371194616130"><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_text5371194616130"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_text5371194616130"></a>节点</span>执行失败后的操作：</p>
<a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_ul281538102858"></a><a name="zh-cn_topic_0101095437_zh-cn_topic_0099822521_ul281538102858"></a><ul id="zh-cn_topic_0101095437_zh-cn_topic_0099822521_ul281538102858"><li>终止当前作业执行计划</li><li>继续执行下一作业</li><li>挂起当前作业执行计划</li></ul>
</td>
</tr>
</tbody>
</table>

