# 新建数据表（DDL模式）<a name="dayu_01_0417"></a>

用户可以通过DDL模式新建永久数据表和临时数据表。数据表新建完成后，可以提供给脚本和作业使用。

目前支持新建如下数据表：

-   DLI
-   DWS
-   MRS Hive

## 前提条件<a name="zh-cn_topic_0125513555_section20635154952011"></a>

-   已开通相应的云服务并在云服务中创建数据库。例如，新建DLI表前，请确保DLI服务已开通，并在DLI服务中创建好数据库。
-   已在DLF中创建与数据表类型匹配的数据连接，请参见[创建数据连接](创建数据连接-0.md)。

## 操作步骤<a name="zh-cn_topic_0125513555_section1598220213195"></a>

1.  通过“右侧区域“页面
    1.  在数据开发主界面的左侧导航栏，选择“数据开发  \>  脚本开发“/“数据开发  \>  作业开发“，进入“右侧区域“页面。
    2.  在左侧菜单选择![](figures/icon-DLF-data_connection.png)，右键单击数据表“tables“，选择“新建数据表“。

2.  单击“DDL模式建表“，选择如[表1](#zh-cn_topic_0125513555_table1129115213117)所示的参数，并在下方的编辑器中输入SQL语句。

    **表 1**  数据表参数

    <a name="zh-cn_topic_0125513555_table1129115213117"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0125513555_row22911229112"><th class="cellrowborder" valign="top" width="33%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0125513555_p629112141115"><a name="zh-cn_topic_0125513555_p629112141115"></a><a name="zh-cn_topic_0125513555_p629112141115"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="67%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0125513555_p629110261118"><a name="zh-cn_topic_0125513555_p629110261118"></a><a name="zh-cn_topic_0125513555_p629110261118"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0125513555_row1629111210113"><td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0125513555_p1469124513239"><a name="zh-cn_topic_0125513555_p1469124513239"></a><a name="zh-cn_topic_0125513555_p1469124513239"></a>数据连接类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="67%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0125513555_p329152131118"><a name="zh-cn_topic_0125513555_p329152131118"></a><a name="zh-cn_topic_0125513555_p329152131118"></a>选择数据表所属的数据连接类型。</p>
    <a name="zh-cn_topic_0125513555_ul15405134191316"></a><a name="zh-cn_topic_0125513555_ul15405134191316"></a><ul id="zh-cn_topic_0125513555_ul15405134191316"><li><span id="zh-cn_topic_0125513555_text192162011317"><a name="zh-cn_topic_0125513555_text192162011317"></a><a name="zh-cn_topic_0125513555_text192162011317"></a>DLI</span></li><li>DWS</li><li>HIVE</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0125513555_row5291621114"><td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0125513555_p12550184854213"><a name="zh-cn_topic_0125513555_p12550184854213"></a><a name="zh-cn_topic_0125513555_p12550184854213"></a>数据连接</p>
    </td>
    <td class="cellrowborder" valign="top" width="67%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0125513555_p1231407154314"><a name="zh-cn_topic_0125513555_p1231407154314"></a><a name="zh-cn_topic_0125513555_p1231407154314"></a>选择数据表所属的数据连接。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0125513555_row1229112214118"><td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0125513555_p172911025112"><a name="zh-cn_topic_0125513555_p172911025112"></a><a name="zh-cn_topic_0125513555_p172911025112"></a>数据库</p>
    </td>
    <td class="cellrowborder" valign="top" width="67%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0125513555_p1973642216431"><a name="zh-cn_topic_0125513555_p1973642216431"></a><a name="zh-cn_topic_0125513555_p1973642216431"></a>选择数据表所属的数据库。</p>
    </td>
    </tr>
    </tbody>
    </table>

3.  单击“确定“，新建数据表。

