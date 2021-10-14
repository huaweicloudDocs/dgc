# 配置CloudTable连接<a name="dgc_01_0027"></a>

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
<td class="cellrowborder" valign="top" width="61.650000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275355_p1712015325114"><a name="zh-cn_topic_0108275355_p1712015325114"></a><a name="zh-cn_topic_0108275355_p1712015325114"></a>如果所需连接的CloudTable集群在创建时开启了<span class="parmname" id="zh-cn_topic_0108275355_parmname6621256019"><a name="zh-cn_topic_0108275355_parmname6621256019"></a><a name="zh-cn_topic_0108275355_parmname6621256019"></a>“IAM统一身份认证”</span>，该参数需设置为<span class="parmvalue" id="zh-cn_topic_0108275355_parmvalue978203214523"><a name="zh-cn_topic_0108275355_parmvalue978203214523"></a><a name="zh-cn_topic_0108275355_parmvalue978203214523"></a>“是”</span>，否则设置为<span class="parmvalue" id="zh-cn_topic_0108275355_parmvalue17601034125214"><a name="zh-cn_topic_0108275355_parmvalue17601034125214"></a><a name="zh-cn_topic_0108275355_parmvalue17601034125214"></a>“否”</span>。</p>
<p id="zh-cn_topic_0108275355_p1849619268381"><a name="zh-cn_topic_0108275355_p1849619268381"></a><a name="zh-cn_topic_0108275355_p1849619268381"></a>当选择IAM统一身份认证时，需要输入用户名、AK和SK。</p>
</td>
<td class="cellrowborder" valign="top" width="20.849999999999998%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275355_p12496926183816"><a name="zh-cn_topic_0108275355_p12496926183816"></a><a name="zh-cn_topic_0108275355_p12496926183816"></a>否</p>
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
<p id="zh-cn_topic_0108275355_p2396698815212"><a name="zh-cn_topic_0108275355_p2396698815212"></a><a name="zh-cn_topic_0108275355_p2396698815212"></a>您需要先创建当前账号的访问密钥，并获得对应的AK和SK。</p>
</td>
<td class="cellrowborder" valign="top" width="20.849999999999998%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275355_p1152794519391"><a name="zh-cn_topic_0108275355_p1152794519391"></a><a name="zh-cn_topic_0108275355_p1152794519391"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275355_row16131546183916"><td class="cellrowborder" valign="top" width="17.5%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275355_p41344611390"><a name="zh-cn_topic_0108275355_p41344611390"></a><a name="zh-cn_topic_0108275355_p41344611390"></a>SK</p>
</td>
<td class="cellrowborder" valign="top" width="61.650000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275355_p813194633919"><a name="zh-cn_topic_0108275355_p813194633919"></a><a name="zh-cn_topic_0108275355_p813194633919"></a>登录CloudTable集群的密钥。</p>
<p id="zh-cn_topic_0108275355_p01204209218"><a name="zh-cn_topic_0108275355_p01204209218"></a><a name="zh-cn_topic_0108275355_p01204209218"></a>您需要先创建当前账号的访问密钥，并获得对应的AK和SK。</p>
</td>
<td class="cellrowborder" valign="top" width="20.849999999999998%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275355_p21316464393"><a name="zh-cn_topic_0108275355_p21316464393"></a><a name="zh-cn_topic_0108275355_p21316464393"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275355_row1474555371514"><td class="cellrowborder" valign="top" width="17.5%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275355_p1386613414718"><a name="zh-cn_topic_0108275355_p1386613414718"></a><a name="zh-cn_topic_0108275355_p1386613414718"></a>是否使用集群配置</p>
</td>
<td class="cellrowborder" valign="top" width="61.650000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275355_p188661341078"><a name="zh-cn_topic_0108275355_p188661341078"></a><a name="zh-cn_topic_0108275355_p188661341078"></a>您可以通过使用集群配置，简化Hadoop连接参数配置。</p>
</td>
<td class="cellrowborder" valign="top" width="20.849999999999998%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275355_p986610420717"><a name="zh-cn_topic_0108275355_p986610420717"></a><a name="zh-cn_topic_0108275355_p986610420717"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275355_row3953125531519"><td class="cellrowborder" valign="top" width="17.5%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275355_p20866946711"><a name="zh-cn_topic_0108275355_p20866946711"></a><a name="zh-cn_topic_0108275355_p20866946711"></a>集群配置名</p>
</td>
<td class="cellrowborder" valign="top" width="61.650000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275355_p15866341979"><a name="zh-cn_topic_0108275355_p15866341979"></a><a name="zh-cn_topic_0108275355_p15866341979"></a>仅当“是否使用集群配置”为“是”时，此参数有效。此参数用于选择用户已经创建好的集群配置。</p>
<p id="zh-cn_topic_0108275355_p1786610418710"><a name="zh-cn_topic_0108275355_p1786610418710"></a><a name="zh-cn_topic_0108275355_p1786610418710"></a>集群配置的创建方法请参见<a href="管理集群配置.md#dgc_01_1096">管理集群配置</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="20.849999999999998%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275355_p1210410291174"><a name="zh-cn_topic_0108275355_p1210410291174"></a><a name="zh-cn_topic_0108275355_p1210410291174"></a>hadoop_01</p>
</td>
</tr>
</tbody>
</table>

单击“显示高级属性“，然后单击“添加“，您可以添加客户端的配置属性。所添加的每个属性需配置属性名称和值。对于不再需要的属性，可单击属性后的“删除“按钮进行删除。

