# CS Job<a name="dayu_01_0449"></a>

## 功能<a name="zh-cn_topic_0118184396_section44280035173841"></a>

通过CS Job节点执行一个预先定义的CS作业，实现实时流式大数据分析。

## 背景信息<a name="zh-cn_topic_0118184396_section0314101341011"></a>

该节点方便用户启动或者查询CS作业是否正在运行。当选择作业类型不是‘选择已存在的实时作业’时，DLF会根据在节点中配置的作业情况，进行创建和启动作业。方便用户自定义作业以及使用DLF作业参数。

## 参数<a name="zh-cn_topic_0118184396_section6331447317395"></a>

用户可参考[表1](#zh-cn_topic_0118184396_table107571217101312)和[表2](#zh-cn_topic_0118184396_table58040457102411)配置CS Job节点的参数。

**表 1**  属性参数

<a name="zh-cn_topic_0118184396_table107571217101312"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118184396_row9757117131310"><th class="cellrowborder" valign="top" width="28.622862286228624%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118184396_p47841334181318"><a name="zh-cn_topic_0118184396_p47841334181318"></a><a name="zh-cn_topic_0118184396_p47841334181318"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="15.271527152715272%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118184396_p13784834101314"><a name="zh-cn_topic_0118184396_p13784834101314"></a><a name="zh-cn_topic_0118184396_p13784834101314"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="56.10561056105611%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118184396_p378418347131"><a name="zh-cn_topic_0118184396_p378418347131"></a><a name="zh-cn_topic_0118184396_p378418347131"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118184396_row137571017101315"><td class="cellrowborder" valign="top" width="28.622862286228624%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_p775771715138"><a name="zh-cn_topic_0118184396_p775771715138"></a><a name="zh-cn_topic_0118184396_p775771715138"></a>作业类型</p>
</td>
<td class="cellrowborder" valign="top" width="15.271527152715272%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_p1075781718137"><a name="zh-cn_topic_0118184396_p1075781718137"></a><a name="zh-cn_topic_0118184396_p1075781718137"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.10561056105611%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p19757917141310"><a name="zh-cn_topic_0118184396_p19757917141310"></a><a name="zh-cn_topic_0118184396_p19757917141310"></a>选择CS的作业类型：</p>
<a name="zh-cn_topic_0118184396_ul10176119151411"></a><a name="zh-cn_topic_0118184396_ul10176119151411"></a><ul id="zh-cn_topic_0118184396_ul10176119151411"><li>选择已存在的实时流作业</li><li>Flink SQL作业</li><li>Flink自定义作业</li><li>Spark自定义作业</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row1075701714133"><td class="cellrowborder" colspan="3" valign="top" headers="mcps1.2.4.1.1 mcps1.2.4.1.2 mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p675791713133"><a name="zh-cn_topic_0118184396_p675791713133"></a><a name="zh-cn_topic_0118184396_p675791713133"></a><strong id="zh-cn_topic_0118184396_b152355578237"><a name="zh-cn_topic_0118184396_b152355578237"></a><a name="zh-cn_topic_0118184396_b152355578237"></a>选择已存在的实时流作业</strong></p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row875711791310"><td class="cellrowborder" valign="top" width="28.622862286228624%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_p97571817171315"><a name="zh-cn_topic_0118184396_p97571817171315"></a><a name="zh-cn_topic_0118184396_p97571817171315"></a>实时流作业名称</p>
</td>
<td class="cellrowborder" valign="top" width="15.271527152715272%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_p27571317101312"><a name="zh-cn_topic_0118184396_p27571317101312"></a><a name="zh-cn_topic_0118184396_p27571317101312"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.10561056105611%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p9254133612259"><a name="zh-cn_topic_0118184396_p9254133612259"></a><a name="zh-cn_topic_0118184396_p9254133612259"></a>选择需要执行的CS作业。</p>
<div class="p" id="zh-cn_topic_0118184396_p525483642519"><a name="zh-cn_topic_0118184396_p525483642519"></a><a name="zh-cn_topic_0118184396_p525483642519"></a>如需新建CS作业，请参考以下方法：<a name="zh-cn_topic_0118184396_ul0254236172512"></a><a name="zh-cn_topic_0118184396_ul0254236172512"></a><ul id="zh-cn_topic_0118184396_ul0254236172512"><li>单击<a name="zh-cn_topic_0118184396_image154725484238"></a><a name="zh-cn_topic_0118184396_image154725484238"></a><span><img id="zh-cn_topic_0118184396_image154725484238" src="figures/icon-dlf-view.png"></span>，前往<span id="zh-cn_topic_0118184396_text14254153617251"><a name="zh-cn_topic_0118184396_text14254153617251"></a><a name="zh-cn_topic_0118184396_text14254153617251"></a>DLF</span>的<span class="menucascade" id="zh-cn_topic_0118184396_menucascade62541336132510"><a name="zh-cn_topic_0118184396_menucascade62541336132510"></a><a name="zh-cn_topic_0118184396_menucascade62541336132510"></a>“<span class="uicontrol" id="zh-cn_topic_0118184396_uicontrol1125411365255"><a name="zh-cn_topic_0118184396_uicontrol1125411365255"></a><a name="zh-cn_topic_0118184396_uicontrol1125411365255"></a><span id="zh-cn_topic_0118184396_text17254436112513"><a name="zh-cn_topic_0118184396_text17254436112513"></a><a name="zh-cn_topic_0118184396_text17254436112513"></a>数据集成</span></span>”</span>页面新建CS作业。</li><li>前往CS管理控制台进行新建。</li></ul>
</div>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row57572170135"><td class="cellrowborder" valign="top" width="28.622862286228624%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_p19757121711137"><a name="zh-cn_topic_0118184396_p19757121711137"></a><a name="zh-cn_topic_0118184396_p19757121711137"></a>节点名称</p>
</td>
<td class="cellrowborder" valign="top" width="15.271527152715272%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_p27572017121317"><a name="zh-cn_topic_0118184396_p27572017121317"></a><a name="zh-cn_topic_0118184396_p27572017121317"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.10561056105611%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p53971545123915"><a name="zh-cn_topic_0118184396_p53971545123915"></a><a name="zh-cn_topic_0118184396_p53971545123915"></a><span id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text44323307153939"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text44323307153939"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text44323307153939"></a>节点</span>名称，可以包含中文、英文字母、数字、<span class="parmvalue" id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a>“_”</span>、<span class="parmvalue" id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a>“-”</span>、<span class="parmvalue" id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_parmvalue3773104413412"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_parmvalue3773104413412"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_parmvalue3773104413412"></a>“/”</span>、<span class="parmvalue" id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a>“&lt;”</span>、<span class="parmvalue" id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a>“&gt;”</span>等各类特殊字符，长度为1～128个字符。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row4757117181311"><td class="cellrowborder" colspan="3" valign="top" headers="mcps1.2.4.1.1 mcps1.2.4.1.2 mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p4757617121312"><a name="zh-cn_topic_0118184396_p4757617121312"></a><a name="zh-cn_topic_0118184396_p4757617121312"></a><strong id="zh-cn_topic_0118184396_b7329246121010"><a name="zh-cn_topic_0118184396_b7329246121010"></a><a name="zh-cn_topic_0118184396_b7329246121010"></a>Flink SQL作业</strong></p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row57571117191310"><td class="cellrowborder" valign="top" width="28.622862286228624%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_p475731719134"><a name="zh-cn_topic_0118184396_p475731719134"></a><a name="zh-cn_topic_0118184396_p475731719134"></a>SQL脚本</p>
</td>
<td class="cellrowborder" valign="top" width="15.271527152715272%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_p2561551134618"><a name="zh-cn_topic_0118184396_p2561551134618"></a><a name="zh-cn_topic_0118184396_p2561551134618"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.10561056105611%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p14704011164827"><a name="zh-cn_topic_0118184396_p14704011164827"></a><a name="zh-cn_topic_0118184396_p14704011164827"></a>选择需要执行的脚本。如果脚本未创建，请参考<a href="新建脚本.md">新建脚本</a>和<a href="开发SQL脚本.md">开发SQL脚本</a>先创建和开发脚本。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row67578177138"><td class="cellrowborder" valign="top" width="28.622862286228624%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_p075791714135"><a name="zh-cn_topic_0118184396_p075791714135"></a><a name="zh-cn_topic_0118184396_p075791714135"></a>脚本参数</p>
</td>
<td class="cellrowborder" valign="top" width="15.271527152715272%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_p20757217181318"><a name="zh-cn_topic_0118184396_p20757217181318"></a><a name="zh-cn_topic_0118184396_p20757217181318"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.10561056105611%" headers="mcps1.2.4.1.3 "><p id="p1968518451852"><a name="p1968518451852"></a><a name="p1968518451852"></a>关联的SQL脚本如果使用了参数，此处显示参数名称，请在参数名称后的输入框配置参数值。参数值支持使用<a href="函数概述.md#dayu_01_0471">内置函数</a>和<a href="表达式概述.md#dayu_01_0494">EL表达式</a>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row12757517121318"><td class="cellrowborder" valign="top" width="28.622862286228624%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_p14757191781310"><a name="zh-cn_topic_0118184396_p14757191781310"></a><a name="zh-cn_topic_0118184396_p14757191781310"></a>CloudStream集群</p>
</td>
<td class="cellrowborder" valign="top" width="15.271527152715272%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_p2757171715131"><a name="zh-cn_topic_0118184396_p2757171715131"></a><a name="zh-cn_topic_0118184396_p2757171715131"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.10561056105611%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p13757131715136"><a name="zh-cn_topic_0118184396_p13757131715136"></a><a name="zh-cn_topic_0118184396_p13757131715136"></a>选择CS集群。如需创建新的CS集群，请前往CS控制台操作。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row875719177132"><td class="cellrowborder" valign="top" width="28.622862286228624%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_p1175711720131"><a name="zh-cn_topic_0118184396_p1175711720131"></a><a name="zh-cn_topic_0118184396_p1175711720131"></a>SPUs</p>
</td>
<td class="cellrowborder" valign="top" width="15.271527152715272%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_p1375741712138"><a name="zh-cn_topic_0118184396_p1375741712138"></a><a name="zh-cn_topic_0118184396_p1375741712138"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.10561056105611%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p075719178132"><a name="zh-cn_topic_0118184396_p075719178132"></a><a name="zh-cn_topic_0118184396_p075719178132"></a>选择流处理单元，1SPU=1核4G的资源配置。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row14757191711139"><td class="cellrowborder" valign="top" width="28.622862286228624%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_p11757817161316"><a name="zh-cn_topic_0118184396_p11757817161316"></a><a name="zh-cn_topic_0118184396_p11757817161316"></a>并行数</p>
</td>
<td class="cellrowborder" valign="top" width="15.271527152715272%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_p575781710131"><a name="zh-cn_topic_0118184396_p575781710131"></a><a name="zh-cn_topic_0118184396_p575781710131"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.10561056105611%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p1175721711134"><a name="zh-cn_topic_0118184396_p1175721711134"></a><a name="zh-cn_topic_0118184396_p1175721711134"></a>选择同时运行CS作业的任务数，建议设置为SPU的1~2倍。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row651042763016"><td class="cellrowborder" valign="top" width="28.622862286228624%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_p15101827103012"><a name="zh-cn_topic_0118184396_p15101827103012"></a><a name="zh-cn_topic_0118184396_p15101827103012"></a>UDF Jar</p>
</td>
<td class="cellrowborder" valign="top" width="15.271527152715272%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_p85101227193014"><a name="zh-cn_topic_0118184396_p85101227193014"></a><a name="zh-cn_topic_0118184396_p85101227193014"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="56.10561056105611%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p16885155195119"><a name="zh-cn_topic_0118184396_p16885155195119"></a><a name="zh-cn_topic_0118184396_p16885155195119"></a>SQL中可调用插入Jar包中的自定义函数。用户需先将Jar包上传至OBS桶中。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row1277261731314"><td class="cellrowborder" valign="top" width="28.622862286228624%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_p1377241731318"><a name="zh-cn_topic_0118184396_p1377241731318"></a><a name="zh-cn_topic_0118184396_p1377241731318"></a>异常自动启动</p>
</td>
<td class="cellrowborder" valign="top" width="15.271527152715272%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_p137721917121313"><a name="zh-cn_topic_0118184396_p137721917121313"></a><a name="zh-cn_topic_0118184396_p137721917121313"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="56.10561056105611%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p16772141761315"><a name="zh-cn_topic_0118184396_p16772141761315"></a><a name="zh-cn_topic_0118184396_p16772141761315"></a>设置是否启动异常自动重启功能，当CS作业异常时自动重启并恢复CS作业。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row1321610692"><td class="cellrowborder" valign="top" width="28.622862286228624%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_p1034101014916"><a name="zh-cn_topic_0118184396_p1034101014916"></a><a name="zh-cn_topic_0118184396_p1034101014916"></a>实时流作业名称</p>
</td>
<td class="cellrowborder" valign="top" width="15.271527152715272%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_p193419102919"><a name="zh-cn_topic_0118184396_p193419102919"></a><a name="zh-cn_topic_0118184396_p193419102919"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.10561056105611%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p13601191313536"><a name="zh-cn_topic_0118184396_p13601191313536"></a><a name="zh-cn_topic_0118184396_p13601191313536"></a>Flink SQL作业名称，只能由字母、中文、数字、中划线和下划线组成，并且长度为1～57字节。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row877221771313"><td class="cellrowborder" valign="top" width="28.622862286228624%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_p18772417121311"><a name="zh-cn_topic_0118184396_p18772417121311"></a><a name="zh-cn_topic_0118184396_p18772417121311"></a>节点名称</p>
</td>
<td class="cellrowborder" valign="top" width="15.271527152715272%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_p16772617151317"><a name="zh-cn_topic_0118184396_p16772617151317"></a><a name="zh-cn_topic_0118184396_p16772617151317"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.10561056105611%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p13563123565513"><a name="zh-cn_topic_0118184396_p13563123565513"></a><a name="zh-cn_topic_0118184396_p13563123565513"></a><span id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text44323307153939_1"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text44323307153939_1"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text44323307153939_1"></a>节点</span>名称，可以包含中文、英文字母、数字、<span class="parmvalue" id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253_1"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253_1"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253_1"></a>“_”</span>、<span class="parmvalue" id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253_1"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253_1"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253_1"></a>“-”</span>、<span class="parmvalue" id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_parmvalue3773104413412_1"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_parmvalue3773104413412_1"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_parmvalue3773104413412_1"></a>“/”</span>、<span class="parmvalue" id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253_1"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253_1"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253_1"></a>“&lt;”</span>、<span class="parmvalue" id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253_1"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253_1"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253_1"></a>“&gt;”</span>等各类特殊字符，长度为1～128个字符。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row1777291741313"><td class="cellrowborder" colspan="3" valign="top" headers="mcps1.2.4.1.1 mcps1.2.4.1.2 mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p14772141731313"><a name="zh-cn_topic_0118184396_p14772141731313"></a><a name="zh-cn_topic_0118184396_p14772141731313"></a><strong id="zh-cn_topic_0118184396_b18600623155618"><a name="zh-cn_topic_0118184396_b18600623155618"></a><a name="zh-cn_topic_0118184396_b18600623155618"></a>Flink自定义作业</strong></p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row167722175133"><td class="cellrowborder" valign="top" width="28.622862286228624%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_p2772111711138"><a name="zh-cn_topic_0118184396_p2772111711138"></a><a name="zh-cn_topic_0118184396_p2772111711138"></a>jar包路径</p>
</td>
<td class="cellrowborder" valign="top" width="15.271527152715272%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_p16772171718130"><a name="zh-cn_topic_0118184396_p16772171718130"></a><a name="zh-cn_topic_0118184396_p16772171718130"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.10561056105611%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p10772917101315"><a name="zh-cn_topic_0118184396_p10772917101315"></a><a name="zh-cn_topic_0118184396_p10772917101315"></a>用户需先上传自定义的Jar包至OBS桶中，在此处才能选择对应Jar包的OBS路径。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row47721417171311"><td class="cellrowborder" valign="top" width="28.622862286228624%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_p3772141741314"><a name="zh-cn_topic_0118184396_p3772141741314"></a><a name="zh-cn_topic_0118184396_p3772141741314"></a>入口类</p>
</td>
<td class="cellrowborder" valign="top" width="15.271527152715272%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_p1477216174134"><a name="zh-cn_topic_0118184396_p1477216174134"></a><a name="zh-cn_topic_0118184396_p1477216174134"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="56.10561056105611%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p16772417101314"><a name="zh-cn_topic_0118184396_p16772417101314"></a><a name="zh-cn_topic_0118184396_p16772417101314"></a>指定加载的Jar包入口类名（如：KafkaMessageStreaming）。若不指定，则根据Jar包文件的Manifest文件确定。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row14772151731315"><td class="cellrowborder" valign="top" width="28.622862286228624%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_p167721173130"><a name="zh-cn_topic_0118184396_p167721173130"></a><a name="zh-cn_topic_0118184396_p167721173130"></a>入口参数</p>
</td>
<td class="cellrowborder" valign="top" width="15.271527152715272%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_p47726175136"><a name="zh-cn_topic_0118184396_p47726175136"></a><a name="zh-cn_topic_0118184396_p47726175136"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="56.10561056105611%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p1277291761319"><a name="zh-cn_topic_0118184396_p1277291761319"></a><a name="zh-cn_topic_0118184396_p1277291761319"></a>指定入口类的参数列表，参数之间使用空格分隔（如:test tmp/result.txt）。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row117722179138"><td class="cellrowborder" valign="top" width="28.622862286228624%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_p969162531111"><a name="zh-cn_topic_0118184396_p969162531111"></a><a name="zh-cn_topic_0118184396_p969162531111"></a>CloudStream集群</p>
</td>
<td class="cellrowborder" valign="top" width="15.271527152715272%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_p106911252113"><a name="zh-cn_topic_0118184396_p106911252113"></a><a name="zh-cn_topic_0118184396_p106911252113"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.10561056105611%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p56911257111"><a name="zh-cn_topic_0118184396_p56911257111"></a><a name="zh-cn_topic_0118184396_p56911257111"></a>选择CS集群。如需创建新的CS集群，请前往CS控制台操作。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row1113135101119"><td class="cellrowborder" valign="top" width="28.622862286228624%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_p166571342151416"><a name="zh-cn_topic_0118184396_p166571342151416"></a><a name="zh-cn_topic_0118184396_p166571342151416"></a>SPUs</p>
</td>
<td class="cellrowborder" valign="top" width="15.271527152715272%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_p1065714212149"><a name="zh-cn_topic_0118184396_p1065714212149"></a><a name="zh-cn_topic_0118184396_p1065714212149"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.10561056105611%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p265724214143"><a name="zh-cn_topic_0118184396_p265724214143"></a><a name="zh-cn_topic_0118184396_p265724214143"></a>选择流处理单元，1SPU=1核4G的资源配置。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row14942193114112"><td class="cellrowborder" valign="top" width="28.622862286228624%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_p1794273141111"><a name="zh-cn_topic_0118184396_p1794273141111"></a><a name="zh-cn_topic_0118184396_p1794273141111"></a>管理单元</p>
</td>
<td class="cellrowborder" valign="top" width="15.271527152715272%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_p99421831201113"><a name="zh-cn_topic_0118184396_p99421831201113"></a><a name="zh-cn_topic_0118184396_p99421831201113"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.10561056105611%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p39420310118"><a name="zh-cn_topic_0118184396_p39420310118"></a><a name="zh-cn_topic_0118184396_p39420310118"></a>设置Driver节点使用的SPU数量。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row101911293115"><td class="cellrowborder" valign="top" width="28.622862286228624%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_p2729651121713"><a name="zh-cn_topic_0118184396_p2729651121713"></a><a name="zh-cn_topic_0118184396_p2729651121713"></a>并行数</p>
</td>
<td class="cellrowborder" valign="top" width="15.271527152715272%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_p1372945116178"><a name="zh-cn_topic_0118184396_p1372945116178"></a><a name="zh-cn_topic_0118184396_p1372945116178"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.10561056105611%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p172905119178"><a name="zh-cn_topic_0118184396_p172905119178"></a><a name="zh-cn_topic_0118184396_p172905119178"></a>选择同时运行CS作业的任务数，建议设置为SPU的1~2倍。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row8153115491919"><td class="cellrowborder" valign="top" width="28.622862286228624%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_p18840217132015"><a name="zh-cn_topic_0118184396_p18840217132015"></a><a name="zh-cn_topic_0118184396_p18840217132015"></a>异常自动启动</p>
</td>
<td class="cellrowborder" valign="top" width="15.271527152715272%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_p1840617152012"><a name="zh-cn_topic_0118184396_p1840617152012"></a><a name="zh-cn_topic_0118184396_p1840617152012"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="56.10561056105611%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p8840141712206"><a name="zh-cn_topic_0118184396_p8840141712206"></a><a name="zh-cn_topic_0118184396_p8840141712206"></a>设置是否启动异常自动重启功能，当CS作业异常时自动重启并恢复CS作业。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row10671506243"><td class="cellrowborder" valign="top" width="28.622862286228624%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_p13897155102514"><a name="zh-cn_topic_0118184396_p13897155102514"></a><a name="zh-cn_topic_0118184396_p13897155102514"></a>实时流作业名称</p>
</td>
<td class="cellrowborder" valign="top" width="15.271527152715272%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_p19671150112415"><a name="zh-cn_topic_0118184396_p19671150112415"></a><a name="zh-cn_topic_0118184396_p19671150112415"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.10561056105611%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p489332115720"><a name="zh-cn_topic_0118184396_p489332115720"></a><a name="zh-cn_topic_0118184396_p489332115720"></a>Flink自定义作业名称，只能由字母、中文、数字、中划线和下划线组成，并且长度为1～57字节。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row8121950181913"><td class="cellrowborder" valign="top" width="28.622862286228624%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_p20840517192012"><a name="zh-cn_topic_0118184396_p20840517192012"></a><a name="zh-cn_topic_0118184396_p20840517192012"></a>节点名称</p>
</td>
<td class="cellrowborder" valign="top" width="15.271527152715272%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_p48571817182015"><a name="zh-cn_topic_0118184396_p48571817182015"></a><a name="zh-cn_topic_0118184396_p48571817182015"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.10561056105611%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p385791712206"><a name="zh-cn_topic_0118184396_p385791712206"></a><a name="zh-cn_topic_0118184396_p385791712206"></a><span id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text44323307153939_2"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text44323307153939_2"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text44323307153939_2"></a>节点</span>名称，可以包含中文、英文字母、数字、<span class="parmvalue" id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253_2"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253_2"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253_2"></a>“_”</span>、<span class="parmvalue" id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253_2"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253_2"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253_2"></a>“-”</span>、<span class="parmvalue" id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_parmvalue3773104413412_2"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_parmvalue3773104413412_2"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_parmvalue3773104413412_2"></a>“/”</span>、<span class="parmvalue" id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253_2"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253_2"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253_2"></a>“&lt;”</span>、<span class="parmvalue" id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253_2"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253_2"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253_2"></a>“&gt;”</span>等各类特殊字符，长度为1～128个字符。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row8371113714193"><td class="cellrowborder" colspan="3" valign="top" headers="mcps1.2.4.1.1 mcps1.2.4.1.2 mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p4371037161912"><a name="zh-cn_topic_0118184396_p4371037161912"></a><a name="zh-cn_topic_0118184396_p4371037161912"></a><strong id="zh-cn_topic_0118184396_b1927415715232"><a name="zh-cn_topic_0118184396_b1927415715232"></a><a name="zh-cn_topic_0118184396_b1927415715232"></a>Spark自定义作业</strong></p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row812164614194"><td class="cellrowborder" valign="top" width="28.622862286228624%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_p251951619243"><a name="zh-cn_topic_0118184396_p251951619243"></a><a name="zh-cn_topic_0118184396_p251951619243"></a>jar包路径</p>
</td>
<td class="cellrowborder" valign="top" width="15.271527152715272%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_p1951916161245"><a name="zh-cn_topic_0118184396_p1951916161245"></a><a name="zh-cn_topic_0118184396_p1951916161245"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.10561056105611%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p15535111622413"><a name="zh-cn_topic_0118184396_p15535111622413"></a><a name="zh-cn_topic_0118184396_p15535111622413"></a>用户需先上传自定义的Jar包至OBS桶中，在此处才能选择对应Jar包的OBS路径。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row7838194622313"><td class="cellrowborder" valign="top" width="28.622862286228624%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_p1344212352258"><a name="zh-cn_topic_0118184396_p1344212352258"></a><a name="zh-cn_topic_0118184396_p1344212352258"></a>入口类</p>
</td>
<td class="cellrowborder" valign="top" width="15.271527152715272%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_p1744212353251"><a name="zh-cn_topic_0118184396_p1744212353251"></a><a name="zh-cn_topic_0118184396_p1744212353251"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="56.10561056105611%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p14442735192513"><a name="zh-cn_topic_0118184396_p14442735192513"></a><a name="zh-cn_topic_0118184396_p14442735192513"></a>指定加载的Jar包入口类名（如：KafkaMessageStreaming）。若不指定，则根据Jar包文件的Manifest文件确定。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row11870130182312"><td class="cellrowborder" valign="top" width="28.622862286228624%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_p14421635122514"><a name="zh-cn_topic_0118184396_p14421635122514"></a><a name="zh-cn_topic_0118184396_p14421635122514"></a>入口参数</p>
</td>
<td class="cellrowborder" valign="top" width="15.271527152715272%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_p1544213552518"><a name="zh-cn_topic_0118184396_p1544213552518"></a><a name="zh-cn_topic_0118184396_p1544213552518"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="56.10561056105611%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p3458113522519"><a name="zh-cn_topic_0118184396_p3458113522519"></a><a name="zh-cn_topic_0118184396_p3458113522519"></a>指定入口类的参数列表，参数之间使用空格分隔（如:test tmp/result.txt）。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row194142819235"><td class="cellrowborder" valign="top" width="28.622862286228624%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_p1897650142820"><a name="zh-cn_topic_0118184396_p1897650142820"></a><a name="zh-cn_topic_0118184396_p1897650142820"></a>CloudStream集群</p>
</td>
<td class="cellrowborder" valign="top" width="15.271527152715272%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_p199761901281"><a name="zh-cn_topic_0118184396_p199761901281"></a><a name="zh-cn_topic_0118184396_p199761901281"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.10561056105611%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p1099219011281"><a name="zh-cn_topic_0118184396_p1099219011281"></a><a name="zh-cn_topic_0118184396_p1099219011281"></a>选择CS集群。如需创建新的CS集群，请前往CS控制台操作。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row86198255239"><td class="cellrowborder" valign="top" width="28.622862286228624%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_p5992508283"><a name="zh-cn_topic_0118184396_p5992508283"></a><a name="zh-cn_topic_0118184396_p5992508283"></a>SPUs</p>
</td>
<td class="cellrowborder" valign="top" width="15.271527152715272%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_p899219015284"><a name="zh-cn_topic_0118184396_p899219015284"></a><a name="zh-cn_topic_0118184396_p899219015284"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.10561056105611%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p7992808286"><a name="zh-cn_topic_0118184396_p7992808286"></a><a name="zh-cn_topic_0118184396_p7992808286"></a>选择流处理单元，1SPU=1核4G的资源配置。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row13635122116238"><td class="cellrowborder" valign="top" width="28.622862286228624%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_p881415284"><a name="zh-cn_topic_0118184396_p881415284"></a><a name="zh-cn_topic_0118184396_p881415284"></a>管理单元</p>
</td>
<td class="cellrowborder" valign="top" width="15.271527152715272%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_p8810116285"><a name="zh-cn_topic_0118184396_p8810116285"></a><a name="zh-cn_topic_0118184396_p8810116285"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.10561056105611%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p13818116287"><a name="zh-cn_topic_0118184396_p13818116287"></a><a name="zh-cn_topic_0118184396_p13818116287"></a>设置Driver节点使用的SPU数量。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row8823818172313"><td class="cellrowborder" valign="top" width="28.622862286228624%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_p8823141814234"><a name="zh-cn_topic_0118184396_p8823141814234"></a><a name="zh-cn_topic_0118184396_p8823141814234"></a>Executor个数</p>
</td>
<td class="cellrowborder" valign="top" width="15.271527152715272%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_p582316182236"><a name="zh-cn_topic_0118184396_p582316182236"></a><a name="zh-cn_topic_0118184396_p582316182236"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.10561056105611%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p382341815231"><a name="zh-cn_topic_0118184396_p382341815231"></a><a name="zh-cn_topic_0118184396_p382341815231"></a>设置Executor节点的数量。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row19119216132310"><td class="cellrowborder" valign="top" width="28.622862286228624%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_p1611915169233"><a name="zh-cn_topic_0118184396_p1611915169233"></a><a name="zh-cn_topic_0118184396_p1611915169233"></a>Executor SPUs</p>
</td>
<td class="cellrowborder" valign="top" width="15.271527152715272%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_p2011931612236"><a name="zh-cn_topic_0118184396_p2011931612236"></a><a name="zh-cn_topic_0118184396_p2011931612236"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.10561056105611%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p711911161231"><a name="zh-cn_topic_0118184396_p711911161231"></a><a name="zh-cn_topic_0118184396_p711911161231"></a>设置每个Executor节点使用的SPU数量。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row8400179162320"><td class="cellrowborder" valign="top" width="28.622862286228624%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_p1789192073418"><a name="zh-cn_topic_0118184396_p1789192073418"></a><a name="zh-cn_topic_0118184396_p1789192073418"></a>异常自动启动</p>
</td>
<td class="cellrowborder" valign="top" width="15.271527152715272%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_p117899200349"><a name="zh-cn_topic_0118184396_p117899200349"></a><a name="zh-cn_topic_0118184396_p117899200349"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="56.10561056105611%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p1178972073418"><a name="zh-cn_topic_0118184396_p1178972073418"></a><a name="zh-cn_topic_0118184396_p1178972073418"></a>设置是否启动异常自动重启功能，当CS作业异常时自动重启并恢复CS作业。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row1445922112712"><td class="cellrowborder" valign="top" width="28.622862286228624%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_p4445142216279"><a name="zh-cn_topic_0118184396_p4445142216279"></a><a name="zh-cn_topic_0118184396_p4445142216279"></a>实时流作业名称</p>
</td>
<td class="cellrowborder" valign="top" width="15.271527152715272%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_p444582217271"><a name="zh-cn_topic_0118184396_p444582217271"></a><a name="zh-cn_topic_0118184396_p444582217271"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.10561056105611%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p8673101015589"><a name="zh-cn_topic_0118184396_p8673101015589"></a><a name="zh-cn_topic_0118184396_p8673101015589"></a>Spark自定义作业名称，只能由字母、中文、数字、中划线和下划线组成，并且长度为1～57字节。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_row1482119108238"><td class="cellrowborder" valign="top" width="28.622862286228624%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_p2804122016347"><a name="zh-cn_topic_0118184396_p2804122016347"></a><a name="zh-cn_topic_0118184396_p2804122016347"></a>节点名称</p>
</td>
<td class="cellrowborder" valign="top" width="15.271527152715272%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_p1980462033410"><a name="zh-cn_topic_0118184396_p1980462033410"></a><a name="zh-cn_topic_0118184396_p1980462033410"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.10561056105611%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_p1380418204341"><a name="zh-cn_topic_0118184396_p1380418204341"></a><a name="zh-cn_topic_0118184396_p1380418204341"></a><span id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text44323307153939_3"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text44323307153939_3"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text44323307153939_3"></a>节点</span>名称，可以包含中文、英文字母、数字、<span class="parmvalue" id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253_3"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253_3"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253_3"></a>“_”</span>、<span class="parmvalue" id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253_3"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253_3"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253_3"></a>“-”</span>、<span class="parmvalue" id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_parmvalue3773104413412_3"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_parmvalue3773104413412_3"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_parmvalue3773104413412_3"></a>“/”</span>、<span class="parmvalue" id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253_3"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253_3"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253_3"></a>“&lt;”</span>、<span class="parmvalue" id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253_3"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253_3"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253_3"></a>“&gt;”</span>等各类特殊字符，长度为1～128个字符。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  高级参数

<a name="zh-cn_topic_0118184396_table58040457102411"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_row27216578102411"><th class="cellrowborder" valign="top" width="28.07%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p57059205102411"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p57059205102411"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p57059205102411"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="15.659999999999998%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p58392901102411"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p58392901102411"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p58392901102411"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="56.269999999999996%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p32204521102411"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p32204521102411"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p32204521102411"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_row51612113175"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p416115112178"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p416115112178"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p416115112178"></a>节点状态轮询时间（秒）</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p101615110176"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p101615110176"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p101615110176"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p4161191101716"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p4161191101716"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p4161191101716"></a>设置轮询时间（1~60秒），每隔x秒查询一次<span id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text1526241235118"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text1526241235118"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text1526241235118"></a>节点</span>是否执行完成。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_row5101045193916"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p147314419397"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p147314419397"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p147314419397"></a>节点执行的最长时间</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p610124511390"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p610124511390"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p610124511390"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p11011456393"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p11011456393"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p11011456393"></a>设置<span id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text380131541112"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text380131541112"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text380131541112"></a>节点</span>执行的超时时间，如果<span id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text1944213322118"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text1944213322118"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text1944213322118"></a>节点</span>配置了重试，在超时时间内未执行完成，该节点将不会再重试，直接置为失败状态。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_row58429402102411"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p5533912102858"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p5533912102858"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p5533912102858"></a>失败重试</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p45593742102858"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p45593742102858"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p45593742102858"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p2105628102858"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p2105628102858"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p2105628102858"></a><span id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text29185571161243"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text29185571161243"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text29185571161243"></a>节点</span>执行失败后，是否重新执行<span id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text58583828161245"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text58583828161245"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text58583828161245"></a>节点</span>。</p>
<a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_ul18950660102858"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_ul18950660102858"></a><ul id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_ul18950660102858"><li>是：重新执行<span id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text19139245161248"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text19139245161248"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text19139245161248"></a>节点</span>，请配置以下参数。<a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_ul58608523102858"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_ul58608523102858"></a><ul id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_ul58608523102858"><li>最大重试次数</li><li>重试间隔时间（秒）</li></ul>
</li><li>否：默认值，不重新执行<span id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text1328324161254"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text1328324161254"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text1328324161254"></a>节点</span>。</li></ul>
<div class="note" id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_note69071033105815"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_note69071033105815"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_note69071033105815"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p1590733314581"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p1590733314581"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p1590733314581"></a>如果作业节点配置了重试，并且配置了超时时间，该节点执行超时后将不会再重试，直接置为失败状态。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_row29541959102411"><td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p13154928102858"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p13154928102858"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p13154928102858"></a>失败策略</p>
</td>
<td class="cellrowborder" valign="top" width="15.659999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p58916261102858"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p58916261102858"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p58916261102858"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.269999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p7487822102858"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p7487822102858"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_p7487822102858"></a><span id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text5371194616130"><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text5371194616130"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_text5371194616130"></a>节点</span>执行失败后的操作：</p>
<a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_ul281538102858"></a><a name="zh-cn_topic_0118184396_zh-cn_topic_0099822521_ul281538102858"></a><ul id="zh-cn_topic_0118184396_zh-cn_topic_0099822521_ul281538102858"><li>终止当前作业执行计划</li><li>继续执行下一作业</li><li>挂起当前作业执行计划</li></ul>
</td>
</tr>
</tbody>
</table>

