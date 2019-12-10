# 配置Plugin<a name="dayu_01_0230"></a>

DIS Flume Plugin 分为Source与Sink插件，安装包中的dis-flume-plugin.conf.template文件列出了配置方法，本节介绍各种插件的配置项具体含义。

>![](public_sys-resources/icon-note.gif) **说明：**   
>dis-flume-plugin.conf.template只是一个dis插件的配置样例，并不是实际运行Flume时会读取的配置文件。Flume自身提供了样例配置文件，路径为\{FLUME\_HOME\}/conf/flume-conf.properties.template，其中\{FLUME\_HOME\}是Flume的安装路径，用户可以基于此配置文件修改。  

## 配置DIS Source<a name="zh-cn_topic_0120206024_sdc010a07c78b4a82a7acc8af677303e1"></a>

**表 1**  DIS Source配置项说明

<a name="zh-cn_topic_0120206024_table57792315343"></a>
<table><thead align="left"><tr id="zh-cn_topic_0120206024_row18779123193412"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0120206024_p162781023123415"><a name="zh-cn_topic_0120206024_p162781023123415"></a><a name="zh-cn_topic_0120206024_p162781023123415"></a>配置项</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0120206024_p10278192333419"><a name="zh-cn_topic_0120206024_p10278192333419"></a><a name="zh-cn_topic_0120206024_p10278192333419"></a>是否必填</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0120206024_p122781123153418"><a name="zh-cn_topic_0120206024_p122781123153418"></a><a name="zh-cn_topic_0120206024_p122781123153418"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0120206024_p1027862316345"><a name="zh-cn_topic_0120206024_p1027862316345"></a><a name="zh-cn_topic_0120206024_p1027862316345"></a>默认值</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0120206024_row12779338344"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0120206024_p142983593412"><a name="zh-cn_topic_0120206024_p142983593412"></a><a name="zh-cn_topic_0120206024_p142983593412"></a>channels</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0120206024_p19294353341"><a name="zh-cn_topic_0120206024_p19294353341"></a><a name="zh-cn_topic_0120206024_p19294353341"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0120206024_p129183518343"><a name="zh-cn_topic_0120206024_p129183518343"></a><a name="zh-cn_topic_0120206024_p129183518343"></a>Flume channel的名称。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0120206024_p42911356345"><a name="zh-cn_topic_0120206024_p42911356345"></a><a name="zh-cn_topic_0120206024_p42911356345"></a>请根据实际情况配置</p>
</td>
</tr>
<tr id="zh-cn_topic_0120206024_row15779183193414"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0120206024_p82781479341"><a name="zh-cn_topic_0120206024_p82781479341"></a><a name="zh-cn_topic_0120206024_p82781479341"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0120206024_p1227810478341"><a name="zh-cn_topic_0120206024_p1227810478341"></a><a name="zh-cn_topic_0120206024_p1227810478341"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0120206024_p627824763410"><a name="zh-cn_topic_0120206024_p627824763410"></a><a name="zh-cn_topic_0120206024_p627824763410"></a>Source的类型。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0120206024_p14157133921311"><a name="zh-cn_topic_0120206024_p14157133921311"></a><a name="zh-cn_topic_0120206024_p14157133921311"></a>com.huaweicloud.dis.adapter.flume.source.DISSource</p>
</td>
</tr>
<tr id="zh-cn_topic_0120206024_row4779153103415"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0120206024_p21363573617"><a name="zh-cn_topic_0120206024_p21363573617"></a><a name="zh-cn_topic_0120206024_p21363573617"></a>streams</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0120206024_p813193513369"><a name="zh-cn_topic_0120206024_p813193513369"></a><a name="zh-cn_topic_0120206024_p813193513369"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0120206024_p61343515363"><a name="zh-cn_topic_0120206024_p61343515363"></a><a name="zh-cn_topic_0120206024_p61343515363"></a>指定在DIS服务上创建的通道名称。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0120206024_p2131935163612"><a name="zh-cn_topic_0120206024_p2131935163612"></a><a name="zh-cn_topic_0120206024_p2131935163612"></a>与DIS控制台“购买接入通道”时配置的“通道名称”取值一致。</p>
</td>
</tr>
<tr id="zh-cn_topic_0120206024_row37792393418"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0120206024_p13310104173813"><a name="zh-cn_topic_0120206024_p13310104173813"></a><a name="zh-cn_topic_0120206024_p13310104173813"></a>ak</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0120206024_p9326134110388"><a name="zh-cn_topic_0120206024_p9326134110388"></a><a name="zh-cn_topic_0120206024_p9326134110388"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0120206024_p532664183816"><a name="zh-cn_topic_0120206024_p532664183816"></a><a name="zh-cn_topic_0120206024_p532664183816"></a>用户的Access Key。</p>
<p id="zh-cn_topic_0120206024_p10326441193817"><a name="zh-cn_topic_0120206024_p10326441193817"></a><a name="zh-cn_topic_0120206024_p10326441193817"></a>获取方式请参见<a href="安装DIS-Flume-Plugin前准备.md#zh-cn_topic_0120206067_section65401174173650">检查认证信息</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0120206024_p132694193818"><a name="zh-cn_topic_0120206024_p132694193818"></a><a name="zh-cn_topic_0120206024_p132694193818"></a>请根据实际情况配置</p>
</td>
</tr>
<tr id="zh-cn_topic_0120206024_row3779038348"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0120206024_p3326441163810"><a name="zh-cn_topic_0120206024_p3326441163810"></a><a name="zh-cn_topic_0120206024_p3326441163810"></a>sk</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0120206024_p93267415385"><a name="zh-cn_topic_0120206024_p93267415385"></a><a name="zh-cn_topic_0120206024_p93267415385"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0120206024_p2032674115381"><a name="zh-cn_topic_0120206024_p2032674115381"></a><a name="zh-cn_topic_0120206024_p2032674115381"></a>用户的Secret Key。</p>
<p id="zh-cn_topic_0120206024_p43261141173812"><a name="zh-cn_topic_0120206024_p43261141173812"></a><a name="zh-cn_topic_0120206024_p43261141173812"></a>获取方式请参见<a href="安装DIS-Flume-Plugin前准备.md#zh-cn_topic_0120206067_section65401174173650">检查认证信息</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0120206024_p14342164143819"><a name="zh-cn_topic_0120206024_p14342164143819"></a><a name="zh-cn_topic_0120206024_p14342164143819"></a>请根据实际情况配置</p>
</td>
</tr>
<tr id="zh-cn_topic_0120206024_row1779103143417"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0120206024_p1134220418386"><a name="zh-cn_topic_0120206024_p1134220418386"></a><a name="zh-cn_topic_0120206024_p1134220418386"></a>region</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0120206024_p1734234113816"><a name="zh-cn_topic_0120206024_p1734234113816"></a><a name="zh-cn_topic_0120206024_p1734234113816"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0120206024_p73421441113819"><a name="zh-cn_topic_0120206024_p73421441113819"></a><a name="zh-cn_topic_0120206024_p73421441113819"></a>将数据上传到指定Region的DIS服务。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0120206024_p938952855413"><a name="zh-cn_topic_0120206024_p938952855413"></a><a name="zh-cn_topic_0120206024_p938952855413"></a>请根据实际情况配置</p>
</td>
</tr>
<tr id="zh-cn_topic_0120206024_row777910314344"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0120206024_p13575414385"><a name="zh-cn_topic_0120206024_p13575414385"></a><a name="zh-cn_topic_0120206024_p13575414385"></a>projectId</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0120206024_p83577412388"><a name="zh-cn_topic_0120206024_p83577412388"></a><a name="zh-cn_topic_0120206024_p83577412388"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0120206024_p1035764115386"><a name="zh-cn_topic_0120206024_p1035764115386"></a><a name="zh-cn_topic_0120206024_p1035764115386"></a>用户所属区域的项目ID。</p>
<p id="zh-cn_topic_0120206024_p1335711419383"><a name="zh-cn_topic_0120206024_p1335711419383"></a><a name="zh-cn_topic_0120206024_p1335711419383"></a>获取方式请参见<a href="安装DIS-Flume-Plugin前准备.md#zh-cn_topic_0120206067_section65401174173650">检查认证信息</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0120206024_p83571641193816"><a name="zh-cn_topic_0120206024_p83571641193816"></a><a name="zh-cn_topic_0120206024_p83571641193816"></a>请根据实际情况配置</p>
</td>
</tr>
<tr id="zh-cn_topic_0120206024_row11873153118377"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0120206024_p16357184113818"><a name="zh-cn_topic_0120206024_p16357184113818"></a><a name="zh-cn_topic_0120206024_p16357184113818"></a>endpoint</p>
<p id="zh-cn_topic_0120206024_p16372174143815"><a name="zh-cn_topic_0120206024_p16372174143815"></a><a name="zh-cn_topic_0120206024_p16372174143815"></a></p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0120206024_p2037234118382"><a name="zh-cn_topic_0120206024_p2037234118382"></a><a name="zh-cn_topic_0120206024_p2037234118382"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0120206024_p113721941103811"><a name="zh-cn_topic_0120206024_p113721941103811"></a><a name="zh-cn_topic_0120206024_p113721941103811"></a>DIS对应Region的数据接口地址。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0120206024_p13587036556"><a name="zh-cn_topic_0120206024_p13587036556"></a><a name="zh-cn_topic_0120206024_p13587036556"></a>请根据实际情况配置</p>
</td>
</tr>
<tr id="zh-cn_topic_0120206024_row7284529385"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0120206024_p13288521382"><a name="zh-cn_topic_0120206024_p13288521382"></a><a name="zh-cn_topic_0120206024_p13288521382"></a>group.id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0120206024_p42835211381"><a name="zh-cn_topic_0120206024_p42835211381"></a><a name="zh-cn_topic_0120206024_p42835211381"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0120206024_p112091820428"><a name="zh-cn_topic_0120206024_p112091820428"></a><a name="zh-cn_topic_0120206024_p112091820428"></a>DIS App名称，用于标识一个消费组，由英文字符、数字、-、_组成。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0120206024_p7120218174210"><a name="zh-cn_topic_0120206024_p7120218174210"></a><a name="zh-cn_topic_0120206024_p7120218174210"></a>请根据实际情况配置</p>
</td>
</tr>
</tbody>
</table>

