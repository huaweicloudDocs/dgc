# 配置CloudTable连接<a name="dayu_01_0027"></a>

连接CloudTable时，相关参数如[表1](#zh-cn_topic_0108275355_table34037531171418)所示。

**表 1**  CloudTable连接参数

<a name="zh-cn_topic_0108275355_table34037531171418"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108275355_row56630393171418"><th class="cellrowborder" valign="top" width="17.5%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108275355_p23659124171418"><a name="zh-cn_topic_0108275355_p23659124171418"></a><a name="zh-cn_topic_0108275355_p23659124171418"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="61.650000000000006%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108275355_p37340867171418"><a name="zh-cn_topic_0108275355_p37340867171418"></a><a name="zh-cn_topic_0108275355_p37340867171418"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="20.849999999999998%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108275355_p4711375171418"><a name="zh-cn_topic_0108275355_p4711375171418"></a><a name="zh-cn_topic_0108275355_p4711375171418"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108275355_row46077055171418"><td class="cellrowborder" valign="top" width="17.5%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275355_p41253947171418"><a name="zh-cn_topic_0108275355_p41253947171418"></a><a name="zh-cn_topic_0108275355_p41253947171418"></a>名称</p>
</td>
<td class="cellrowborder" valign="top" width="61.650000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275355_p1369564463813"><a name="zh-cn_topic_0108275355_p1369564463813"></a><a name="zh-cn_topic_0108275355_p1369564463813"></a>连接的名称，根据连接的数据源类型，用户可自定义便于记忆、区分的连接名。</p>
</td>
<td class="cellrowborder" valign="top" width="20.849999999999998%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275355_p42147213114142"><a name="zh-cn_topic_0108275355_p42147213114142"></a><a name="zh-cn_topic_0108275355_p42147213114142"></a>cloudtable_link</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275355_row19710159171418"><td class="cellrowborder" valign="top" width="17.5%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275355_p62657656114131"><a name="zh-cn_topic_0108275355_p62657656114131"></a><a name="zh-cn_topic_0108275355_p62657656114131"></a>ZK链接地址</p>
</td>
<td class="cellrowborder" valign="top" width="61.650000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275355_p31524870114139"><a name="zh-cn_topic_0108275355_p31524870114139"></a><a name="zh-cn_topic_0108275355_p31524870114139"></a>可通过CloudTable服务的集群管理界面获取该参数值。</p>
</td>
<td class="cellrowborder" valign="top" width="20.849999999999998%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275355_p4536548114142"><a name="zh-cn_topic_0108275355_p4536548114142"></a><a name="zh-cn_topic_0108275355_p4536548114142"></a>cloudtable-cdm-zk1.cloudtable.com:2181,cloudtable-cdm-zk2.cloudtable.com:2181</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275355_row7494172615386"><td class="cellrowborder" valign="top" width="17.5%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275355_p14496102663811"><a name="zh-cn_topic_0108275355_p14496102663811"></a><a name="zh-cn_topic_0108275355_p14496102663811"></a>IAM统一身份认证</p>
</td>
<td class="cellrowborder" valign="top" width="61.650000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275355_p1849619268381"><a name="zh-cn_topic_0108275355_p1849619268381"></a><a name="zh-cn_topic_0108275355_p1849619268381"></a>当选择IAM统一身份认证时，需要输入用户名、AK和SK。</p>
</td>
<td class="cellrowborder" valign="top" width="20.849999999999998%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275355_p12496926183816"><a name="zh-cn_topic_0108275355_p12496926183816"></a><a name="zh-cn_topic_0108275355_p12496926183816"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275355_row111582914398"><td class="cellrowborder" valign="top" width="17.5%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275355_p1115815917397"><a name="zh-cn_topic_0108275355_p1115815917397"></a><a name="zh-cn_topic_0108275355_p1115815917397"></a>运行模式</p>
</td>
<td class="cellrowborder" valign="top" width="61.650000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275355_p357864774616"><a name="zh-cn_topic_0108275355_p357864774616"></a><a name="zh-cn_topic_0108275355_p357864774616"></a>选择HBase连接的运行模式：</p>
<a name="zh-cn_topic_0108275355_ul2077619371261"></a><a name="zh-cn_topic_0108275355_ul2077619371261"></a><ul id="zh-cn_topic_0108275355_ul2077619371261"><li>EMBEDDED：连接实例与CDM运行在一起，该模式性能较好。</li><li>STANDALONE：连接实例运行在独立进程。如果CDM需要对接多个Hadoop数据源（MRS、Hadoop或CloudTable），并且既有KERBEROS认证模式又有SIMPLE认证模式，只能使用STANDALONE模式或者配置不同的Agent。</li><li>Agent：连接实例运行在Agent上。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="20.849999999999998%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275355_p1421621144410"><a name="zh-cn_topic_0108275355_p1421621144410"></a><a name="zh-cn_topic_0108275355_p1421621144410"></a>EMBEDDED</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275355_row1795014420394"><td class="cellrowborder" valign="top" width="17.5%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275355_p14952184416394"><a name="zh-cn_topic_0108275355_p14952184416394"></a><a name="zh-cn_topic_0108275355_p14952184416394"></a>用户名</p>
</td>
<td class="cellrowborder" valign="top" width="61.650000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275355_p13952124417392"><a name="zh-cn_topic_0108275355_p13952124417392"></a><a name="zh-cn_topic_0108275355_p13952124417392"></a>登录CloudTable集群的用户名。</p>
</td>
<td class="cellrowborder" valign="top" width="20.849999999999998%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275355_p6952644143912"><a name="zh-cn_topic_0108275355_p6952644143912"></a><a name="zh-cn_topic_0108275355_p6952644143912"></a>admin</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275355_row35276451399"><td class="cellrowborder" valign="top" width="17.5%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275355_p1552720455396"><a name="zh-cn_topic_0108275355_p1552720455396"></a><a name="zh-cn_topic_0108275355_p1552720455396"></a>AK</p>
</td>
<td class="cellrowborder" valign="top" width="61.650000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275355_p8527134543910"><a name="zh-cn_topic_0108275355_p8527134543910"></a><a name="zh-cn_topic_0108275355_p8527134543910"></a>登录CloudTable集群的访问标识。</p>
</td>
<td class="cellrowborder" valign="top" width="20.849999999999998%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275355_p1152794519391"><a name="zh-cn_topic_0108275355_p1152794519391"></a><a name="zh-cn_topic_0108275355_p1152794519391"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275355_row16131546183916"><td class="cellrowborder" valign="top" width="17.5%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275355_p41344611390"><a name="zh-cn_topic_0108275355_p41344611390"></a><a name="zh-cn_topic_0108275355_p41344611390"></a>SK</p>
</td>
<td class="cellrowborder" valign="top" width="61.650000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275355_p813194633919"><a name="zh-cn_topic_0108275355_p813194633919"></a><a name="zh-cn_topic_0108275355_p813194633919"></a>登录CloudTable集群的秘钥。</p>
</td>
<td class="cellrowborder" valign="top" width="20.849999999999998%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275355_p21316464393"><a name="zh-cn_topic_0108275355_p21316464393"></a><a name="zh-cn_topic_0108275355_p21316464393"></a>-</p>
</td>
</tr>
</tbody>
</table>

