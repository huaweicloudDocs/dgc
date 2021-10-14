# DLI Flink  Job<a name="dgc_01_0536"></a>

## 功能<a name="zh-cn_topic_0226206976_section17228524131210"></a>

通过DLI Flink Job节点执行一个预先定义的DLI作业，实现实时流式大数据分析。

## 原理<a name="zh-cn_topic_0226206976_section07401729201213"></a>

该节点方便用户启动或者查询DLI作业是否正在运行。当作业类型不是“选择已存在的Flink作业”时，系统会根据在节点中配置的作业情况，进行创建和启动作业。方便用户自定义作业以及作业参数。

## 参数<a name="zh-cn_topic_0226206976_section8827835191215"></a>

DLI Flink Job的参数配置，请参考以下内容：

-   属性参数：
    -   **选择已存在的Flink作业**：请参见[表1](#zh-cn_topic_0226206976_table647011333413)。
    -   **Flink SQL作业**：请参见[表2](#zh-cn_topic_0226206976_table0855143818117)。
    -   **Flink自定义作业**：请参见[表3](#zh-cn_topic_0226206976_table3764823994826)。

-   [表4](#zh-cn_topic_0226206976_table58040457102411)

**表 1**  已存在的Flink作业-属性参数

<a name="zh-cn_topic_0226206976_table647011333413"></a>
<table><thead align="left"><tr id="zh-cn_topic_0226206976_row34705331412"><th class="cellrowborder" valign="top" width="24.88%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0226206976_p54708331840"><a name="zh-cn_topic_0226206976_p54708331840"></a><a name="zh-cn_topic_0226206976_p54708331840"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="10.38%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0226206976_p747011337414"><a name="zh-cn_topic_0226206976_p747011337414"></a><a name="zh-cn_topic_0226206976_p747011337414"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="64.74%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0226206976_p14470203313410"><a name="zh-cn_topic_0226206976_p14470203313410"></a><a name="zh-cn_topic_0226206976_p14470203313410"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0226206976_row647013331646"><td class="cellrowborder" valign="top" width="24.88%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226206976_p2047013331042"><a name="zh-cn_topic_0226206976_p2047013331042"></a><a name="zh-cn_topic_0226206976_p2047013331042"></a>作业类型</p>
</td>
<td class="cellrowborder" valign="top" width="10.38%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226206976_p1470103313411"><a name="zh-cn_topic_0226206976_p1470103313411"></a><a name="zh-cn_topic_0226206976_p1470103313411"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="64.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226206976_p1547011332412"><a name="zh-cn_topic_0226206976_p1547011332412"></a><a name="zh-cn_topic_0226206976_p1547011332412"></a>选择<span class="parmname" id="zh-cn_topic_0226206976_parmname15213548917"><a name="zh-cn_topic_0226206976_parmname15213548917"></a><a name="zh-cn_topic_0226206976_parmname15213548917"></a>“选择已存在的Flink作业”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0226206976_row2470163315410"><td class="cellrowborder" valign="top" width="24.88%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226206976_p104702331748"><a name="zh-cn_topic_0226206976_p104702331748"></a><a name="zh-cn_topic_0226206976_p104702331748"></a>作业名称</p>
</td>
<td class="cellrowborder" valign="top" width="10.38%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226206976_p64706331749"><a name="zh-cn_topic_0226206976_p64706331749"></a><a name="zh-cn_topic_0226206976_p64706331749"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="64.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226206976_p8470183320416"><a name="zh-cn_topic_0226206976_p8470183320416"></a><a name="zh-cn_topic_0226206976_p8470183320416"></a>选择一个已存在的DLI Flink作业。</p>
</td>
</tr>
<tr id="zh-cn_topic_0226206976_row14706331041"><td class="cellrowborder" valign="top" width="24.88%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226206976_p1470103314418"><a name="zh-cn_topic_0226206976_p1470103314418"></a><a name="zh-cn_topic_0226206976_p1470103314418"></a>节点名称</p>
</td>
<td class="cellrowborder" valign="top" width="10.38%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226206976_p1647020331146"><a name="zh-cn_topic_0226206976_p1647020331146"></a><a name="zh-cn_topic_0226206976_p1647020331146"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="64.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226206976_p1346974112913"><a name="zh-cn_topic_0226206976_p1346974112913"></a><a name="zh-cn_topic_0226206976_p1346974112913"></a><span id="zh-cn_topic_0099822521_text44323307153939"><a name="zh-cn_topic_0099822521_text44323307153939"></a><a name="zh-cn_topic_0099822521_text44323307153939"></a>节点</span>名称，可以包含中文、英文字母、数字、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253"></a>“_”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253"></a>“-”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_parmvalue3773104413412"><a name="zh-cn_topic_0099822521_parmvalue3773104413412"></a><a name="zh-cn_topic_0099822521_parmvalue3773104413412"></a>“/”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253"></a>“&lt;”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253"></a>“&gt;”</span>等各类特殊字符，长度为1～128个字符。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  Flink SQL作业-属性参数

<a name="zh-cn_topic_0226206976_table0855143818117"></a>
<table><thead align="left"><tr id="zh-cn_topic_0226206976_row1285573816118"><th class="cellrowborder" valign="top" width="24.88%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0226206976_p585514385111"><a name="zh-cn_topic_0226206976_p585514385111"></a><a name="zh-cn_topic_0226206976_p585514385111"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="10.38%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0226206976_p15855123811112"><a name="zh-cn_topic_0226206976_p15855123811112"></a><a name="zh-cn_topic_0226206976_p15855123811112"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="64.74%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0226206976_p98551538161114"><a name="zh-cn_topic_0226206976_p98551538161114"></a><a name="zh-cn_topic_0226206976_p98551538161114"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0226206976_row785533818110"><td class="cellrowborder" valign="top" width="24.88%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226206976_p8855238191118"><a name="zh-cn_topic_0226206976_p8855238191118"></a><a name="zh-cn_topic_0226206976_p8855238191118"></a>作业类型</p>
</td>
<td class="cellrowborder" valign="top" width="10.38%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226206976_p9856153813116"><a name="zh-cn_topic_0226206976_p9856153813116"></a><a name="zh-cn_topic_0226206976_p9856153813116"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="64.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226206976_p12856038181115"><a name="zh-cn_topic_0226206976_p12856038181115"></a><a name="zh-cn_topic_0226206976_p12856038181115"></a>选择<span class="parmvalue" id="zh-cn_topic_0226206976_parmvalue12519312101517"><a name="zh-cn_topic_0226206976_parmvalue12519312101517"></a><a name="zh-cn_topic_0226206976_parmvalue12519312101517"></a>“Flink SQL作业”</span>。用户采用编写SQL语句来启动作业。</p>
</td>
</tr>
<tr id="zh-cn_topic_0226206976_row138569387115"><td class="cellrowborder" valign="top" width="24.88%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226206976_p1485663820111"><a name="zh-cn_topic_0226206976_p1485663820111"></a><a name="zh-cn_topic_0226206976_p1485663820111"></a>脚本路径</p>
</td>
<td class="cellrowborder" valign="top" width="10.38%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226206976_p385614384119"><a name="zh-cn_topic_0226206976_p385614384119"></a><a name="zh-cn_topic_0226206976_p385614384119"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="64.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226206976_p14856838191110"><a name="zh-cn_topic_0226206976_p14856838191110"></a><a name="zh-cn_topic_0226206976_p14856838191110"></a>选择需要执行的Flink SQL脚本。如果脚本未创建，请参考<a href="新建脚本.md">新建脚本</a>和<a href="开发SQL脚本.md">开发SQL脚本</a>创建和开发Flink SQL脚本。</p>
</td>
</tr>
<tr id="zh-cn_topic_0226206976_row208561238101119"><td class="cellrowborder" valign="top" width="24.88%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226206976_p1485623811118"><a name="zh-cn_topic_0226206976_p1485623811118"></a><a name="zh-cn_topic_0226206976_p1485623811118"></a>DLI队列</p>
</td>
<td class="cellrowborder" valign="top" width="10.38%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226206976_p1985619384115"><a name="zh-cn_topic_0226206976_p1985619384115"></a><a name="zh-cn_topic_0226206976_p1985619384115"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="64.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226206976_p985653861114"><a name="zh-cn_topic_0226206976_p985653861114"></a><a name="zh-cn_topic_0226206976_p985653861114"></a>默认选择“共享队列”，用户也可以选择自定义的独享队列。</p>
<div class="note" id="zh-cn_topic_0226206976_note118562038181115"><a name="zh-cn_topic_0226206976_note118562038181115"></a><a name="zh-cn_topic_0226206976_note118562038181115"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0226206976_p12856153891111"><a name="zh-cn_topic_0226206976_p12856153891111"></a><a name="zh-cn_topic_0226206976_p12856153891111"></a>当子用户在创建作业时，子用户只能选择已经被分配的队列。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0226206976_row168561538161113"><td class="cellrowborder" valign="top" width="24.88%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226206976_p1985620380113"><a name="zh-cn_topic_0226206976_p1985620380113"></a><a name="zh-cn_topic_0226206976_p1985620380113"></a>CUs</p>
</td>
<td class="cellrowborder" valign="top" width="10.38%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226206976_p88561238141120"><a name="zh-cn_topic_0226206976_p88561238141120"></a><a name="zh-cn_topic_0226206976_p88561238141120"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="64.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226206976_p285633861114"><a name="zh-cn_topic_0226206976_p285633861114"></a><a name="zh-cn_topic_0226206976_p285633861114"></a>CUs为DLI计费单位，一个CU是1核4G的资源配置。</p>
</td>
</tr>
<tr id="zh-cn_topic_0226206976_row1585663821120"><td class="cellrowborder" valign="top" width="24.88%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226206976_p1485614380111"><a name="zh-cn_topic_0226206976_p1485614380111"></a><a name="zh-cn_topic_0226206976_p1485614380111"></a>并发数</p>
</td>
<td class="cellrowborder" valign="top" width="10.38%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226206976_p2085673819119"><a name="zh-cn_topic_0226206976_p2085673819119"></a><a name="zh-cn_topic_0226206976_p2085673819119"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="64.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226206976_p8856123851118"><a name="zh-cn_topic_0226206976_p8856123851118"></a><a name="zh-cn_topic_0226206976_p8856123851118"></a>并发数是指同时运行Flink SQL作业的任务数。</p>
<div class="note" id="zh-cn_topic_0226206976_note6856183851120"><a name="zh-cn_topic_0226206976_note6856183851120"></a><a name="zh-cn_topic_0226206976_note6856183851120"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0226206976_p108561338151110"><a name="zh-cn_topic_0226206976_p108561338151110"></a><a name="zh-cn_topic_0226206976_p108561338151110"></a>并发数不能大于计算单元（CUs-1）的4倍。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0226206976_row1856173851110"><td class="cellrowborder" valign="top" width="24.88%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226206976_p108561038201118"><a name="zh-cn_topic_0226206976_p108561038201118"></a><a name="zh-cn_topic_0226206976_p108561038201118"></a>UDF Jar</p>
</td>
<td class="cellrowborder" valign="top" width="10.38%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226206976_p685643810118"><a name="zh-cn_topic_0226206976_p685643810118"></a><a name="zh-cn_topic_0226206976_p685643810118"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="64.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226206976_p98561638141118"><a name="zh-cn_topic_0226206976_p98561638141118"></a><a name="zh-cn_topic_0226206976_p98561638141118"></a>当作业所属集群选择独享集群时，该参数有效。在选择UDF Jar之前，您需要将UDF Jar包上传至OBS桶中，并在<span class="wintitle" id="zh-cn_topic_0226206976_wintitle17856163815117"><a name="zh-cn_topic_0226206976_wintitle17856163815117"></a><a name="zh-cn_topic_0226206976_wintitle17856163815117"></a>“资源管理”</span>页面中新建资源，具体操作请参考<a href="管理资源.md#zh-cn_topic_0165312432_section6325757145320">新建资源</a>。</p>
<p id="zh-cn_topic_0226206976_p0856133818115"><a name="zh-cn_topic_0226206976_p0856133818115"></a><a name="zh-cn_topic_0226206976_p0856133818115"></a>用户可以在SQL中调用插入Jar包中的自定义函数。</p>
</td>
</tr>
<tr id="zh-cn_topic_0226206976_row1385613816115"><td class="cellrowborder" valign="top" width="24.88%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226206976_p9856103851112"><a name="zh-cn_topic_0226206976_p9856103851112"></a><a name="zh-cn_topic_0226206976_p9856103851112"></a>异常自动启动</p>
</td>
<td class="cellrowborder" valign="top" width="10.38%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226206976_p3856123816114"><a name="zh-cn_topic_0226206976_p3856123816114"></a><a name="zh-cn_topic_0226206976_p3856123816114"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="64.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226206976_p685633861114"><a name="zh-cn_topic_0226206976_p685633861114"></a><a name="zh-cn_topic_0226206976_p685633861114"></a>设置是否启动异常自动重启功能，当作业异常时将自动重启并恢复作业。</p>
</td>
</tr>
<tr id="zh-cn_topic_0226206976_row154385524168"><td class="cellrowborder" valign="top" width="24.88%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226206976_p159901126171910"><a name="zh-cn_topic_0226206976_p159901126171910"></a><a name="zh-cn_topic_0226206976_p159901126171910"></a>作业名称</p>
</td>
<td class="cellrowborder" valign="top" width="10.38%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226206976_p14990112618193"><a name="zh-cn_topic_0226206976_p14990112618193"></a><a name="zh-cn_topic_0226206976_p14990112618193"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="64.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226206976_p1157571072712"><a name="zh-cn_topic_0226206976_p1157571072712"></a><a name="zh-cn_topic_0226206976_p1157571072712"></a>填写<span id="zh-cn_topic_0226206976_text857517101274"><a name="zh-cn_topic_0226206976_text857517101274"></a><a name="zh-cn_topic_0226206976_text857517101274"></a>DLI</span> Flink作业的名称，只能包含英文字母、数字、<span class="parmvalue" id="zh-cn_topic_0226206976_parmvalue17575181018278"><a name="zh-cn_topic_0226206976_parmvalue17575181018278"></a><a name="zh-cn_topic_0226206976_parmvalue17575181018278"></a>“_”</span>，且长度为1~64个字符。默认与节点的名称一致。</p>
</td>
</tr>
<tr id="zh-cn_topic_0226206976_row155021755131619"><td class="cellrowborder" valign="top" width="24.88%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226206976_p1110013509178"><a name="zh-cn_topic_0226206976_p1110013509178"></a><a name="zh-cn_topic_0226206976_p1110013509178"></a>作业名称添加工作空间前缀</p>
</td>
<td class="cellrowborder" valign="top" width="10.38%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226206976_p18100050171711"><a name="zh-cn_topic_0226206976_p18100050171711"></a><a name="zh-cn_topic_0226206976_p18100050171711"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="64.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226206976_p11100185015175"><a name="zh-cn_topic_0226206976_p11100185015175"></a><a name="zh-cn_topic_0226206976_p11100185015175"></a>设置是否为创建的作业名称添加工作空间前缀。</p>
</td>
</tr>
<tr id="zh-cn_topic_0226206976_row4654115816163"><td class="cellrowborder" valign="top" width="24.88%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226206976_p1588029191712"><a name="zh-cn_topic_0226206976_p1588029191712"></a><a name="zh-cn_topic_0226206976_p1588029191712"></a>节点名称</p>
</td>
<td class="cellrowborder" valign="top" width="10.38%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226206976_p588017919171"><a name="zh-cn_topic_0226206976_p588017919171"></a><a name="zh-cn_topic_0226206976_p588017919171"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="64.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226206976_p1808831182913"><a name="zh-cn_topic_0226206976_p1808831182913"></a><a name="zh-cn_topic_0226206976_p1808831182913"></a><span id="zh-cn_topic_0099822521_text44323307153939_1"><a name="zh-cn_topic_0099822521_text44323307153939_1"></a><a name="zh-cn_topic_0099822521_text44323307153939_1"></a>节点</span>名称，可以包含中文、英文字母、数字、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253_1"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253_1"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253_1"></a>“_”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253_1"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253_1"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253_1"></a>“-”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_parmvalue3773104413412_1"><a name="zh-cn_topic_0099822521_parmvalue3773104413412_1"></a><a name="zh-cn_topic_0099822521_parmvalue3773104413412_1"></a>“/”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253_1"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253_1"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253_1"></a>“&lt;”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253_1"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253_1"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253_1"></a>“&gt;”</span>等各类特殊字符，长度为1～128个字符。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  Flink自定义作业-属性参数

<a name="zh-cn_topic_0226206976_table3764823994826"></a>
<table><thead align="left"><tr id="zh-cn_topic_0226206976_row3170822394826"><th class="cellrowborder" valign="top" width="24.88%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0226206976_p2984581994826"><a name="zh-cn_topic_0226206976_p2984581994826"></a><a name="zh-cn_topic_0226206976_p2984581994826"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="10.38%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0226206976_p159227094826"><a name="zh-cn_topic_0226206976_p159227094826"></a><a name="zh-cn_topic_0226206976_p159227094826"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="64.74%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0226206976_p6186505494826"><a name="zh-cn_topic_0226206976_p6186505494826"></a><a name="zh-cn_topic_0226206976_p6186505494826"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0226206976_row1991457694826"><td class="cellrowborder" valign="top" width="24.88%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226206976_p246794194826"><a name="zh-cn_topic_0226206976_p246794194826"></a><a name="zh-cn_topic_0226206976_p246794194826"></a>作业类型</p>
</td>
<td class="cellrowborder" valign="top" width="10.38%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226206976_p6568554794826"><a name="zh-cn_topic_0226206976_p6568554794826"></a><a name="zh-cn_topic_0226206976_p6568554794826"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="64.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226206976_p1988554433211"><a name="zh-cn_topic_0226206976_p1988554433211"></a><a name="zh-cn_topic_0226206976_p1988554433211"></a>选择<span class="parmvalue" id="zh-cn_topic_0226206976_parmvalue1979515194325"><a name="zh-cn_topic_0226206976_parmvalue1979515194325"></a><a name="zh-cn_topic_0226206976_parmvalue1979515194325"></a>“Flink自定义作业”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0226206976_row2373117113320"><td class="cellrowborder" valign="top" width="24.88%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226206976_p593755817332"><a name="zh-cn_topic_0226206976_p593755817332"></a><a name="zh-cn_topic_0226206976_p593755817332"></a>jar包路径</p>
</td>
<td class="cellrowborder" valign="top" width="10.38%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226206976_p109375581337"><a name="zh-cn_topic_0226206976_p109375581337"></a><a name="zh-cn_topic_0226206976_p109375581337"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="64.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226206976_p8937165814338"><a name="zh-cn_topic_0226206976_p8937165814338"></a><a name="zh-cn_topic_0226206976_p8937165814338"></a>用户自定义的程序包。在选择程序包之前，您需要将对应的jar包上传至OBS桶中，并在<span class="wintitle" id="zh-cn_topic_0226206976_wintitle587551417421"><a name="zh-cn_topic_0226206976_wintitle587551417421"></a><a name="zh-cn_topic_0226206976_wintitle587551417421"></a>“资源管理”</span>页面中新建资源，具体操作请参考<a href="管理资源.md#zh-cn_topic_0165312432_section6325757145320">新建资源</a>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0226206976_row5411245337"><td class="cellrowborder" valign="top" width="24.88%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226206976_p16937158143319"><a name="zh-cn_topic_0226206976_p16937158143319"></a><a name="zh-cn_topic_0226206976_p16937158143319"></a>入口类</p>
</td>
<td class="cellrowborder" valign="top" width="10.38%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226206976_p793765819334"><a name="zh-cn_topic_0226206976_p793765819334"></a><a name="zh-cn_topic_0226206976_p793765819334"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="64.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226206976_p993765813333"><a name="zh-cn_topic_0226206976_p993765813333"></a><a name="zh-cn_topic_0226206976_p993765813333"></a>指定加载的Jar包类名，如KafkaMessageStreaming。</p>
<a name="zh-cn_topic_0226206976_ul1893715813338"></a><a name="zh-cn_topic_0226206976_ul1893715813338"></a><ul id="zh-cn_topic_0226206976_ul1893715813338"><li>默认：根据Jar包文件的Manifest文件指定。</li><li>指定：需要输入类名并确定类参数列表（参数间用空格分隔）。<div class="note" id="zh-cn_topic_0226206976_note4937258203311"><a name="zh-cn_topic_0226206976_note4937258203311"></a><a name="zh-cn_topic_0226206976_note4937258203311"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0226206976_p10937105843313"><a name="zh-cn_topic_0226206976_p10937105843313"></a><a name="zh-cn_topic_0226206976_p10937105843313"></a>当类属于某个包时，需携带包路径，例如：packagePath.KafkaMessageStreaming。</p>
</div></div>
</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0226206976_row20703270338"><td class="cellrowborder" valign="top" width="24.88%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226206976_p14937155815334"><a name="zh-cn_topic_0226206976_p14937155815334"></a><a name="zh-cn_topic_0226206976_p14937155815334"></a>入口参数</p>
</td>
<td class="cellrowborder" valign="top" width="10.38%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226206976_p8937155863320"><a name="zh-cn_topic_0226206976_p8937155863320"></a><a name="zh-cn_topic_0226206976_p8937155863320"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="64.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226206976_p199371958183315"><a name="zh-cn_topic_0226206976_p199371958183315"></a><a name="zh-cn_topic_0226206976_p199371958183315"></a>指定类的参数列表，参数之间使用空格分隔。</p>
</td>
</tr>
<tr id="zh-cn_topic_0226206976_row122771015182816"><td class="cellrowborder" valign="top" width="24.88%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226206976_p627781582811"><a name="zh-cn_topic_0226206976_p627781582811"></a><a name="zh-cn_topic_0226206976_p627781582811"></a>DLI队列</p>
</td>
<td class="cellrowborder" valign="top" width="10.38%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226206976_p15277121514282"><a name="zh-cn_topic_0226206976_p15277121514282"></a><a name="zh-cn_topic_0226206976_p15277121514282"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="64.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226206976_p1729691164515"><a name="zh-cn_topic_0226206976_p1729691164515"></a><a name="zh-cn_topic_0226206976_p1729691164515"></a>默认选择“共享队列”，用户也可以选择自定义的独享队列。</p>
<div class="note" id="zh-cn_topic_0226206976_note3382019194514"><a name="zh-cn_topic_0226206976_note3382019194514"></a><a name="zh-cn_topic_0226206976_note3382019194514"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0226206976_p638331911452"><a name="zh-cn_topic_0226206976_p638331911452"></a><a name="zh-cn_topic_0226206976_p638331911452"></a>当子用户在创建作业时，子用户只能选择已经被分配的队列。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0226206976_row10221856183111"><td class="cellrowborder" valign="top" width="24.88%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226206976_p122213564314"><a name="zh-cn_topic_0226206976_p122213564314"></a><a name="zh-cn_topic_0226206976_p122213564314"></a>作业特性</p>
</td>
<td class="cellrowborder" valign="top" width="10.38%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226206976_p202214564316"><a name="zh-cn_topic_0226206976_p202214564316"></a><a name="zh-cn_topic_0226206976_p202214564316"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="64.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226206976_p152211856163116"><a name="zh-cn_topic_0226206976_p152211856163116"></a><a name="zh-cn_topic_0226206976_p152211856163116"></a>选择自定义镜像和对应版本。仅当DLI队列为容器化队列类型时，出现本参数。</p>
<p id="zh-cn_topic_0226206976_p338903163413"><a name="zh-cn_topic_0226206976_p338903163413"></a><a name="zh-cn_topic_0226206976_p338903163413"></a>自定义镜像是DLI的特性。用户可以依赖DLI提供的Spark或者Flink基础镜像，使用Dockerfile将作业运行需要的依赖（文件、jar包或者软件）打包到镜像中，生成自己的自定义镜像，然后将镜像发布到SWR（容器镜像服务）中，最后在此选择自己生成的镜像，运行作业。</p>
<p id="zh-cn_topic_0226206976_p5526915183410"><a name="zh-cn_topic_0226206976_p5526915183410"></a><a name="zh-cn_topic_0226206976_p5526915183410"></a>自定义镜像可以改变Spark作业和Flink作业的容器运行环境。用户可以将一些私有能力内置到自定义镜像中，从而增强作业的功能、性能。关于自定义镜像的更多详情，请参见<a href="https://support.huaweicloud.com/usermanual-dli/dli_01_0494.html" target="_blank" rel="noopener noreferrer">自定义镜像</a>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0226206976_row13747161216288"><td class="cellrowborder" valign="top" width="24.88%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226206976_p1074731217283"><a name="zh-cn_topic_0226206976_p1074731217283"></a><a name="zh-cn_topic_0226206976_p1074731217283"></a>CUs</p>
</td>
<td class="cellrowborder" valign="top" width="10.38%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226206976_p197471312182818"><a name="zh-cn_topic_0226206976_p197471312182818"></a><a name="zh-cn_topic_0226206976_p197471312182818"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="64.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226206976_p1747212112818"><a name="zh-cn_topic_0226206976_p1747212112818"></a><a name="zh-cn_topic_0226206976_p1747212112818"></a>CUs为DLI计费单位，一个CU是1核4G的资源配置。</p>
</td>
</tr>
<tr id="zh-cn_topic_0226206976_row187071737183412"><td class="cellrowborder" valign="top" width="24.88%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226206976_p4706858183419"><a name="zh-cn_topic_0226206976_p4706858183419"></a><a name="zh-cn_topic_0226206976_p4706858183419"></a>管理节点CU数量</p>
</td>
<td class="cellrowborder" valign="top" width="10.38%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226206976_p97064588342"><a name="zh-cn_topic_0226206976_p97064588342"></a><a name="zh-cn_topic_0226206976_p97064588342"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="64.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226206976_p10706658143418"><a name="zh-cn_topic_0226206976_p10706658143418"></a><a name="zh-cn_topic_0226206976_p10706658143418"></a>设置管理单元的CU数，支持设置1~4个CU数，默认值为1个CU。</p>
</td>
</tr>
<tr id="zh-cn_topic_0226206976_row188432916286"><td class="cellrowborder" valign="top" width="24.88%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226206976_p38431592282"><a name="zh-cn_topic_0226206976_p38431592282"></a><a name="zh-cn_topic_0226206976_p38431592282"></a>并发数</p>
</td>
<td class="cellrowborder" valign="top" width="10.38%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226206976_p1884311917284"><a name="zh-cn_topic_0226206976_p1884311917284"></a><a name="zh-cn_topic_0226206976_p1884311917284"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="64.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226206976_p664419442043"><a name="zh-cn_topic_0226206976_p664419442043"></a><a name="zh-cn_topic_0226206976_p664419442043"></a>并发数是指同时运行Flink SQL作业的任务数。</p>
<div class="note" id="zh-cn_topic_0226206976_note2065315501645"><a name="zh-cn_topic_0226206976_note2065315501645"></a><a name="zh-cn_topic_0226206976_note2065315501645"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0226206976_p865312501840"><a name="zh-cn_topic_0226206976_p865312501840"></a><a name="zh-cn_topic_0226206976_p865312501840"></a>并发数不能大于计算单元（CUs-1）的4倍。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0226206976_row18491104011299"><td class="cellrowborder" valign="top" width="24.88%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226206976_p10492154082916"><a name="zh-cn_topic_0226206976_p10492154082916"></a><a name="zh-cn_topic_0226206976_p10492154082916"></a>异常自动启动</p>
</td>
<td class="cellrowborder" valign="top" width="10.38%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226206976_p1949234002916"><a name="zh-cn_topic_0226206976_p1949234002916"></a><a name="zh-cn_topic_0226206976_p1949234002916"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="64.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226206976_p949215408296"><a name="zh-cn_topic_0226206976_p949215408296"></a><a name="zh-cn_topic_0226206976_p949215408296"></a>设置是否启动异常自动重启功能，当作业异常时将自动重启并恢复作业。</p>
</td>
</tr>
<tr id="zh-cn_topic_0226206976_row189085613317"><td class="cellrowborder" valign="top" width="24.88%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226206976_p361764933110"><a name="zh-cn_topic_0226206976_p361764933110"></a><a name="zh-cn_topic_0226206976_p361764933110"></a>作业名称</p>
</td>
<td class="cellrowborder" valign="top" width="10.38%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226206976_p5617949163116"><a name="zh-cn_topic_0226206976_p5617949163116"></a><a name="zh-cn_topic_0226206976_p5617949163116"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="64.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226206976_p36171949103118"><a name="zh-cn_topic_0226206976_p36171949103118"></a><a name="zh-cn_topic_0226206976_p36171949103118"></a>填写<span id="zh-cn_topic_0226206976_text13617124943111"><a name="zh-cn_topic_0226206976_text13617124943111"></a><a name="zh-cn_topic_0226206976_text13617124943111"></a>DLI</span> Flink作业的名称，只能包含英文字母、数字、<span class="parmvalue" id="zh-cn_topic_0226206976_parmvalue15618154916313"><a name="zh-cn_topic_0226206976_parmvalue15618154916313"></a><a name="zh-cn_topic_0226206976_parmvalue15618154916313"></a>“_”</span>，且长度为1~64个字符。默认与节点的名称一致。</p>
</td>
</tr>
<tr id="zh-cn_topic_0226206976_row1718310103317"><td class="cellrowborder" valign="top" width="24.88%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226206976_p55541039133113"><a name="zh-cn_topic_0226206976_p55541039133113"></a><a name="zh-cn_topic_0226206976_p55541039133113"></a>作业名称添加工作空间前缀</p>
</td>
<td class="cellrowborder" valign="top" width="10.38%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226206976_p185545391318"><a name="zh-cn_topic_0226206976_p185545391318"></a><a name="zh-cn_topic_0226206976_p185545391318"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="64.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226206976_p655493943114"><a name="zh-cn_topic_0226206976_p655493943114"></a><a name="zh-cn_topic_0226206976_p655493943114"></a>设置是否为创建的作业添加工作空间前缀。</p>
</td>
</tr>
<tr id="zh-cn_topic_0226206976_row2860171393113"><td class="cellrowborder" valign="top" width="24.88%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226206976_p285222953120"><a name="zh-cn_topic_0226206976_p285222953120"></a><a name="zh-cn_topic_0226206976_p285222953120"></a>节点名称</p>
</td>
<td class="cellrowborder" valign="top" width="10.38%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226206976_p19852102913117"><a name="zh-cn_topic_0226206976_p19852102913117"></a><a name="zh-cn_topic_0226206976_p19852102913117"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="64.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226206976_p1085215296315"><a name="zh-cn_topic_0226206976_p1085215296315"></a><a name="zh-cn_topic_0226206976_p1085215296315"></a><span id="zh-cn_topic_0099822521_text44323307153939_2"><a name="zh-cn_topic_0099822521_text44323307153939_2"></a><a name="zh-cn_topic_0099822521_text44323307153939_2"></a>节点</span>名称，可以包含中文、英文字母、数字、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253_2"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253_2"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue38166764101253_2"></a>“_”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253_2"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253_2"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue4500149101253_2"></a>“-”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_parmvalue3773104413412_2"><a name="zh-cn_topic_0099822521_parmvalue3773104413412_2"></a><a name="zh-cn_topic_0099822521_parmvalue3773104413412_2"></a>“/”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253_2"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253_2"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue28967750101253_2"></a>“&lt;”</span>、<span class="parmvalue" id="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253_2"><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253_2"></a><a name="zh-cn_topic_0099822521_zh-cn_topic_0099822521_parmvalue64686408101253_2"></a>“&gt;”</span>等各类特殊字符，长度为1～128个字符。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  高级参数

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
<a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_ul281538102858"></a><a name="zh-cn_topic_0226206976_zh-cn_topic_0099822521_ul281538102858"></a><ul id="zh-cn_topic_0226206976_zh-cn_topic_0099822521_ul281538102858"><li>终止当前作业执行计划</li><li>继续执行下一作业</li><li>挂起当前作业执行计划</li></ul>
</td>
</tr>
</tbody>
</table>

