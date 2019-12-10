# getTimeUnitValue<a name="dayu_01_0475"></a>

传入一个长整形时间戳及单位，返回这个时间点单位所代表的部分。

## 函数格式<a name="zh-cn_topic_0126423662_section1644216138434"></a>

String  **getTimeUnitValue**\(String dateStamp, String unit\)

## 参数<a name="zh-cn_topic_0126423662_section16381557184317"></a>

-   dateStamp

    合法的长整形（java.lang.Long）时间戳。

-   unit

    日期单位，取值范围：

    **表 1**  日期单位

    <a name="zh-cn_topic_0126423662_table516631023212"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0126423662_row201661110163211"><th class="cellrowborder" valign="top" width="41%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0126423662_p10166101023220"><a name="zh-cn_topic_0126423662_p10166101023220"></a><a name="zh-cn_topic_0126423662_p10166101023220"></a>字母</p>
    </th>
    <th class="cellrowborder" valign="top" width="59%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0126423662_p11166191053210"><a name="zh-cn_topic_0126423662_p11166191053210"></a><a name="zh-cn_topic_0126423662_p11166191053210"></a>含义</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0126423662_row10166210153215"><td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0126423662_p1516611019327"><a name="zh-cn_topic_0126423662_p1516611019327"></a><a name="zh-cn_topic_0126423662_p1516611019327"></a>y</p>
    </td>
    <td class="cellrowborder" valign="top" width="59%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0126423662_p51661310183217"><a name="zh-cn_topic_0126423662_p51661310183217"></a><a name="zh-cn_topic_0126423662_p51661310183217"></a>年</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0126423662_row818116103327"><td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0126423662_p91817106329"><a name="zh-cn_topic_0126423662_p91817106329"></a><a name="zh-cn_topic_0126423662_p91817106329"></a>m</p>
    </td>
    <td class="cellrowborder" valign="top" width="59%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0126423662_p5181111018321"><a name="zh-cn_topic_0126423662_p5181111018321"></a><a name="zh-cn_topic_0126423662_p5181111018321"></a>月</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0126423662_row8181210183218"><td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0126423662_p12181810163212"><a name="zh-cn_topic_0126423662_p12181810163212"></a><a name="zh-cn_topic_0126423662_p12181810163212"></a>d</p>
    </td>
    <td class="cellrowborder" valign="top" width="59%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0126423662_p141811510103217"><a name="zh-cn_topic_0126423662_p141811510103217"></a><a name="zh-cn_topic_0126423662_p141811510103217"></a>一个月份的第几天</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0126423662_row5827128173312"><td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0126423662_p13827228133313"><a name="zh-cn_topic_0126423662_p13827228133313"></a><a name="zh-cn_topic_0126423662_p13827228133313"></a>h</p>
    </td>
    <td class="cellrowborder" valign="top" width="59%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0126423662_p1482752863312"><a name="zh-cn_topic_0126423662_p1482752863312"></a><a name="zh-cn_topic_0126423662_p1482752863312"></a>小时</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0126423662_row21811710193217"><td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0126423662_p17181151073213"><a name="zh-cn_topic_0126423662_p17181151073213"></a><a name="zh-cn_topic_0126423662_p17181151073213"></a>mi</p>
    </td>
    <td class="cellrowborder" valign="top" width="59%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0126423662_p1818111105328"><a name="zh-cn_topic_0126423662_p1818111105328"></a><a name="zh-cn_topic_0126423662_p1818111105328"></a>分钟</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0126423662_row141811710193220"><td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0126423662_p15181410113210"><a name="zh-cn_topic_0126423662_p15181410113210"></a><a name="zh-cn_topic_0126423662_p15181410113210"></a>s</p>
    </td>
    <td class="cellrowborder" valign="top" width="59%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0126423662_p1918181013220"><a name="zh-cn_topic_0126423662_p1918181013220"></a><a name="zh-cn_topic_0126423662_p1918181013220"></a>秒</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0126423662_row1618151033215"><td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0126423662_p13197810113217"><a name="zh-cn_topic_0126423662_p13197810113217"></a><a name="zh-cn_topic_0126423662_p13197810113217"></a>ms</p>
    </td>
    <td class="cellrowborder" valign="top" width="59%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0126423662_p2019731053219"><a name="zh-cn_topic_0126423662_p2019731053219"></a><a name="zh-cn_topic_0126423662_p2019731053219"></a>毫秒</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0126423662_row1119771010328"><td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0126423662_p219712105325"><a name="zh-cn_topic_0126423662_p219712105325"></a><a name="zh-cn_topic_0126423662_p219712105325"></a>day</p>
    </td>
    <td class="cellrowborder" valign="top" width="59%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0126423662_p2019781053211"><a name="zh-cn_topic_0126423662_p2019781053211"></a><a name="zh-cn_topic_0126423662_p2019781053211"></a>周几</p>
    </td>
    </tr>
    </tbody>
    </table>


## 示例<a name="zh-cn_topic_0126423662_section20520313194417"></a>

函数形式：$getTimeUnitValue\(1521600390000L,@@y@@\)

返回值：2018

