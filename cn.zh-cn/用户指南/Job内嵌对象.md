# Job内嵌对象<a name="dayu_01_0498"></a>

Job为作业对象，提供了获取作业中上一节点的输出消息、作业调度计划时间、作业执行时间等属性和方法。

## 属性和方法<a name="zh-cn_topic_0132846497_section9326172819469"></a>

**表 1**  属性说明

<a name="zh-cn_topic_0132846497_table5983152818447"></a>
<table><thead align="left"><tr id="zh-cn_topic_0132846497_row1098352817443"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0132846497_p798322834416"><a name="zh-cn_topic_0132846497_p798322834416"></a><a name="zh-cn_topic_0132846497_p798322834416"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0132846497_p19832281441"><a name="zh-cn_topic_0132846497_p19832281441"></a><a name="zh-cn_topic_0132846497_p19832281441"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0132846497_p179833288448"><a name="zh-cn_topic_0132846497_p179833288448"></a><a name="zh-cn_topic_0132846497_p179833288448"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0132846497_row498322818449"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0132846497_p5983182814418"><a name="zh-cn_topic_0132846497_p5983182814418"></a><a name="zh-cn_topic_0132846497_p5983182814418"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0132846497_p19983132884416"><a name="zh-cn_topic_0132846497_p19983132884416"></a><a name="zh-cn_topic_0132846497_p19983132884416"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0132846497_p6983182804419"><a name="zh-cn_topic_0132846497_p6983182804419"></a><a name="zh-cn_topic_0132846497_p6983182804419"></a>作业名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0132846497_row7983132884414"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0132846497_p998392804417"><a name="zh-cn_topic_0132846497_p998392804417"></a><a name="zh-cn_topic_0132846497_p998392804417"></a>planTime</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0132846497_p13983122894418"><a name="zh-cn_topic_0132846497_p13983122894418"></a><a name="zh-cn_topic_0132846497_p13983122894418"></a>java.util.Date</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0132846497_p0983228164415"><a name="zh-cn_topic_0132846497_p0983228164415"></a><a name="zh-cn_topic_0132846497_p0983228164415"></a>作业调度计划时间，即周期调度配置的时间，例如每天凌晨1:01调度作业。</p>
</td>
</tr>
<tr id="zh-cn_topic_0132846497_row7983428164410"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0132846497_p1798310287443"><a name="zh-cn_topic_0132846497_p1798310287443"></a><a name="zh-cn_topic_0132846497_p1798310287443"></a>startTime</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0132846497_p9983828184414"><a name="zh-cn_topic_0132846497_p9983828184414"></a><a name="zh-cn_topic_0132846497_p9983828184414"></a>java.util.Date</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0132846497_p19831628184412"><a name="zh-cn_topic_0132846497_p19831628184412"></a><a name="zh-cn_topic_0132846497_p19831628184412"></a>作业执行时间，有可能与planTime同一个时间，也有可能晚于planTime（由于作业引擎繁忙等）。</p>
</td>
</tr>
<tr id="zh-cn_topic_0132846497_row1698314282448"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0132846497_p1498313282447"><a name="zh-cn_topic_0132846497_p1498313282447"></a><a name="zh-cn_topic_0132846497_p1498313282447"></a>eventData</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0132846497_p13983182820446"><a name="zh-cn_topic_0132846497_p13983182820446"></a><a name="zh-cn_topic_0132846497_p13983182820446"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0132846497_p39837283444"><a name="zh-cn_topic_0132846497_p39837283444"></a><a name="zh-cn_topic_0132846497_p39837283444"></a>当作业使用事件驱动调度时，从DIS通道获取的消息。</p>
</td>
</tr>
<tr id="zh-cn_topic_0132846497_row5983628124410"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0132846497_p698392819446"><a name="zh-cn_topic_0132846497_p698392819446"></a><a name="zh-cn_topic_0132846497_p698392819446"></a>projectId</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0132846497_p20983728174411"><a name="zh-cn_topic_0132846497_p20983728174411"></a><a name="zh-cn_topic_0132846497_p20983728174411"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0132846497_p1498352874416"><a name="zh-cn_topic_0132846497_p1498352874416"></a><a name="zh-cn_topic_0132846497_p1498352874416"></a>当前DLF所处项目ID。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  方法说明

