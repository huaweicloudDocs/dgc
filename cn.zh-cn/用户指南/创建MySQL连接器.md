# 创建MySQL连接器<a name="dgc_01_0131"></a>

MySQL连接适用于第三方云MySQL服务，以及用户在本地数据中心或ECS上自建的MySQL。本教程为您介绍如何创建MySQL连接器。

## 前提条件<a name="zh-cn_topic_0000001147041354_section5103527113413"></a>

-   已获取连接MySQL数据库的IP地址、端口、数据库名称、用户名、密码，且该用户拥有MySQL数据库的读写权限。
-   本地MySQL数据库可通过公网访问。如果MySQL服务器是在本地数据中心或第三方云上，需要确保MySQL可以通过公网IP访问，或者是已经建立好了企业内部数据中心到云服务平台的VPN通道或专线。
-   已创建CDM集群。

## 新建MySQL连接器<a name="zh-cn_topic_0000001147041354_section652045153919"></a>

1.  进入CDM主界面，单击左侧导航上的“集群管理“，选择CDM集群后的“作业管理  \>  连接管理  \>  驱动管理“，进入驱动管理页面。

    **图 1**  上传驱动<a name="zh-cn_topic_0000001147041354_fig1243121125516"></a>  
    ![](figures/上传驱动-6.png "上传驱动-6")

