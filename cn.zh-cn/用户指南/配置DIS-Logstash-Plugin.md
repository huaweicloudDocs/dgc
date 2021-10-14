# 配置DIS Logstash Plugin<a name="dgc_01_0239"></a>

DIS Logstash Plugins 分为Input与Output插件，本节介绍插件的各个配置项具体含义。

## 配置DIS Logstash Input<a name="zh-cn_topic_0194140892_section627651944620"></a>

配置模板如下：（该模板为从DIS通道下载数据写入本地文件）

```
input
{
   dis {
        streams => ["YOU_DIS_STREAM_NAME"]
        endpoint => "https://${endpoint}"
        ak => "YOU_ACCESS_KEY_ID"
        sk => "YOU_SECRET_KEY_ID"
        region => "${region}"
        project_id => "YOU_PROJECT_ID"
        group_id => "YOU_APP_ID"
        auto_offset_reset => "earliest"
    }
}
output
{
    file {
       path => ["/tmp/test.log"]
   }
}
```

**表 1**  DIS Logstash Input配置项说明

<a name="zh-cn_topic_0194140892_table57792315343"></a>
<table><thead align="left"><tr id="zh-cn_topic_0194140892_row18779123193412"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0194140892_p162781023123415"><a name="zh-cn_topic_0194140892_p162781023123415"></a><a name="zh-cn_topic_0194140892_p162781023123415"></a>配置项</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0194140892_p10278192333419"><a name="zh-cn_topic_0194140892_p10278192333419"></a><a name="zh-cn_topic_0194140892_p10278192333419"></a>是否必填</p>
</th>
<th class="cellrowborder" valign="top" width="24.97%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0194140892_p122781123153418"><a name="zh-cn_topic_0194140892_p122781123153418"></a><a name="zh-cn_topic_0194140892_p122781123153418"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="25.03%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0194140892_p1027862316345"><a name="zh-cn_topic_0194140892_p1027862316345"></a><a name="zh-cn_topic_0194140892_p1027862316345"></a>默认值</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0194140892_row4779153103415"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140892_p21363573617"><a name="zh-cn_topic_0194140892_p21363573617"></a><a name="zh-cn_topic_0194140892_p21363573617"></a>stream</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140892_p813193513369"><a name="zh-cn_topic_0194140892_p813193513369"></a><a name="zh-cn_topic_0194140892_p813193513369"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="24.97%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140892_p61343515363"><a name="zh-cn_topic_0194140892_p61343515363"></a><a name="zh-cn_topic_0194140892_p61343515363"></a>指定在DIS服务上创建的通道名称。</p>
</td>
<td class="cellrowborder" valign="top" width="25.03%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140892_p2131935163612"><a name="zh-cn_topic_0194140892_p2131935163612"></a><a name="zh-cn_topic_0194140892_p2131935163612"></a>与DIS控制台配置的“通道名称”取值一致。</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140892_row37792393418"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140892_p13310104173813"><a name="zh-cn_topic_0194140892_p13310104173813"></a><a name="zh-cn_topic_0194140892_p13310104173813"></a>ak</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140892_p9326134110388"><a name="zh-cn_topic_0194140892_p9326134110388"></a><a name="zh-cn_topic_0194140892_p9326134110388"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="24.97%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140892_p532664183816"><a name="zh-cn_topic_0194140892_p532664183816"></a><a name="zh-cn_topic_0194140892_p532664183816"></a>用户的Access Key。</p>
<p id="zh-cn_topic_0194140892_p10326441193817"><a name="zh-cn_topic_0194140892_p10326441193817"></a><a name="zh-cn_topic_0194140892_p10326441193817"></a>获取方式请参见<a href="安装前准备.md#zh-cn_topic_0194140940_s929153773cb54e1b801a8399b2ef9b2f">检查认证信息</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="25.03%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140892_p132694193818"><a name="zh-cn_topic_0194140892_p132694193818"></a><a name="zh-cn_topic_0194140892_p132694193818"></a>请根据实际情况配置</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140892_row3779038348"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140892_p3326441163810"><a name="zh-cn_topic_0194140892_p3326441163810"></a><a name="zh-cn_topic_0194140892_p3326441163810"></a>sk</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140892_p93267415385"><a name="zh-cn_topic_0194140892_p93267415385"></a><a name="zh-cn_topic_0194140892_p93267415385"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="24.97%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140892_p2032674115381"><a name="zh-cn_topic_0194140892_p2032674115381"></a><a name="zh-cn_topic_0194140892_p2032674115381"></a>用户的Secret Key。</p>
<p id="zh-cn_topic_0194140892_p43261141173812"><a name="zh-cn_topic_0194140892_p43261141173812"></a><a name="zh-cn_topic_0194140892_p43261141173812"></a>获取方式请参见<a href="安装前准备.md#zh-cn_topic_0194140940_s929153773cb54e1b801a8399b2ef9b2f">检查认证信息</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="25.03%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140892_p14342164143819"><a name="zh-cn_topic_0194140892_p14342164143819"></a><a name="zh-cn_topic_0194140892_p14342164143819"></a>请根据实际情况配置</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140892_row1779103143417"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140892_p1134220418386"><a name="zh-cn_topic_0194140892_p1134220418386"></a><a name="zh-cn_topic_0194140892_p1134220418386"></a>region</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140892_p1734234113816"><a name="zh-cn_topic_0194140892_p1734234113816"></a><a name="zh-cn_topic_0194140892_p1734234113816"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="24.97%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140892_p73421441113819"><a name="zh-cn_topic_0194140892_p73421441113819"></a><a name="zh-cn_topic_0194140892_p73421441113819"></a>将数据上传到指定Region的DIS服务。</p>
</td>
<td class="cellrowborder" valign="top" width="25.03%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140892_p13421541173811"><a name="zh-cn_topic_0194140892_p13421541173811"></a><a name="zh-cn_topic_0194140892_p13421541173811"></a>cn-north-1</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140892_row777910314344"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140892_p146708551799"><a name="zh-cn_topic_0194140892_p146708551799"></a><a name="zh-cn_topic_0194140892_p146708551799"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140892_p83577412388"><a name="zh-cn_topic_0194140892_p83577412388"></a><a name="zh-cn_topic_0194140892_p83577412388"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="24.97%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140892_p1035764115386"><a name="zh-cn_topic_0194140892_p1035764115386"></a><a name="zh-cn_topic_0194140892_p1035764115386"></a>用户所属区域的项目ID。</p>
<p id="zh-cn_topic_0194140892_p1335711419383"><a name="zh-cn_topic_0194140892_p1335711419383"></a><a name="zh-cn_topic_0194140892_p1335711419383"></a>获取方式请参见<a href="安装前准备.md#zh-cn_topic_0194140940_s929153773cb54e1b801a8399b2ef9b2f">检查认证信息</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="25.03%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140892_p83571641193816"><a name="zh-cn_topic_0194140892_p83571641193816"></a><a name="zh-cn_topic_0194140892_p83571641193816"></a>请根据实际情况配置</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140892_row11873153118377"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140892_p16357184113818"><a name="zh-cn_topic_0194140892_p16357184113818"></a><a name="zh-cn_topic_0194140892_p16357184113818"></a>endpoint</p>
<p id="zh-cn_topic_0194140892_p16372174143815"><a name="zh-cn_topic_0194140892_p16372174143815"></a><a name="zh-cn_topic_0194140892_p16372174143815"></a></p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140892_p2037234118382"><a name="zh-cn_topic_0194140892_p2037234118382"></a><a name="zh-cn_topic_0194140892_p2037234118382"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="24.97%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140892_p113721941103811"><a name="zh-cn_topic_0194140892_p113721941103811"></a><a name="zh-cn_topic_0194140892_p113721941103811"></a>DIS对应Region的数据接口地址。</p>
</td>
<td class="cellrowborder" valign="top" width="25.03%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140892_p209652334114"><a name="zh-cn_topic_0194140892_p209652334114"></a><a name="zh-cn_topic_0194140892_p209652334114"></a>https://dis.cn-north-1.myhuaweicloud.com</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140892_row7284529385"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140892_p859315420105"><a name="zh-cn_topic_0194140892_p859315420105"></a><a name="zh-cn_topic_0194140892_p859315420105"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140892_p42835211381"><a name="zh-cn_topic_0194140892_p42835211381"></a><a name="zh-cn_topic_0194140892_p42835211381"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="24.97%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140892_p112091820428"><a name="zh-cn_topic_0194140892_p112091820428"></a><a name="zh-cn_topic_0194140892_p112091820428"></a>DIS App名称，用于标识一个消费组，值可以为任意字符串</p>
</td>
<td class="cellrowborder" valign="top" width="25.03%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140892_p7120218174210"><a name="zh-cn_topic_0194140892_p7120218174210"></a><a name="zh-cn_topic_0194140892_p7120218174210"></a>请根据实际情况配置</p>
</td>
</tr>
</tbody>
</table>