<a name="zh-cn_topic_0132846497_table14461689017"></a>
<table><thead align="left"><tr id="zh-cn_topic_0132846497_row2446087010"><th class="cellrowborder" valign="top" width="38%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0132846497_p444698004"><a name="zh-cn_topic_0132846497_p444698004"></a><a name="zh-cn_topic_0132846497_p444698004"></a>方法</p>
</th>
<th class="cellrowborder" valign="top" width="62%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0132846497_p14461485016"><a name="zh-cn_topic_0132846497_p14461485016"></a><a name="zh-cn_topic_0132846497_p14461485016"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0132846497_row1440191316465"><td class="cellrowborder" valign="top" width="38%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0132846497_p144411113164610"><a name="zh-cn_topic_0132846497_p144411113164610"></a><a name="zh-cn_topic_0132846497_p144411113164610"></a>String getNodeStatus(String nodeName)</p>
</td>
<td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0132846497_p54411313204616"><a name="zh-cn_topic_0132846497_p54411313204616"></a><a name="zh-cn_topic_0132846497_p54411313204616"></a>获取指定节点运行状态，成功状态返回success，失败状态返回fail。</p>
</td>
</tr>
<tr id="zh-cn_topic_0132846497_row74461885010"><td class="cellrowborder" valign="top" width="38%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0132846497_p1044611814010"><a name="zh-cn_topic_0132846497_p1044611814010"></a><a name="zh-cn_topic_0132846497_p1044611814010"></a>String getNodeOutput(String nodeName)</p>
</td>
<td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0132846497_p104461088020"><a name="zh-cn_topic_0132846497_p104461088020"></a><a name="zh-cn_topic_0132846497_p104461088020"></a>获取指定节点的输出。此方法只能获取前面依赖节点的输出。目前只支持获取<span id="zh-cn_topic_0132846497_text156797322310"><a name="zh-cn_topic_0132846497_text156797322310"></a><a name="zh-cn_topic_0132846497_text156797322310"></a>Rest Client</span>节点的输出，即REST请求的返回消息。</p>
</td>
</tr>
<tr id="zh-cn_topic_0132846497_row1244611818019"><td class="cellrowborder" valign="top" width="38%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0132846497_p1446581604"><a name="zh-cn_topic_0132846497_p1446581604"></a><a name="zh-cn_topic_0132846497_p1446581604"></a>String getParam(String key)</p>
</td>
<td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0132846497_p144462081400"><a name="zh-cn_topic_0132846497_p144462081400"></a><a name="zh-cn_topic_0132846497_p144462081400"></a>获取作业参数。</p>
</td>
</tr>
<tr id="zh-cn_topic_0132846497_row1344688307"><td class="cellrowborder" valign="top" width="38%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0132846497_p24461781011"><a name="zh-cn_topic_0132846497_p24461781011"></a><a name="zh-cn_topic_0132846497_p24461781011"></a>String getPlanTime(String pattern)</p>
</td>
<td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0132846497_p204461881204"><a name="zh-cn_topic_0132846497_p204461881204"></a><a name="zh-cn_topic_0132846497_p204461881204"></a>获取指定pattern的计划时间字符串，pattern为日期、时间模式，请参考<a href="日期和时间模式.md#dayu_01_0496">日期和时间模式</a>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0132846497_row14461083020"><td class="cellrowborder" valign="top" width="38%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0132846497_p2446148805"><a name="zh-cn_topic_0132846497_p2446148805"></a><a name="zh-cn_topic_0132846497_p2446148805"></a>String getYesterday(String pattern)</p>
</td>
<td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0132846497_p10446383018"><a name="zh-cn_topic_0132846497_p10446383018"></a><a name="zh-cn_topic_0132846497_p10446383018"></a>获取执行pattern的计划时间前一天的时间字符串，pattern为日期、时间模式，请参考<a href="日期和时间模式.md#dayu_01_0496">日期和时间模式</a>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0132846497_row184461381903"><td class="cellrowborder" valign="top" width="38%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0132846497_p194461688018"><a name="zh-cn_topic_0132846497_p194461688018"></a><a name="zh-cn_topic_0132846497_p194461688018"></a>String getLastHour(String pattern)</p>
</td>
<td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0132846497_p11446108105"><a name="zh-cn_topic_0132846497_p11446108105"></a><a name="zh-cn_topic_0132846497_p11446108105"></a>获取执行pattern的计划时间前一小时的时间字符串，pattern为日期、时间模式，请参考<a href="日期和时间模式.md#dayu_01_0496">日期和时间模式</a>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0132846497_row39069153012"><td class="cellrowborder" valign="top" width="38%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0132846497_p1906191510013"><a name="zh-cn_topic_0132846497_p1906191510013"></a><a name="zh-cn_topic_0132846497_p1906191510013"></a>String getRunningData(String nodeName)</p>
</td>
<td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0132846497_p99753402494"><a name="zh-cn_topic_0132846497_p99753402494"></a><a name="zh-cn_topic_0132846497_p99753402494"></a>获取指定节点运行中记录的数据。此方法只能获取前面依赖节点的输出。当前只支持获取DLI SQL节点运行中记录的DLI作业id，例如，想要获取DLI节点第3条语句的job ID（DLI节点名为DLI_INSERT_DATA），可以这样使用：#{JSONUtil.path(Job.getRunningData("DLI_INSERT_DATA"),"jobIds[2]")}。</p>
</td>
</tr>
<tr id="zh-cn_topic_0132846497_row1121919124015"><td class="cellrowborder" valign="top" width="38%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0132846497_p1622018121203"><a name="zh-cn_topic_0132846497_p1622018121203"></a><a name="zh-cn_topic_0132846497_p1622018121203"></a>String getInsertJobId(String nodeName)</p>
</td>
<td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0132846497_p142205128020"><a name="zh-cn_topic_0132846497_p142205128020"></a><a name="zh-cn_topic_0132846497_p142205128020"></a>返回指定DLI SQL或Transform Load节点第一个DLI Insert SQL语句的作业ID，不指定参数nodeName时，获取前面一个节点第一个DLI Insert SQL语句的作业ID，如果无法获取到作业ID，返回null值。</p>
</td>
</tr>
</tbody>
</table>

## 举例<a name="zh-cn_topic_0132846497_section1259817279715"></a>

获取作业中节点名称为**test**的输出，EL表达式如下：

```
#{Job.getNodeOutput("test")}
```

