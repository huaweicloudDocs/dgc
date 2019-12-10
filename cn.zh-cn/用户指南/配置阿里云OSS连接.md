# 配置阿里云OSS连接<a name="dayu_01_0043"></a>

连接阿里云的OSS时，相关连接参数如[表1](#zh-cn_topic_0108275478_table56513226152843)所示。

**表 1**  OSS连接的参数

<a name="zh-cn_topic_0108275478_table56513226152843"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108275478_row51765490152843"><th class="cellrowborder" valign="top" width="20.18%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108275478_p25915791152843"><a name="zh-cn_topic_0108275478_p25915791152843"></a><a name="zh-cn_topic_0108275478_p25915791152843"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="52.400000000000006%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108275478_p38360350165510"><a name="zh-cn_topic_0108275478_p38360350165510"></a><a name="zh-cn_topic_0108275478_p38360350165510"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="27.42%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108275478_p64999942163911"><a name="zh-cn_topic_0108275478_p64999942163911"></a><a name="zh-cn_topic_0108275478_p64999942163911"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108275478_row172676953014"><td class="cellrowborder" valign="top" width="20.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275478_p426714916301"><a name="zh-cn_topic_0108275478_p426714916301"></a><a name="zh-cn_topic_0108275478_p426714916301"></a>名称</p>
</td>
<td class="cellrowborder" valign="top" width="52.400000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275478_p6573133312010"><a name="zh-cn_topic_0108275478_p6573133312010"></a><a name="zh-cn_topic_0108275478_p6573133312010"></a>连接的名称，根据连接的数据源类型，用户可自定义便于记忆、区分的连接名。</p>
</td>
<td class="cellrowborder" valign="top" width="27.42%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275478_p1826719919305"><a name="zh-cn_topic_0108275478_p1826719919305"></a><a name="zh-cn_topic_0108275478_p1826719919305"></a>oss_link</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275478_row58346992152843"><td class="cellrowborder" valign="top" width="20.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275478_p25657651152843"><a name="zh-cn_topic_0108275478_p25657651152843"></a><a name="zh-cn_topic_0108275478_p25657651152843"></a>OSS访问域名</p>
</td>
<td class="cellrowborder" valign="top" width="52.400000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275478_p24017490165510"><a name="zh-cn_topic_0108275478_p24017490165510"></a><a name="zh-cn_topic_0108275478_p24017490165510"></a>阿里云OSS的外网Endpoint。</p>
</td>
<td class="cellrowborder" valign="top" width="27.42%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275478_p75588220114"><a name="zh-cn_topic_0108275478_p75588220114"></a><a name="zh-cn_topic_0108275478_p75588220114"></a>oss-cn-hangzhou.aliyuncs.com</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275478_row55420632152843"><td class="cellrowborder" valign="top" width="20.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275478_p18947563152843"><a name="zh-cn_topic_0108275478_p18947563152843"></a><a name="zh-cn_topic_0108275478_p18947563152843"></a>身份认证方式</p>
</td>
<td class="cellrowborder" valign="top" width="52.400000000000006%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108275478_p169368251213"><a name="zh-cn_topic_0108275478_p169368251213"></a><a name="zh-cn_topic_0108275478_p169368251213"></a>选择身份认证方式：<a name="zh-cn_topic_0108275478_ul1557618228122"></a><a name="zh-cn_topic_0108275478_ul1557618228122"></a><ul id="zh-cn_topic_0108275478_ul1557618228122"><li>访问密钥：使用长期密钥访问OSS。</li><li>临时访问凭证：使用临时密钥和安全令牌访问OSS。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="27.42%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275478_p023121321110"><a name="zh-cn_topic_0108275478_p023121321110"></a><a name="zh-cn_topic_0108275478_p023121321110"></a>访问密钥</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275478_row55275051152843"><td class="cellrowborder" valign="top" width="20.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275478_p3311745152843"><a name="zh-cn_topic_0108275478_p3311745152843"></a><a name="zh-cn_topic_0108275478_p3311745152843"></a>访问标识(AK)</p>
</td>
<td class="cellrowborder" valign="top" width="52.400000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275478_p41664200165510"><a name="zh-cn_topic_0108275478_p41664200165510"></a><a name="zh-cn_topic_0108275478_p41664200165510"></a>登录OSS服务器的访问标识。</p>
</td>
<td class="cellrowborder" valign="top" width="27.42%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275478_p28831327163911"><a name="zh-cn_topic_0108275478_p28831327163911"></a><a name="zh-cn_topic_0108275478_p28831327163911"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275478_row3886299152843"><td class="cellrowborder" valign="top" width="20.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275478_p63749320152843"><a name="zh-cn_topic_0108275478_p63749320152843"></a><a name="zh-cn_topic_0108275478_p63749320152843"></a>密钥(SK)</p>
</td>
<td class="cellrowborder" valign="top" width="52.400000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275478_p39995786165510"><a name="zh-cn_topic_0108275478_p39995786165510"></a><a name="zh-cn_topic_0108275478_p39995786165510"></a>登录OSS服务器的密钥。</p>
</td>
<td class="cellrowborder" valign="top" width="27.42%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275478_p12963499163911"><a name="zh-cn_topic_0108275478_p12963499163911"></a><a name="zh-cn_topic_0108275478_p12963499163911"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275478_row1838723418115"><td class="cellrowborder" valign="top" width="20.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275478_p4387143491118"><a name="zh-cn_topic_0108275478_p4387143491118"></a><a name="zh-cn_topic_0108275478_p4387143491118"></a>安全令牌</p>
</td>
<td class="cellrowborder" valign="top" width="52.400000000000006%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275478_p1538717341111"><a name="zh-cn_topic_0108275478_p1538717341111"></a><a name="zh-cn_topic_0108275478_p1538717341111"></a>使用<span class="parmvalue" id="zh-cn_topic_0108275478_parmvalue115169521310"><a name="zh-cn_topic_0108275478_parmvalue115169521310"></a><a name="zh-cn_topic_0108275478_parmvalue115169521310"></a>“临时访问凭证”</span>时，这里还需要配置阿里云STS（Security Token Service）提供的临时令牌。</p>
</td>
<td class="cellrowborder" valign="top" width="27.42%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275478_p1538717346117"><a name="zh-cn_topic_0108275478_p1538717346117"></a><a name="zh-cn_topic_0108275478_p1538717346117"></a>-</p>
</td>
</tr>
</tbody>
</table>

