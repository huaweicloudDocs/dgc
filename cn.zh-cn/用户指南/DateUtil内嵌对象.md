# DateUtil内嵌对象<a name="dgc_01_0500"></a>

DateUtil内嵌对象提供了一系列时间格式化、时间计算方法。

## 方法<a name="zh-cn_topic_0132846499_section18841149151713"></a>

**表 1**  方法说明

<a name="zh-cn_topic_0132846499_table662281718176"></a>
<table><thead align="left"><tr id="zh-cn_topic_0132846499_row46221117141716"><th class="cellrowborder" valign="top" width="46%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0132846499_p462211713178"><a name="zh-cn_topic_0132846499_p462211713178"></a><a name="zh-cn_topic_0132846499_p462211713178"></a>方法</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0132846499_p76223174172"><a name="zh-cn_topic_0132846499_p76223174172"></a><a name="zh-cn_topic_0132846499_p76223174172"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0132846499_row1362211771712"><td class="cellrowborder" valign="top" width="46%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0132846499_p1862213172179"><a name="zh-cn_topic_0132846499_p1862213172179"></a><a name="zh-cn_topic_0132846499_p1862213172179"></a>String format(Date date, String pattern)</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0132846499_p76225177173"><a name="zh-cn_topic_0132846499_p76225177173"></a><a name="zh-cn_topic_0132846499_p76225177173"></a>将Date类型时间按指定pattern格式为字符串。</p>
</td>
</tr>
<tr id="zh-cn_topic_0132846499_row106221717141711"><td class="cellrowborder" valign="top" width="46%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0132846499_p962251761716"><a name="zh-cn_topic_0132846499_p962251761716"></a><a name="zh-cn_topic_0132846499_p962251761716"></a>Date addMonths(Date date, int amount)</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0132846499_p1962281716170"><a name="zh-cn_topic_0132846499_p1962281716170"></a><a name="zh-cn_topic_0132846499_p1962281716170"></a>给date添加指定月数后，返回新Date对象，amount可以是负数。</p>
</td>
</tr>
<tr id="zh-cn_topic_0132846499_row962291716173"><td class="cellrowborder" valign="top" width="46%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0132846499_p36229173170"><a name="zh-cn_topic_0132846499_p36229173170"></a><a name="zh-cn_topic_0132846499_p36229173170"></a>Date addDays(Date date, int amount)</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0132846499_p762291715173"><a name="zh-cn_topic_0132846499_p762291715173"></a><a name="zh-cn_topic_0132846499_p762291715173"></a>给date添加指定天数后，返回新Date对象，amount可以是负数。</p>
</td>
</tr>
<tr id="zh-cn_topic_0132846499_row4622317151718"><td class="cellrowborder" valign="top" width="46%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0132846499_p16226172179"><a name="zh-cn_topic_0132846499_p16226172179"></a><a name="zh-cn_topic_0132846499_p16226172179"></a>Date addHours(Date date, int amount)</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0132846499_p206228179177"><a name="zh-cn_topic_0132846499_p206228179177"></a><a name="zh-cn_topic_0132846499_p206228179177"></a>给date添加指定小时数后，返回新Date对象，amount可以是负数。</p>
</td>
</tr>
<tr id="zh-cn_topic_0132846499_row2062217172171"><td class="cellrowborder" valign="top" width="46%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0132846499_p262271717175"><a name="zh-cn_topic_0132846499_p262271717175"></a><a name="zh-cn_topic_0132846499_p262271717175"></a>Date addMinutes(Date date, int amount)</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0132846499_p162281781713"><a name="zh-cn_topic_0132846499_p162281781713"></a><a name="zh-cn_topic_0132846499_p162281781713"></a>给date添加指定分钟数后，返回新Date对象，amount可以是负数。</p>
</td>
</tr>
<tr id="zh-cn_topic_0132846499_row186221917161712"><td class="cellrowborder" valign="top" width="46%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0132846499_p1762211718175"><a name="zh-cn_topic_0132846499_p1762211718175"></a><a name="zh-cn_topic_0132846499_p1762211718175"></a>int getDay(Date date)</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0132846499_p1862281719176"><a name="zh-cn_topic_0132846499_p1862281719176"></a><a name="zh-cn_topic_0132846499_p1862281719176"></a>从date获取天，例如：date为2018-09-14，则返回14。</p>
</td>
</tr>
<tr id="zh-cn_topic_0132846499_row152311126192317"><td class="cellrowborder" valign="top" width="46%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0132846499_p17246226152319"><a name="zh-cn_topic_0132846499_p17246226152319"></a><a name="zh-cn_topic_0132846499_p17246226152319"></a>int getMonth(Date date)</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0132846499_p1624632642314"><a name="zh-cn_topic_0132846499_p1624632642314"></a><a name="zh-cn_topic_0132846499_p1624632642314"></a>从date获取月，例如：date为2018-09-14，则返回9。</p>
</td>
</tr>
<tr id="zh-cn_topic_0132846499_row136221917161712"><td class="cellrowborder" valign="top" width="46%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0132846499_p1622131710172"><a name="zh-cn_topic_0132846499_p1622131710172"></a><a name="zh-cn_topic_0132846499_p1622131710172"></a>int getYear(Date date)</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0132846499_p1862214170171"><a name="zh-cn_topic_0132846499_p1862214170171"></a><a name="zh-cn_topic_0132846499_p1862214170171"></a>从date获取年，例如：date为2018-09-14，则返回2018。</p>
</td>
</tr>
<tr id="zh-cn_topic_0132846499_row453518713244"><td class="cellrowborder" valign="top" width="46%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0132846499_p453537132411"><a name="zh-cn_topic_0132846499_p453537132411"></a><a name="zh-cn_topic_0132846499_p453537132411"></a>Date now()</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0132846499_p053597152414"><a name="zh-cn_topic_0132846499_p053597152414"></a><a name="zh-cn_topic_0132846499_p053597152414"></a>返回当前时间。</p>
</td>
</tr>
<tr id="zh-cn_topic_0132846499_row08793413247"><td class="cellrowborder" valign="top" width="46%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0132846499_p5879104152420"><a name="zh-cn_topic_0132846499_p5879104152420"></a><a name="zh-cn_topic_0132846499_p5879104152420"></a>long getTime(Date date)</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0132846499_p987912482412"><a name="zh-cn_topic_0132846499_p987912482412"></a><a name="zh-cn_topic_0132846499_p987912482412"></a>将Date类型时间转换为long类型。</p>
</td>
</tr>
<tr id="zh-cn_topic_0132846499_row95165818237"><td class="cellrowborder" valign="top" width="46%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0132846499_p45155892313"><a name="zh-cn_topic_0132846499_p45155892313"></a><a name="zh-cn_topic_0132846499_p45155892313"></a>Date parseDate(String str, String pattern)</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0132846499_p1251185852320"><a name="zh-cn_topic_0132846499_p1251185852320"></a><a name="zh-cn_topic_0132846499_p1251185852320"></a>字符串按pattern转换为Date类型，pattern为日期、时间模式，请参考<a href="日期和时间模式.md">日期和时间模式</a>。</p>
</td>
</tr>
</tbody>
</table>

## 举例<a name="zh-cn_topic_0132846499_section4812102915281"></a>

以作业调度计划时间的前一天时间作为子目录名称，生成一个OBS路径，EL表达式如下：

```
#{"obs://test/"+DateUtil.format(DateUtil.addDays(Job.planTime,-1),"yyyy-MM-dd")}
```

