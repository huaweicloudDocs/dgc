# Loop内嵌对象<a name="dgc_01_0534"></a>

使用Loop内嵌对象可获取For Each数据集中的数据。

## 属性<a name="zh-cn_topic_0226521571_section18267348332"></a>

**表 1**  属性说明

<a name="zh-cn_topic_0226521571_table874717402336"></a>
<table><thead align="left"><tr id="zh-cn_topic_0226521571_row167470408331"><th class="cellrowborder" valign="top" width="29.959999999999997%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0226521571_p1774714014337"><a name="zh-cn_topic_0226521571_p1774714014337"></a><a name="zh-cn_topic_0226521571_p1774714014337"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="16.400000000000002%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0226521571_p1427019552810"><a name="zh-cn_topic_0226521571_p1427019552810"></a><a name="zh-cn_topic_0226521571_p1427019552810"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="53.64%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0226521571_p177471640193311"><a name="zh-cn_topic_0226521571_p177471640193311"></a><a name="zh-cn_topic_0226521571_p177471640193311"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0226521571_row1747740123312"><td class="cellrowborder" valign="top" width="29.959999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226521571_p14227161014914"><a name="zh-cn_topic_0226521571_p14227161014914"></a><a name="zh-cn_topic_0226521571_p14227161014914"></a>dataArray</p>
</td>
<td class="cellrowborder" valign="top" width="16.400000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226521571_p5270165520819"><a name="zh-cn_topic_0226521571_p5270165520819"></a><a name="zh-cn_topic_0226521571_p5270165520819"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.64%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226521571_p15624131220911"><a name="zh-cn_topic_0226521571_p15624131220911"></a><a name="zh-cn_topic_0226521571_p15624131220911"></a>For循环算子输入的数据集，是一个二维数组。</p>
</td>
</tr>
<tr id="zh-cn_topic_0226521571_row3747154018335"><td class="cellrowborder" valign="top" width="29.959999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226521571_p722615101794"><a name="zh-cn_topic_0226521571_p722615101794"></a><a name="zh-cn_topic_0226521571_p722615101794"></a>current</p>
</td>
<td class="cellrowborder" valign="top" width="16.400000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226521571_p1827116553813"><a name="zh-cn_topic_0226521571_p1827116553813"></a><a name="zh-cn_topic_0226521571_p1827116553813"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.64%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226521571_p1162212123917"><a name="zh-cn_topic_0226521571_p1162212123917"></a><a name="zh-cn_topic_0226521571_p1162212123917"></a>For循环算子当前遍历到的数据行,是一个一维数组。</p>
</td>
</tr>
<tr id="zh-cn_topic_0226521571_row197471240123319"><td class="cellrowborder" valign="top" width="29.959999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0226521571_p7191210195"><a name="zh-cn_topic_0226521571_p7191210195"></a><a name="zh-cn_topic_0226521571_p7191210195"></a>offset</p>
</td>
<td class="cellrowborder" valign="top" width="16.400000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0226521571_p92711554820"><a name="zh-cn_topic_0226521571_p92711554820"></a><a name="zh-cn_topic_0226521571_p92711554820"></a>Int</p>
</td>
<td class="cellrowborder" valign="top" width="53.64%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0226521571_p7883167101113"><a name="zh-cn_topic_0226521571_p7883167101113"></a><a name="zh-cn_topic_0226521571_p7883167101113"></a>For循环当前的偏移量，从0开始。</p>
<p id="zh-cn_topic_0226521571_p362114125910"><a name="zh-cn_topic_0226521571_p362114125910"></a><a name="zh-cn_topic_0226521571_p362114125910"></a>Loop.dataArray[Loop.offset] = Loop.current。</p>
</td>
</tr>
</tbody>
</table>

