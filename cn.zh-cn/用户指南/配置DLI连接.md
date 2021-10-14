# 配置DLI连接<a name="dgc_01_0036"></a>

连接数据湖探索（DLI）服务时，相关参数如[表1](#zh-cn_topic_0108275410_table22075105144748)所示。

**表 1**  DLI连接参数

<a name="zh-cn_topic_0108275410_table22075105144748"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108275410_row19905440144748"><th class="cellrowborder" valign="top" width="19.509999999999998%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108275410_p1727937144748"><a name="zh-cn_topic_0108275410_p1727937144748"></a><a name="zh-cn_topic_0108275410_p1727937144748"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="58.75%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108275410_p5745174144748"><a name="zh-cn_topic_0108275410_p5745174144748"></a><a name="zh-cn_topic_0108275410_p5745174144748"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="21.740000000000002%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108275410_p62705927144748"><a name="zh-cn_topic_0108275410_p62705927144748"></a><a name="zh-cn_topic_0108275410_p62705927144748"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108275410_row11298866916"><td class="cellrowborder" valign="top" width="19.509999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275410_p15298176296"><a name="zh-cn_topic_0108275410_p15298176296"></a><a name="zh-cn_topic_0108275410_p15298176296"></a>名称</p>
</td>
<td class="cellrowborder" valign="top" width="58.75%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275410_p1369564463813"><a name="zh-cn_topic_0108275410_p1369564463813"></a><a name="zh-cn_topic_0108275410_p1369564463813"></a>连接的名称，根据连接的数据源类型，用户可自定义便于记忆、区分的连接名。</p>
</td>
<td class="cellrowborder" valign="top" width="21.740000000000002%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275410_p19298156493"><a name="zh-cn_topic_0108275410_p19298156493"></a><a name="zh-cn_topic_0108275410_p19298156493"></a>dli_link</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275410_row46015358144748"><td class="cellrowborder" valign="top" width="19.509999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275410_p31612872145433"><a name="zh-cn_topic_0108275410_p31612872145433"></a><a name="zh-cn_topic_0108275410_p31612872145433"></a>访问标识(AK)</p>
</td>
<td class="cellrowborder" rowspan="2" valign="top" width="58.75%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275410_p181471423104"><a name="zh-cn_topic_0108275410_p181471423104"></a><a name="zh-cn_topic_0108275410_p181471423104"></a>访问DLI数据库时鉴权所需的AK和SK。</p>
<p id="zh-cn_topic_0108275410_p2087724103311"><a name="zh-cn_topic_0108275410_p2087724103311"></a><a name="zh-cn_topic_0108275410_p2087724103311"></a>您需要先创建当前账号的访问密钥，并获得对应的AK和SK。</p>
<a name="zh-cn_topic_0108275410_ol1361418377715"></a><a name="zh-cn_topic_0108275410_ol1361418377715"></a><ol id="zh-cn_topic_0108275410_ol1361418377715"><li>登录控制台，在用户名额下拉列表中选择“我的凭证”。</li><li>进入<span class="wintitle" id="zh-cn_topic_0108275410_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_wintitle471885516555"><a name="zh-cn_topic_0108275410_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_wintitle471885516555"></a><a name="zh-cn_topic_0108275410_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_wintitle471885516555"></a>“我的<span id="zh-cn_topic_0108275410_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_text95491317711"><a name="zh-cn_topic_0108275410_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_text95491317711"></a><a name="zh-cn_topic_0108275410_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_text95491317711"></a>凭</span>证”</span>页面，选择<span class="menucascade" id="zh-cn_topic_0108275410_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_menucascade10281112416374"><a name="zh-cn_topic_0108275410_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_menucascade10281112416374"></a><a name="zh-cn_topic_0108275410_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_menucascade10281112416374"></a>“<span class="uicontrol" id="zh-cn_topic_0108275410_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_uicontrol128182416375"><a name="zh-cn_topic_0108275410_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_uicontrol128182416375"></a><a name="zh-cn_topic_0108275410_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_uicontrol128182416375"></a>访问密钥 &gt; 新增访问密钥</span>”</span>，如<a href="#zh-cn_topic_0108275410_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_fig1552229194615">图1</a>所示。<div class="fignone" id="zh-cn_topic_0108275410_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_fig1552229194615"><a name="zh-cn_topic_0108275410_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_fig1552229194615"></a><a name="zh-cn_topic_0108275410_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_fig1552229194615"></a><span class="figcap"><b>图1 </b>单击新增访问密钥</span><br><a name="zh-cn_topic_0108275410_zh-cn_topic_0000001129241845_image20389043111611"></a><a name="zh-cn_topic_0108275410_zh-cn_topic_0000001129241845_image20389043111611"></a><span><img id="zh-cn_topic_0108275410_zh-cn_topic_0000001129241845_image20389043111611" src="figures/单击新增访问密钥.png" width="274.3125" height="82.927362"></span></div>
</li><li>单击“确定”，根据浏览器提示，保存密钥文件。密钥文件会直接保存到浏览器默认的下载文件夹中。打开名称为“credentials.csv”的文件，即可查看访问密钥（Access Key Id和Secret Access Key）。</li></ol>
</td>
<td class="cellrowborder" valign="top" width="21.740000000000002%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275410_p5195678145433"><a name="zh-cn_topic_0108275410_p5195678145433"></a><a name="zh-cn_topic_0108275410_p5195678145433"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275410_row23643456144748"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275410_p29552890145433"><a name="zh-cn_topic_0108275410_p29552890145433"></a><a name="zh-cn_topic_0108275410_p29552890145433"></a>密钥(SK)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275410_p32797946145433"><a name="zh-cn_topic_0108275410_p32797946145433"></a><a name="zh-cn_topic_0108275410_p32797946145433"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275410_row12160822504"><td class="cellrowborder" valign="top" width="19.509999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275410_p1016019285015"><a name="zh-cn_topic_0108275410_p1016019285015"></a><a name="zh-cn_topic_0108275410_p1016019285015"></a>项目ID</p>
</td>
<td class="cellrowborder" valign="top" width="58.75%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275410_p1637616424613"><a name="zh-cn_topic_0108275410_p1637616424613"></a><a name="zh-cn_topic_0108275410_p1637616424613"></a>DLI服务所在区域的项目ID。</p>
<div class="p" id="zh-cn_topic_0108275410_p1668482916813"><a name="zh-cn_topic_0108275410_p1668482916813"></a><a name="zh-cn_topic_0108275410_p1668482916813"></a>项目ID表示租户的资源，帐号ID对应当前帐号。用户可在对应页面下查看不同Region对应的项目ID和帐号ID。<a name="zh-cn_topic_0108275410_zh-cn_topic_0000001129537317_ol6260200121819"></a><a name="zh-cn_topic_0108275410_zh-cn_topic_0000001129537317_ol6260200121819"></a><ol id="zh-cn_topic_0108275410_zh-cn_topic_0000001129537317_ol6260200121819"><li>注册并登录管理控制台。</li><li>在用户名的下拉列表中单击<span class="uicontrol" id="zh-cn_topic_0108275410_zh-cn_topic_0000001129537317_uicontrol0260130191818"><a name="zh-cn_topic_0108275410_zh-cn_topic_0000001129537317_uicontrol0260130191818"></a><a name="zh-cn_topic_0108275410_zh-cn_topic_0000001129537317_uicontrol0260130191818"></a>“我的凭证”</span>。</li><li>在<span class="wintitle" id="zh-cn_topic_0108275410_zh-cn_topic_0000001129537317_wintitle132611102181"><a name="zh-cn_topic_0108275410_zh-cn_topic_0000001129537317_wintitle132611102181"></a><a name="zh-cn_topic_0108275410_zh-cn_topic_0000001129537317_wintitle132611102181"></a>“我的凭证”</span>页面，查看帐号名和帐号ID，在项目列表中查看项目ID。</li></ol>
</div>
</td>
<td class="cellrowborder" valign="top" width="21.740000000000002%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275410_p11608245019"><a name="zh-cn_topic_0108275410_p11608245019"></a><a name="zh-cn_topic_0108275410_p11608245019"></a>-</p>
</td>
</tr>
</tbody>
</table>