## 配置DIS Sink<a name="zh-cn_topic_0120206024_section144801213114319"></a>

**表 2**  DIS Sink配置项说明

<a name="zh-cn_topic_0120206024_table1440315456433"></a>
<table><thead align="left"><tr id="zh-cn_topic_0120206024_row17403164516438"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0120206024_p15137201113465"><a name="zh-cn_topic_0120206024_p15137201113465"></a><a name="zh-cn_topic_0120206024_p15137201113465"></a>配置项</p>
</th>
<th class="cellrowborder" valign="top" width="13.55%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0120206024_p16137911154611"><a name="zh-cn_topic_0120206024_p16137911154611"></a><a name="zh-cn_topic_0120206024_p16137911154611"></a>是否必填</p>
</th>
<th class="cellrowborder" valign="top" width="36.449999999999996%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0120206024_p013713116469"><a name="zh-cn_topic_0120206024_p013713116469"></a><a name="zh-cn_topic_0120206024_p013713116469"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0120206024_p1813718114462"><a name="zh-cn_topic_0120206024_p1813718114462"></a><a name="zh-cn_topic_0120206024_p1813718114462"></a>默认值</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0120206024_row13403114516433"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0120206024_p777882120402"><a name="zh-cn_topic_0120206024_p777882120402"></a><a name="zh-cn_topic_0120206024_p777882120402"></a>channel</p>
</td>
<td class="cellrowborder" valign="top" width="13.55%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0120206024_p41845399462"><a name="zh-cn_topic_0120206024_p41845399462"></a><a name="zh-cn_topic_0120206024_p41845399462"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="36.449999999999996%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0120206024_p111841839164615"><a name="zh-cn_topic_0120206024_p111841839164615"></a><a name="zh-cn_topic_0120206024_p111841839164615"></a>Flume channel的名称。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0120206024_p19184839184619"><a name="zh-cn_topic_0120206024_p19184839184619"></a><a name="zh-cn_topic_0120206024_p19184839184619"></a>请根据实际情况配置</p>
</td>
</tr>
<tr id="zh-cn_topic_0120206024_row440354514436"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0120206024_p61162016124015"><a name="zh-cn_topic_0120206024_p61162016124015"></a><a name="zh-cn_topic_0120206024_p61162016124015"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13.55%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0120206024_p2184173944614"><a name="zh-cn_topic_0120206024_p2184173944614"></a><a name="zh-cn_topic_0120206024_p2184173944614"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="36.449999999999996%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0120206024_p1184173964619"><a name="zh-cn_topic_0120206024_p1184173964619"></a><a name="zh-cn_topic_0120206024_p1184173964619"></a>Sink的类型。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0120206024_p118769815144"><a name="zh-cn_topic_0120206024_p118769815144"></a><a name="zh-cn_topic_0120206024_p118769815144"></a>com.huaweicloud.dis.adapter.flume.sink.DISSink</p>
</td>
</tr>
<tr id="zh-cn_topic_0120206024_row240394518430"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0120206024_p101841139184616"><a name="zh-cn_topic_0120206024_p101841139184616"></a><a name="zh-cn_topic_0120206024_p101841139184616"></a>streamName</p>
</td>
<td class="cellrowborder" valign="top" width="13.55%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0120206024_p151842397466"><a name="zh-cn_topic_0120206024_p151842397466"></a><a name="zh-cn_topic_0120206024_p151842397466"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="36.449999999999996%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0120206024_p61845398469"><a name="zh-cn_topic_0120206024_p61845398469"></a><a name="zh-cn_topic_0120206024_p61845398469"></a>指定在DIS服务上创建的通道名称。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0120206024_p1118417390469"><a name="zh-cn_topic_0120206024_p1118417390469"></a><a name="zh-cn_topic_0120206024_p1118417390469"></a>与DIS控制台“购买接入通道”时配置的“通道名称”取值一致。</p>
</td>
</tr>
<tr id="zh-cn_topic_0120206024_row17403745114311"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0120206024_p618410396466"><a name="zh-cn_topic_0120206024_p618410396466"></a><a name="zh-cn_topic_0120206024_p618410396466"></a>ak</p>
</td>
<td class="cellrowborder" valign="top" width="13.55%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0120206024_p1018443915462"><a name="zh-cn_topic_0120206024_p1018443915462"></a><a name="zh-cn_topic_0120206024_p1018443915462"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="36.449999999999996%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0120206024_p161845396464"><a name="zh-cn_topic_0120206024_p161845396464"></a><a name="zh-cn_topic_0120206024_p161845396464"></a>用户的Access Key。</p>
<p id="zh-cn_topic_0120206024_p151841539174618"><a name="zh-cn_topic_0120206024_p151841539174618"></a><a name="zh-cn_topic_0120206024_p151841539174618"></a>获取方式请参见<a href="安装DIS-Flume-Plugin前准备.md#zh-cn_topic_0120206067_section65401174173650">检查认证信息</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0120206024_p1518414398467"><a name="zh-cn_topic_0120206024_p1518414398467"></a><a name="zh-cn_topic_0120206024_p1518414398467"></a>请根据实际情况配置</p>
</td>
</tr>
<tr id="zh-cn_topic_0120206024_row1440324594314"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0120206024_p1184639204610"><a name="zh-cn_topic_0120206024_p1184639204610"></a><a name="zh-cn_topic_0120206024_p1184639204610"></a>sk</p>
</td>
<td class="cellrowborder" valign="top" width="13.55%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0120206024_p61841739104611"><a name="zh-cn_topic_0120206024_p61841739104611"></a><a name="zh-cn_topic_0120206024_p61841739104611"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="36.449999999999996%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0120206024_p51842391463"><a name="zh-cn_topic_0120206024_p51842391463"></a><a name="zh-cn_topic_0120206024_p51842391463"></a>用户的Secret Key。</p>
<p id="zh-cn_topic_0120206024_p11184439104620"><a name="zh-cn_topic_0120206024_p11184439104620"></a><a name="zh-cn_topic_0120206024_p11184439104620"></a>获取方式请参见<a href="安装DIS-Flume-Plugin前准备.md#zh-cn_topic_0120206067_section65401174173650">检查认证信息</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0120206024_p1118463964613"><a name="zh-cn_topic_0120206024_p1118463964613"></a><a name="zh-cn_topic_0120206024_p1118463964613"></a>请根据实际情况配置</p>
</td>
</tr>
<tr id="zh-cn_topic_0120206024_row540364515439"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0120206024_p1518419393467"><a name="zh-cn_topic_0120206024_p1518419393467"></a><a name="zh-cn_topic_0120206024_p1518419393467"></a>region</p>
</td>
<td class="cellrowborder" valign="top" width="13.55%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0120206024_p11841539114617"><a name="zh-cn_topic_0120206024_p11841539114617"></a><a name="zh-cn_topic_0120206024_p11841539114617"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="36.449999999999996%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0120206024_p418433911465"><a name="zh-cn_topic_0120206024_p418433911465"></a><a name="zh-cn_topic_0120206024_p418433911465"></a>将数据上传到指定Region的DIS服务。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0120206024_p161848392464"><a name="zh-cn_topic_0120206024_p161848392464"></a><a name="zh-cn_topic_0120206024_p161848392464"></a>cn-north-1</p>
</td>
</tr>
<tr id="zh-cn_topic_0120206024_row124031745174315"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0120206024_p7184113964610"><a name="zh-cn_topic_0120206024_p7184113964610"></a><a name="zh-cn_topic_0120206024_p7184113964610"></a>projectId</p>
</td>
<td class="cellrowborder" valign="top" width="13.55%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0120206024_p141848395469"><a name="zh-cn_topic_0120206024_p141848395469"></a><a name="zh-cn_topic_0120206024_p141848395469"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="36.449999999999996%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0120206024_p91844398464"><a name="zh-cn_topic_0120206024_p91844398464"></a><a name="zh-cn_topic_0120206024_p91844398464"></a>用户所属区域的项目ID。</p>
<p id="zh-cn_topic_0120206024_p20184239184617"><a name="zh-cn_topic_0120206024_p20184239184617"></a><a name="zh-cn_topic_0120206024_p20184239184617"></a>获取方式请参见<a href="安装DIS-Flume-Plugin前准备.md#zh-cn_topic_0120206067_section65401174173650">检查认证信息</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0120206024_p61842391462"><a name="zh-cn_topic_0120206024_p61842391462"></a><a name="zh-cn_topic_0120206024_p61842391462"></a>请根据实际情况配置</p>
</td>
</tr>
<tr id="zh-cn_topic_0120206024_row184341858458"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0120206024_p01841139194616"><a name="zh-cn_topic_0120206024_p01841139194616"></a><a name="zh-cn_topic_0120206024_p01841139194616"></a>endpoint</p>
</td>
<td class="cellrowborder" valign="top" width="13.55%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0120206024_p131840392469"><a name="zh-cn_topic_0120206024_p131840392469"></a><a name="zh-cn_topic_0120206024_p131840392469"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="36.449999999999996%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0120206024_p141848394461"><a name="zh-cn_topic_0120206024_p141848394461"></a><a name="zh-cn_topic_0120206024_p141848394461"></a>DIS对应Region的数据接口地址。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0120206024_p3184163914612"><a name="zh-cn_topic_0120206024_p3184163914612"></a><a name="zh-cn_topic_0120206024_p3184163914612"></a>https://dis.cn-north-1.myhuaweicloud.com</p>
</td>
</tr>
<tr id="zh-cn_topic_0120206024_row25121310104515"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0120206024_p15184239164616"><a name="zh-cn_topic_0120206024_p15184239164616"></a><a name="zh-cn_topic_0120206024_p15184239164616"></a>partitionNumber</p>
</td>
<td class="cellrowborder" valign="top" width="13.55%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0120206024_p1818423916464"><a name="zh-cn_topic_0120206024_p1818423916464"></a><a name="zh-cn_topic_0120206024_p1818423916464"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="36.449999999999996%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0120206024_p11184203904616"><a name="zh-cn_topic_0120206024_p11184203904616"></a><a name="zh-cn_topic_0120206024_p11184203904616"></a>通道的分区数量。</p>
<p id="zh-cn_topic_0120206024_p61841539154615"><a name="zh-cn_topic_0120206024_p61841539154615"></a><a name="zh-cn_topic_0120206024_p61841539154615"></a>用于计算batchSize的大小。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0120206024_p13184103916469"><a name="zh-cn_topic_0120206024_p13184103916469"></a><a name="zh-cn_topic_0120206024_p13184103916469"></a>1</p>
</td>
</tr>
<tr id="zh-cn_topic_0120206024_row97461143154511"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0120206024_p0184939124619"><a name="zh-cn_topic_0120206024_p0184939124619"></a><a name="zh-cn_topic_0120206024_p0184939124619"></a>batchSize</p>
</td>
<td class="cellrowborder" valign="top" width="13.55%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0120206024_p1818414398465"><a name="zh-cn_topic_0120206024_p1818414398465"></a><a name="zh-cn_topic_0120206024_p1818414398465"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="36.449999999999996%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0120206024_p718443994615"><a name="zh-cn_topic_0120206024_p718443994615"></a><a name="zh-cn_topic_0120206024_p718443994615"></a>一个Flume事务内批量处理的数据集大小。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0120206024_p101841439134619"><a name="zh-cn_topic_0120206024_p101841439134619"></a><a name="zh-cn_topic_0120206024_p101841439134619"></a>（“partitionNumber”配置的值）*250</p>
</td>
</tr>
<tr id="zh-cn_topic_0120206024_row7215135514513"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0120206024_p1418443914460"><a name="zh-cn_topic_0120206024_p1418443914460"></a><a name="zh-cn_topic_0120206024_p1418443914460"></a>sendingThreadSize</p>
</td>
<td class="cellrowborder" valign="top" width="13.55%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0120206024_p8184439114613"><a name="zh-cn_topic_0120206024_p8184439114613"></a><a name="zh-cn_topic_0120206024_p8184439114613"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="36.449999999999996%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0120206024_p191841139154610"><a name="zh-cn_topic_0120206024_p191841139154610"></a><a name="zh-cn_topic_0120206024_p191841139154610"></a>发送线程数。默认单线程发送。</p>
<div class="note" id="zh-cn_topic_0120206024_note360613812464"><a name="zh-cn_topic_0120206024_note360613812464"></a><a name="zh-cn_topic_0120206024_note360613812464"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0120206024_p41841239104610"><a name="zh-cn_topic_0120206024_p41841239104610"></a><a name="zh-cn_topic_0120206024_p41841239104610"></a>使用多线程会出现如下情况：</p>
<a name="zh-cn_topic_0120206024_ul4184183904620"></a><a name="zh-cn_topic_0120206024_ul4184183904620"></a><ul id="zh-cn_topic_0120206024_ul4184183904620"><li>发送不保证顺序。</li><li>当程序从异常停止恢复时重传部分数据。</li></ul>
</div></div>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0120206024_p71841239144611"><a name="zh-cn_topic_0120206024_p71841239144611"></a><a name="zh-cn_topic_0120206024_p71841239144611"></a>1</p>
</td>
</tr>
<tr id="zh-cn_topic_0120206024_row1573195184511"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0120206024_p13184153994613"><a name="zh-cn_topic_0120206024_p13184153994613"></a><a name="zh-cn_topic_0120206024_p13184153994613"></a>sendingRecordSize</p>
</td>
<td class="cellrowborder" valign="top" width="13.55%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0120206024_p1018417394463"><a name="zh-cn_topic_0120206024_p1018417394463"></a><a name="zh-cn_topic_0120206024_p1018417394463"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="36.449999999999996%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0120206024_p161846396463"><a name="zh-cn_topic_0120206024_p161846396463"></a><a name="zh-cn_topic_0120206024_p161846396463"></a>单次调用DIS数据发送接口时的数据集大小。</p>
<div class="note" id="zh-cn_topic_0120206024_note86211138154613"><a name="zh-cn_topic_0120206024_note86211138154613"></a><a name="zh-cn_topic_0120206024_note86211138154613"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0120206024_p11341320102119"><a name="zh-cn_topic_0120206024_p11341320102119"></a><a name="zh-cn_topic_0120206024_p11341320102119"></a>“batchSize”表示一个事务的批量值(如1000)，而“sendingRecordSize”表示一个Rest请求的批量值(如250表示会发起四次请求)。当“batchSize”的数据全部发送成功之后，才会完成Flume的事务，否则事务不提交，重启时导致数据重传。当“sendingThreadSize”配置为“1”时，表示“sendingRecordSize”与“batchSize”配置相同值，避免数据重新上传。</p>
</div></div>
<p id="zh-cn_topic_0120206024_p121849391464"><a name="zh-cn_topic_0120206024_p121849391464"></a><a name="zh-cn_topic_0120206024_p121849391464"></a></p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0120206024_p12184123914611"><a name="zh-cn_topic_0120206024_p12184123914611"></a><a name="zh-cn_topic_0120206024_p12184123914611"></a>250</p>
</td>
</tr>
<tr id="zh-cn_topic_0120206024_row28401247174517"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0120206024_p1118423994613"><a name="zh-cn_topic_0120206024_p1118423994613"></a><a name="zh-cn_topic_0120206024_p1118423994613"></a>retrySize</p>
</td>
<td class="cellrowborder" valign="top" width="13.55%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0120206024_p418443974618"><a name="zh-cn_topic_0120206024_p418443974618"></a><a name="zh-cn_topic_0120206024_p418443974618"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="36.449999999999996%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0120206024_p4184839194610"><a name="zh-cn_topic_0120206024_p4184839194610"></a><a name="zh-cn_topic_0120206024_p4184839194610"></a>Sink程序调用DIS接口异常时尝试重新调用的次数。</p>
<p id="zh-cn_topic_0120206024_p718415397467"><a name="zh-cn_topic_0120206024_p718415397467"></a><a name="zh-cn_topic_0120206024_p718415397467"></a>建议使用默认值2147483647，表示会无限重试。</p>
<p id="zh-cn_topic_0120206024_p1718443916469"><a name="zh-cn_topic_0120206024_p1718443916469"></a><a name="zh-cn_topic_0120206024_p1718443916469"></a>重试时会使用指数退避算法，并等待一段时间，以减轻异常时服务器压力。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0120206024_p11847393461"><a name="zh-cn_topic_0120206024_p11847393461"></a><a name="zh-cn_topic_0120206024_p11847393461"></a>2147483647</p>
</td>
</tr>
<tr id="zh-cn_topic_0120206024_row629353512452"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0120206024_p0184239144610"><a name="zh-cn_topic_0120206024_p0184239144610"></a><a name="zh-cn_topic_0120206024_p0184239144610"></a>resultLogLevel</p>
</td>
<td class="cellrowborder" valign="top" width="13.55%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0120206024_p818412393461"><a name="zh-cn_topic_0120206024_p818412393461"></a><a name="zh-cn_topic_0120206024_p818412393461"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="36.449999999999996%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0120206024_p1618473916461"><a name="zh-cn_topic_0120206024_p1618473916461"></a><a name="zh-cn_topic_0120206024_p1618473916461"></a>每次调用DIS接口后输出最新sequenceNumber到日志的级别。</p>
<p id="zh-cn_topic_0120206024_p118493915462"><a name="zh-cn_topic_0120206024_p118493915462"></a><a name="zh-cn_topic_0120206024_p118493915462"></a>有效值与级别由低到高为 OFF &lt; DEBUG &lt; INFO &lt; WARN &lt; ERROR。</p>
<p id="zh-cn_topic_0120206024_p3184173919465"><a name="zh-cn_topic_0120206024_p3184173919465"></a><a name="zh-cn_topic_0120206024_p3184173919465"></a>OFF：不输出日志。</p>
<p id="zh-cn_topic_0120206024_p2018413924614"><a name="zh-cn_topic_0120206024_p2018413924614"></a><a name="zh-cn_topic_0120206024_p2018413924614"></a>如果Flume log4j配置的日志级别高于resultLogLevel配置的的值，则日志也不会输出。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0120206024_p14184139114619"><a name="zh-cn_topic_0120206024_p14184139114619"></a><a name="zh-cn_topic_0120206024_p14184139114619"></a>OFF</p>
</td>
</tr>
<tr id="zh-cn_topic_0120206024_row116213396454"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0120206024_p418423994614"><a name="zh-cn_topic_0120206024_p418423994614"></a><a name="zh-cn_topic_0120206024_p418423994614"></a>maxBufferAgeMillis</p>
</td>
<td class="cellrowborder" valign="top" width="13.55%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0120206024_p1918493915465"><a name="zh-cn_topic_0120206024_p1918493915465"></a><a name="zh-cn_topic_0120206024_p1918493915465"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="36.449999999999996%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0120206024_p18184239114612"><a name="zh-cn_topic_0120206024_p18184239114612"></a><a name="zh-cn_topic_0120206024_p18184239114612"></a>最长上传等待时间。</p>
<p id="zh-cn_topic_0120206024_p51841639174615"><a name="zh-cn_topic_0120206024_p51841639174615"></a><a name="zh-cn_topic_0120206024_p51841639174615"></a>单位：毫秒</p>
<a name="zh-cn_topic_0120206024_ul1218433944614"></a><a name="zh-cn_topic_0120206024_ul1218433944614"></a><ul id="zh-cn_topic_0120206024_ul1218433944614"><li>记录队列满则立即上传。</li><li>记录队列未满，等待此配</li></ul>
<p id="zh-cn_topic_0120206024_p1718415398461"><a name="zh-cn_topic_0120206024_p1718415398461"></a><a name="zh-cn_topic_0120206024_p1718415398461"></a>置项配置的时间后上传。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0120206024_p01841439124610"><a name="zh-cn_topic_0120206024_p01841439124610"></a><a name="zh-cn_topic_0120206024_p01841439124610"></a>5000</p>
</td>
</tr>
<tr id="zh-cn_topic_0120206024_row1243181611458"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0120206024_p2018416398467"><a name="zh-cn_topic_0120206024_p2018416398467"></a><a name="zh-cn_topic_0120206024_p2018416398467"></a>connectionTimeOutSeconds</p>
</td>
<td class="cellrowborder" valign="top" width="13.55%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0120206024_p121845399465"><a name="zh-cn_topic_0120206024_p121845399465"></a><a name="zh-cn_topic_0120206024_p121845399465"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="36.449999999999996%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0120206024_p118419398468"><a name="zh-cn_topic_0120206024_p118419398468"></a><a name="zh-cn_topic_0120206024_p118419398468"></a>连接DIS接口超时时间。</p>
<p id="zh-cn_topic_0120206024_p9184639174618"><a name="zh-cn_topic_0120206024_p9184639174618"></a><a name="zh-cn_topic_0120206024_p9184639174618"></a>单位：秒。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0120206024_p12184439144611"><a name="zh-cn_topic_0120206024_p12184439144611"></a><a name="zh-cn_topic_0120206024_p12184439144611"></a>30</p>
</td>
</tr>
<tr id="zh-cn_topic_0120206024_row181201825144510"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0120206024_p15184039194611"><a name="zh-cn_topic_0120206024_p15184039194611"></a><a name="zh-cn_topic_0120206024_p15184039194611"></a>socketTimeOutSeconds</p>
</td>
<td class="cellrowborder" valign="top" width="13.55%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0120206024_p71841739124613"><a name="zh-cn_topic_0120206024_p71841739124613"></a><a name="zh-cn_topic_0120206024_p71841739124613"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="36.449999999999996%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0120206024_p6184173911463"><a name="zh-cn_topic_0120206024_p6184173911463"></a><a name="zh-cn_topic_0120206024_p6184173911463"></a>接口响应超时时间。</p>
<p id="zh-cn_topic_0120206024_p7184173916467"><a name="zh-cn_topic_0120206024_p7184173916467"></a><a name="zh-cn_topic_0120206024_p7184173916467"></a>单位：秒。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0120206024_p8184153915469"><a name="zh-cn_topic_0120206024_p8184153915469"></a><a name="zh-cn_topic_0120206024_p8184153915469"></a>60</p>
</td>
</tr>
<tr id="zh-cn_topic_0120206024_row1896532911453"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0120206024_p1218463944618"><a name="zh-cn_topic_0120206024_p1218463944618"></a><a name="zh-cn_topic_0120206024_p1218463944618"></a>dataEncryptEnabled</p>
</td>
<td class="cellrowborder" valign="top" width="13.55%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0120206024_p3184163974616"><a name="zh-cn_topic_0120206024_p3184163974616"></a><a name="zh-cn_topic_0120206024_p3184163974616"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="36.449999999999996%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0120206024_p10184133984617"><a name="zh-cn_topic_0120206024_p10184133984617"></a><a name="zh-cn_topic_0120206024_p10184133984617"></a>数据是否使用AES加密。</p>
<a name="zh-cn_topic_0120206024_ul1118413912461"></a><a name="zh-cn_topic_0120206024_ul1118413912461"></a><ul id="zh-cn_topic_0120206024_ul1118413912461"><li>是：true。</li><li>否：false。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0120206024_p218443924615"><a name="zh-cn_topic_0120206024_p218443924615"></a><a name="zh-cn_topic_0120206024_p218443924615"></a>false</p>
</td>
</tr>
<tr id="zh-cn_topic_0120206024_row3387202111452"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0120206024_p118473913467"><a name="zh-cn_topic_0120206024_p118473913467"></a><a name="zh-cn_topic_0120206024_p118473913467"></a>dataPassword</p>
</td>
<td class="cellrowborder" valign="top" width="13.55%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0120206024_p7184739164610"><a name="zh-cn_topic_0120206024_p7184739164610"></a><a name="zh-cn_topic_0120206024_p7184739164610"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="36.449999999999996%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0120206024_p16184133974616"><a name="zh-cn_topic_0120206024_p16184133974616"></a><a name="zh-cn_topic_0120206024_p16184133974616"></a>数据加密或解密时使用的密码。</p>
<p id="zh-cn_topic_0120206024_p01846398469"><a name="zh-cn_topic_0120206024_p01846398469"></a><a name="zh-cn_topic_0120206024_p01846398469"></a>当“dataEncryptEnabled”配置项配置为“false”时无需配置“dataPassword”。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0120206024_p15184123984614"><a name="zh-cn_topic_0120206024_p15184123984614"></a><a name="zh-cn_topic_0120206024_p15184123984614"></a>请根据实际情况配置</p>
</td>
</tr>
<tr id="zh-cn_topic_0120206024_row51217264519"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0120206024_p18184133914619"><a name="zh-cn_topic_0120206024_p18184133914619"></a><a name="zh-cn_topic_0120206024_p18184133914619"></a>bodySerializeType</p>
</td>
<td class="cellrowborder" valign="top" width="13.55%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0120206024_p1518414394463"><a name="zh-cn_topic_0120206024_p1518414394463"></a><a name="zh-cn_topic_0120206024_p1518414394463"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="36.449999999999996%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0120206024_p118413984615"><a name="zh-cn_topic_0120206024_p118413984615"></a><a name="zh-cn_topic_0120206024_p118413984615"></a>DIS数据包上传格式(非原始数据格式)。</p>
<a name="zh-cn_topic_0120206024_ul8184173913469"></a><a name="zh-cn_topic_0120206024_ul8184173913469"></a><ul id="zh-cn_topic_0120206024_ul8184173913469"><li>json：DIS数据包封装为json格式，满足普通使用。</li><li>protobuf：DIS数据包封装为二进制格式，可以减少体积约1/3，在数据量较大的情况下推荐使用此格式。</li></ul>
<p id="zh-cn_topic_0120206024_p8184133914467"><a name="zh-cn_topic_0120206024_p8184133914467"></a><a name="zh-cn_topic_0120206024_p8184133914467"></a></p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0120206024_p11184239174610"><a name="zh-cn_topic_0120206024_p11184239174610"></a><a name="zh-cn_topic_0120206024_p11184239174610"></a>json</p>
</td>
</tr>
</tbody>
</table>

