# 配置目的端HBase/CloudTable目的端参数<a name="dayu_01_0064"></a>

作业中目的连接为[配置HBase连接](配置HBase连接.md)或[配置CloudTable连接](配置CloudTable连接.md)时，即导入数据到以下数据源时，目的端作业参数如[表1](#zh-cn_topic_0108275309_table5046103815165)所示。

-   MRS HBase
-   FusionInsight HBase
-   Apache HBase
-   CloudTable

**表 1**  HBase/CloudTable作为目的端时的作业参数

<a name="zh-cn_topic_0108275309_table5046103815165"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108275309_row585315215165"><th class="cellrowborder" valign="top" width="24.97%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108275309_p1626397215165"><a name="zh-cn_topic_0108275309_p1626397215165"></a><a name="zh-cn_topic_0108275309_p1626397215165"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="55.03%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108275309_p4231334915165"><a name="zh-cn_topic_0108275309_p4231334915165"></a><a name="zh-cn_topic_0108275309_p4231334915165"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108275309_p482921015165"><a name="zh-cn_topic_0108275309_p482921015165"></a><a name="zh-cn_topic_0108275309_p482921015165"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108275309_row4012116315165"><td class="cellrowborder" valign="top" width="24.97%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275309_p2858877215165"><a name="zh-cn_topic_0108275309_p2858877215165"></a><a name="zh-cn_topic_0108275309_p2858877215165"></a>表名</p>
</td>
<td class="cellrowborder" valign="top" width="55.03%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275309_p3398923015165"><a name="zh-cn_topic_0108275309_p3398923015165"></a><a name="zh-cn_topic_0108275309_p3398923015165"></a>写入数据的HBase表名。如果是创建新HBase表，支持从源端拷贝字段名。单击输入框后面的按钮可进入表的选择界面。</p>
<p id="zh-cn_topic_0108275442_p1210244910548"><a name="zh-cn_topic_0108275442_p1210244910548"></a><a name="zh-cn_topic_0108275442_p1210244910548"></a>该参数支持配置为时间宏变量，且一个路径名中可以有多个宏定义变量。使用时间宏变量和定时任务配合，可以实现定期同步新增数据，详细说明请参见<a href="使用时间宏变量完成增量同步.md">使用时间宏变量完成增量同步</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275309_p166427315165"><a name="zh-cn_topic_0108275309_p166427315165"></a><a name="zh-cn_topic_0108275309_p166427315165"></a>TBL_2</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275309_row14607720151241"><td class="cellrowborder" valign="top" width="24.97%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275309_p9799599151241"><a name="zh-cn_topic_0108275309_p9799599151241"></a><a name="zh-cn_topic_0108275309_p9799599151241"></a>导入前清空数据</p>
</td>
<td class="cellrowborder" valign="top" width="55.03%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108275309_p49350536142510"><a name="zh-cn_topic_0108275309_p49350536142510"></a><a name="zh-cn_topic_0108275309_p49350536142510"></a>选择目的端表中数据的处理方式：<a name="zh-cn_topic_0108275481_ua1819b93796044cd9f46f9dfb3e78f6b"></a><a name="zh-cn_topic_0108275481_ua1819b93796044cd9f46f9dfb3e78f6b"></a><ul id="zh-cn_topic_0108275481_ua1819b93796044cd9f46f9dfb3e78f6b"><li>是：任务启动前会清除目标表中数据。</li><li>否：导入前不清空目标表中的数据，如果选<span class="parmvalue" id="zh-cn_topic_0108275481_p47d3026f5a84445ebd15d358a7cc2720"><a name="zh-cn_topic_0108275481_p47d3026f5a84445ebd15d358a7cc2720"></a><a name="zh-cn_topic_0108275481_p47d3026f5a84445ebd15d358a7cc2720"></a>“否”</span>且表中有数据，则数据会追加到已有的表中。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275309_p4879287151241"><a name="zh-cn_topic_0108275309_p4879287151241"></a><a name="zh-cn_topic_0108275309_p4879287151241"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275309_row222701815165"><td class="cellrowborder" valign="top" width="24.97%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275309_p3385126816013"><a name="zh-cn_topic_0108275309_p3385126816013"></a><a name="zh-cn_topic_0108275309_p3385126816013"></a>Row key拼接分隔符</p>
</td>
<td class="cellrowborder" valign="top" width="55.03%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275309_p5345668716027"><a name="zh-cn_topic_0108275309_p5345668716027"></a><a name="zh-cn_topic_0108275309_p5345668716027"></a>可选参数，用于多列合并作为rowkey，默认为空格。</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275309_p322507154548"><a name="zh-cn_topic_0108275309_p322507154548"></a><a name="zh-cn_topic_0108275309_p322507154548"></a>,</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275309_row29420512145148"><td class="cellrowborder" valign="top" width="24.97%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275309_p22891711145148"><a name="zh-cn_topic_0108275309_p22891711145148"></a><a name="zh-cn_topic_0108275309_p22891711145148"></a>Rowkey冗余</p>
</td>
<td class="cellrowborder" valign="top" width="55.03%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275309_p42289313145148"><a name="zh-cn_topic_0108275309_p42289313145148"></a><a name="zh-cn_topic_0108275309_p42289313145148"></a>可选参数，是否将选做Rowkey的数据同时写入HBase的列，默认值<span class="parmvalue" id="zh-cn_topic_0108275309_parmvalue63955938145255"><a name="zh-cn_topic_0108275309_parmvalue63955938145255"></a><a name="zh-cn_topic_0108275309_parmvalue63955938145255"></a>“否”</span>。</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275309_p2882352145148"><a name="zh-cn_topic_0108275309_p2882352145148"></a><a name="zh-cn_topic_0108275309_p2882352145148"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275309_row12086944145153"><td class="cellrowborder" valign="top" width="24.97%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275309_p46874800145153"><a name="zh-cn_topic_0108275309_p46874800145153"></a><a name="zh-cn_topic_0108275309_p46874800145153"></a>压缩算法</p>
</td>
<td class="cellrowborder" valign="top" width="55.03%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108275309_p38762485145153"><a name="zh-cn_topic_0108275309_p38762485145153"></a><a name="zh-cn_topic_0108275309_p38762485145153"></a>可选参数，创建新HBase表时采用的压缩算法，默认为值<span class="parmvalue" id="zh-cn_topic_0108275309_parmvalue25185961145424"><a name="zh-cn_topic_0108275309_parmvalue25185961145424"></a><a name="zh-cn_topic_0108275309_parmvalue25185961145424"></a>“NONE”</span>。<a name="zh-cn_topic_0108275309_ul59671921145439"></a><a name="zh-cn_topic_0108275309_ul59671921145439"></a><ul id="zh-cn_topic_0108275309_ul59671921145439"><li>NONE：不压缩。</li><li>SNAPPY：压缩为Snappy格式。</li><li>GZ：压缩为GZ格式。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275309_p52753603145153"><a name="zh-cn_topic_0108275309_p52753603145153"></a><a name="zh-cn_topic_0108275309_p52753603145153"></a>NONE</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275309_row5532119162618"><td class="cellrowborder" valign="top" width="24.97%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275309_p8532121910267"><a name="zh-cn_topic_0108275309_p8532121910267"></a><a name="zh-cn_topic_0108275309_p8532121910267"></a>WAL开关</p>
</td>
<td class="cellrowborder" valign="top" width="55.03%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275309_p791673125616"><a name="zh-cn_topic_0108275309_p791673125616"></a><a name="zh-cn_topic_0108275309_p791673125616"></a>选择是否开启HBase的预写日志机制（WAL，Write Ahead Log）。</p>
<a name="zh-cn_topic_0108275309_ul1899132517107"></a><a name="zh-cn_topic_0108275309_ul1899132517107"></a><ul id="zh-cn_topic_0108275309_ul1899132517107"><li>是：开启后如果出现HBase服务器宕机，则可以从WAL中回放执行之前没有完成的操作。</li><li>否：关闭时能提升写入性能，但如果HBase服务器宕机可能会造成数据丢失。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275309_p11532151914268"><a name="zh-cn_topic_0108275309_p11532151914268"></a><a name="zh-cn_topic_0108275309_p11532151914268"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275309_row13472310174"><td class="cellrowborder" valign="top" width="24.97%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275309_p6474110971"><a name="zh-cn_topic_0108275309_p6474110971"></a><a name="zh-cn_topic_0108275309_p6474110971"></a>匹配数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="55.03%" headers="mcps1.2.4.1.2 "><a name="zh-cn_topic_0108275309_ul4509123194219"></a><a name="zh-cn_topic_0108275309_ul4509123194219"></a><ul id="zh-cn_topic_0108275309_ul4509123194219"><li>是：源端数据库中的Short、Int、Long、Float、Double、Decimal类型列的数据，会转换为Byte[]数组（二进制）写入HBase，其他类型的按字符串写入。如果这几种类型中，有合并做rowkey的，则依然当字符串写入。<p id="zh-cn_topic_0108275309_p12731115251120"><a name="zh-cn_topic_0108275309_p12731115251120"></a><a name="zh-cn_topic_0108275309_p12731115251120"></a>该功能作用是：降低存储占用空间，存储更高效；特定场景下rowkey分布更均匀。</p>
</li><li>否：源端数据库中所有类型的数据，都会按照字符串写入HBase。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275309_p24742101873"><a name="zh-cn_topic_0108275309_p24742101873"></a><a name="zh-cn_topic_0108275309_p24742101873"></a>否</p>
</td>
</tr>
</tbody>
</table>