2.  单击“驱动管理“页面左上角“驱动下载地址“链接下载MySQL的驱动，详情请参见[如何获取驱动](管理驱动.md#zh-cn_topic_0286032703_section631855342818)。
3.  在“驱动管理“页面中，选择以下方式上传MySQL驱动。

    方式一：单击对应驱动名称右侧操作列的“上传“，选择本地已下载的驱动。

    方式二：单击对应驱动名称右侧操作列的“从sftp复制”，配置sftp连接器名称和驱动文件路径。

4.  在“集群管理“界面，单击集群后的“作业管理“，选择“连接管理  \>  新建连接“，进入连接器类型的选择界面，如[图2](#zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_fig15373426133913)所示。

    **图 2**  选择连接器类型<a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_fig15373426133913"></a>  
    ![](figures/选择连接器类型-7.png "选择连接器类型-7")

5.  选择“MySQL“后单击“下一步“，配置MySQL连接的参数，参数如[表1](#zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_table5321744015490)所示。

    **图 3**  创建MySQL连接<a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_fig17438459415"></a>  
    ![](figures/创建MySQL连接.png "创建MySQL连接")

    **表 1**  MySQL连接参数

    <a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_table5321744015490"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_row185605615490"><th class="cellrowborder" valign="top" width="21.39%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p3088488815490"><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p3088488815490"></a><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p3088488815490"></a>参数名</p>
    </th>
    <th class="cellrowborder" valign="top" width="46.01%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1864797615490"><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1864797615490"></a><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1864797615490"></a>说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="32.6%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p12195902165556"><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p12195902165556"></a><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p12195902165556"></a>取值样例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_row6448267615421"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p5571423915421"><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p5571423915421"></a><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p5571423915421"></a>名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1655951515421"><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1655951515421"></a><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1655951515421"></a>输入便于记忆和区分的连接名称。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p6625233515421"><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p6625233515421"></a><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p6625233515421"></a>mysqllink</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_row23645714155554"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p36254680155554"><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p36254680155554"></a><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p36254680155554"></a>数据库服务器</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p57055815164650"><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p57055815164650"></a><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p57055815164650"></a>MySQL数据库的IP地址或域名。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p54006514165556"><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p54006514165556"></a><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p54006514165556"></a>192.168.1.110</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_row35721234155558"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p7738819155558"><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p7738819155558"></a><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p7738819155558"></a>端口</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p44462215165646"><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p44462215165646"></a><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p44462215165646"></a>MySQL数据库的端口。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p44954710165556"><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p44954710165556"></a><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p44954710165556"></a>3306</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_row58054787162632"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p4817321162632"><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p4817321162632"></a><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p4817321162632"></a>数据库名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p23569444165647"><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p23569444165647"></a><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p23569444165647"></a>MySQL数据库的名称。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p22858665165556"><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p22858665165556"></a><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p22858665165556"></a>sqoop</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_row121116115490"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p3099525315490"><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p3099525315490"></a><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p3099525315490"></a>用户名</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p2758753215490"><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p2758753215490"></a><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p2758753215490"></a>拥有MySQL数据库的读、写和删除权限的用户。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p14053644165556"><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p14053644165556"></a><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p14053644165556"></a>admin</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_row4576104015490"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1565673415490"><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1565673415490"></a><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1565673415490"></a>密码</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p6023590815490"><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p6023590815490"></a><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p6023590815490"></a>用户的密码。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p44559445165556"><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p44559445165556"></a><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p44559445165556"></a>-</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001147041354_row1695382013335"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001147041354_p1395410209337"><a name="zh-cn_topic_0000001147041354_p1395410209337"></a><a name="zh-cn_topic_0000001147041354_p1395410209337"></a>使用本地API</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001147041354_p16954220143310"><a name="zh-cn_topic_0000001147041354_p16954220143310"></a><a name="zh-cn_topic_0000001147041354_p16954220143310"></a>使用数据库本地API加速（系统会尝试启用MySQL数据库的local_infile系统变量）。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001147041354_p195462013337"><a name="zh-cn_topic_0000001147041354_p195462013337"></a><a name="zh-cn_topic_0000001147041354_p195462013337"></a>是</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_row117692617437"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p18773153334318"><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p18773153334318"></a><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p18773153334318"></a>使用Agent</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p877373317439"><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p877373317439"></a><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p877373317439"></a>是否选择通过Agent从源端提取数据。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1977311335439"><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1977311335439"></a><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0284710796_zh-cn_topic_0111325168_zh-cn_topic_0108275298_p1977311335439"></a>是</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001147041354_row1785145420225"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001147041354_zh-cn_topic_0108275298_p2077320332430"><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0108275298_p2077320332430"></a><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0108275298_p2077320332430"></a>Agent</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001147041354_zh-cn_topic_0108275298_p1877310336437"><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0108275298_p1877310336437"></a><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0108275298_p1877310336437"></a>单击<span class="uicontrol" id="zh-cn_topic_0000001147041354_zh-cn_topic_0108275298_uicontrol1773183344318"><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0108275298_uicontrol1773183344318"></a><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0108275298_uicontrol1773183344318"></a>“选择”</span>，选择<a href="管理Agent.md#zh-cn_topic_0207402273_zh-cn_topic_0191978474_section1072083564713">连接Agent</a>中已创建的Agent。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001147041354_zh-cn_topic_0108275298_p16773533154317"><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0108275298_p16773533154317"></a><a name="zh-cn_topic_0000001147041354_zh-cn_topic_0108275298_p16773533154317"></a>-</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001147041354_row198311582349"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001147041354_p6841581349"><a name="zh-cn_topic_0000001147041354_p6841581349"></a><a name="zh-cn_topic_0000001147041354_p6841581349"></a>一次请求行数</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001147041354_p684105863419"><a name="zh-cn_topic_0000001147041354_p684105863419"></a><a name="zh-cn_topic_0000001147041354_p684105863419"></a>指定每次请求获取的行数。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001147041354_p1784115893412"><a name="zh-cn_topic_0000001147041354_p1784115893412"></a><a name="zh-cn_topic_0000001147041354_p1784115893412"></a>1000</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001147041354_row18386135893414"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001147041354_p17387105817349"><a name="zh-cn_topic_0000001147041354_p17387105817349"></a><a name="zh-cn_topic_0000001147041354_p17387105817349"></a>一次提交行数</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001147041354_p9322192916373"><a name="zh-cn_topic_0000001147041354_p9322192916373"></a><a name="zh-cn_topic_0000001147041354_p9322192916373"></a>支持通过agent从源端提取数据</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001147041354_p173871458113417"><a name="zh-cn_topic_0000001147041354_p173871458113417"></a><a name="zh-cn_topic_0000001147041354_p173871458113417"></a>1000</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001147041354_row753265813344"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001147041354_p153375816344"><a name="zh-cn_topic_0000001147041354_p153375816344"></a><a name="zh-cn_topic_0000001147041354_p153375816344"></a>连接属性</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001147041354_p8533158183416"><a name="zh-cn_topic_0000001147041354_p8533158183416"></a><a name="zh-cn_topic_0000001147041354_p8533158183416"></a>自定义连接属性。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001147041354_p353312586341"><a name="zh-cn_topic_0000001147041354_p353312586341"></a><a name="zh-cn_topic_0000001147041354_p353312586341"></a>useCompression=true</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001147041354_row1477817242359"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001147041354_p14778824153516"><a name="zh-cn_topic_0000001147041354_p14778824153516"></a><a name="zh-cn_topic_0000001147041354_p14778824153516"></a>引用符号</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001147041354_p4174143123613"><a name="zh-cn_topic_0000001147041354_p4174143123613"></a><a name="zh-cn_topic_0000001147041354_p4174143123613"></a>连接引用表名或列名时的分隔符号。默认为空。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001147041354_p1477819242350"><a name="zh-cn_topic_0000001147041354_p1477819242350"></a><a name="zh-cn_topic_0000001147041354_p1477819242350"></a>'</p>
    </td>
    </tr>
    </tbody>
    </table>

6.  单击“保存“回到连接管理界面，完成MySQL连接器的配置。

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >如果保存时出错，一般是由于MySQL数据库的安全设置问题，需要设置允许CDM集群的EIP访问MySQL数据库。


