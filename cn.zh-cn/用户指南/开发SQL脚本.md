# 开发SQL脚本<a name="dayu_01_0424"></a>

对SQL脚本进行在线开发、调试和执行，开发完成的脚本也可以在作业中执行（请参见[开发作业](开发作业.md)）。

## 前提条件<a name="zh-cn_topic_0104967365_section536330414847"></a>

-   已开通相应的云服务并在云服务中创建数据库。例如，开发DLI的脚本前，请确保DLI服务已开通，并在DLI服务中创建好数据库。Flink SQL脚本不涉及。
-   已在DLF中创建与脚本的数据连接类型匹配的数据连接，请参见[创建数据连接](创建数据连接-0.md)。Flink SQL脚本不涉及。
-   已新增SQL脚本，请参见[新建脚本](新建脚本.md#zh-cn_topic_0104967364_section3093294014851)。

## 操作步骤<a name="zh-cn_topic_0104967365_section3093294014851"></a>

1.  在数据开发主界面的左侧导航栏，选择“数据开发  \>  脚本开发“。
2.  在脚本目录中，双击脚本名称，进入脚本开发页面。
3.  在编辑器上方，选择如[表1](#zh-cn_topic_0104967365_table18459183312499)所示的属性。Flink SQL脚本不涉及，请跳过该步骤。

    **表 1**  SQL脚本属性

    <a name="zh-cn_topic_0104967365_table18459183312499"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0104967365_row144598332490"><th class="cellrowborder" valign="top" width="32%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0104967365_p3475163304919"><a name="zh-cn_topic_0104967365_p3475163304919"></a><a name="zh-cn_topic_0104967365_p3475163304919"></a>属性</p>
    </th>
    <th class="cellrowborder" valign="top" width="68%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0104967365_p447543364917"><a name="zh-cn_topic_0104967365_p447543364917"></a><a name="zh-cn_topic_0104967365_p447543364917"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0104967365_row0475533134913"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0104967365_p18475123313491"><a name="zh-cn_topic_0104967365_p18475123313491"></a><a name="zh-cn_topic_0104967365_p18475123313491"></a>数据连接</p>
    </td>
    <td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0104967365_p8475153311497"><a name="zh-cn_topic_0104967365_p8475153311497"></a><a name="zh-cn_topic_0104967365_p8475153311497"></a>选择数据连接。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0104967365_row1649013331499"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0104967365_p194901533194919"><a name="zh-cn_topic_0104967365_p194901533194919"></a><a name="zh-cn_topic_0104967365_p194901533194919"></a>资源队列</p>
    </td>
    <td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0104967365_p9490233194919"><a name="zh-cn_topic_0104967365_p9490233194919"></a><a name="zh-cn_topic_0104967365_p9490233194919"></a>选择执行<span id="zh-cn_topic_0104967365_text134901933194914"><a name="zh-cn_topic_0104967365_text134901933194914"></a><a name="zh-cn_topic_0104967365_text134901933194914"></a>DLI</span>作业的资源队列。当脚本为<span id="zh-cn_topic_0104967365_text2062413313190"><a name="zh-cn_topic_0104967365_text2062413313190"></a><a name="zh-cn_topic_0104967365_text2062413313190"></a>DLI</span> SQL时，配置该参数。</p>
    <div class="p" id="zh-cn_topic_0104967365_p4632865112"><a name="zh-cn_topic_0104967365_p4632865112"></a><a name="zh-cn_topic_0104967365_p4632865112"></a>如需新建资源队列，请参考以下方法：<a name="zh-cn_topic_0104967365_zh-cn_topic_0099822521_ul46080727105259"></a><a name="zh-cn_topic_0104967365_zh-cn_topic_0099822521_ul46080727105259"></a><ul id="zh-cn_topic_0104967365_zh-cn_topic_0099822521_ul46080727105259"><li>单击<a name="zh-cn_topic_0104967365_image4422159103310"></a><a name="zh-cn_topic_0104967365_image4422159103310"></a><span><img id="zh-cn_topic_0104967365_image4422159103310" src="figures/queue_add.png"></span>，进入<span id="zh-cn_topic_0104967365_text66132110547"><a name="zh-cn_topic_0104967365_text66132110547"></a><a name="zh-cn_topic_0104967365_text66132110547"></a>DLI</span>的<span class="wintitle" id="zh-cn_topic_0104967365_wintitle154711403146"><a name="zh-cn_topic_0104967365_wintitle154711403146"></a><a name="zh-cn_topic_0104967365_wintitle154711403146"></a>“队列管理”</span>页面新建资源队列。</li><li>前往<span id="zh-cn_topic_0104967365_text155328398531"><a name="zh-cn_topic_0104967365_text155328398531"></a><a name="zh-cn_topic_0104967365_text155328398531"></a>DLI</span>管理控制台进行新建。</li></ul>
    </div>
    <p id="zh-cn_topic_0104967365_p18631105416596"><a name="zh-cn_topic_0104967365_p18631105416596"></a><a name="zh-cn_topic_0104967365_p18631105416596"></a>如需以<span class="parmvalue" id="zh-cn_topic_0104967365_parmvalue01563426512"><a name="zh-cn_topic_0104967365_parmvalue01563426512"></a><a name="zh-cn_topic_0104967365_parmvalue01563426512"></a>“key/value”</span>的形式设置提交SQL作业的属性，请单击<a name="zh-cn_topic_0104967365_image1839611418218"></a><a name="zh-cn_topic_0104967365_image1839611418218"></a><span><img id="zh-cn_topic_0104967365_image1839611418218" src="figures/script_dli_set.png"></span>。最多可设置10个属性，属性说明如下：</p>
    <a name="zh-cn_topic_0104967365_ul45587104143542"></a><a name="zh-cn_topic_0104967365_ul45587104143542"></a><ul id="zh-cn_topic_0104967365_ul45587104143542"><li>dli.sql.autoBroadcastJoinThreshold（自动使用BroadcastJoin的数据量阈值）</li><li>dli.sql.shuffle.partitions（指定Shuffle过程中Partition的个数）</li><li>dli.sql.cbo.enabled（是否打开CBO优化策略）</li><li>dli.sql.cbo.joinReorder.enabled（开启CBO优化时，是否允许重新调整join的顺序）</li><li>dli.sql.multiLevelDir.enabled（OBS表的指定目录或OBS表分区表的分区目录下有子目录时，是否查询子目录的内容；默认不查询）</li><li>dli.sql.dynamicPartitionOverwrite.enabled（在动态分区模式时，只会重写查询中的数据涉及的分区，未涉及的分区不删除）</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0104967365_row14490183354917"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0104967365_p17506733134919"><a name="zh-cn_topic_0104967365_p17506733134919"></a><a name="zh-cn_topic_0104967365_p17506733134919"></a>数据库</p>
    </td>
    <td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0104967365_p8506193364916"><a name="zh-cn_topic_0104967365_p8506193364916"></a><a name="zh-cn_topic_0104967365_p8506193364916"></a>选择数据库。</p>
    </td>
    </tr>
    </tbody>
    </table>

4.  在编辑器中输入SQL语句（支持输入多条SQL语句），如需单独执行某部分SQL语句，请选中SQL语句再运行。为了方便脚本开发，DLF提供了系统函数和脚本参数功能（Flink SQL和RDS SQL脚本除外）。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >SQL语句之间以“;“分隔。如果其它地方使用“;“，请通过“\\“进行转义。例如：  
    >```  
    >select 1;  
    >select * from a where b="dsfa\;";  --example 1\;example 2.  
    >```  

    -   系统函数

        单击编辑器右侧的“系统函数“，显示该数据连接类型支持的函数，您可以拖动函数到编辑器中使用。

    -   脚本参数

        在SQL语句中直接写入脚本参数，调试脚本时可以在脚本编辑器下方输入参数值。如果脚本被作业引用，在作业开发页面可以配置参数值，参数值支持使用内置函数（参见[函数概述](函数概述.md)）和EL表达式（参见[表达式概述](表达式概述.md)）。

        脚本示例如下：

        ```
        select ${str1} from data;
        ```

        其中，str1是参数名称，只支持英文字母、数字、-、\_、<和\>，最大长度为16字符，且参数名称不允许重名。

5.  （可选）在编辑器上方，单击“格式化“，格式化SQL语句。Flink SQL脚本不涉及，请跳过该步骤。
6.  在编辑器上方，单击“运行“。SQL语句运行完成后，在编辑器下方可以查看脚本的执行历史、执行结果。Flink SQL脚本不涉及，请跳过该步骤。

    用户可根据需求下载或转储执行结果，参考如下：

    -   下载结果：下载CSV格式的结果文件到本地。
    -   转储结果：转储CSV格式的结果文件到OBS中，请参见[表2](#zh-cn_topic_0104967365_table271113311538)。

        **表 2**  转储结果

        <a name="zh-cn_topic_0104967365_table271113311538"></a>
        <table><thead align="left"><tr id="zh-cn_topic_0104967365_row8711193355312"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0104967365_p1072723355315"><a name="zh-cn_topic_0104967365_p1072723355315"></a><a name="zh-cn_topic_0104967365_p1072723355315"></a>参数</p>
        </th>
        <th class="cellrowborder" valign="top" width="12%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0104967365_p11727233155318"><a name="zh-cn_topic_0104967365_p11727233155318"></a><a name="zh-cn_topic_0104967365_p11727233155318"></a>是否必选</p>
        </th>
        <th class="cellrowborder" valign="top" width="63%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0104967365_p10727103345319"><a name="zh-cn_topic_0104967365_p10727103345319"></a><a name="zh-cn_topic_0104967365_p10727103345319"></a>说明</p>
        </th>
        </tr>
        </thead>
        <tbody><tr id="zh-cn_topic_0104967365_row1072783316537"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0104967365_p972711339538"><a name="zh-cn_topic_0104967365_p972711339538"></a><a name="zh-cn_topic_0104967365_p972711339538"></a>数据格式</p>
        </td>
        <td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0104967365_p14727103312536"><a name="zh-cn_topic_0104967365_p14727103312536"></a><a name="zh-cn_topic_0104967365_p14727103312536"></a>是</p>
        </td>
        <td class="cellrowborder" valign="top" width="63%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0104967365_p11742143320532"><a name="zh-cn_topic_0104967365_p11742143320532"></a><a name="zh-cn_topic_0104967365_p11742143320532"></a>目前仅支持导出CSV格式的结果文件。</p>
        </td>
        </tr>
        <tr id="zh-cn_topic_0104967365_row11742123325320"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0104967365_p1174216331534"><a name="zh-cn_topic_0104967365_p1174216331534"></a><a name="zh-cn_topic_0104967365_p1174216331534"></a>资源队列</p>
        </td>
        <td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0104967365_p19742933155311"><a name="zh-cn_topic_0104967365_p19742933155311"></a><a name="zh-cn_topic_0104967365_p19742933155311"></a>否</p>
        </td>
        <td class="cellrowborder" valign="top" width="63%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0104967365_p474214337538"><a name="zh-cn_topic_0104967365_p474214337538"></a><a name="zh-cn_topic_0104967365_p474214337538"></a>选择执行导出操作的<span id="zh-cn_topic_0104967365_text9742533105317"><a name="zh-cn_topic_0104967365_text9742533105317"></a><a name="zh-cn_topic_0104967365_text9742533105317"></a>DLI</span>队列。当脚本为<span id="zh-cn_topic_0104967365_text38851857225"><a name="zh-cn_topic_0104967365_text38851857225"></a><a name="zh-cn_topic_0104967365_text38851857225"></a>DLI</span> SQL时，配置该参数。</p>
        </td>
        </tr>
        <tr id="zh-cn_topic_0104967365_row4757173311539"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0104967365_p47571633205319"><a name="zh-cn_topic_0104967365_p47571633205319"></a><a name="zh-cn_topic_0104967365_p47571633205319"></a>压缩格式</p>
        </td>
        <td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0104967365_p675743313533"><a name="zh-cn_topic_0104967365_p675743313533"></a><a name="zh-cn_topic_0104967365_p675743313533"></a>否</p>
        </td>
        <td class="cellrowborder" valign="top" width="63%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0104967365_p137571533115319"><a name="zh-cn_topic_0104967365_p137571533115319"></a><a name="zh-cn_topic_0104967365_p137571533115319"></a>选择压缩格式。当脚本为<span id="zh-cn_topic_0104967365_text18698425112210"><a name="zh-cn_topic_0104967365_text18698425112210"></a><a name="zh-cn_topic_0104967365_text18698425112210"></a>DLI</span> SQL时，配置该参数。</p>
        <a name="zh-cn_topic_0104967365_ul9757163335311"></a><a name="zh-cn_topic_0104967365_ul9757163335311"></a><ul id="zh-cn_topic_0104967365_ul9757163335311"><li>none</li><li>bzip2</li><li>deflate</li><li>gzip</li></ul>
        </td>
        </tr>
        <tr id="zh-cn_topic_0104967365_row1757333135315"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0104967365_p15774333165319"><a name="zh-cn_topic_0104967365_p15774333165319"></a><a name="zh-cn_topic_0104967365_p15774333165319"></a>存储路径</p>
        </td>
        <td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0104967365_p127741833145317"><a name="zh-cn_topic_0104967365_p127741833145317"></a><a name="zh-cn_topic_0104967365_p127741833145317"></a>是</p>
        </td>
        <td class="cellrowborder" valign="top" width="63%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0104967365_p87742033165316"><a name="zh-cn_topic_0104967365_p87742033165316"></a><a name="zh-cn_topic_0104967365_p87742033165316"></a>设置结果文件的OBS存储路径。选择OBS路径后，您需要在选择的路径后方自定义一个文件夹名称，系统将在OBS路径下创建文件夹，用于存放结果文件。</p>
        </td>
        </tr>
        <tr id="zh-cn_topic_0104967365_row1277412339533"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0104967365_p1977483317537"><a name="zh-cn_topic_0104967365_p1977483317537"></a><a name="zh-cn_topic_0104967365_p1977483317537"></a>覆盖类型</p>
        </td>
        <td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0104967365_p1977415336534"><a name="zh-cn_topic_0104967365_p1977415336534"></a><a name="zh-cn_topic_0104967365_p1977415336534"></a>是</p>
        </td>
        <td class="cellrowborder" valign="top" width="63%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0104967365_p1577453335312"><a name="zh-cn_topic_0104967365_p1577453335312"></a><a name="zh-cn_topic_0104967365_p1577453335312"></a>如果<span class="parmname" id="zh-cn_topic_0104967365_parmname167744333531"><a name="zh-cn_topic_0104967365_parmname167744333531"></a><a name="zh-cn_topic_0104967365_parmname167744333531"></a>“存储路径”</span>中，您自定义的文件夹在OBS路径中已存在，选择覆盖类型。当脚本为<span id="zh-cn_topic_0104967365_text3323143715223"><a name="zh-cn_topic_0104967365_text3323143715223"></a><a name="zh-cn_topic_0104967365_text3323143715223"></a>DLI</span> SQL时，配置该参数。</p>
        <a name="zh-cn_topic_0104967365_ul14789433165313"></a><a name="zh-cn_topic_0104967365_ul14789433165313"></a><ul id="zh-cn_topic_0104967365_ul14789433165313"><li>覆盖：删除OBS路径中已有的重名文件夹，重新创建自定义的文件夹。</li><li>存在即报错：系统返回错误信息，退出导出操作。</li></ul>
        </td>
        </tr>
        </tbody>
        </table>

7.  在编辑器上方，单击![](figures/icon-dlf-save.png)，保存脚本。

    如果脚本是新建且未保存过的，请配置如[表3](#zh-cn_topic_0104967365_table35383235269)所示的参数。

    **表 3**  保存脚本

    <a name="zh-cn_topic_0104967365_table35383235269"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0104967365_row55381123202616"><th class="cellrowborder" valign="top" width="31.39%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0104967365_p1153817231264"><a name="zh-cn_topic_0104967365_p1153817231264"></a><a name="zh-cn_topic_0104967365_p1153817231264"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="14.469999999999999%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0104967365_p195381623142618"><a name="zh-cn_topic_0104967365_p195381623142618"></a><a name="zh-cn_topic_0104967365_p195381623142618"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="54.14%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0104967365_p75541123192614"><a name="zh-cn_topic_0104967365_p75541123192614"></a><a name="zh-cn_topic_0104967365_p75541123192614"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0104967365_row5554122311266"><td class="cellrowborder" valign="top" width="31.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0104967365_p155414231262"><a name="zh-cn_topic_0104967365_p155414231262"></a><a name="zh-cn_topic_0104967365_p155414231262"></a>脚本名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.469999999999999%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0104967365_p7554122342613"><a name="zh-cn_topic_0104967365_p7554122342613"></a><a name="zh-cn_topic_0104967365_p7554122342613"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="54.14%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0104967365_p255482312611"><a name="zh-cn_topic_0104967365_p255482312611"></a><a name="zh-cn_topic_0104967365_p255482312611"></a>脚本的名称，只能包含英文字母、数字、中文字符、<span class="parmvalue" id="zh-cn_topic_0104967365_parmvalue145549230262"><a name="zh-cn_topic_0104967365_parmvalue145549230262"></a><a name="zh-cn_topic_0104967365_parmvalue145549230262"></a>“_”</span>、<span class="parmvalue" id="zh-cn_topic_0104967365_parmvalue1554102352619"><a name="zh-cn_topic_0104967365_parmvalue1554102352619"></a><a name="zh-cn_topic_0104967365_parmvalue1554102352619"></a>“-”</span>，且长度为1~128个字符。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0104967365_row155541323182616"><td class="cellrowborder" valign="top" width="31.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0104967365_p655422312266"><a name="zh-cn_topic_0104967365_p655422312266"></a><a name="zh-cn_topic_0104967365_p655422312266"></a>描述</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.469999999999999%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0104967365_p4554122316263"><a name="zh-cn_topic_0104967365_p4554122316263"></a><a name="zh-cn_topic_0104967365_p4554122316263"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="54.14%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0104967365_p13554112392618"><a name="zh-cn_topic_0104967365_p13554112392618"></a><a name="zh-cn_topic_0104967365_p13554112392618"></a>脚本的描述信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0104967365_row25851239261"><td class="cellrowborder" valign="top" width="31.39%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0104967365_p18585623182610"><a name="zh-cn_topic_0104967365_p18585623182610"></a><a name="zh-cn_topic_0104967365_p18585623182610"></a>选择目录</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.469999999999999%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0104967365_p16585112317266"><a name="zh-cn_topic_0104967365_p16585112317266"></a><a name="zh-cn_topic_0104967365_p16585112317266"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="54.14%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0104967365_p9585102317266"><a name="zh-cn_topic_0104967365_p9585102317266"></a><a name="zh-cn_topic_0104967365_p9585102317266"></a>选择脚本所属的目录，默认为根目录。</p>
    </td>
    </tr>
    </tbody>
    </table>