## 配置DIS Logstash Output<a name="zh-cn_topic_0194140892_section1160265515521"></a>

配置模板如下：（该模板为读取本地文件数据并上传到DIS通道）

```
input
{
   file {
       path => ["/tmp/test.log"]
       type => "log4j"
       start_position => "beginning"
   }
}
output
{
    dis {
        stream => ["YOU_DIS_STREAM_NAME"]
        endpoint => "https://dis.${endpoint}"
        ak => "YOU_ACCESS_KEY_ID"
        sk => "YOU_SECRET_KEY_ID"
        region => "${region}"
        project_id => "YOU_PROJECT_ID"
    }
}
```

**表 2**  DIS Logstash Output配置项说明

<a name="zh-cn_topic_0194140892_table151821388539"></a>
<table><thead align="left"><tr id="zh-cn_topic_0194140892_row71822384532"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0194140892_p20182153805310"><a name="zh-cn_topic_0194140892_p20182153805310"></a><a name="zh-cn_topic_0194140892_p20182153805310"></a>配置项</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0194140892_p7182113810538"><a name="zh-cn_topic_0194140892_p7182113810538"></a><a name="zh-cn_topic_0194140892_p7182113810538"></a>是否必填</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0194140892_p0182103885319"><a name="zh-cn_topic_0194140892_p0182103885319"></a><a name="zh-cn_topic_0194140892_p0182103885319"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0194140892_p6198203817532"><a name="zh-cn_topic_0194140892_p6198203817532"></a><a name="zh-cn_topic_0194140892_p6198203817532"></a>默认值</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0194140892_row519863835315"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140892_p1219803819533"><a name="zh-cn_topic_0194140892_p1219803819533"></a><a name="zh-cn_topic_0194140892_p1219803819533"></a>stream</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140892_p11198538205312"><a name="zh-cn_topic_0194140892_p11198538205312"></a><a name="zh-cn_topic_0194140892_p11198538205312"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140892_p119863814536"><a name="zh-cn_topic_0194140892_p119863814536"></a><a name="zh-cn_topic_0194140892_p119863814536"></a>指定在DIS服务上创建的通道名称。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140892_p119863819539"><a name="zh-cn_topic_0194140892_p119863819539"></a><a name="zh-cn_topic_0194140892_p119863819539"></a>与DIS控制台配置的“通道名称”取值一致。</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140892_row2198143816533"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140892_p12198123817534"><a name="zh-cn_topic_0194140892_p12198123817534"></a><a name="zh-cn_topic_0194140892_p12198123817534"></a>ak</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140892_p1419818388534"><a name="zh-cn_topic_0194140892_p1419818388534"></a><a name="zh-cn_topic_0194140892_p1419818388534"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140892_p191983386539"><a name="zh-cn_topic_0194140892_p191983386539"></a><a name="zh-cn_topic_0194140892_p191983386539"></a>用户的Access Key。</p>
<p id="zh-cn_topic_0194140892_p71983386534"><a name="zh-cn_topic_0194140892_p71983386534"></a><a name="zh-cn_topic_0194140892_p71983386534"></a>获取方式请参见<a href="安装前准备.md#zh-cn_topic_0194140940_s929153773cb54e1b801a8399b2ef9b2f">检查认证信息</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140892_p131981838105311"><a name="zh-cn_topic_0194140892_p131981838105311"></a><a name="zh-cn_topic_0194140892_p131981838105311"></a>请根据实际情况配置</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140892_row152125387537"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140892_p2212193810532"><a name="zh-cn_topic_0194140892_p2212193810532"></a><a name="zh-cn_topic_0194140892_p2212193810532"></a>sk</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140892_p3212538165319"><a name="zh-cn_topic_0194140892_p3212538165319"></a><a name="zh-cn_topic_0194140892_p3212538165319"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140892_p52128384537"><a name="zh-cn_topic_0194140892_p52128384537"></a><a name="zh-cn_topic_0194140892_p52128384537"></a>用户的Secret Key。</p>
<p id="zh-cn_topic_0194140892_p1212183815538"><a name="zh-cn_topic_0194140892_p1212183815538"></a><a name="zh-cn_topic_0194140892_p1212183815538"></a>获取方式请参见<a href="安装前准备.md#zh-cn_topic_0194140940_s929153773cb54e1b801a8399b2ef9b2f">检查认证信息</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140892_p18212538115318"><a name="zh-cn_topic_0194140892_p18212538115318"></a><a name="zh-cn_topic_0194140892_p18212538115318"></a>请根据实际情况配置</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140892_row421203845312"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140892_p1721211386532"><a name="zh-cn_topic_0194140892_p1721211386532"></a><a name="zh-cn_topic_0194140892_p1721211386532"></a>region</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140892_p19212738115318"><a name="zh-cn_topic_0194140892_p19212738115318"></a><a name="zh-cn_topic_0194140892_p19212738115318"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140892_p32122382539"><a name="zh-cn_topic_0194140892_p32122382539"></a><a name="zh-cn_topic_0194140892_p32122382539"></a>将数据上传到指定Region的DIS服务。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140892_p821283855316"><a name="zh-cn_topic_0194140892_p821283855316"></a><a name="zh-cn_topic_0194140892_p821283855316"></a>cn-north-1</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140892_row18212538125317"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140892_p13576214191014"><a name="zh-cn_topic_0194140892_p13576214191014"></a><a name="zh-cn_topic_0194140892_p13576214191014"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140892_p14212738125312"><a name="zh-cn_topic_0194140892_p14212738125312"></a><a name="zh-cn_topic_0194140892_p14212738125312"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140892_p1921263815312"><a name="zh-cn_topic_0194140892_p1921263815312"></a><a name="zh-cn_topic_0194140892_p1921263815312"></a>用户所属区域的项目ID。</p>
<p id="zh-cn_topic_0194140892_p13228838105312"><a name="zh-cn_topic_0194140892_p13228838105312"></a><a name="zh-cn_topic_0194140892_p13228838105312"></a>获取方式请参见<a href="安装前准备.md#zh-cn_topic_0194140940_s929153773cb54e1b801a8399b2ef9b2f">检查认证信息</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140892_p1522814381531"><a name="zh-cn_topic_0194140892_p1522814381531"></a><a name="zh-cn_topic_0194140892_p1522814381531"></a>请根据实际情况配置</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140892_row12406131572110"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140892_p12407141522115"><a name="zh-cn_topic_0194140892_p12407141522115"></a><a name="zh-cn_topic_0194140892_p12407141522115"></a>body_compress_enabled</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140892_p13407131552116"><a name="zh-cn_topic_0194140892_p13407131552116"></a><a name="zh-cn_topic_0194140892_p13407131552116"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140892_p18407131592112"><a name="zh-cn_topic_0194140892_p18407131592112"></a><a name="zh-cn_topic_0194140892_p18407131592112"></a>是否开启传输数据压缩。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140892_p14071215202114"><a name="zh-cn_topic_0194140892_p14071215202114"></a><a name="zh-cn_topic_0194140892_p14071215202114"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140892_row206195713450"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140892_p2061457114514"><a name="zh-cn_topic_0194140892_p2061457114514"></a><a name="zh-cn_topic_0194140892_p2061457114514"></a>body_compress_type</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140892_p17611057134518"><a name="zh-cn_topic_0194140892_p17611057134518"></a><a name="zh-cn_topic_0194140892_p17611057134518"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140892_p1861957164519"><a name="zh-cn_topic_0194140892_p1861957164519"></a><a name="zh-cn_topic_0194140892_p1861957164519"></a>数据压缩类型，当前支持的压缩算法：</p>
<p id="zh-cn_topic_0194140892_p173731511152816"><a name="zh-cn_topic_0194140892_p173731511152816"></a><a name="zh-cn_topic_0194140892_p173731511152816"></a>lz4：综合来看效率最高的压缩算法,更加侧重压缩解压速度,压缩比并不是第一。</p>
<p id="zh-cn_topic_0194140892_p15968538102811"><a name="zh-cn_topic_0194140892_p15968538102811"></a><a name="zh-cn_topic_0194140892_p15968538102811"></a>zstd：一种新的无损压缩算法，旨在提供快速压缩，并实现高压缩比。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140892_p1061757124511"><a name="zh-cn_topic_0194140892_p1061757124511"></a><a name="zh-cn_topic_0194140892_p1061757124511"></a>lz4</p>
</td>
</tr>
</tbody>
</table>

