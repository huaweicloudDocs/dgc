# 配置Hive目的端参数<a name="dgc_01_0066"></a>

作业中目的连接为[配置Hive连接](配置Hive连接.md#dgc_01_0026)时，目的端作业参数如[表1](#zh-cn_topic_0108275481_table31823995163953)所示。

**表 1**  Hive作为目的端时的作业参数

<a name="zh-cn_topic_0108275481_table31823995163953"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108275481_row18653487163953"><th class="cellrowborder" valign="top" width="18.28%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108275481_p15314298163953"><a name="zh-cn_topic_0108275481_p15314298163953"></a><a name="zh-cn_topic_0108275481_p15314298163953"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="62.34%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108275481_p32498630163953"><a name="zh-cn_topic_0108275481_p32498630163953"></a><a name="zh-cn_topic_0108275481_p32498630163953"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="19.380000000000003%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108275481_p15143370163953"><a name="zh-cn_topic_0108275481_p15143370163953"></a><a name="zh-cn_topic_0108275481_p15143370163953"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108275481_row1928353163953"><td class="cellrowborder" valign="top" width="18.28%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275481_p28108739161524"><a name="zh-cn_topic_0108275481_p28108739161524"></a><a name="zh-cn_topic_0108275481_p28108739161524"></a>数据库名称</p>
</td>
<td class="cellrowborder" valign="top" width="62.34%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275481_p17702619155928"><a name="zh-cn_topic_0108275481_p17702619155928"></a><a name="zh-cn_topic_0108275481_p17702619155928"></a>输入或选择写入数据的数据库名称。单击输入框后面的按钮可进入数据库选择界面。</p>
</td>
<td class="cellrowborder" valign="top" width="19.380000000000003%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275481_p64647157163953"><a name="zh-cn_topic_0108275481_p64647157163953"></a><a name="zh-cn_topic_0108275481_p64647157163953"></a>default</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275481_row36864132115613"><td class="cellrowborder" valign="top" width="18.28%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275481_p33204741115613"><a name="zh-cn_topic_0108275481_p33204741115613"></a><a name="zh-cn_topic_0108275481_p33204741115613"></a>自动创表</p>
</td>
<td class="cellrowborder" valign="top" width="62.34%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108275481_p5229539115613"><a name="zh-cn_topic_0108275481_p5229539115613"></a><a name="zh-cn_topic_0108275481_p5229539115613"></a>只有当源端为关系数据库时，才有该参数。表示写入表数据时，用户选择的操作：<a name="zh-cn_topic_0108275481_zh-cn_topic_0108275472_ul12109569172733"></a><a name="zh-cn_topic_0108275481_zh-cn_topic_0108275472_ul12109569172733"></a><ul id="zh-cn_topic_0108275481_zh-cn_topic_0108275472_ul12109569172733"><li>不自动创建：不自动建表。</li><li>不存在时创建：当目的端的数据库没有<span class="parmname" id="zh-cn_topic_0108275481_zh-cn_topic_0108275472_parmname42948736113514"><a name="zh-cn_topic_0108275481_zh-cn_topic_0108275472_parmname42948736113514"></a><a name="zh-cn_topic_0108275481_zh-cn_topic_0108275472_parmname42948736113514"></a>“表名”</span>参数中指定的表时，CDM会自动创建该表。如果<span class="parmname" id="zh-cn_topic_0108275481_zh-cn_topic_0108275472_parmname13354101333310"><a name="zh-cn_topic_0108275481_zh-cn_topic_0108275472_parmname13354101333310"></a><a name="zh-cn_topic_0108275481_zh-cn_topic_0108275472_parmname13354101333310"></a>“表名”</span>参数配置的表已存在，则不创建，数据写入到已存在的表中。</li><li>先删除后创建：CDM先删除<span class="parmname" id="zh-cn_topic_0108275481_zh-cn_topic_0108275472_parmname55972483114928"><a name="zh-cn_topic_0108275481_zh-cn_topic_0108275472_parmname55972483114928"></a><a name="zh-cn_topic_0108275481_zh-cn_topic_0108275472_parmname55972483114928"></a>“表名”</span>参数中指定的表，然后再重新创建该表。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="19.380000000000003%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275481_p20939525115613"><a name="zh-cn_topic_0108275481_p20939525115613"></a><a name="zh-cn_topic_0108275481_p20939525115613"></a>不自动创建</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275481_row11687830163953"><td class="cellrowborder" valign="top" width="18.28%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275481_p23518636161524"><a name="zh-cn_topic_0108275481_p23518636161524"></a><a name="zh-cn_topic_0108275481_p23518636161524"></a>表名</p>
</td>
<td class="cellrowborder" valign="top" width="62.34%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275481_p17984995155931"><a name="zh-cn_topic_0108275481_p17984995155931"></a><a name="zh-cn_topic_0108275481_p17984995155931"></a>输入或选择写入数据的目标表名。</p>
<p id="zh-cn_topic_0108275481_p63592058163953"><a name="zh-cn_topic_0108275481_p63592058163953"></a><a name="zh-cn_topic_0108275481_p63592058163953"></a>单击输入框后面的按钮可进入表的选择界面。</p>
<p id="zh-cn_topic_0108275481_p1210244910548"><a name="zh-cn_topic_0108275481_p1210244910548"></a><a name="zh-cn_topic_0108275481_p1210244910548"></a>该参数支持配置为时间宏变量，且一个路径名中可以有多个宏定义变量。使用时间宏变量和定时任务配合，可以实现定期同步新增数据，详细说明请参见<a href="https://support.huaweicloud.com/bestpractice-dgc/dgc_05_0006.html" target="_blank" rel="noopener noreferrer">使用时间宏变量完成增量同步</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="19.380000000000003%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275481_p50683068163953"><a name="zh-cn_topic_0108275481_p50683068163953"></a><a name="zh-cn_topic_0108275481_p50683068163953"></a>TBL_X</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275481_row43042085151531"><td class="cellrowborder" valign="top" width="18.28%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275481_p21324079151542"><a name="zh-cn_topic_0108275481_p21324079151542"></a><a name="zh-cn_topic_0108275481_p21324079151542"></a>导入前清空数据</p>
</td>
<td class="cellrowborder" valign="top" width="62.34%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108275481_p348084512021"><a name="zh-cn_topic_0108275481_p348084512021"></a><a name="zh-cn_topic_0108275481_p348084512021"></a>选择目的端表中数据的处理方式：<a name="zh-cn_topic_0108275481_ua1819b93796044cd9f46f9dfb3e78f6b"></a><a name="zh-cn_topic_0108275481_ua1819b93796044cd9f46f9dfb3e78f6b"></a><ul id="zh-cn_topic_0108275481_ua1819b93796044cd9f46f9dfb3e78f6b"><li>是：任务启动前会清除目标表中数据。</li><li>否：导入前不清空目标表中的数据，如果选<span class="parmvalue" id="zh-cn_topic_0108275481_p47d3026f5a84445ebd15d358a7cc2720"><a name="zh-cn_topic_0108275481_p47d3026f5a84445ebd15d358a7cc2720"></a><a name="zh-cn_topic_0108275481_p47d3026f5a84445ebd15d358a7cc2720"></a>“否”</span>且表中有数据，则数据会追加到已有的表中。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="19.380000000000003%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275481_p23412518151542"><a name="zh-cn_topic_0108275481_p23412518151542"></a><a name="zh-cn_topic_0108275481_p23412518151542"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275481_row11284228135717"><td class="cellrowborder" valign="top" width="18.28%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275481_p1628472814572"><a name="zh-cn_topic_0108275481_p1628472814572"></a><a name="zh-cn_topic_0108275481_p1628472814572"></a>待清空分区</p>
</td>
<td class="cellrowborder" valign="top" width="62.34%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275481_p6622439171414"><a name="zh-cn_topic_0108275481_p6622439171414"></a><a name="zh-cn_topic_0108275481_p6622439171414"></a>“导入前清空数据”设置为“是”时，呈现此参数。</p>
<p id="zh-cn_topic_0108275481_p196521522121320"><a name="zh-cn_topic_0108275481_p196521522121320"></a><a name="zh-cn_topic_0108275481_p196521522121320"></a>填写待清空分区信息后，表示清空该分区的数据。</p>
</td>
<td class="cellrowborder" valign="top" width="19.380000000000003%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275481_p1368112410119"><a name="zh-cn_topic_0108275481_p1368112410119"></a><a name="zh-cn_topic_0108275481_p1368112410119"></a>单分区：year=2020,location=sun;</p>
<p id="zh-cn_topic_0108275481_p1017720191219"><a name="zh-cn_topic_0108275481_p1017720191219"></a><a name="zh-cn_topic_0108275481_p1017720191219"></a>多分区：['year=2020,location=sun', 'year=2021,location=earth'].</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：** 
>1.  Hive作为目的端时，会自动创建存储格式为ORC的表。
>2.  Hive作为迁移的目的时，如果存储格式为Textfile，在Hive创建表的语句中需要显式指定分隔符。例如：
>    ```
>    CREATE TABLE csv_tbl(
>    smallint_value smallint,
>    tinyint_value tinyint,
>    int_value int,
>    bigint_value bigint,
>    float_value float,
>    double_value double,
>    decimal_value decimal(9, 7),
>    timestmamp_value timestamp,
>    date_value date,
>    varchar_value varchar(100),
>    string_value string,
>    char_value char(20),
>    boolean_value boolean,
>    binary_value binary,
>    varchar_null varchar(100),
>    string_null string,
>    char_null char(20),
>    int_null int
>    )
>    ROW FORMAT SERDE 'org.apache.hadoop.hive.serde2.OpenCSVSerde'
>    WITH SERDEPROPERTIES (
>    "separatorChar" = "\t",
>    "quoteChar"     = "'",
>    "escapeChar"    = "\\"
>    )
>    STORED AS TEXTFILE;
>    ```

