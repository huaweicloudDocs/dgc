# MySQL整库迁移到云上RDS服务<a name="dayu_01_0098"></a>

## 操作场景<a name="zh-cn_topic_0108275389_section21020958143223"></a>

本章节介绍使用CDM整库迁移功能，将本地MySQL数据库迁移到云服务RDS中。

当前CDM支持将本地MySQL数据库，整库迁移到RDS上的MySQL、PostgreSQL或者Microsoft SQL Server任意一种数据库中。这里以整库迁移到RDS上的MySQL数据库（云数据库 MySQL）为例进行介绍，使用流程如下：

1.  [创建CDM集群并绑定EIP](#zh-cn_topic_0108275389_section563314494359)
2.  [创建MySQL连接](#zh-cn_topic_0108275389_section3392631930)
3.  [创建RDS连接](#zh-cn_topic_0108275389_section196516591234)
4.  [创建整库迁移作业](#zh-cn_topic_0108275389_section1508747294234)

## 前提条件<a name="zh-cn_topic_0108275389_section5787168294234"></a>

-   用户拥有EIP配额。
-   用户已购买RDS数据库实例，该实例的数据库引擎为MySQL。
-   本地MySQL数据库可通过公网访问。如果MySQL服务器是在本地数据中心或第三方云上，需要确保MySQL可以通过公网IP访问，或者是已经建立好了企业内部数据中心到华为云的VPN通道或专线。
-   已获取本地MySQL数据库和RDS上MySQL数据库的IP地址、数据库名称、用户名和密码。

## 创建CDM集群并绑定EIP<a name="zh-cn_topic_0108275389_section563314494359"></a>

1.  创建CDM集群，具体操作请参见[创建集群](创建集群.md)。关键配置如下：
    -   CDM集群的规格，按待迁移的数据量选择，一般选择cdm.medium即可，满足大部分迁移场景。
    -   CDM集群的VPC，选择和RDS的MySQL数据库实例所在的VPC一致，且推荐子网、安全组也与RDS上的MySQL一致。
    -   如果安全控制原因不能使用相同子网和安全组，则可以修改安全组规则，允许CDM访问RDS。

2.  CDM集群创建完成后，选择集群操作列的“绑定弹性IP“，CDM通过EIP访问本地MySQL数据库。

    **图 1**  绑定EIP<a name="zh-cn_topic_0108275389_fig570312018444"></a>  
    ![](figures/绑定EIP-0.png "绑定EIP-0")

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >如果用户对本地数据源的访问通道做了SSL加密，则CDM无法通过弹性IP连接数据源。  


## 创建MySQL连接<a name="zh-cn_topic_0108275389_section3392631930"></a>

1.  在集群管理界面，单击集群后的“作业管理“，选择“连接管理  \>  新建连接“，进入连接器类型的选择界面，如[图2](#dayu_01_0092_zh-cn_topic_0111325168_fig15373426133913)所示。

    **图 2**  选择连接器类型<a name="dayu_01_0092_zh-cn_topic_0111325168_fig15373426133913"></a>  
    ![](figures/选择连接器类型.png "选择连接器类型")

2.  选择“MySQL“后单击“下一步“，配置MySQL连接的参数。

    **图 3**  创建MySQL连接5<a name="dayu_01_0092_zh-cn_topic_0108275298_fig32415531174450"></a>  
    ![](figures/创建MySQL连接5.png "创建MySQL连接5")

    单击“显示高级属性“可查看更多可选参数，具体请参见[配置关系数据库连接](配置关系数据库连接.md)。这里保持默认，必填参数如[表1](#dayu_01_0092_zh-cn_topic_0108275298_table5321744015490)所示。

    **表 1**  MySQL连接参数

    <a name="dayu_01_0092_zh-cn_topic_0108275298_table5321744015490"></a>
    <table><thead align="left"><tr id="dayu_01_0092_zh-cn_topic_0108275298_row185605615490"><th class="cellrowborder" valign="top" width="21.39%" id="mcps1.2.4.1.1"><p id="dayu_01_0092_zh-cn_topic_0108275298_p3088488815490"><a name="dayu_01_0092_zh-cn_topic_0108275298_p3088488815490"></a><a name="dayu_01_0092_zh-cn_topic_0108275298_p3088488815490"></a>参数名</p>
    </th>
    <th class="cellrowborder" valign="top" width="46.01%" id="mcps1.2.4.1.2"><p id="dayu_01_0092_zh-cn_topic_0108275298_p1864797615490"><a name="dayu_01_0092_zh-cn_topic_0108275298_p1864797615490"></a><a name="dayu_01_0092_zh-cn_topic_0108275298_p1864797615490"></a>说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="32.6%" id="mcps1.2.4.1.3"><p id="dayu_01_0092_zh-cn_topic_0108275298_p12195902165556"><a name="dayu_01_0092_zh-cn_topic_0108275298_p12195902165556"></a><a name="dayu_01_0092_zh-cn_topic_0108275298_p12195902165556"></a>取值样例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="dayu_01_0092_zh-cn_topic_0108275298_row6448267615421"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="dayu_01_0092_zh-cn_topic_0108275298_p5571423915421"><a name="dayu_01_0092_zh-cn_topic_0108275298_p5571423915421"></a><a name="dayu_01_0092_zh-cn_topic_0108275298_p5571423915421"></a>名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="dayu_01_0092_zh-cn_topic_0108275298_p1655951515421"><a name="dayu_01_0092_zh-cn_topic_0108275298_p1655951515421"></a><a name="dayu_01_0092_zh-cn_topic_0108275298_p1655951515421"></a>输入便于记忆和区分的连接名称。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="dayu_01_0092_zh-cn_topic_0108275298_p6625233515421"><a name="dayu_01_0092_zh-cn_topic_0108275298_p6625233515421"></a><a name="dayu_01_0092_zh-cn_topic_0108275298_p6625233515421"></a>mysqllink</p>
    </td>
    </tr>
    <tr id="dayu_01_0092_zh-cn_topic_0108275298_row23645714155554"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="dayu_01_0092_zh-cn_topic_0108275298_p36254680155554"><a name="dayu_01_0092_zh-cn_topic_0108275298_p36254680155554"></a><a name="dayu_01_0092_zh-cn_topic_0108275298_p36254680155554"></a>数据库服务器</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="dayu_01_0092_zh-cn_topic_0108275298_p57055815164650"><a name="dayu_01_0092_zh-cn_topic_0108275298_p57055815164650"></a><a name="dayu_01_0092_zh-cn_topic_0108275298_p57055815164650"></a>MySQL数据库的IP地址或域名。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="dayu_01_0092_zh-cn_topic_0108275298_p54006514165556"><a name="dayu_01_0092_zh-cn_topic_0108275298_p54006514165556"></a><a name="dayu_01_0092_zh-cn_topic_0108275298_p54006514165556"></a>192.168.0.1</p>
    </td>
    </tr>
    <tr id="dayu_01_0092_zh-cn_topic_0108275298_row35721234155558"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="dayu_01_0092_zh-cn_topic_0108275298_p7738819155558"><a name="dayu_01_0092_zh-cn_topic_0108275298_p7738819155558"></a><a name="dayu_01_0092_zh-cn_topic_0108275298_p7738819155558"></a>端口</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="dayu_01_0092_zh-cn_topic_0108275298_p44462215165646"><a name="dayu_01_0092_zh-cn_topic_0108275298_p44462215165646"></a><a name="dayu_01_0092_zh-cn_topic_0108275298_p44462215165646"></a>MySQL数据库的端口。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="dayu_01_0092_zh-cn_topic_0108275298_p44954710165556"><a name="dayu_01_0092_zh-cn_topic_0108275298_p44954710165556"></a><a name="dayu_01_0092_zh-cn_topic_0108275298_p44954710165556"></a>3306</p>
    </td>
    </tr>
    <tr id="dayu_01_0092_zh-cn_topic_0108275298_row58054787162632"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="dayu_01_0092_zh-cn_topic_0108275298_p4817321162632"><a name="dayu_01_0092_zh-cn_topic_0108275298_p4817321162632"></a><a name="dayu_01_0092_zh-cn_topic_0108275298_p4817321162632"></a>数据库名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="dayu_01_0092_zh-cn_topic_0108275298_p23569444165647"><a name="dayu_01_0092_zh-cn_topic_0108275298_p23569444165647"></a><a name="dayu_01_0092_zh-cn_topic_0108275298_p23569444165647"></a>MySQL数据库的名称。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="dayu_01_0092_zh-cn_topic_0108275298_p22858665165556"><a name="dayu_01_0092_zh-cn_topic_0108275298_p22858665165556"></a><a name="dayu_01_0092_zh-cn_topic_0108275298_p22858665165556"></a>sqoop</p>
    </td>
    </tr>
    <tr id="dayu_01_0092_zh-cn_topic_0108275298_row121116115490"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="dayu_01_0092_zh-cn_topic_0108275298_p3099525315490"><a name="dayu_01_0092_zh-cn_topic_0108275298_p3099525315490"></a><a name="dayu_01_0092_zh-cn_topic_0108275298_p3099525315490"></a>用户名</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="dayu_01_0092_zh-cn_topic_0108275298_p2758753215490"><a name="dayu_01_0092_zh-cn_topic_0108275298_p2758753215490"></a><a name="dayu_01_0092_zh-cn_topic_0108275298_p2758753215490"></a>拥有MySQL数据库的读、写和删除权限的用户。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="dayu_01_0092_zh-cn_topic_0108275298_p14053644165556"><a name="dayu_01_0092_zh-cn_topic_0108275298_p14053644165556"></a><a name="dayu_01_0092_zh-cn_topic_0108275298_p14053644165556"></a>admin</p>
    </td>
    </tr>
    <tr id="dayu_01_0092_zh-cn_topic_0108275298_row4576104015490"><td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.2.4.1.1 "><p id="dayu_01_0092_zh-cn_topic_0108275298_p1565673415490"><a name="dayu_01_0092_zh-cn_topic_0108275298_p1565673415490"></a><a name="dayu_01_0092_zh-cn_topic_0108275298_p1565673415490"></a>密码</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="dayu_01_0092_zh-cn_topic_0108275298_p6023590815490"><a name="dayu_01_0092_zh-cn_topic_0108275298_p6023590815490"></a><a name="dayu_01_0092_zh-cn_topic_0108275298_p6023590815490"></a>用户的密码。</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.6%" headers="mcps1.2.4.1.3 "><p id="dayu_01_0092_zh-cn_topic_0108275298_p44559445165556"><a name="dayu_01_0092_zh-cn_topic_0108275298_p44559445165556"></a><a name="dayu_01_0092_zh-cn_topic_0108275298_p44559445165556"></a>-</p>
    </td>
    </tr>
    </tbody>
    </table>

3.  单击“保存“回到连接管理界面。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >如果保存时出错，一般是由于MySQL数据库的安全设置问题，需要设置允许CDM集群的EIP访问MySQL数据库。  


## 创建RDS连接<a name="zh-cn_topic_0108275389_section196516591234"></a>

1.  在连接器类型界面选择“云数据库 MySQL“后单击“下一步“，配置连接参数：

    -   名称：用户自定义连接名称，例如：“rds\_link“。
    -   数据库服务器、端口：配置为RDS上MySQL数据库的连接地址、端口。
    -   数据库名称：配置为RDS上MySQL数据库的名称。
    -   用户名、密码：登录数据库的用户和密码。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >-   创建RDS连接时，“使用本地API“设置为“是“时，可以使用MySQL的LOAD DATA功能加快数据导入，提高导入数据到MySQL的性能。  
    >-   由于RDS上的MySQL默认没有开启LOAD DATA功能，所以同时需要修改MySQL实例的参数组，将“local\_infile“设置为“ON“，开启该功能。  
    >-   如果“local\_infile“参数组不可编辑，则说明是默认参数组，需要先创建一个新的参数组，再修改该参数值，并应用到RDS的MySQL实例上。  

2.  单击“保存“回到连接管理界面。

## 创建整库迁移作业<a name="zh-cn_topic_0108275389_section1508747294234"></a>

1.  两个连接创建完成后，选择“整库迁移  \>  新建作业“，开始创建迁移任务，如[图4](#zh-cn_topic_0108275389_fig4434922711956)所示。

    **图 4**  创建整库迁移作业3<a name="zh-cn_topic_0108275389_fig4434922711956"></a>  
    ![](figures/创建整库迁移作业3.png "创建整库迁移作业3")

    -   作业名称：用户自定义整库迁移的任务名称。
    -   源端作业配置
        -   源连接名称：选择[创建MySQL连接](#zh-cn_topic_0108275389_section3392631930)中的“mysql\_link“。
        -   模式或表空间：选择从本地MySQL的哪个数据库导出数据。

    -   目的端作业配置
        -   目的连接名称：选择[创建RDS连接](#zh-cn_topic_0108275389_section196516591234)中的“rds\_link“。
        -   模式或表空间：选择将数据导入到RDS的哪个数据库。
        -   自动创表：选择“不存在时创建“，当RDS数据库中没有本地MySQL数据库里的表时，CDM会自动在RDS数据库中创建那些表。
        -   导入前清空数据：选择“是“，当RDS数据库中存在与本地MySQL数据库重名的表时，CDM会清除RDS中重名表里的数据。
        -   高级属性里的可选参数保持默认即可。

2.  单击“下一步“，进入选择待迁移表的界面，您可以选择全部或者部分表进行迁移。
3.  单击“保存并运行“，CDM会立即开始执行整库迁移任务。

    作业任务启动后，每个待迁移的表都会生成一个子任务，单击整库迁移的作业名称，可查看子任务列表。

4.  单击作业操作列的“历史记录“，可查看该作业的历史执行记录、读取和写入的统计数据。

    整库迁移的作业没有日志，子作业才有。在子作业的历史记录界面单击“日志“，可查看作业的日志信息。


