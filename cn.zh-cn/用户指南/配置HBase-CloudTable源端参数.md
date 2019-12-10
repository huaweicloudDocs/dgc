# 配置HBase/CloudTable源端参数<a name="dayu_01_0050"></a>

作业中源连接为[配置HBase连接](配置HBase连接.md)或[配置CloudTable连接](配置CloudTable连接.md)时，即从MRS HBase、FusionInsight HBase、Apache HBase或者CloudTable导出数据时，源端作业参数如[表1](#zh-cn_topic_0108275276_table5046103815165)所示。

>![](public_sys-resources/icon-note.gif) **说明：**   
>1.  CloudTable或HBase作为源端时，CDM会读取表的首行数据作为字段列表样例，如果首行数据未包含该表的所有字段，用户需要自己手工添加字段。  
>2.  由于HBase的无Schema技术特点，CDM无法获知数据类型，如果数据内容是使用二进制格式存储的，CDM会无法解析。  
>1.  从HBase/CloudTable导出数据时，由于HBase/CloudTable是无Schema的存储系统，CDM要求源端数值型字段是以字符串格式存储，而不能是二进制格式，例如数值100需存储格式是字符串“100“，不能是二进制“01100100“。  

**表 1**  HBase作为源端时的作业参数

<a name="zh-cn_topic_0108275276_table5046103815165"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108275276_row585315215165"><th class="cellrowborder" valign="top" width="20.919999999999998%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108275276_p1626397215165"><a name="zh-cn_topic_0108275276_p1626397215165"></a><a name="zh-cn_topic_0108275276_p1626397215165"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="57.02%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108275276_p4231334915165"><a name="zh-cn_topic_0108275276_p4231334915165"></a><a name="zh-cn_topic_0108275276_p4231334915165"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="22.06%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108275276_p482921015165"><a name="zh-cn_topic_0108275276_p482921015165"></a><a name="zh-cn_topic_0108275276_p482921015165"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108275276_row4012116315165"><td class="cellrowborder" valign="top" width="20.919999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275276_p2858877215165"><a name="zh-cn_topic_0108275276_p2858877215165"></a><a name="zh-cn_topic_0108275276_p2858877215165"></a>表名</p>
</td>
<td class="cellrowborder" valign="top" width="57.02%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275276_p3398923015165"><a name="zh-cn_topic_0108275276_p3398923015165"></a><a name="zh-cn_topic_0108275276_p3398923015165"></a>导出数据的HBase表名。</p>
<p id="zh-cn_topic_0108275442_p1210244910548"><a name="zh-cn_topic_0108275442_p1210244910548"></a><a name="zh-cn_topic_0108275442_p1210244910548"></a>该参数支持配置为时间宏变量，且一个路径名中可以有多个宏定义变量。使用时间宏变量和定时任务配合，可以实现定期同步新增数据，详细说明请参见<a href="使用时间宏变量完成增量同步.md">使用时间宏变量完成增量同步</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="22.06%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275276_p166427315165"><a name="zh-cn_topic_0108275276_p166427315165"></a><a name="zh-cn_topic_0108275276_p166427315165"></a>TBL_2</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275276_row2085795312515"><td class="cellrowborder" valign="top" width="20.919999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275276_p9857953135118"><a name="zh-cn_topic_0108275276_p9857953135118"></a><a name="zh-cn_topic_0108275276_p9857953135118"></a>列族</p>
</td>
<td class="cellrowborder" valign="top" width="57.02%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275276_p168572535513"><a name="zh-cn_topic_0108275276_p168572535513"></a><a name="zh-cn_topic_0108275276_p168572535513"></a>可选参数，导出数据所属的列族。</p>
</td>
<td class="cellrowborder" valign="top" width="22.06%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275276_p11857175335116"><a name="zh-cn_topic_0108275276_p11857175335116"></a><a name="zh-cn_topic_0108275276_p11857175335116"></a>CF1&amp;CF2</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275276_row68131455163415"><td class="cellrowborder" valign="top" width="20.919999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275276_p198131455173412"><a name="zh-cn_topic_0108275276_p198131455173412"></a><a name="zh-cn_topic_0108275276_p198131455173412"></a>切分Rowkey</p>
</td>
<td class="cellrowborder" valign="top" width="57.02%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275276_p14813655143413"><a name="zh-cn_topic_0108275276_p14813655143413"></a><a name="zh-cn_topic_0108275276_p14813655143413"></a>可选参数，选择是否拆分Rowkey，默认为<span class="parmvalue" id="zh-cn_topic_0108275276_parmvalue10921715103718"><a name="zh-cn_topic_0108275276_parmvalue10921715103718"></a><a name="zh-cn_topic_0108275276_parmvalue10921715103718"></a>“否”</span>。</p>
</td>
<td class="cellrowborder" valign="top" width="22.06%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275276_p881355511346"><a name="zh-cn_topic_0108275276_p881355511346"></a><a name="zh-cn_topic_0108275276_p881355511346"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275276_row1431725743415"><td class="cellrowborder" valign="top" width="20.919999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275276_p3317457133416"><a name="zh-cn_topic_0108275276_p3317457133416"></a><a name="zh-cn_topic_0108275276_p3317457133416"></a>Rowkey分隔符</p>
</td>
<td class="cellrowborder" valign="top" width="57.02%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275276_p1631810574340"><a name="zh-cn_topic_0108275276_p1631810574340"></a><a name="zh-cn_topic_0108275276_p1631810574340"></a>可选参数，用于拆分Rowkey的分隔符，若不设置则不切分。</p>
</td>
<td class="cellrowborder" valign="top" width="22.06%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275276_p15318175714341"><a name="zh-cn_topic_0108275276_p15318175714341"></a><a name="zh-cn_topic_0108275276_p15318175714341"></a>|</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275276_row667043895219"><td class="cellrowborder" valign="top" width="20.919999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275276_p1967023835217"><a name="zh-cn_topic_0108275276_p1967023835217"></a><a name="zh-cn_topic_0108275276_p1967023835217"></a>起始时间</p>
</td>
<td class="cellrowborder" valign="top" width="57.02%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275276_p091005834018"><a name="zh-cn_topic_0108275276_p091005834018"></a><a name="zh-cn_topic_0108275276_p091005834018"></a>可选参数，<span id="zh-cn_topic_0108275276_ph5654161619427"><a name="zh-cn_topic_0108275276_ph5654161619427"></a><a name="zh-cn_topic_0108275276_ph5654161619427"></a>起始时间（包含该值），格式为<span class="uicontrol" id="zh-cn_topic_0108275276_uicontrol1791019582400"><a name="zh-cn_topic_0108275276_uicontrol1791019582400"></a><a name="zh-cn_topic_0108275276_uicontrol1791019582400"></a>“yyyy-MM-dd HH:mm:ss”</span>，表示只抽取该时间及以后的数据。</span></p>
<p id="zh-cn_topic_0108275276_p116711580415"><a name="zh-cn_topic_0108275276_p116711580415"></a><a name="zh-cn_topic_0108275276_p116711580415"></a>该参数支持配置为时间宏变量，使用时间宏变量和定时任务配合，可以实现定期同步新增数据，详细说明请参见<a href="使用时间宏变量完成增量同步.md">使用时间宏变量完成增量同步</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="22.06%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275276_p17670173812526"><a name="zh-cn_topic_0108275276_p17670173812526"></a><a name="zh-cn_topic_0108275276_p17670173812526"></a>2019-01-01 20:00:00</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275276_row6700144113522"><td class="cellrowborder" valign="top" width="20.919999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275276_p1970004165215"><a name="zh-cn_topic_0108275276_p1970004165215"></a><a name="zh-cn_topic_0108275276_p1970004165215"></a>终止时间</p>
</td>
<td class="cellrowborder" valign="top" width="57.02%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275276_p2700041145210"><a name="zh-cn_topic_0108275276_p2700041145210"></a><a name="zh-cn_topic_0108275276_p2700041145210"></a>可选参数，<span id="zh-cn_topic_0108275276_ph5201142410429"><a name="zh-cn_topic_0108275276_ph5201142410429"></a><a name="zh-cn_topic_0108275276_ph5201142410429"></a>终止时间（不包含该值），格式为<span class="uicontrol" id="zh-cn_topic_0108275276_uicontrol922161113549"><a name="zh-cn_topic_0108275276_uicontrol922161113549"></a><a name="zh-cn_topic_0108275276_uicontrol922161113549"></a>“yyyy-MM-dd HH:mm:ss”</span>，表示只抽取该时间以前的数据。</span></p>
<p id="zh-cn_topic_0108275276_p92671211101710"><a name="zh-cn_topic_0108275276_p92671211101710"></a><a name="zh-cn_topic_0108275276_p92671211101710"></a>该参数支持配置为时间宏变量，详细说明请参见<a href="使用时间宏变量完成增量同步.md">使用时间宏变量完成增量同步</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="22.06%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275276_p17007416523"><a name="zh-cn_topic_0108275276_p17007416523"></a><a name="zh-cn_topic_0108275276_p17007416523"></a>2019-02-01 20:00:00</p>
</td>
</tr>
</tbody>
</table>

