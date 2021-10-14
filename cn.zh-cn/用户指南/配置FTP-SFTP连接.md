# 配置FTP/SFTP连接<a name="dgc_01_0028"></a>

FTP/SFTP连接适用于从线下文件服务器或ECS服务器上迁移文件到OBS或数据库。

>![](public_sys-resources/icon-note.gif) **说明：** 
>当前仅支持Linux操作系统的FTP 服务器。

连接FTP或SFTP服务器时，他们的连接参数相同，如[表1](#zh-cn_topic_0108275400_table34037531171418)所示。

**表 1**  FTP/SFTP连接参数

<a name="zh-cn_topic_0108275400_table34037531171418"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108275400_row56630393171418"><th class="cellrowborder" valign="top" width="18.060000000000002%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108275400_p23659124171418"><a name="zh-cn_topic_0108275400_p23659124171418"></a><a name="zh-cn_topic_0108275400_p23659124171418"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="61.31999999999999%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108275400_p37340867171418"><a name="zh-cn_topic_0108275400_p37340867171418"></a><a name="zh-cn_topic_0108275400_p37340867171418"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="20.62%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108275400_p4711375171418"><a name="zh-cn_topic_0108275400_p4711375171418"></a><a name="zh-cn_topic_0108275400_p4711375171418"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108275400_row9394134114537"><td class="cellrowborder" valign="top" width="18.060000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275400_p4394104110532"><a name="zh-cn_topic_0108275400_p4394104110532"></a><a name="zh-cn_topic_0108275400_p4394104110532"></a>名称</p>
</td>
<td class="cellrowborder" valign="top" width="61.31999999999999%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275400_p1369564463813"><a name="zh-cn_topic_0108275400_p1369564463813"></a><a name="zh-cn_topic_0108275400_p1369564463813"></a>连接的名称，根据连接的数据源类型，用户可自定义便于记忆、区分的连接名。</p>
</td>
<td class="cellrowborder" valign="top" width="20.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275400_p739484115530"><a name="zh-cn_topic_0108275400_p739484115530"></a><a name="zh-cn_topic_0108275400_p739484115530"></a>ftp_link</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275400_row46077055171418"><td class="cellrowborder" valign="top" width="18.060000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275400_p41253947171418"><a name="zh-cn_topic_0108275400_p41253947171418"></a><a name="zh-cn_topic_0108275400_p41253947171418"></a>主机名或IP</p>
</td>
<td class="cellrowborder" valign="top" width="61.31999999999999%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275400_p53235436171418"><a name="zh-cn_topic_0108275400_p53235436171418"></a><a name="zh-cn_topic_0108275400_p53235436171418"></a>FTP或SFTP服务器的IP地址或者主机名。</p>
</td>
<td class="cellrowborder" valign="top" width="20.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275400_p17103098171418"><a name="zh-cn_topic_0108275400_p17103098171418"></a><a name="zh-cn_topic_0108275400_p17103098171418"></a>ftp.apache.org</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275400_row19710159171418"><td class="cellrowborder" valign="top" width="18.060000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275400_p53019059171418"><a name="zh-cn_topic_0108275400_p53019059171418"></a><a name="zh-cn_topic_0108275400_p53019059171418"></a>端口</p>
</td>
<td class="cellrowborder" valign="top" width="61.31999999999999%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275400_p66685350171418"><a name="zh-cn_topic_0108275400_p66685350171418"></a><a name="zh-cn_topic_0108275400_p66685350171418"></a>FTP或SFTP服务器的端口，默认值为21。</p>
</td>
<td class="cellrowborder" valign="top" width="20.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275400_p32804307171418"><a name="zh-cn_topic_0108275400_p32804307171418"></a><a name="zh-cn_topic_0108275400_p32804307171418"></a>21</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275400_row26803310171418"><td class="cellrowborder" valign="top" width="18.060000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275400_p23584482171418"><a name="zh-cn_topic_0108275400_p23584482171418"></a><a name="zh-cn_topic_0108275400_p23584482171418"></a>用户名</p>
</td>
<td class="cellrowborder" valign="top" width="61.31999999999999%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275400_p31294883171418"><a name="zh-cn_topic_0108275400_p31294883171418"></a><a name="zh-cn_topic_0108275400_p31294883171418"></a>登录FTP或SFTP服务器的用户名。</p>
</td>
<td class="cellrowborder" valign="top" width="20.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275400_p39712809171418"><a name="zh-cn_topic_0108275400_p39712809171418"></a><a name="zh-cn_topic_0108275400_p39712809171418"></a>cdm</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275400_row21870968171418"><td class="cellrowborder" valign="top" width="18.060000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275400_p26718016171418"><a name="zh-cn_topic_0108275400_p26718016171418"></a><a name="zh-cn_topic_0108275400_p26718016171418"></a>密码</p>
</td>
<td class="cellrowborder" valign="top" width="61.31999999999999%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275400_p16675672171418"><a name="zh-cn_topic_0108275400_p16675672171418"></a><a name="zh-cn_topic_0108275400_p16675672171418"></a>登录FTP或SFTP服务器的密码。</p>
</td>
<td class="cellrowborder" valign="top" width="20.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275400_p8552168171418"><a name="zh-cn_topic_0108275400_p8552168171418"></a><a name="zh-cn_topic_0108275400_p8552168171418"></a>-</p>
</td>
</tr>
</tbody>
</table>

