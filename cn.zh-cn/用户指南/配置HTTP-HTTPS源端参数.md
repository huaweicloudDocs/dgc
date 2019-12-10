# 配置HTTP/HTTPS源端参数<a name="dayu_01_0053"></a>

作业中源连接为HTTP连接时，源端作业参数如[表1](#zh-cn_topic_0114711714_table5046103815165)所示。当前只支持从HTTP/HTTPS URL导出数据，不支持导入。

**表 1**  HTTP作为源端时的作业参数

<a name="zh-cn_topic_0114711714_table5046103815165"></a>
<table><thead align="left"><tr id="zh-cn_topic_0114711714_row585315215165"><th class="cellrowborder" valign="top" width="23.77237723772377%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0114711714_p1626397215165"><a name="zh-cn_topic_0114711714_p1626397215165"></a><a name="zh-cn_topic_0114711714_p1626397215165"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="55.17551755175517%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0114711714_p4231334915165"><a name="zh-cn_topic_0114711714_p4231334915165"></a><a name="zh-cn_topic_0114711714_p4231334915165"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="21.052105210521052%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0114711714_p482921015165"><a name="zh-cn_topic_0114711714_p482921015165"></a><a name="zh-cn_topic_0114711714_p482921015165"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0114711714_row4012116315165"><td class="cellrowborder" valign="top" width="23.77237723772377%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0114711714_p2858877215165"><a name="zh-cn_topic_0114711714_p2858877215165"></a><a name="zh-cn_topic_0114711714_p2858877215165"></a>文件URL</p>
</td>
<td class="cellrowborder" valign="top" width="55.17551755175517%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0114711714_p41044235294"><a name="zh-cn_topic_0114711714_p41044235294"></a><a name="zh-cn_topic_0114711714_p41044235294"></a>通过使用GET方法，从HTTP/HTTPS协议的URL中获取数据。</p>
<p id="zh-cn_topic_0114711714_p0123115172917"><a name="zh-cn_topic_0114711714_p0123115172917"></a><a name="zh-cn_topic_0114711714_p0123115172917"></a>用于读取一个公网HTTP/HTTPS URL的文件，包括第三方对象存储的公共读取场景和网盘场景。</p>
</td>
<td class="cellrowborder" valign="top" width="21.052105210521052%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0114711714_p18854181112917"><a name="zh-cn_topic_0114711714_p18854181112917"></a><a name="zh-cn_topic_0114711714_p18854181112917"></a>https://bucket.obs.myhuaweicloud.com/object-key</p>
</td>
</tr>
<tr id="zh-cn_topic_0114711714_row1497845915165"><td class="cellrowborder" valign="top" width="23.77237723772377%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0114711714_p529563715165"><a name="zh-cn_topic_0114711714_p529563715165"></a><a name="zh-cn_topic_0114711714_p529563715165"></a>文件格式</p>
</td>
<td class="cellrowborder" valign="top" width="55.17551755175517%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0114711714_p16728112982816"><a name="zh-cn_topic_0114711714_p16728112982816"></a><a name="zh-cn_topic_0114711714_p16728112982816"></a>当前CDM只支持选择<span class="parmvalue" id="zh-cn_topic_0114711714_parmvalue1472811294289"><a name="zh-cn_topic_0114711714_parmvalue1472811294289"></a><a name="zh-cn_topic_0114711714_parmvalue1472811294289"></a>“二进制格式”</span>，不解析文件内容直接传输，不要求原文件格式必须为二进制。</p>
</td>
<td class="cellrowborder" valign="top" width="21.052105210521052%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0114711714_p3753014815165"><a name="zh-cn_topic_0114711714_p3753014815165"></a><a name="zh-cn_topic_0114711714_p3753014815165"></a>二进制格式</p>
</td>
</tr>
<tr id="zh-cn_topic_0114711714_row195259453167"><td class="cellrowborder" valign="top" width="23.77237723772377%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0114711714_p5526745191614"><a name="zh-cn_topic_0114711714_p5526745191614"></a><a name="zh-cn_topic_0114711714_p5526745191614"></a>压缩格式</p>
</td>
<td class="cellrowborder" valign="top" width="55.17551755175517%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0114711714_p2806544011518"><a name="zh-cn_topic_0114711714_p2806544011518"></a><a name="zh-cn_topic_0114711714_p2806544011518"></a>选择对应压缩格式的源文件进行迁移：<a name="zh-cn_topic_0114711714_zh-cn_topic_0108272831_ul64234801103023"></a><a name="zh-cn_topic_0114711714_zh-cn_topic_0108272831_ul64234801103023"></a><ul id="zh-cn_topic_0114711714_zh-cn_topic_0108272831_ul64234801103023"><li>NONE：表示传输所有格式的文件。</li><li>GZIP：表示只传输GZIP格式的文件。</li><li>ZIP：表示只传输ZIP格式的文件。</li><li>TAR.GZ：表示只传输TAR.GZ格式的文件。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="21.052105210521052%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0114711714_p165261145181617"><a name="zh-cn_topic_0114711714_p165261145181617"></a><a name="zh-cn_topic_0114711714_p165261145181617"></a>NONE</p>
</td>
</tr>
<tr id="zh-cn_topic_0114711714_row24820469167"><td class="cellrowborder" valign="top" width="23.77237723772377%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0114711714_p24911467163"><a name="zh-cn_topic_0114711714_p24911467163"></a><a name="zh-cn_topic_0114711714_p24911467163"></a>压缩文件后缀</p>
</td>
<td class="cellrowborder" valign="top" width="55.17551755175517%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0114711714_p13187191714515"><a name="zh-cn_topic_0114711714_p13187191714515"></a><a name="zh-cn_topic_0114711714_p13187191714515"></a>需要解压缩的文件后缀名。当一批文件中以该值为后缀时，才会执行解压缩操作，否则则保持原样传输。当输入*或为空时，所有文件都会被解压。</p>
</td>
<td class="cellrowborder" valign="top" width="21.052105210521052%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0114711714_p549646101615"><a name="zh-cn_topic_0114711714_p549646101615"></a><a name="zh-cn_topic_0114711714_p549646101615"></a>*</p>
</td>
</tr>
<tr id="zh-cn_topic_0114711714_row175761546101619"><td class="cellrowborder" valign="top" width="23.77237723772377%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0114711714_p4577104611615"><a name="zh-cn_topic_0114711714_p4577104611615"></a><a name="zh-cn_topic_0114711714_p4577104611615"></a>文件分隔符</p>
</td>
<td class="cellrowborder" valign="top" width="55.17551755175517%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0114711714_p8813175612198"><a name="zh-cn_topic_0114711714_p8813175612198"></a><a name="zh-cn_topic_0114711714_p8813175612198"></a>传输多个文件时，CDM使用这里配置的文件分隔符来区分各个文件，默认为|。</p>
</td>
<td class="cellrowborder" valign="top" width="21.052105210521052%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0114711714_p11577154631620"><a name="zh-cn_topic_0114711714_p11577154631620"></a><a name="zh-cn_topic_0114711714_p11577154631620"></a>|</p>
</td>
</tr>
<tr id="zh-cn_topic_0114711714_row1539591785713"><td class="cellrowborder" valign="top" width="23.77237723772377%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0114711714_p173961917165716"><a name="zh-cn_topic_0114711714_p173961917165716"></a><a name="zh-cn_topic_0114711714_p173961917165716"></a>QUERY参数</p>
</td>
<td class="cellrowborder" valign="top" width="55.17551755175517%" headers="mcps1.2.4.1.2 "><a name="zh-cn_topic_0114711714_ul887516311069"></a><a name="zh-cn_topic_0114711714_ul887516311069"></a><ul id="zh-cn_topic_0114711714_ul887516311069"><li>该参数设置为<span class="parmvalue" id="zh-cn_topic_0114711714_parmvalue8561326597"><a name="zh-cn_topic_0114711714_parmvalue8561326597"></a><a name="zh-cn_topic_0114711714_parmvalue8561326597"></a>“是”</span>时，上传到OBS的对象使用的对象名，为去掉query参数后的字符。</li><li>该参数设置为<span class="parmvalue" id="zh-cn_topic_0114711714_parmvalue598043819711"><a name="zh-cn_topic_0114711714_parmvalue598043819711"></a><a name="zh-cn_topic_0114711714_parmvalue598043819711"></a>“否”</span>时，上传到OBS的对象使用的对象名，包含query参数。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="21.052105210521052%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0114711714_p143961517125716"><a name="zh-cn_topic_0114711714_p143961517125716"></a><a name="zh-cn_topic_0114711714_p143961517125716"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0114711714_row1825392374119"><td class="cellrowborder" valign="top" width="23.77237723772377%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0114711714_p1273915511715"><a name="zh-cn_topic_0114711714_p1273915511715"></a><a name="zh-cn_topic_0114711714_p1273915511715"></a>加密方式</p>
</td>
<td class="cellrowborder" valign="top" width="55.17551755175517%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0114711714_p943615213200"><a name="zh-cn_topic_0114711714_p943615213200"></a><a name="zh-cn_topic_0114711714_p943615213200"></a>如果源端数据是被加密过的，则CDM支持解密后再导出。这里选择是否对源端数据解密，以及选择解密算法：<a name="zh-cn_topic_0108275319_ul44410501486"></a><a name="zh-cn_topic_0108275319_ul44410501486"></a><ul id="zh-cn_topic_0108275319_ul44410501486"><li>无：不解密，直接导出。</li><li>AES-256-GCM：使用长度为256byte的AES对称加密算法，目前加密算法只支持AES-256-GCM（NoPadding）。该参数在目的端为加密，在源端为解密。</li></ul>
</div>
<p id="zh-cn_topic_0108275442_p1440312818259"><a name="zh-cn_topic_0108275442_p1440312818259"></a><a name="zh-cn_topic_0108275442_p1440312818259"></a>详细使用方法请参见<a href="迁移文件时加解密.md">迁移文件时加解密</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="21.052105210521052%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0114711714_p1173985171713"><a name="zh-cn_topic_0114711714_p1173985171713"></a><a name="zh-cn_topic_0114711714_p1173985171713"></a>AES-256-GCM</p>
</td>
</tr>
<tr id="zh-cn_topic_0114711714_row543132624117"><td class="cellrowborder" valign="top" width="23.77237723772377%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0114711714_p2560191135113"><a name="zh-cn_topic_0114711714_p2560191135113"></a><a name="zh-cn_topic_0114711714_p2560191135113"></a>数据加密密钥</p>
</td>
<td class="cellrowborder" valign="top" width="55.17551755175517%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0114711714_p13560410513"><a name="zh-cn_topic_0114711714_p13560410513"></a><a name="zh-cn_topic_0114711714_p13560410513"></a><span class="parmname" id="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmname776612385559"><a name="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmname776612385559"></a><a name="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmname776612385559"></a>“加密方式”</span>选择<span class="parmvalue" id="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmvalue0767193814558"><a name="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmvalue0767193814558"></a><a name="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmvalue0767193814558"></a>“AES-256-GCM”</span>时显示该参数，密钥由长度64的十六进制数组成，且必须与加密时配置的<span class="parmname" id="zh-cn_topic_0108275319_parmname48334346128"><a name="zh-cn_topic_0108275319_parmname48334346128"></a><a name="zh-cn_topic_0108275319_parmname48334346128"></a>“数据加密密钥”</span>一致。如果不一致系统不会报异常，只是解密出来的数据会错误。</p>
</td>
<td class="cellrowborder" valign="top" width="21.052105210521052%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0114711714_p10560111155111"><a name="zh-cn_topic_0114711714_p10560111155111"></a><a name="zh-cn_topic_0114711714_p10560111155111"></a>DD0AE00DFECD78BF051BCFDA25BD4E320DB0A7AC75A1F3FC3D3C56A457DCDC1B</p>
</td>
</tr>
<tr id="zh-cn_topic_0114711714_row86157268413"><td class="cellrowborder" valign="top" width="23.77237723772377%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0114711714_p24773525117"><a name="zh-cn_topic_0114711714_p24773525117"></a><a name="zh-cn_topic_0114711714_p24773525117"></a>初始化向量</p>
</td>
<td class="cellrowborder" valign="top" width="55.17551755175517%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0114711714_p24771354512"><a name="zh-cn_topic_0114711714_p24771354512"></a><a name="zh-cn_topic_0114711714_p24771354512"></a><span class="parmname" id="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmname9947565563"><a name="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmname9947565563"></a><a name="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmname9947565563"></a>“加密方式”</span>选择<span class="parmvalue" id="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmvalue179471468565"><a name="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmvalue179471468565"></a><a name="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmvalue179471468565"></a>“AES-256-GCM”</span>时显示该参数，初始化向量由长度32的十六进制数组成，且必须与加密时配置的<span class="parmname" id="zh-cn_topic_0108275319_parmname163755565172"><a name="zh-cn_topic_0108275319_parmname163755565172"></a><a name="zh-cn_topic_0108275319_parmname163755565172"></a>“初始化向量”</span>一致。如果不一致系统不会报异常，只是解密出来的数据会错误。</p>
</td>
<td class="cellrowborder" valign="top" width="21.052105210521052%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0114711714_p647775195111"><a name="zh-cn_topic_0114711714_p647775195111"></a><a name="zh-cn_topic_0114711714_p647775195111"></a>5C91687BA886EDCD12ACBC3FF19A3C3F</p>
</td>
</tr>
<tr id="zh-cn_topic_0114711714_row10363922103613"><td class="cellrowborder" valign="top" width="23.77237723772377%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0114711714_p116778319321"><a name="zh-cn_topic_0114711714_p116778319321"></a><a name="zh-cn_topic_0114711714_p116778319321"></a>MD5文件名后缀</p>
</td>
<td class="cellrowborder" valign="top" width="55.17551755175517%" headers="mcps1.2.4.1.2 "><p id="p1929618329481"><a name="p1929618329481"></a><a name="p1929618329481"></a>校验CDM抽取的文件，是否与源文件一致，详细请参见<a href="MD5校验文件一致性.md">MD5校验文件一致性</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="21.052105210521052%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0114711714_p267718319321"><a name="zh-cn_topic_0114711714_p267718319321"></a><a name="zh-cn_topic_0114711714_p267718319321"></a>.md5</p>
</td>
</tr>
</tbody>
</table>

