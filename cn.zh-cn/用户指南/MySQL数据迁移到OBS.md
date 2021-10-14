# MySQL数据迁移到OBS<a name="dgc_01_0100"></a>

## 操作场景<a name="zh-cn_topic_0284710796_section2353196237"></a>

CDM支持表到文件类数据的迁移，本章节以MySQL--\>OBS为例，介绍如何通过CDM将表数据迁移到文件中。流程如下：

1.  [创建CDM集群并绑定EIP](#zh-cn_topic_0284710796_section1596917553011)
2.  [创建MySQL连接](#zh-cn_topic_0284710796_section4972205516016)
3.  [创建OBS连接](#zh-cn_topic_0284710796_section5774720191611)
4.  [创建迁移作业](#zh-cn_topic_0284710796_section119151411712)

## 前提条件<a name="zh-cn_topic_0284710796_section563405015518"></a>

-   已获取OBS的访问域名、端口，以及AK、SK。
-   已获取连接MySQL数据库的IP地址、端口、数据库名称、用户名、密码，且该用户拥有MySQL数据库的读写权限。
-   用户已参考[管理驱动](管理驱动.md#dgc_01_0132)，上传了MySQL数据库驱动。

## 创建CDM集群并绑定EIP<a name="zh-cn_topic_0284710796_section1596917553011"></a>

1.  如果是独立CDM服务，参考[创建集群](https://support.huaweicloud.com/usermanual-cdm/cdm_01_0018.html)创建CDM集群；如果是作为DGC服务CDM组件使用，参考[创建集群](https://support.huaweicloud.com/usermanual-dgc/dgc_01_0576.html)创建CDM集群。

    关键配置如下：

    CDM集群的规格，按待迁移的数据量选择，一般选择cdm.medium即可，满足大部分迁移场景。

2.  CDM集群创建完成后，选择集群操作列的“绑定弹性IP“，CDM通过EIP访问MySQL。

    **图 1**  集群列表<a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_fig570312018444"></a>  
    ![](figures/集群列表.png "集群列表")

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >如果用户对本地数据源的访问通道做了SSL加密，则CDM无法通过弹性IP连接数据源。


## 创建MySQL连接<a name="zh-cn_topic_0284710796_section4972205516016"></a>

1.  在集群管理界面，单击集群后的“作业管理“，选择“连接管理  \>  新建连接“，进入连接器类型的选择界面，如[图2](#zh-cn_topic_0284710796_zh-cn_topic_0111325168_fig15373426133913)所示。

    **图 2**  选择连接器类型<a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_fig15373426133913"></a>  
    ![](figures/选择连接器类型.png "选择连接器类型")

2.  选择“MySQL“后单击“下一步“，配置MySQL连接的参数。

    **图 3**  创建MySQL连接<a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_fig17438459415"></a>  
    ![](figures/创建MySQL连接-8.png "创建MySQL连接-8")

    单击“显示高级属性“可查看更多可选参数，具体请参见[配置关系数据库连接](配置关系数据库连接.md#dgc_01_0044)。这里保持默认，必填参数如[表1](#zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_table5321744015490)所示。

    **表 1**  MySQL连接参数

    <a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_table5321744015490"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_row185605615490"><th class="cellrowborder" valign="top" width="21.39%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p3088488815490"><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p3088488815490"></a><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p3088488815490"></a>参数名</p>
    </th>
    <th class="cellrowborder" valign="top" width="46.01%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1864797615490"><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1864797615490"></a><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1864797615490"></a>说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="32.6%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p12195902165556"><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p12195902165556"></a><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p12195902165556"></a>取值样例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_row6448267615421"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p5571423915421"><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p5571423915421"></a><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p5571423915421"></a>名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1655951515421"><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1655951515421"></a><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1655951515421"></a>输入便于记忆和区分的连接名称。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p6625233515421"><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p6625233515421"></a><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p6625233515421"></a>mysqllink</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_row23645714155554"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p36254680155554"><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p36254680155554"></a><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p36254680155554"></a>数据库服务器</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p57055815164650"><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p57055815164650"></a><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p57055815164650"></a>MySQL数据库的IP地址或域名。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p54006514165556"><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p54006514165556"></a><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p54006514165556"></a>192.168.1.110</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_row35721234155558"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p7738819155558"><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p7738819155558"></a><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p7738819155558"></a>端口</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p44462215165646"><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p44462215165646"></a><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p44462215165646"></a>MySQL数据库的端口。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p44954710165556"><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p44954710165556"></a><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p44954710165556"></a>3306</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_row58054787162632"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p4817321162632"><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p4817321162632"></a><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p4817321162632"></a>数据库名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p23569444165647"><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p23569444165647"></a><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p23569444165647"></a>MySQL数据库的名称。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p22858665165556"><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p22858665165556"></a><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p22858665165556"></a>sqoop</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_row121116115490"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p3099525315490"><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p3099525315490"></a><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p3099525315490"></a>用户名</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p2758753215490"><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p2758753215490"></a><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p2758753215490"></a>拥有MySQL数据库的读、写和删除权限的用户。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p14053644165556"><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p14053644165556"></a><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p14053644165556"></a>admin</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_row4576104015490"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1565673415490"><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1565673415490"></a><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1565673415490"></a>密码</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p6023590815490"><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p6023590815490"></a><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p6023590815490"></a>用户的密码。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p44559445165556"><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p44559445165556"></a><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p44559445165556"></a>-</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_row117692617437"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p18773153334318"><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p18773153334318"></a><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p18773153334318"></a>使用Agent</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p877373317439"><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p877373317439"></a><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p877373317439"></a>是否选择通过Agent从源端提取数据。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1977311335439"><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1977311335439"></a><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1977311335439"></a>是</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_row1178882914433"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p2077320332430"><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p2077320332430"></a><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p2077320332430"></a>Agent</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1877310336437"><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1877310336437"></a><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1877310336437"></a>单击<span class="uicontrol" id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_uicontrol1773183344318"><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_uicontrol1773183344318"></a><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_uicontrol1773183344318"></a>“选择”</span>，选择<a href="管理Agent.md#zh-cn_topic_0207402273_zh-cn_topic_0191978474_section1072083564713">连接Agent</a>中已创建的Agent。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p16773533154317"><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p16773533154317"></a><a name="zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p16773533154317"></a>-</p>
    </td>
    </tr>
    </tbody>
    </table>

3.  单击“保存“回到连接管理界面。

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >如果保存时出错，一般是由于MySQL数据库的安全设置问题，需要设置允许CDM集群的EIP访问MySQL数据库。


## 创建OBS连接<a name="zh-cn_topic_0284710796_section5774720191611"></a>

1.  在连接管理界面单击“新建连接“，连接器类型选择“对象存储服务（OBS）“后，单击“下一步“配置OBS连接参数，如[图4](#zh-cn_topic_0284710796_zh-cn_topic_0123434187_fig27331126173315)所示。

    -   名称：用户自定义连接名称，例如“obslink“。
    -   OBS服务器、端口：配置为OBS实际的地址信息。
    -   访问标识（AK）、密钥（SK）：登录OBS的AK、SK。

    **图 4**  创建OBS连接<a name="zh-cn_topic_0284710796_zh-cn_topic_0123434187_fig27331126173315"></a>  
    ![](figures/创建OBS连接.png "创建OBS连接")

2.  单击“保存“回到连接管理界面。

## 创建迁移作业<a name="zh-cn_topic_0284710796_section119151411712"></a>

1.  选择“表/文件迁移  \>  新建作业“，开始创建从MySQL导出数据到OBS的任务。

    **图 5**  创建MySQL到OBS的迁移任务<a name="zh-cn_topic_0284710796_fig2095091110254"></a>  
    ![](figures/创建MySQL到OBS的迁移任务.jpg "创建MySQL到OBS的迁移任务")

    -   作业名称：用户自定义便于记忆、区分的任务名称。
    -   源端作业配置
        -   源连接名称：选择[创建MySQL连接](#zh-cn_topic_0284710796_section4972205516016)中的“mysqllink“。
        -   使用SQL语句：否。
        -   模式或表空间：待抽取数据的模式或表空间名称。。
        -   表名：要抽取的表名。
        -   其他可选参数一般情况下保持默认即可，详细说明请参见[配置关系数据库源端参数](配置关系数据库源端参数.md#dgc_01_0054)。

    -   目的端作业配置
        -   目的连接名称：选择[创建OBS连接](#zh-cn_topic_0284710796_section5774720191611)中的“obslink“。
        -   桶名：待迁移数据的桶。
        -   写入目录：写入数据到OBS服务器的目录。
        -   文件格式：迁移数据表到文件时，文件格式选择“CSV格式“。
        -   高级属性里的可选参数一般情况下保持默认既可，详细说明请参见[配置OBS目的端参数](配置OBS目的端参数.md#dgc_01_0062)。

2.  单击“下一步“进入字段映射界面，CDM会自动匹配源和目的字段，如[图6](#zh-cn_topic_0284710796_fig231883016327)所示。

    -   如果字段映射顺序不匹配，可通过拖拽字段调整。
    -   CDM的表达式已经预置常用字符串、日期、数值等类型的字段内容转换，详细请参见[字段转换](https://support.huaweicloud.com/bestpractice-dgc/dgc_05_0012.html)。

    **图 6**  表到文件的字段映射<a name="zh-cn_topic_0284710796_fig231883016327"></a>  
    ![](figures/表到文件的字段映射.jpg "表到文件的字段映射")

3.  单击“下一步“配置任务参数，一般情况下全部保持默认即可。

    该步骤用户可以配置如下可选功能：

    -   作业失败重试：如果作业执行失败，可选择是否自动重试，这里保持默认值“不重试“。
    -   作业分组：选择作业所属的分组，默认分组为“DEFAULT“。在CDM“作业管理“界面，支持作业分组显示、按组批量启动作业、按分组导出作业等操作。
    -   是否定时执行：如果需要配置作业定时自动执行，请参见[配置定时任务](配置定时任务.md#dgc_01_0082)。这里保持默认值“否“。
    -   抽取并发数：设置同时执行的抽取任务数。CDM支持并发抽取MySQL数据，如果源表配置了索引，可调大抽取并发数提升迁移速率。
    -   是否写入脏数据：如果需要将作业执行过程中处理失败的数据、或者被清洗过滤掉的数据写入OBS中，以便后面查看，可通过该参数配置，写入脏数据前需要先配置好OBS连接。针对文件到表类迁移的数据，建议配置写入脏数据。
    -   作业运行完是否删除：这里保持默认值“不删除“。根据使用场景，也可配置为“删除”，防止迁移作业堆积。

4.  单击“保存并运行“，回到作业管理界面，在作业管理界面可查看作业执行进度和结果。
5.  作业执行成功后，单击作业操作列的“历史记录“，可查看该作业的历史执行记录、读取和写入的统计数据。

    在历史记录界面单击“日志“，可查看作业的日志信息。


