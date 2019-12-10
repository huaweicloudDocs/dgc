# MySQL数据库迁移到云上MRS Hive分区表<a name="dayu_01_0092"></a>

[MapReduce服务](https://www.huaweicloud.com/product/mrs.html)（MapReduce Service，简称MRS）是华为云提供的企业级大数据集群云服务，里面包含HDFS、Hive、Spark等组件，适用于企业海量数据分析。

其中Hive提供类SQL查询语言，帮助用户对大规模的数据进行提取、转换和加载，即通常所称的ETL（Extraction，Transformation，and Loading）操作。对庞大的数据集查询需要耗费大量的时间去处理，在许多场景下，可以通过建立Hive分区方法减少每一次扫描的总数据量，这种做法可以显著地改善性能。

Hive的分区使用HDFS的子目录功能实现，每一个子目录包含了分区对应的列名和每一列的值。当分区很多时，会有很多HDFS子目录，如果不依赖工具，将外部数据加载到Hive表各分区不是一件容易的事情。云数据迁移服务（CDM）可以请轻松将外部数据源（关系数据库、对象存储服务、文件系统服务等）加载到Hive分区表。

下面使用CDM将MySQL数据导入到MRS Hive分区表为例进行介绍。

## 操作场景<a name="zh-cn_topic_0111325168_section848194854517"></a>

假设MySQL上有一张表trip\_data，保存了自行车骑行记录，里面有起始时间、结束时间，起始站点、结束站点、骑手ID等信息，trip\_data表字段定义如[图1](#zh-cn_topic_0111325168_fig5406153795610)所示。

**图 1**  MySQL表字段<a name="zh-cn_topic_0111325168_fig5406153795610"></a>  
![](figures/MySQL表字段.png "MySQL表字段")

使用CDM将MySQL中的表trip\_data导入到MRS Hive分区表，流程如下：

1.  [在MRS Hive上创建Hive分区表](#zh-cn_topic_0111325168_section143383811272)
2.  [创建CDM集群并绑定EIP](#zh-cn_topic_0111325168_section563314494359)
3.  [创建MySQL连接](#zh-cn_topic_0111325168_section459563891734)
4.  [创建Hive连接](#zh-cn_topic_0111325168_section209397834812)
5.  [创建迁移作业](#zh-cn_topic_0111325168_section1821596484)

## 前提条件<a name="zh-cn_topic_0111325168_section425442671733"></a>

-   已经购买了MRS。
-   拥有EIP配额。
-   已获取连接MySQL数据库的IP地址、端口、数据库名称、用户名、密码，且该用户拥有MySQL数据库的读写权限。

## 在MRS Hive上创建Hive分区表<a name="zh-cn_topic_0111325168_section143383811272"></a>

在MRS的Hive上使用下面SQL语句创建一张Hive分区表，表名与MySQL上的表trip\_data一致，且Hive表比MySQL表多建三个字段y、ym、ymd，作为Hive的分区字段。SQL语句如下：

```
create table trip_data(TripID int,Duration int,StartDate timestamp,StartStation varchar(64),StartTerminal int,EndDate timestamp,EndStation varchar(64),EndTerminal int,Bike int,SubscriberType varchar(32),ZipCodev varchar(10))partitioned by (y int,ym int,ymd int);
```

>![](public_sys-resources/icon-note.gif) **说明：**   
>Hive表trip\_data有三个分区字段：骑行起始时间的年、骑行起始时间的年月、骑行起始时间的年月日，例如一条骑行记录的起始时间为2018/5/11 9:40，那么这条记录会保存在分区trip\_data/2018/201805/20180511下面。对trip\_data进行按时间维度统计汇总时，只需要对局部数据扫描，大大提升性能。  

## 创建CDM集群并绑定EIP<a name="zh-cn_topic_0111325168_section563314494359"></a>

1.  创建CDM集群，具体操作请参见[创建集群](创建集群.md)。关键配置如下：
    -   CDM集群的规格，按待迁移的数据量选择，一般选择cdm.medium即可，满足大部分迁移场景。
    -   CDM集群所在VPC、子网、安全组，选择与MRS集群所在的网络一致。

2.  CDM集群创建完成后，选择集群操作列的“绑定弹性IP“，CDM通过EIP访问MySQL。

    **图 2**  绑定EIP<a name="zh-cn_topic_0111325168_fig570312018444"></a>  
    ![](figures/绑定EIP-0.png "绑定EIP-0")

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >如果用户对本地数据源的访问通道做了SSL加密，则CDM无法通过弹性IP连接数据源。  


## 创建MySQL连接<a name="zh-cn_topic_0111325168_section459563891734"></a>

1.  在集群管理界面，单击集群后的“作业管理“，选择“连接管理  \>  新建连接“，进入连接器类型的选择界面，如[图3](#zh-cn_topic_0111325168_fig15373426133913)所示。

    **图 3**  选择连接器类型<a name="zh-cn_topic_0111325168_fig15373426133913"></a>  
    ![](figures/选择连接器类型.png "选择连接器类型")

2.  选择“MySQL“后单击“下一步“，配置MySQL连接的参数。

    **图 4**  创建MySQL连接5<a name="zh-cn_topic_0108275298_fig32415531174450"></a>  
    ![](figures/创建MySQL连接5.png "创建MySQL连接5")

    单击“显示高级属性“可查看更多可选参数，具体请参见[配置关系数据库连接](配置关系数据库连接.md)。这里保持默认，必填参数如[表1](#zh-cn_topic_0108275298_table5321744015490)所示。

    **表 1**  MySQL连接参数

    <a name="zh-cn_topic_0108275298_table5321744015490"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0108275298_row185605615490"><th class="cellrowborder" valign="top" width="21.39%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108275298_p3088488815490"><a name="zh-cn_topic_0108275298_p3088488815490"></a><a name="zh-cn_topic_0108275298_p3088488815490"></a>参数名</p>
    </th>
    <th class="cellrowborder" valign="top" width="46.01%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108275298_p1864797615490"><a name="zh-cn_topic_0108275298_p1864797615490"></a><a name="zh-cn_topic_0108275298_p1864797615490"></a>说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="32.6%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108275298_p12195902165556"><a name="zh-cn_topic_0108275298_p12195902165556"></a><a name="zh-cn_topic_0108275298_p12195902165556"></a>取值样例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0108275298_row6448267615421"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275298_p5571423915421"><a name="zh-cn_topic_0108275298_p5571423915421"></a><a name="zh-cn_topic_0108275298_p5571423915421"></a>名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275298_p1655951515421"><a name="zh-cn_topic_0108275298_p1655951515421"></a><a name="zh-cn_topic_0108275298_p1655951515421"></a>输入便于记忆和区分的连接名称。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275298_p6625233515421"><a name="zh-cn_topic_0108275298_p6625233515421"></a><a name="zh-cn_topic_0108275298_p6625233515421"></a>mysqllink</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108275298_row23645714155554"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275298_p36254680155554"><a name="zh-cn_topic_0108275298_p36254680155554"></a><a name="zh-cn_topic_0108275298_p36254680155554"></a>数据库服务器</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275298_p57055815164650"><a name="zh-cn_topic_0108275298_p57055815164650"></a><a name="zh-cn_topic_0108275298_p57055815164650"></a>MySQL数据库的IP地址或域名。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275298_p54006514165556"><a name="zh-cn_topic_0108275298_p54006514165556"></a><a name="zh-cn_topic_0108275298_p54006514165556"></a>192.168.0.1</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108275298_row35721234155558"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275298_p7738819155558"><a name="zh-cn_topic_0108275298_p7738819155558"></a><a name="zh-cn_topic_0108275298_p7738819155558"></a>端口</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275298_p44462215165646"><a name="zh-cn_topic_0108275298_p44462215165646"></a><a name="zh-cn_topic_0108275298_p44462215165646"></a>MySQL数据库的端口。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275298_p44954710165556"><a name="zh-cn_topic_0108275298_p44954710165556"></a><a name="zh-cn_topic_0108275298_p44954710165556"></a>3306</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108275298_row58054787162632"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275298_p4817321162632"><a name="zh-cn_topic_0108275298_p4817321162632"></a><a name="zh-cn_topic_0108275298_p4817321162632"></a>数据库名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275298_p23569444165647"><a name="zh-cn_topic_0108275298_p23569444165647"></a><a name="zh-cn_topic_0108275298_p23569444165647"></a>MySQL数据库的名称。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275298_p22858665165556"><a name="zh-cn_topic_0108275298_p22858665165556"></a><a name="zh-cn_topic_0108275298_p22858665165556"></a>sqoop</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108275298_row121116115490"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275298_p3099525315490"><a name="zh-cn_topic_0108275298_p3099525315490"></a><a name="zh-cn_topic_0108275298_p3099525315490"></a>用户名</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275298_p2758753215490"><a name="zh-cn_topic_0108275298_p2758753215490"></a><a name="zh-cn_topic_0108275298_p2758753215490"></a>拥有MySQL数据库的读、写和删除权限的用户。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275298_p14053644165556"><a name="zh-cn_topic_0108275298_p14053644165556"></a><a name="zh-cn_topic_0108275298_p14053644165556"></a>admin</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108275298_row4576104015490"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275298_p1565673415490"><a name="zh-cn_topic_0108275298_p1565673415490"></a><a name="zh-cn_topic_0108275298_p1565673415490"></a>密码</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275298_p6023590815490"><a name="zh-cn_topic_0108275298_p6023590815490"></a><a name="zh-cn_topic_0108275298_p6023590815490"></a>用户的密码。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275298_p44559445165556"><a name="zh-cn_topic_0108275298_p44559445165556"></a><a name="zh-cn_topic_0108275298_p44559445165556"></a>-</p>
    </td>
    </tr>
    </tbody>
    </table>

3.  单击“保存“回到连接管理界面。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >如果保存时出错，一般是由于MySQL数据库的安全设置问题，需要设置允许CDM集群的EIP访问MySQL数据库。  


## 创建Hive连接<a name="zh-cn_topic_0111325168_section209397834812"></a>

1.  在连接管理界面，单击“新建连接“，连接器类型选择“MRS Hive“。
2.  单击“下一步“配置Hive连接参数，如[图5](#zh-cn_topic_0111325168_fig1219924816)所示。

    **图 5**  创建Hive连接<a name="zh-cn_topic_0111325168_fig1219924816"></a>  
    ![](figures/创建Hive连接.png "创建Hive连接")

    各参数说明如[表2](#zh-cn_topic_0111325168_table6441152003419)所示，需要您根据实际情况配置。

    **表 2**  Hive连接参数

    <a name="zh-cn_topic_0111325168_table6441152003419"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0108618545_row15441220123417"><th class="cellrowborder" valign="top" width="16.72%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108618545_p18441202093413"><a name="zh-cn_topic_0108618545_p18441202093413"></a><a name="zh-cn_topic_0108618545_p18441202093413"></a>参数名</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.1%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108618545_p1544152053412"><a name="zh-cn_topic_0108618545_p1544152053412"></a><a name="zh-cn_topic_0108618545_p1544152053412"></a>说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.18%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108618545_p4441112010341"><a name="zh-cn_topic_0108618545_p4441112010341"></a><a name="zh-cn_topic_0108618545_p4441112010341"></a>取值样例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0108618545_row11441182012346"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p4456620113417"><a name="zh-cn_topic_0108618545_p4456620113417"></a><a name="zh-cn_topic_0108618545_p4456620113417"></a>名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p6456820183418"><a name="zh-cn_topic_0108618545_p6456820183418"></a><a name="zh-cn_topic_0108618545_p6456820183418"></a>连接的名称，根据连接的数据源类型，用户可自定义便于记忆、区分的连接名。</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p13456112023418"><a name="zh-cn_topic_0108618545_p13456112023418"></a><a name="zh-cn_topic_0108618545_p13456112023418"></a>hivelink</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108618545_row2456122053415"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p13456172019344"><a name="zh-cn_topic_0108618545_p13456172019344"></a><a name="zh-cn_topic_0108618545_p13456172019344"></a>Manager IP</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p1345602010341"><a name="zh-cn_topic_0108618545_p1345602010341"></a><a name="zh-cn_topic_0108618545_p1345602010341"></a>MRS Manager的IP地址，可以单击输入框后的<span class="uicontrol" id="zh-cn_topic_0108618545_zh-cn_topic_0108275286_uicontrol926725316310"><a name="zh-cn_topic_0108618545_zh-cn_topic_0108275286_uicontrol926725316310"></a><a name="zh-cn_topic_0108618545_zh-cn_topic_0108275286_uicontrol926725316310"></a>“选择”</span>来选定已创建的MRS集群，CDM会自动填充下面的鉴权参数。</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p13456420143418"><a name="zh-cn_topic_0108618545_p13456420143418"></a><a name="zh-cn_topic_0108618545_p13456420143418"></a>127.0.0.1</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108618545_row4332334184015"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p06421125396"><a name="zh-cn_topic_0108618545_p06421125396"></a><a name="zh-cn_topic_0108618545_p06421125396"></a>认证类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108618545_p3642111243916"><a name="zh-cn_topic_0108618545_p3642111243916"></a><a name="zh-cn_topic_0108618545_p3642111243916"></a>访问MRS的认证类型：<a name="zh-cn_topic_0108618545_zh-cn_topic_0108275286_ul552304715358"></a><a name="zh-cn_topic_0108618545_zh-cn_topic_0108275286_ul552304715358"></a><ul id="zh-cn_topic_0108618545_zh-cn_topic_0108275286_ul552304715358"><li>SIMPLE：非安全模式选择Simple鉴权。</li><li>KERBEROS：安全模式选择Kerberos鉴权。</li></ul>
    </div>
    </td>
    <td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p76428123396"><a name="zh-cn_topic_0108618545_p76428123396"></a><a name="zh-cn_topic_0108618545_p76428123396"></a>SIMPLE</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108618545_row16456152011347"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p94561620113420"><a name="zh-cn_topic_0108618545_p94561620113420"></a><a name="zh-cn_topic_0108618545_p94561620113420"></a>用户名</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p64738206349"><a name="zh-cn_topic_0108618545_p64738206349"></a><a name="zh-cn_topic_0108618545_p64738206349"></a>选择KERBEROS鉴权时，需要配置MRS Manager的用户名和密码。</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p3473020113416"><a name="zh-cn_topic_0108618545_p3473020113416"></a><a name="zh-cn_topic_0108618545_p3473020113416"></a>cdm</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108618545_row20456320123419"><td class="cellrowborder" valign="top" width="16.72%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108618545_p647322020346"><a name="zh-cn_topic_0108618545_p647322020346"></a><a name="zh-cn_topic_0108618545_p647322020346"></a>密码</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.1%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108618545_p174737206340"><a name="zh-cn_topic_0108618545_p174737206340"></a><a name="zh-cn_topic_0108618545_p174737206340"></a>访问MRS Manager的用户密码。</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108618545_p204731920153414"><a name="zh-cn_topic_0108618545_p204731920153414"></a><a name="zh-cn_topic_0108618545_p204731920153414"></a>-</p>
    </td>
    </tr>
    </tbody>
    </table>

3.  单击“保存“回到连接管理界面。

## 创建迁移作业<a name="zh-cn_topic_0111325168_section1821596484"></a>

1.  选择“表/文件迁移  \>  新建作业“，开始创建数据迁移任务，如[图6](#zh-cn_topic_0111325168_fig125979433490)所示。

    **图 6**  创建MySQL到Hive的迁移任务<a name="zh-cn_topic_0111325168_fig125979433490"></a>  
    ![](figures/创建MySQL到Hive的迁移任务.png "创建MySQL到Hive的迁移任务")

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >“导入前清空数据“选“是“，这样每次导入前，会将之前已经导入到Hive表的数据清空。  

2.  作业参数配置完成后，单击“下一步“，进入字段映射界面，如[图7](#zh-cn_topic_0111325168_fig1461204384916)所示。

    映射MySQL表和Hive表字段，Hive表比MySQL表多三个字段y、ym、ymd，即是Hive的分区字段。由于没有源表字段直接对应，需要配置表达式从源表的StartDate字段抽取。

    **图 7**  Hive字段映射<a name="zh-cn_topic_0111325168_fig1461204384916"></a>  
    ![](figures/Hive字段映射.png "Hive字段映射")

3.  单击![](figures/5-1字段转换小图标02-0-1.png)进入转换器列表界面，再选择“新建转换器  \>  表达式转换“，如[图8](#zh-cn_topic_0111325168_fig261294344916)所示。

    y、ym、ymd字段的表达式分别配置如下：

    **DateUtils.format\(DateUtils.parseDate\(row\[2\],"yyyy-MM-dd HH:mm:ss.SSS"\),"yyyy"\)**

    **DateUtils.format\(DateUtils.parseDate\(row\[2\],"yyyy-MM-dd HH:mm:ss.SSS"\),"yyyyMM"\)**

    **DateUtils.format\(DateUtils.parseDate\(row\[2\],"yyyy-MM-dd HH:mm:ss.SSS"\),"yyyyMMdd"\)**

    **图 8**  配置表达式<a name="zh-cn_topic_0111325168_fig261294344916"></a>  
    ![](figures/配置表达式.png "配置表达式")

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >CDM的表达式已经预置常用字符串、日期、数值等类型的字段内容转换，详情请参见[字段转换](字段转换.md)。  

4.  单击“下一步“配置任务参数，一般情况下全部保持默认即可。

    该步骤用户可以配置如下可选功能：

    -   作业失败重试：如果作业执行失败，可选择是否自动重试，这里保持默认值“不重试“。
    -   作业分组：选择作业所属的分组，默认分组为“DEFAULT“。在CDM“作业管理“界面，支持作业分组显示、按组批量启动作业、按分组导出作业等操作。
    -   是否定时执行：如果需要配置作业定时自动执行，请参见[配置定时任务](配置定时任务.md)。这里保持默认值“否“。
    -   抽取并发数：设置同时执行的抽取任务数。这里保持默认值“1“。
    -   是否写入脏数据：如果需要将作业执行过程中处理失败的数据、或者被清洗过滤掉的数据写入OBS中，以便后面查看，可通过该参数配置，写入脏数据前需要先配置好OBS连接。这里保持默认值“否“即可，不记录脏数据。
    -   作业运行完是否删除：这里保持默认值“不删除“。

5.  单击“保存并运行“，回到作业管理界面，在作业管理界面可查看作业执行进度和结果。
6.  作业执行成功后，单击作业操作列的“历史记录“，可查看该作业的历史执行记录、读取和写入的统计数据。

    在历史记录界面单击“日志“，可查看作业的日志信息。


