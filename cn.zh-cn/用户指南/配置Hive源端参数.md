# 配置Hive源端参数<a name="dgc_01_0051"></a>

作业中源连接为[配置Hive连接](配置Hive连接.md#dgc_01_0026)时，源端作业参数如[表1](#zh-cn_topic_0108275424_table31823995163953)所示。

**表 1**  Hive作为源端时的作业参数

<a name="zh-cn_topic_0108275424_table31823995163953"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108275424_row18653487163953"><th class="cellrowborder" valign="top" width="15.690000000000001%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108275424_p15314298163953"><a name="zh-cn_topic_0108275424_p15314298163953"></a><a name="zh-cn_topic_0108275424_p15314298163953"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="47.03%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108275424_p32498630163953"><a name="zh-cn_topic_0108275424_p32498630163953"></a><a name="zh-cn_topic_0108275424_p32498630163953"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="37.28%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108275424_p15143370163953"><a name="zh-cn_topic_0108275424_p15143370163953"></a><a name="zh-cn_topic_0108275424_p15143370163953"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108275424_row1928353163953"><td class="cellrowborder" valign="top" width="15.690000000000001%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275424_p28108739161524"><a name="zh-cn_topic_0108275424_p28108739161524"></a><a name="zh-cn_topic_0108275424_p28108739161524"></a>数据库名称</p>
</td>
<td class="cellrowborder" valign="top" width="47.03%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275424_p17702619155928"><a name="zh-cn_topic_0108275424_p17702619155928"></a><a name="zh-cn_topic_0108275424_p17702619155928"></a>输入或选择数据库名称。单击输入框后面的按钮可进入数据库选择界面。</p>
</td>
<td class="cellrowborder" valign="top" width="37.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275424_p64647157163953"><a name="zh-cn_topic_0108275424_p64647157163953"></a><a name="zh-cn_topic_0108275424_p64647157163953"></a>default</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275424_row11687830163953"><td class="cellrowborder" valign="top" width="15.690000000000001%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275424_p23518636161524"><a name="zh-cn_topic_0108275424_p23518636161524"></a><a name="zh-cn_topic_0108275424_p23518636161524"></a>表名</p>
</td>
<td class="cellrowborder" valign="top" width="47.03%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275424_p17984995155931"><a name="zh-cn_topic_0108275424_p17984995155931"></a><a name="zh-cn_topic_0108275424_p17984995155931"></a>输入或选择Hive表名。单击输入框后面的按钮可进入表的选择界面。</p>
<p id="zh-cn_topic_0108275424_p1210244910548"><a name="zh-cn_topic_0108275424_p1210244910548"></a><a name="zh-cn_topic_0108275424_p1210244910548"></a>该参数支持配置为时间宏变量，且一个路径名中可以有多个宏定义变量。使用时间宏变量和定时任务配合，可以实现定期同步新增数据，详细说明请参见<a href="https://support.huaweicloud.com/bestpractice-dgc/dgc_05_0006.html" target="_blank" rel="noopener noreferrer">使用时间宏变量完成增量同步</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="37.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275424_p50683068163953"><a name="zh-cn_topic_0108275424_p50683068163953"></a><a name="zh-cn_topic_0108275424_p50683068163953"></a>TBL_E</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275424_row962165734014"><td class="cellrowborder" valign="top" width="15.690000000000001%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275424_p96355710402"><a name="zh-cn_topic_0108275424_p96355710402"></a><a name="zh-cn_topic_0108275424_p96355710402"></a>读取方式</p>
</td>
<td class="cellrowborder" valign="top" width="47.03%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275424_p1656393534412"><a name="zh-cn_topic_0108275424_p1656393534412"></a><a name="zh-cn_topic_0108275424_p1656393534412"></a>包括HDFS和JDBC两种读取方式。默认为HDFS方式，如果没有使用WHERE条件做数据过滤及在字段映射页面添加新字段的需求，选择HDFS方式即可。</p>
<a name="zh-cn_topic_0108275424_ul169421201417"></a><a name="zh-cn_topic_0108275424_ul169421201417"></a><ul id="zh-cn_topic_0108275424_ul169421201417"><li>HDFS文件方式读取数据时，性能较好，但不支持使用WHERE条件做数据过滤及在字段映射页面添加新字段。</li><li>JDBC方式读取数据时，支持使用WHERE条件做数据过滤及在字段映射页面添加新字段。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="37.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275424_p2631557154010"><a name="zh-cn_topic_0108275424_p2631557154010"></a><a name="zh-cn_topic_0108275424_p2631557154010"></a>HDFS</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275424_row4203135418142"><td class="cellrowborder" valign="top" width="15.690000000000001%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275424_p7203154151410"><a name="zh-cn_topic_0108275424_p7203154151410"></a><a name="zh-cn_topic_0108275424_p7203154151410"></a>分区过滤条件</p>
</td>
<td class="cellrowborder" valign="top" width="47.03%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275424_p1219435334515"><a name="zh-cn_topic_0108275424_p1219435334515"></a><a name="zh-cn_topic_0108275424_p1219435334515"></a>读取方式为HDFS时，单击<span class="uicontrol" id="zh-cn_topic_0108275424_uicontrol128295157266"><a name="zh-cn_topic_0108275424_uicontrol128295157266"></a><a name="zh-cn_topic_0108275424_uicontrol128295157266"></a>“显示高级属性”</span>后显示此参数。</p>
<p id="zh-cn_topic_0108275424_p1020335414148"><a name="zh-cn_topic_0108275424_p1020335414148"></a><a name="zh-cn_topic_0108275424_p1020335414148"></a>该参数表示抽取指定值的partition，可以配置多个值（空格分隔），也可以配置范围，接受时间宏函数。时间宏函数的说明请参见<a href="https://support.huaweicloud.com/bestpractice-dgc/dgc_05_0006.html" target="_blank" rel="noopener noreferrer">使用时间宏变量完成增量同步</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="37.28%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0108275424_ul16185646318"></a><a name="zh-cn_topic_0108275424_ul16185646318"></a><ul id="zh-cn_topic_0108275424_ul16185646318"><li>单/多值过滤：<p id="zh-cn_topic_0108275424_p88421435130"><a name="zh-cn_topic_0108275424_p88421435130"></a><a name="zh-cn_topic_0108275424_p88421435130"></a>"${dateformat(yyyyMMdd, -1, DAY)} ${dateformat(yyyyMMdd)}"</p>
</li><li>范围过滤：<p id="zh-cn_topic_0108275424_p22875441038"><a name="zh-cn_topic_0108275424_p22875441038"></a><a name="zh-cn_topic_0108275424_p22875441038"></a>"${value} &gt;= ${dateformat(yyyyMMdd, -7, DAY)} &amp;&amp; ${value} &lt; ${dateformat(yyyyMMdd)}"</p>
</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0108275424_row131351318184611"><td class="cellrowborder" valign="top" width="15.690000000000001%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275424_p54171024164616"><a name="zh-cn_topic_0108275424_p54171024164616"></a><a name="zh-cn_topic_0108275424_p54171024164616"></a>Where子句</p>
</td>
<td class="cellrowborder" valign="top" width="47.03%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275424_p1213520181469"><a name="zh-cn_topic_0108275424_p1213520181469"></a><a name="zh-cn_topic_0108275424_p1213520181469"></a>读取方式为JDBC时，单击<span class="uicontrol" id="zh-cn_topic_0108275424_uicontrol12752132919461"><a name="zh-cn_topic_0108275424_uicontrol12752132919461"></a><a name="zh-cn_topic_0108275424_uicontrol12752132919461"></a>“显示高级属性”</span>后显示此参数。</p>
<p id="zh-cn_topic_0108275424_p976143054712"><a name="zh-cn_topic_0108275424_p976143054712"></a><a name="zh-cn_topic_0108275424_p976143054712"></a>填写该参数表示指定抽取的WHERE子句，不指定则抽取整表。如果要迁移的表中没有WHERE子句的字段，则会迁移失败。</p>
<p id="zh-cn_topic_0108275424_p18740131613716"><a name="zh-cn_topic_0108275424_p18740131613716"></a><a name="zh-cn_topic_0108275424_p18740131613716"></a>该参数支持配置为时间宏变量，实现抽取指定日期的数据，详细说明请参见<a href="https://support.huaweicloud.com/bestpractice-dgc/dgc_05_0005.html" target="_blank" rel="noopener noreferrer">关系数据库增量迁移</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="37.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275424_p8135518144617"><a name="zh-cn_topic_0108275424_p8135518144617"></a><a name="zh-cn_topic_0108275424_p8135518144617"></a>age &gt; 18 and age &lt;= 60</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：** 
>Hive作为数据源，CDM自动使用Hive数据分片文件进行数据分区。

