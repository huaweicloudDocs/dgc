# 配置OBS连接<a name="dgc_01_0045"></a>

OBS连接目的端OBS桶需添加读写权限，并在连接时不需要认证文件。

连接OBS时，相关连接参数如[表1](#zh-cn_topic_0108275368_table56513226152843)所示。

**表 1**  OBS连接的参数

<a name="zh-cn_topic_0108275368_table56513226152843"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108275368_row51765490152843"><th class="cellrowborder" valign="top" width="16.5%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108275368_p25915791152843"><a name="zh-cn_topic_0108275368_p25915791152843"></a><a name="zh-cn_topic_0108275368_p25915791152843"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="62.870000000000005%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108275368_p38360350165510"><a name="zh-cn_topic_0108275368_p38360350165510"></a><a name="zh-cn_topic_0108275368_p38360350165510"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="20.630000000000003%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108275368_p64999942163911"><a name="zh-cn_topic_0108275368_p64999942163911"></a><a name="zh-cn_topic_0108275368_p64999942163911"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108275368_row172676953014"><td class="cellrowborder" valign="top" width="16.5%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275368_p426714916301"><a name="zh-cn_topic_0108275368_p426714916301"></a><a name="zh-cn_topic_0108275368_p426714916301"></a>名称</p>
</td>
<td class="cellrowborder" valign="top" width="62.870000000000005%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275368_p6573133312010"><a name="zh-cn_topic_0108275368_p6573133312010"></a><a name="zh-cn_topic_0108275368_p6573133312010"></a>连接的名称，根据连接的数据源类型，用户可自定义便于记忆、区分的连接名。</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275368_p1826719919305"><a name="zh-cn_topic_0108275368_p1826719919305"></a><a name="zh-cn_topic_0108275368_p1826719919305"></a>obs_link</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275368_row58346992152843"><td class="cellrowborder" valign="top" width="16.5%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275368_p25657651152843"><a name="zh-cn_topic_0108275368_p25657651152843"></a><a name="zh-cn_topic_0108275368_p25657651152843"></a>OBS终端节点</p>
</td>
<td class="cellrowborder" valign="top" width="62.870000000000005%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108275368_p11141143515423"><a name="zh-cn_topic_0108275368_p11141143515423"></a><a name="zh-cn_topic_0108275368_p11141143515423"></a>您可以通过以下任一方式获取Endpoint信息：<a name="zh-cn_topic_0108275368_ul36191496587"></a><a name="zh-cn_topic_0108275368_ul36191496587"></a><ul id="zh-cn_topic_0108275368_ul36191496587"><li>OBS桶的Endpoint，可以进入OBS控制台概览页，点击桶名称后查看桶的基本信息获取。</li><li><p id="zh-cn_topic_0108275368_p14896726436"><a name="zh-cn_topic_0108275368_p14896726436"></a><a name="zh-cn_topic_0108275368_p14896726436"></a>终端节点（Endpoint）即调用API的<strong id="zh-cn_topic_0108275368_zh-cn_topic_0000001082451448_b7643811113415"><a name="zh-cn_topic_0108275368_zh-cn_topic_0000001082451448_b7643811113415"></a><a name="zh-cn_topic_0108275368_zh-cn_topic_0000001082451448_b7643811113415"></a>请求地址</strong>，不同服务不同区域的终端节点不同。Endpoint可从<a href="https://developer.huaweicloud.com/endpoint" target="_blank" rel="noopener noreferrer">终端节点及区域说明</a>获取。</p>
</li></ul>
</div>
<p id="zh-cn_topic_0108275368_p138036103816"><a name="zh-cn_topic_0108275368_p138036103816"></a><a name="zh-cn_topic_0108275368_p138036103816"></a>这里支持用户输入桶级别的域名，例如：test.xx.com，则在查询OBS桶的时候，只能查询到test这个桶。</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275368_p89819474596"><a name="zh-cn_topic_0108275368_p89819474596"></a><a name="zh-cn_topic_0108275368_p89819474596"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275368_row55420632152843"><td class="cellrowborder" valign="top" width="16.5%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275368_p18947563152843"><a name="zh-cn_topic_0108275368_p18947563152843"></a><a name="zh-cn_topic_0108275368_p18947563152843"></a>端口</p>
</td>
<td class="cellrowborder" valign="top" width="62.870000000000005%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275368_p60445924165510"><a name="zh-cn_topic_0108275368_p60445924165510"></a><a name="zh-cn_topic_0108275368_p60445924165510"></a>数据传输协议端口，https是443，http是80。</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275368_p25723188163911"><a name="zh-cn_topic_0108275368_p25723188163911"></a><a name="zh-cn_topic_0108275368_p25723188163911"></a>443</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275368_row4804240203017"><td class="cellrowborder" valign="top" width="16.5%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275368_p158041427194014"><a name="zh-cn_topic_0108275368_p158041427194014"></a><a name="zh-cn_topic_0108275368_p158041427194014"></a>OBS桶类型</p>
</td>
<td class="cellrowborder" valign="top" width="62.870000000000005%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275368_p6804122764019"><a name="zh-cn_topic_0108275368_p6804122764019"></a><a name="zh-cn_topic_0108275368_p6804122764019"></a>用户下拉选择即可。</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275368_p208045273406"><a name="zh-cn_topic_0108275368_p208045273406"></a><a name="zh-cn_topic_0108275368_p208045273406"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275368_row55275051152843"><td class="cellrowborder" valign="top" width="16.5%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275368_p3311745152843"><a name="zh-cn_topic_0108275368_p3311745152843"></a><a name="zh-cn_topic_0108275368_p3311745152843"></a>访问标识(AK)</p>
</td>
<td class="cellrowborder" rowspan="2" valign="top" width="62.870000000000005%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275368_zh-cn_topic_0108275368_p41664200165510"><a name="zh-cn_topic_0108275368_zh-cn_topic_0108275368_p41664200165510"></a><a name="zh-cn_topic_0108275368_zh-cn_topic_0108275368_p41664200165510"></a>AK和SK分别为登录OBS服务器的访问标识与密钥。</p>
<p id="zh-cn_topic_0108275368_zh-cn_topic_0108275368_p1660302262810"><a name="zh-cn_topic_0108275368_zh-cn_topic_0108275368_p1660302262810"></a><a name="zh-cn_topic_0108275368_zh-cn_topic_0108275368_p1660302262810"></a>您需要先创建当前帐号的访问密钥，并获得对应的AK和SK。</p>
<div class="p" id="zh-cn_topic_0108275368_p13152215453"><a name="zh-cn_topic_0108275368_p13152215453"></a><a name="zh-cn_topic_0108275368_p13152215453"></a>您可以通过如下方式获取访问密钥。<a name="zh-cn_topic_0108275368_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_ol535183018588"></a><a name="zh-cn_topic_0108275368_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_ol535183018588"></a><ol id="zh-cn_topic_0108275368_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_ol535183018588"><li>登录控制台，在用户名额下拉列表中选择“我的凭证”。</li><li>进入<span class="wintitle" id="zh-cn_topic_0108275368_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_wintitle471885516555"><a name="zh-cn_topic_0108275368_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_wintitle471885516555"></a><a name="zh-cn_topic_0108275368_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_wintitle471885516555"></a>“我的<span id="zh-cn_topic_0108275368_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_text95491317711"><a name="zh-cn_topic_0108275368_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_text95491317711"></a><a name="zh-cn_topic_0108275368_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_text95491317711"></a>凭</span>证”</span>页面，选择<span class="menucascade" id="zh-cn_topic_0108275368_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_menucascade10281112416374"><a name="zh-cn_topic_0108275368_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_menucascade10281112416374"></a><a name="zh-cn_topic_0108275368_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_menucascade10281112416374"></a>“<span class="uicontrol" id="zh-cn_topic_0108275368_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_uicontrol128182416375"><a name="zh-cn_topic_0108275368_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_uicontrol128182416375"></a><a name="zh-cn_topic_0108275368_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_uicontrol128182416375"></a>访问密钥 &gt; 新增访问密钥</span>”</span>，如<a href="#zh-cn_topic_0108275368_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_fig1552229194615">图1</a>所示。<div class="fignone" id="zh-cn_topic_0108275368_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_fig1552229194615"><a name="zh-cn_topic_0108275368_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_fig1552229194615"></a><a name="zh-cn_topic_0108275368_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_fig1552229194615"></a><span class="figcap"><b>图1 </b>单击新增访问密钥</span><br><a name="zh-cn_topic_0108275368_zh-cn_topic_0000001129241845_image20389043111611"></a><a name="zh-cn_topic_0108275368_zh-cn_topic_0000001129241845_image20389043111611"></a><span><img id="zh-cn_topic_0108275368_zh-cn_topic_0000001129241845_image20389043111611" src="figures/单击新增访问密钥.png" width="274.3125" height="82.927362"></span></div>
</li><li>单击“确定”，根据浏览器提示，保存密钥文件。密钥文件会直接保存到浏览器默认的下载文件夹中。打开名称为“credentials.csv”的文件，即可查看访问密钥（Access Key Id和Secret Access Key）。</li></ol>
</div>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275368_p28831327163911"><a name="zh-cn_topic_0108275368_p28831327163911"></a><a name="zh-cn_topic_0108275368_p28831327163911"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275368_row3886299152843"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275368_p63749320152843"><a name="zh-cn_topic_0108275368_p63749320152843"></a><a name="zh-cn_topic_0108275368_p63749320152843"></a>密钥(SK)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275368_p12963499163911"><a name="zh-cn_topic_0108275368_p12963499163911"></a><a name="zh-cn_topic_0108275368_p12963499163911"></a>-</p>
</td>
</tr>
</tbody>
</table>

