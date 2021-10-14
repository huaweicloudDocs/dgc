# Oracle数据迁移到DWS<a name="dgc_01_0133"></a>

## 操作场景<a name="zh-cn_topic_0000001193296031_section21020958143223"></a>

云搜索服务（Cloud Search Service）为用户提供结构化、非结构化文本的多条件检索、统计、报表，本章节介绍如何通过CDM将数据从Oracle迁移到云搜索服务中，流程如下：

这里以数据仓库服务（Data Warehouse Service，简称DWS）为例，介绍如何使用CDM将Oracle数据迁移到DWS，流程如下：

1.  [创建CDM集群并绑定EIP](#zh-cn_topic_0000001193296031_section3548195211)
2.  [创建Oracle连接](#zh-cn_topic_0000001193296031_section1136440015)
3.  [创建DWS连接](#zh-cn_topic_0000001193296031_section796691518119)
4.  [创建迁移作业](#zh-cn_topic_0000001193296031_section383292919118)

## 前提条件<a name="zh-cn_topic_0000001193296031_section5787168294234"></a>

-   已购买DWS集群，并且已获取DWS数据库的IP地址、端口、数据库名称、用户名、密码，且该用户拥有DWS数据库的读、写和删除权限。
-   已获取Oracle数据库的IP、数据库名、用户名和密码。
-   如果Oracle数据库是在本地数据中心或第三方云上，需要确保Oracle可通过公网IP访问，或者已经建立好了企业内部数据中心到华为云的VPN通道或专线。
-   用户已参考[管理驱动](管理驱动.md#dgc_01_0132)，上传了Oracle数据库驱动。

## 创建CDM集群并绑定EIP<a name="zh-cn_topic_0000001193296031_section3548195211"></a>

1.  如果是独立CDM服务，参考[创建集群](https://support.huaweicloud.com/usermanual-cdm/cdm_01_0018.html)创建CDM集群；如果是作为DGC服务CDM组件使用，参考[创建集群](https://support.huaweicloud.com/usermanual-dgc/dgc_01_0576.html)创建CDM集群。

    关键配置如下：

    -   CDM集群的规格，按待迁移的数据量选择，一般选择cdm.medium即可，满足大部分迁移场景。
    -   CDM集群所在VPC、子网、安全组，选择与DWS集群所在的网络一致。
    -   如果安全控制原因不能使用相同子网和安全组，那么需要确保安全组规则能允许CDM访问云搜索服务集群。

2.  CDM集群创建完成后，在集群管理界面选择“绑定弹性IP”，CDM通过EIP访问Oracle数据源。

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >如果用户对本地数据源的访问通道做了SSL加密，则CDM无法通过弹性IP连接数据源。


## 创建Oracle连接<a name="zh-cn_topic_0000001193296031_section1136440015"></a>

1.  单击CDM集群后的“作业管理“，进入作业管理界面，再选择“连接管理  \>  新建连接“，进入选择连接器类型的界面，如[图1](#zh-cn_topic_0000001193296031_zh-cn_topic_0108275298_fig13640155194015)所示。

    **图 1**  选择连接器类型<a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275298_fig13640155194015"></a>  
    ![](figures/选择连接器类型-9.png "选择连接器类型-9")

2.  连接器类型选择“Oracle“后单击“下一步“，配置Oracle连接参数，参数说明如[表1](#zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_table5321744015490)所示。

    **图 2**  创建Oracle连接<a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_fig17438459415"></a>  
    ![](figures/创建Oracle连接.png "创建Oracle连接")

    **表 1**  Oracle连接参数

    <a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_table5321744015490"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_row185605615490"><th class="cellrowborder" valign="top" width="21.39%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p3088488815490"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p3088488815490"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p3088488815490"></a>参数名</p>
    </th>
    <th class="cellrowborder" valign="top" width="46.01%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1864797615490"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1864797615490"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1864797615490"></a>说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="32.6%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p12195902165556"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p12195902165556"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p12195902165556"></a>取值样例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_row6448267615421"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p5571423915421"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p5571423915421"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p5571423915421"></a>名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1655951515421"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1655951515421"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1655951515421"></a>输入便于记忆和区分的连接名称。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p6625233515421"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p6625233515421"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p6625233515421"></a>oracle_link</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_row23645714155554"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p36254680155554"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p36254680155554"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p36254680155554"></a>数据库服务器</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p57055815164650"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p57055815164650"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p57055815164650"></a>数据库服务器域名或IP地址。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p54006514165556"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p54006514165556"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p54006514165556"></a>192.168.0.1</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_row35721234155558"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p7738819155558"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p7738819155558"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p7738819155558"></a>端口</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p44462215165646"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p44462215165646"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p44462215165646"></a>Oracle数据库的端口。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p44954710165556"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p44954710165556"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p44954710165556"></a>3306</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_row58054787162632"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p4817321162632"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p4817321162632"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p4817321162632"></a>数据库连接类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p23569444165647"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p23569444165647"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p23569444165647"></a>Oracle数据库连接类型。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p22858665165556"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p22858665165556"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p22858665165556"></a>Service Name</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001193296031_row16438152014579"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001193296031_p64381120135716"><a name="zh-cn_topic_0000001193296031_p64381120135716"></a><a name="zh-cn_topic_0000001193296031_p64381120135716"></a>数据库名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001193296031_p8438820165715"><a name="zh-cn_topic_0000001193296031_p8438820165715"></a><a name="zh-cn_topic_0000001193296031_p8438820165715"></a>要连接的数据库。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001193296031_p44384208577"><a name="zh-cn_topic_0000001193296031_p44384208577"></a><a name="zh-cn_topic_0000001193296031_p44384208577"></a>db_user</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_row121116115490"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p3099525315490"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p3099525315490"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p3099525315490"></a>用户名</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p2758753215490"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p2758753215490"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p2758753215490"></a>拥有Oracle数据库的读取权限的用户。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p14053644165556"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p14053644165556"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p14053644165556"></a>admin</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_row4576104015490"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1565673415490"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1565673415490"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1565673415490"></a>密码</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p6023590815490"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p6023590815490"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p6023590815490"></a>Oracle数据库的登录密码。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p44559445165556"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p44559445165556"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p44559445165556"></a>-</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_row117692617437"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p18773153334318"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p18773153334318"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p18773153334318"></a>使用Agent</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p877373317439"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p877373317439"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p877373317439"></a>是否选择通过Agent从源端提取数据。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1977311335439"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1977311335439"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1977311335439"></a>是</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001193296031_row243185692016"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275298_p2077320332430"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275298_p2077320332430"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275298_p2077320332430"></a>Agent</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275298_p1877310336437"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275298_p1877310336437"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275298_p1877310336437"></a>单击<span class="uicontrol" id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275298_uicontrol1773183344318"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275298_uicontrol1773183344318"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275298_uicontrol1773183344318"></a>“选择”</span>，选择<a href="管理Agent.md#zh-cn_topic_0207402273_zh-cn_topic_0191978474_section1072083564713">连接Agent</a>中已创建的Agent。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275298_p16773533154317"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275298_p16773533154317"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275298_p16773533154317"></a>-</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001193296031_row0403951155710"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001193296031_p0403205114574"><a name="zh-cn_topic_0000001193296031_p0403205114574"></a><a name="zh-cn_topic_0000001193296031_p0403205114574"></a>ORACLE版本</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001193296031_p194036517575"><a name="zh-cn_topic_0000001193296031_p194036517575"></a><a name="zh-cn_topic_0000001193296031_p194036517575"></a>默认使用最新版本驱动，若不兼容请尝试其他版本。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001193296031_p840355145714"><a name="zh-cn_topic_0000001193296031_p840355145714"></a><a name="zh-cn_topic_0000001193296031_p840355145714"></a>高于12.1</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001193296031_row198311582349"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001193296031_p6841581349"><a name="zh-cn_topic_0000001193296031_p6841581349"></a><a name="zh-cn_topic_0000001193296031_p6841581349"></a>一次请求行数</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001193296031_p684105863419"><a name="zh-cn_topic_0000001193296031_p684105863419"></a><a name="zh-cn_topic_0000001193296031_p684105863419"></a>指定每次请求获取的行数。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001193296031_p1784115893412"><a name="zh-cn_topic_0000001193296031_p1784115893412"></a><a name="zh-cn_topic_0000001193296031_p1784115893412"></a>1000</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001193296031_row753265813344"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001193296031_p153375816344"><a name="zh-cn_topic_0000001193296031_p153375816344"></a><a name="zh-cn_topic_0000001193296031_p153375816344"></a>连接属性</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001193296031_p8533158183416"><a name="zh-cn_topic_0000001193296031_p8533158183416"></a><a name="zh-cn_topic_0000001193296031_p8533158183416"></a>自定义连接属性。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001193296031_p353312586341"><a name="zh-cn_topic_0000001193296031_p353312586341"></a><a name="zh-cn_topic_0000001193296031_p353312586341"></a>useCompression=true</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001193296031_row1477817242359"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001193296031_p14778824153516"><a name="zh-cn_topic_0000001193296031_p14778824153516"></a><a name="zh-cn_topic_0000001193296031_p14778824153516"></a>引用符号</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001193296031_p4174143123613"><a name="zh-cn_topic_0000001193296031_p4174143123613"></a><a name="zh-cn_topic_0000001193296031_p4174143123613"></a>连接引用表名或列名时的分隔符号。默认为空。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001193296031_p1477819242350"><a name="zh-cn_topic_0000001193296031_p1477819242350"></a><a name="zh-cn_topic_0000001193296031_p1477819242350"></a>'</p>
    </td>
    </tr>
    </tbody>
    </table>

3.  单击“保存“回到连接管理界面。

## 创建DWS连接<a name="zh-cn_topic_0000001193296031_section796691518119"></a>

1.  在“连接管理“界面单击“新建连接“，连接器类型选择“数据仓库服务（DWS）“。
2.  单击“下一步“配置DWS连接参数，必填参数如[表2](#zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_table385644710314)所示，可选参数保持默认即可。

    **表 2**  DWS连接参数

    <a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_table385644710314"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_row19841847103118"><th class="cellrowborder" valign="top" width="21.39%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p1384114743120"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p1384114743120"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p1384114743120"></a>参数名</p>
    </th>
    <th class="cellrowborder" valign="top" width="46.01%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p3841204716313"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p3841204716313"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p3841204716313"></a>说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="32.6%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p18841164783118"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p18841164783118"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p18841164783118"></a>取值样例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_row20841154712312"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p13841547173116"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p13841547173116"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p13841547173116"></a>名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p78412047133115"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p78412047133115"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p78412047133115"></a>输入便于记忆和区分的连接名称。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p19841247193118"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p19841247193118"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p19841247193118"></a>dwslink</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_row19841194733113"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p1284104723114"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p1284104723114"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p1284104723114"></a>数据库服务器</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p15841184711314"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p15841184711314"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p15841184711314"></a>DWS数据库的IP地址或域名。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p18841104773115"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p18841104773115"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p18841104773115"></a>192.168.0.3</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_row984144713312"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p9841164773118"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p9841164773118"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p9841164773118"></a>端口</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p3841547123118"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p3841547123118"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p3841547123118"></a>DWS数据库的端口。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p15841204723116"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p15841204723116"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p15841204723116"></a>8000</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_row11841547133120"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p118419479311"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p118419479311"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p118419479311"></a>数据库名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p1484174713114"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p1484174713114"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p1484174713114"></a>DWS数据库的名称。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p1841547193111"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p1841547193111"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p1841547193111"></a>db_demo</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_row16841114716310"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p1984117474317"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p1984117474317"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p1984117474317"></a>用户名</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p17841144773116"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p17841144773116"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p17841144773116"></a>拥有DWS数据库的读、写和删除权限的用户。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p984124773118"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p984124773118"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p984124773118"></a>dbadmin</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_row98411347163117"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p13841194718313"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p13841194718313"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p13841194718313"></a>密码</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p12841347183118"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p12841347183118"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p12841347183118"></a>用户的密码。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p17841174714316"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p17841174714316"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p17841174714316"></a>-</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_row5426134013239"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p815422212356"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p815422212356"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p815422212356"></a>使用Agent</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p1615418228357"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p1615418228357"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p1615418228357"></a>是否选择通过Agent从源端提取数据。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p1415442293513"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p1415442293513"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p1415442293513"></a>是</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_row9800836192314"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p18412133418352"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p18412133418352"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p18412133418352"></a>Agent</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p5412193413515"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p5412193413515"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p5412193413515"></a>单击<span class="uicontrol" id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_uicontrol7592322128"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_uicontrol7592322128"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_uicontrol7592322128"></a>“选择”</span>，选择<a href="管理Agent.md#zh-cn_topic_0207402273_zh-cn_topic_0191978474_section1072083564713">连接Agent</a>中已创建的Agent。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p1241253413354"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p1241253413354"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p1241253413354"></a>-</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_row128561847143117"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p1284114723111"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p1284114723111"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p1284114723111"></a>导入模式</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p39061441407"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p39061441407"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p39061441407"></a>COPY模式：将源数据经过DWS管理节点后拷贝到数据节点。如果需要通过Internet访问DWS，只能使用COPY模式。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p19856164712316"><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p19856164712316"></a><a name="zh-cn_topic_0000001193296031_zh-cn_topic_0108275326_zh-cn_topic_0108275298_p19856164712316"></a>COPY</p>
    </td>
    </tr>
    </tbody>
    </table>

3.  单击“保存“完成创建连接。

## 创建迁移作业<a name="zh-cn_topic_0000001193296031_section383292919118"></a>

1.  选择“表/文件迁移  \>  新建作业“，开始创建从Oracle导出数据到DWS的任务。

    **图 3**  创建Oracle到DWS的迁移任务<a name="zh-cn_topic_0000001193296031_fig151818044718"></a>  
    ![](figures/创建Oracle到DWS的迁移任务.jpg "创建Oracle到DWS的迁移任务")

    -   作业名称：用户自定义便于记忆、区分的任务名称。
    -   源端作业配置
        -   源连接名称：选择[创建Oracle连接](#zh-cn_topic_0000001193296031_section1136440015)中的“oracle\_link“。
        -   模式或表空间：待迁移数据的数据库名称。
        -   表名：待迁移数据的表名。
        -   高级属性里的可选参数一般情况下保持默认既可，详细说明请参见[配置关系数据库源端参数](配置关系数据库源端参数.md#dgc_01_0054)。

    -   目的端作业配置
        -   目的连接名称：选择[创建DWS连接](#zh-cn_topic_0000001193296031_section796691518119)中的连接“dwslink“。
        -   模式或表空间：选择待写入数据的DWS数据库。
        -   自动创表：只有当源端和目的端都为关系数据库时，才有该参数。
        -   表名：待写入数据的表名，可以手动输入一个不存在表名，CDM会在DWS中自动创建该表。
        -   是否压缩：DWS提供的压缩数据能力，如果选择“是“，将进行高级别压缩，CDM提供了适用I/O读写量大，CPU富足（计算相对小）的压缩场景。更多压缩级别详细说明请参见[压缩级别](https://support.huaweicloud.com/bestpractice-dws/dws_05_0011.html#section1)。
        -   存储模式：可以根据具体应用场景，建表的时候选择行存储还是列存储表。一般情况下，如果表的字段比较多（大宽表），查询中涉及到的列不多的情况下，适合列存储。如果表的字段个数比较少，查询大部分字段，那么选择行存储比较好。
        -   扩大字符字段长度：当目的端和源端数据编码格式不一样时，自动建表的字符字段长度可能不够用，配置此选项后CDM自动建表时会将字符字段扩大3倍。
        -   导入前清空数据：任务启动前，是否清除目的表中数据，用户可根据实际需要选择。

2.  单击“下一步“进入字段映射界面，CDM会自动匹配源和目的字段，如[图4](#zh-cn_topic_0000001193296031_fig1534811262293)所示。

    -   如果字段映射顺序不匹配，可通过拖拽字段调整。
    -   单击，可批量映射字段。
    -   CDM的表达式已经预置常用字符串、日期、数值等类型的字段内容转换，详细请参见[字段转换](https://support.huaweicloud.com/bestpractice-dgc/dgc_05_0012.html)。

    **图 4**  表到表的字段映射<a name="zh-cn_topic_0000001193296031_fig1534811262293"></a>  
    ![](figures/表到表的字段映射-10.png "表到表的字段映射-10")

3.  单击“下一步“配置任务参数，一般情况下全部保持默认即可。

    该步骤用户可以配置如下可选功能：

    -   作业失败重试：如果作业执行失败，可选择是否自动重试，这里保持默认值“不重试“。
    -   作业分组：选择作业所属的分组，默认分组为“DEFAULT“。在CDM“作业管理“界面，支持作业分组显示、按组批量启动作业、按分组导出作业等操作。
    -   是否定时执行：如果需要配置作业定时自动执行，请参见[配置定时任务](配置定时任务.md#dgc_01_0082)。这里保持默认值“否“。
    -   抽取并发数：设置同时执行的抽取任务数。可适当调大参数，提升迁移效率。
    -   是否写入脏数据：表到表的迁移容易出现脏数据，建议配置脏数据归档。
    -   作业运行完是否删除：这里保持默认值“不删除“。

4.  单击“保存并运行“，回到作业管理界面，在作业管理界面可查看作业执行进度和结果。
5.  作业执行成功后，单击作业操作列的“历史记录“，可查看该作业的历史执行记录、读取和写入的统计数据。

    在历史记录界面单击“日志“，可查看作业的日志信息。


>![](public_sys-resources/icon-note.gif) **说明：** 
>如遇目的端写太久导致迁移超时，请减少Oracle连接器中“一次请求行数“参数值的设置。

