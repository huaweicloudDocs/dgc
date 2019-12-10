# 配置Hive源端参数<a name="dayu_01_0051"></a>

作业中源连接为[配置Hive连接](配置Hive连接.md)时，源端作业参数如[表1](#zh-cn_topic_0108275424_table31823995163953)所示。

**表 1**  Hive作为源端时的作业参数

<a name="zh-cn_topic_0108275424_table31823995163953"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108275424_row18653487163953"><th class="cellrowborder" valign="top" width="23.36%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108275424_p15314298163953"><a name="zh-cn_topic_0108275424_p15314298163953"></a><a name="zh-cn_topic_0108275424_p15314298163953"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="52.33%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108275424_p32498630163953"><a name="zh-cn_topic_0108275424_p32498630163953"></a><a name="zh-cn_topic_0108275424_p32498630163953"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="24.310000000000002%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108275424_p15143370163953"><a name="zh-cn_topic_0108275424_p15143370163953"></a><a name="zh-cn_topic_0108275424_p15143370163953"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108275424_row1928353163953"><td class="cellrowborder" valign="top" width="23.36%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275424_p28108739161524"><a name="zh-cn_topic_0108275424_p28108739161524"></a><a name="zh-cn_topic_0108275424_p28108739161524"></a>数据库名称</p>
</td>
<td class="cellrowborder" valign="top" width="52.33%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275424_p17702619155928"><a name="zh-cn_topic_0108275424_p17702619155928"></a><a name="zh-cn_topic_0108275424_p17702619155928"></a>输入或选择数据库名称。单击输入框后面的按钮可进入数据库选择界面。</p>
</td>
<td class="cellrowborder" valign="top" width="24.310000000000002%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275424_p64647157163953"><a name="zh-cn_topic_0108275424_p64647157163953"></a><a name="zh-cn_topic_0108275424_p64647157163953"></a>default</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275424_row11687830163953"><td class="cellrowborder" valign="top" width="23.36%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275424_p23518636161524"><a name="zh-cn_topic_0108275424_p23518636161524"></a><a name="zh-cn_topic_0108275424_p23518636161524"></a>表名</p>
</td>
<td class="cellrowborder" valign="top" width="52.33%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275424_p17984995155931"><a name="zh-cn_topic_0108275424_p17984995155931"></a><a name="zh-cn_topic_0108275424_p17984995155931"></a>输入或选择Hive表名。单击输入框后面的按钮可进入表的选择界面。</p>
<p id="zh-cn_topic_0108275442_p1210244910548"><a name="zh-cn_topic_0108275442_p1210244910548"></a><a name="zh-cn_topic_0108275442_p1210244910548"></a>该参数支持配置为时间宏变量，且一个路径名中可以有多个宏定义变量。使用时间宏变量和定时任务配合，可以实现定期同步新增数据，详细说明请参见<a href="使用时间宏变量完成增量同步.md">使用时间宏变量完成增量同步</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="24.310000000000002%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275424_p50683068163953"><a name="zh-cn_topic_0108275424_p50683068163953"></a><a name="zh-cn_topic_0108275424_p50683068163953"></a>TBL_E</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：**   
>Hive作为数据源，CDM自动使用Hive数据分片文件进行数据分区。  

