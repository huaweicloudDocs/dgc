# 配置DCS目的端参数<a name="dgc_01_0070"></a>

当作业将数据导入到分布式缓存服务（DCS）时，目的端作业参数如[表1](#zh-cn_topic_0108275365_table42991210161426)所示。

**表 1**  DCS作为目的端时的作业参数

<a name="zh-cn_topic_0108275365_table42991210161426"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108275365_row39332395161426"><th class="cellrowborder" valign="top" width="17.28%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108275365_p31807393161426"><a name="zh-cn_topic_0108275365_p31807393161426"></a><a name="zh-cn_topic_0108275365_p31807393161426"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="63.88%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108275365_p26262040161426"><a name="zh-cn_topic_0108275365_p26262040161426"></a><a name="zh-cn_topic_0108275365_p26262040161426"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="18.84%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108275365_p46850487161426"><a name="zh-cn_topic_0108275365_p46850487161426"></a><a name="zh-cn_topic_0108275365_p46850487161426"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108275365_row36793127161426"><td class="cellrowborder" valign="top" width="17.28%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275365_p1651645021725"><a name="zh-cn_topic_0108275365_p1651645021725"></a><a name="zh-cn_topic_0108275365_p1651645021725"></a>Redis键前缀</p>
</td>
<td class="cellrowborder" valign="top" width="63.88%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275365_p67100182153822"><a name="zh-cn_topic_0108275365_p67100182153822"></a><a name="zh-cn_topic_0108275365_p67100182153822"></a>键的前缀，类似关系型数据库的表名。</p>
</td>
<td class="cellrowborder" valign="top" width="18.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275365_p9075837153820"><a name="zh-cn_topic_0108275365_p9075837153820"></a><a name="zh-cn_topic_0108275365_p9075837153820"></a>TABLE</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275365_row9852861161426"><td class="cellrowborder" valign="top" width="17.28%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275365_p97388921725"><a name="zh-cn_topic_0108275365_p97388921725"></a><a name="zh-cn_topic_0108275365_p97388921725"></a>值存储类型</p>
</td>
<td class="cellrowborder" valign="top" width="63.88%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108275365_p1177617121725"><a name="zh-cn_topic_0108275365_p1177617121725"></a><a name="zh-cn_topic_0108275365_p1177617121725"></a>仅支持以下数据格式：<a name="zh-cn_topic_0108275365_zh-cn_topic_0108275313_ul2053492417310"></a><a name="zh-cn_topic_0108275365_zh-cn_topic_0108275313_ul2053492417310"></a><ul id="zh-cn_topic_0108275365_zh-cn_topic_0108275313_ul2053492417310"><li>STRING：不带列名，如<span class="uicontrol" id="zh-cn_topic_0108275365_zh-cn_topic_0108275313_uicontrol2441804217642"><a name="zh-cn_topic_0108275365_zh-cn_topic_0108275313_uicontrol2441804217642"></a><a name="zh-cn_topic_0108275365_zh-cn_topic_0108275313_uicontrol2441804217642"></a>“值1，值2”</span>形式。</li><li>HASH：带列名，如<span class="uicontrol" id="zh-cn_topic_0108275365_zh-cn_topic_0108275313_uicontrol1152225917626"><a name="zh-cn_topic_0108275365_zh-cn_topic_0108275313_uicontrol1152225917626"></a><a name="zh-cn_topic_0108275365_zh-cn_topic_0108275313_uicontrol1152225917626"></a>“列名1=值1，列名2=值2”</span>的形式。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="18.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275365_p1434581421725"><a name="zh-cn_topic_0108275365_p1434581421725"></a><a name="zh-cn_topic_0108275365_p1434581421725"></a>STRING</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275365_row7944229161426"><td class="cellrowborder" valign="top" width="17.28%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275365_p5622495421725"><a name="zh-cn_topic_0108275365_p5622495421725"></a><a name="zh-cn_topic_0108275365_p5622495421725"></a>键分隔符</p>
</td>
<td class="cellrowborder" valign="top" width="63.88%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275365_p5792742121725"><a name="zh-cn_topic_0108275365_p5792742121725"></a><a name="zh-cn_topic_0108275365_p5792742121725"></a>用来分隔关系型数据库的表和列名。</p>
</td>
<td class="cellrowborder" valign="top" width="18.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275365_p6160953321725"><a name="zh-cn_topic_0108275365_p6160953321725"></a><a name="zh-cn_topic_0108275365_p6160953321725"></a>_</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275365_row29581508161426"><td class="cellrowborder" valign="top" width="17.28%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275365_p1751972421725"><a name="zh-cn_topic_0108275365_p1751972421725"></a><a name="zh-cn_topic_0108275365_p1751972421725"></a>值分隔符</p>
</td>
<td class="cellrowborder" valign="top" width="63.88%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275365_p981155421725"><a name="zh-cn_topic_0108275365_p981155421725"></a><a name="zh-cn_topic_0108275365_p981155421725"></a>以STRING方式存储时，列之间的分隔符。</p>
</td>
<td class="cellrowborder" valign="top" width="18.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275365_p5653841621725"><a name="zh-cn_topic_0108275365_p5653841621725"></a><a name="zh-cn_topic_0108275365_p5653841621725"></a>;</p>
</td>
</tr>
</tbody>
</table>

