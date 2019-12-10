# 配置NAS/SFS连接<a name="dayu_01_0029"></a>

连接NAS数据源或弹性文件服务SFS Turbo时，相关参数如[表1](#zh-cn_topic_0108275384_table1990636915212)所示。

支持CIFS/SMB/NFS协议，可对接专业文件服务器、Windows系统文件共享、Linux Samba服务器，以及提供CIFS/SMB/NFS协议的文件系统的云服务，例如弹性文件服务SFS。

**表 1**  NAS连接器的参数

<a name="zh-cn_topic_0108275384_table1990636915212"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108275384_row4257242215212"><th class="cellrowborder" valign="top" width="18.060000000000002%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108275384_p3100089215212"><a name="zh-cn_topic_0108275384_p3100089215212"></a><a name="zh-cn_topic_0108275384_p3100089215212"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="61.199999999999996%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108275384_p2804435515212"><a name="zh-cn_topic_0108275384_p2804435515212"></a><a name="zh-cn_topic_0108275384_p2804435515212"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="20.74%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108275384_p5700024515212"><a name="zh-cn_topic_0108275384_p5700024515212"></a><a name="zh-cn_topic_0108275384_p5700024515212"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108275384_row41401222562"><td class="cellrowborder" valign="top" width="18.060000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275384_p914020223566"><a name="zh-cn_topic_0108275384_p914020223566"></a><a name="zh-cn_topic_0108275384_p914020223566"></a>名称</p>
</td>
<td class="cellrowborder" valign="top" width="61.199999999999996%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275384_p1369564463813"><a name="zh-cn_topic_0108275384_p1369564463813"></a><a name="zh-cn_topic_0108275384_p1369564463813"></a>连接的名称，根据连接的数据源类型，用户可自定义便于记忆、区分的连接名。</p>
</td>
<td class="cellrowborder" valign="top" width="20.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275384_p16140152211564"><a name="zh-cn_topic_0108275384_p16140152211564"></a><a name="zh-cn_topic_0108275384_p16140152211564"></a>nas_link</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275384_row4324016315212"><td class="cellrowborder" valign="top" width="18.060000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275384_p1279229115212"><a name="zh-cn_topic_0108275384_p1279229115212"></a><a name="zh-cn_topic_0108275384_p1279229115212"></a>协议</p>
</td>
<td class="cellrowborder" valign="top" width="61.199999999999996%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275384_p2954266015212"><a name="zh-cn_topic_0108275384_p2954266015212"></a><a name="zh-cn_topic_0108275384_p2954266015212"></a>选择NAS文件协议，目前只支持SMB/CIFS/NFS协议。</p>
</td>
<td class="cellrowborder" valign="top" width="20.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275384_p4414526115212"><a name="zh-cn_topic_0108275384_p4414526115212"></a><a name="zh-cn_topic_0108275384_p4414526115212"></a>NFS</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275384_row6176303715212"><td class="cellrowborder" valign="top" width="18.060000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275384_p3675008615212"><a name="zh-cn_topic_0108275384_p3675008615212"></a><a name="zh-cn_topic_0108275384_p3675008615212"></a>共享路径</p>
</td>
<td class="cellrowborder" valign="top" width="61.199999999999996%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275384_p2396698815212"><a name="zh-cn_topic_0108275384_p2396698815212"></a><a name="zh-cn_topic_0108275384_p2396698815212"></a>NAS服务器的共享路径。</p>
</td>
<td class="cellrowborder" valign="top" width="20.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275384_p6227784615212"><a name="zh-cn_topic_0108275384_p6227784615212"></a><a name="zh-cn_topic_0108275384_p6227784615212"></a>\\server\share</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275384_row2362970415212"><td class="cellrowborder" valign="top" width="18.060000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275384_p3495787615212"><a name="zh-cn_topic_0108275384_p3495787615212"></a><a name="zh-cn_topic_0108275384_p3495787615212"></a>用户名</p>
</td>
<td class="cellrowborder" valign="top" width="61.199999999999996%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275384_p1301570415212"><a name="zh-cn_topic_0108275384_p1301570415212"></a><a name="zh-cn_topic_0108275384_p1301570415212"></a>登录NAS服务器的用户名，格式为<span class="uicontrol" id="zh-cn_topic_0108275384_uicontrol67105529153458"><a name="zh-cn_topic_0108275384_uicontrol67105529153458"></a><a name="zh-cn_topic_0108275384_uicontrol67105529153458"></a>“域名\用户名”</span>。</p>
<p id="zh-cn_topic_0108275384_p1840774015113"><a name="zh-cn_topic_0108275384_p1840774015113"></a><a name="zh-cn_topic_0108275384_p1840774015113"></a><span class="parmname" id="zh-cn_topic_0108275384_parmname13781514110"><a name="zh-cn_topic_0108275384_parmname13781514110"></a><a name="zh-cn_topic_0108275384_parmname13781514110"></a>“协议”</span>选择<span class="parmvalue" id="zh-cn_topic_0108275384_parmvalue1431616010215"><a name="zh-cn_topic_0108275384_parmvalue1431616010215"></a><a name="zh-cn_topic_0108275384_parmvalue1431616010215"></a>“NFS”</span>时，没有该参数。</p>
</td>
<td class="cellrowborder" valign="top" width="20.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275384_p4763913315212"><a name="zh-cn_topic_0108275384_p4763913315212"></a><a name="zh-cn_topic_0108275384_p4763913315212"></a>domain01\user</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275384_row21925509153146"><td class="cellrowborder" valign="top" width="18.060000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275384_p31135782153146"><a name="zh-cn_topic_0108275384_p31135782153146"></a><a name="zh-cn_topic_0108275384_p31135782153146"></a>密码</p>
</td>
<td class="cellrowborder" valign="top" width="61.199999999999996%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275384_p38970445153146"><a name="zh-cn_topic_0108275384_p38970445153146"></a><a name="zh-cn_topic_0108275384_p38970445153146"></a>登录NAS服务器的密码。</p>
<p id="zh-cn_topic_0108275384_p18261184191419"><a name="zh-cn_topic_0108275384_p18261184191419"></a><a name="zh-cn_topic_0108275384_p18261184191419"></a><span class="parmname" id="zh-cn_topic_0108275384_parmname162617411419"><a name="zh-cn_topic_0108275384_parmname162617411419"></a><a name="zh-cn_topic_0108275384_parmname162617411419"></a>“协议”</span>选择<span class="parmvalue" id="zh-cn_topic_0108275384_parmvalue1326184171410"><a name="zh-cn_topic_0108275384_parmvalue1326184171410"></a><a name="zh-cn_topic_0108275384_parmvalue1326184171410"></a>“NFS”</span>时，没有该参数。</p>
</td>
<td class="cellrowborder" valign="top" width="20.74%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275384_p2489439153146"><a name="zh-cn_topic_0108275384_p2489439153146"></a><a name="zh-cn_topic_0108275384_p2489439153146"></a>-</p>
</td>
</tr>
</tbody>
</table>

