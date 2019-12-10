# 配置OBS连接<a name="dayu_01_0045"></a>

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
<td class="cellrowborder" valign="top" width="62.870000000000005%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275368_p24017490165510"><a name="zh-cn_topic_0108275368_p24017490165510"></a><a name="zh-cn_topic_0108275368_p24017490165510"></a>OBS桶的Endpoint，可从<a href="https://developer.huaweicloud.com/endpoint?OBS" target="_blank" rel="noopener noreferrer">地区和终端节点</a>获取。</p>
<p id="zh-cn_topic_0108275368_p1013171965116"><a name="zh-cn_topic_0108275368_p1013171965116"></a><a name="zh-cn_topic_0108275368_p1013171965116"></a>这里支持用户输入桶级别的域名，例如：test.obs.myhuaweicloud.com，则在查询OBS桶的时候，只能查询到test这个桶。</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275368_p54900694163911"><a name="zh-cn_topic_0108275368_p54900694163911"></a><a name="zh-cn_topic_0108275368_p54900694163911"></a>obs.cn-north-1.myhuaweicloud.com</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275368_row55420632152843"><td class="cellrowborder" valign="top" width="16.5%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275368_p18947563152843"><a name="zh-cn_topic_0108275368_p18947563152843"></a><a name="zh-cn_topic_0108275368_p18947563152843"></a>端口</p>
</td>
<td class="cellrowborder" valign="top" width="62.870000000000005%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275368_p60445924165510"><a name="zh-cn_topic_0108275368_p60445924165510"></a><a name="zh-cn_topic_0108275368_p60445924165510"></a>数据传输协议端口，https是443，http是80。</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275368_p25723188163911"><a name="zh-cn_topic_0108275368_p25723188163911"></a><a name="zh-cn_topic_0108275368_p25723188163911"></a>443</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275368_row55275051152843"><td class="cellrowborder" valign="top" width="16.5%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275368_p3311745152843"><a name="zh-cn_topic_0108275368_p3311745152843"></a><a name="zh-cn_topic_0108275368_p3311745152843"></a>访问标识(AK)</p>
</td>
<td class="cellrowborder" valign="top" width="62.870000000000005%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275368_p41664200165510"><a name="zh-cn_topic_0108275368_p41664200165510"></a><a name="zh-cn_topic_0108275368_p41664200165510"></a>登录OBS服务器的访问标识。</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275368_p28831327163911"><a name="zh-cn_topic_0108275368_p28831327163911"></a><a name="zh-cn_topic_0108275368_p28831327163911"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275368_row3886299152843"><td class="cellrowborder" valign="top" width="16.5%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275368_p63749320152843"><a name="zh-cn_topic_0108275368_p63749320152843"></a><a name="zh-cn_topic_0108275368_p63749320152843"></a>密钥(SK)</p>
</td>
<td class="cellrowborder" valign="top" width="62.870000000000005%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275368_p39995786165510"><a name="zh-cn_topic_0108275368_p39995786165510"></a><a name="zh-cn_topic_0108275368_p39995786165510"></a>登录OBS服务器的密钥。</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275368_p12963499163911"><a name="zh-cn_topic_0108275368_p12963499163911"></a><a name="zh-cn_topic_0108275368_p12963499163911"></a>-</p>
</td>
</tr>
</tbody>
</table>

