# 开发Python脚本<a name="dgc_01_4503"></a>

对Python脚本进行在线开发、调试和执行，开发完成的脚本也可以在作业中执行（请参见[开发作业](开发作业.md)）。

## 前提条件<a name="zh-cn_topic_0114018164_section536330414847"></a>

-   已新增Python脚本，请参见[新建脚本](新建脚本.md)。
-   已新建主机连接，该主机配有用于执行Python脚本的环境，请参见[主机连接管理](主机连接管理.md)。

## 操作步骤<a name="zh-cn_topic_0114018164_section1916401114318"></a>

1.  登录DGC控制台。选择对应工作空间的“数据开发“模块，进入数据开发页面。

    **图 1**  选择数据开发<a name="dgc_01_0423_fig746051541519"></a>  
    ![](figures/选择数据开发.png "选择数据开发")

2.  在数据开发主界面的左侧导航栏，选择“数据开发  \>  脚本开发“。
3.  在脚本目录中，双击脚本名称，进入脚本开发页面。
4.  在编辑器上方，配置如[表1](#zh-cn_topic_0114018164_table5350135013499)所示的属性。

    **表 1**  Python脚本属性

    <a name="zh-cn_topic_0114018164_table5350135013499"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0114018164_row135045064917"><th class="cellrowborder" valign="top" width="20.25%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0114018164_p13350175044916"><a name="zh-cn_topic_0114018164_p13350175044916"></a><a name="zh-cn_topic_0114018164_p13350175044916"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="79.75%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0114018164_p9350145014913"><a name="zh-cn_topic_0114018164_p9350145014913"></a><a name="zh-cn_topic_0114018164_p9350145014913"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0114018164_row14812567293"><td class="cellrowborder" valign="top" width="20.25%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0114018164_p779714043012"><a name="zh-cn_topic_0114018164_p779714043012"></a><a name="zh-cn_topic_0114018164_p779714043012"></a>主机连接</p>
    </td>
    <td class="cellrowborder" valign="top" width="79.75%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0114018164_p24817565292"><a name="zh-cn_topic_0114018164_p24817565292"></a><a name="zh-cn_topic_0114018164_p24817565292"></a>选择执行Python脚本的主机。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0114018164_row1568281617357"><td class="cellrowborder" valign="top" width="20.25%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0114018164_p186831716203512"><a name="zh-cn_topic_0114018164_p186831716203512"></a><a name="zh-cn_topic_0114018164_p186831716203512"></a>参数</p>
    </td>
    <td class="cellrowborder" valign="top" width="79.75%" headers="mcps1.2.3.1.2 "><p id="p592774111145"><a name="p592774111145"></a><a name="p592774111145"></a>填写执行Python脚本时，向脚本传递的参数，参数之间使用空格分隔，例如：a b c。此处的<span class="parmname" id="parmname292764115142"><a name="parmname292764115142"></a><a name="parmname292764115142"></a>“参数”</span>需要在Python脚本中引用，否则配置无效。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0114018164_row1122617921415"><td class="cellrowborder" valign="top" width="20.25%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0114018164_p1322719141419"><a name="zh-cn_topic_0114018164_p1322719141419"></a><a name="zh-cn_topic_0114018164_p1322719141419"></a>交互式输入</p>
    </td>
    <td class="cellrowborder" valign="top" width="79.75%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0114018164_p20227194146"><a name="zh-cn_topic_0114018164_p20227194146"></a><a name="zh-cn_topic_0114018164_p20227194146"></a>填写交互式参数，即执行Python脚本的过程中，需要用户输入的交互式信息（例如密码）。</p>
    </td>
    </tr>
    </tbody>
    </table>

5.  在编辑器中编辑Python语句。为了方便脚本开发，数据开发模块提供了如下能力：
    -   脚本编辑器支持使用如下快捷键，以提升脚本开发效率。
        -   Ctrl + /：注释或解除注释光标所在行或代码块
        -   Ctrl + S：保存
        -   Ctrl + Z：撤销
        -   Ctrl + Y：重做
        -   Ctrl + F：查找
        -   Ctrl + Shift + R：替换
        -   Ctrl + X：剪切，光标未选中时剪切一行
        -   Alt + 鼠标拖动：列模式编辑，修改一整块内容
        -   Ctrl + 鼠标点选：多列模式编辑，多行缩进
        -   Shift + Ctrl + K：删除当前行
        -   Ctrl + →或Ctrl + ←：向右或向左按单词移动光标
        -   Ctrl + Home或Ctrl + End：移至当前文件的最前或最后
        -   Home或End：移至当前行最前或最后
        -   Ctrl + Shift + L：鼠标双击相同的字符串后，为所有相同的字符串添加光标，实现批量修改

    -   支持脚本参数功能，使用方法如下：
        1.  在Python语句中直接写入脚本参数名称和参数值。当Python脚本被作业引用时，如果作业配置的参数名称与Python脚本的参数名称相同，Python脚本的参数值将被作业的参数值替换。

            脚本示例如下：

            ```
            a=1
            echo ${a}
            ```

            其中，a是参数名称，只支持英文字母、数字、“-”、“\_”、“<”和“\>”，最大长度为16字符，且参数名称不允许重名。

        2.  在编辑器上方配置参数，在执行Python脚本时，参数会向脚本传递。参数之间使用空格分隔，例如：a b c。此处的“参数“需要在Python脚本中引用，否则配置无效。

6.  在编辑器上方，单击“运行“。Python语句运行完成后，在编辑器下方可以查看脚本的执行历史和执行结果。
7.  在编辑器上方，单击![](figures/save.png)，保存脚本。

    如果脚本是新建且未保存过的，请配置如[表2](#zh-cn_topic_0104967365_table35383235269)所示的参数。

    **表 2**  保存脚本

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
    <td class="cellrowborder" valign="top" width="54.14%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0104967365_p255482312611"><a name="zh-cn_topic_0104967365_p255482312611"></a><a name="zh-cn_topic_0104967365_p255482312611"></a>脚本的名称，只能包含字符：英文字母、数字、中文、中划线、下划线和点号，且长度小于等于128个字符。</p>
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

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >如果脚本未保存，重新打开脚本时，可以从本地缓存中恢复脚本内容。


