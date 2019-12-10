# 配置HDFS目的端参数<a name="dayu_01_0063"></a>

作业中目的连接为[配置HDFS连接](配置HDFS连接.md)时，即导入数据到以下数据源时，目的端作业参数如[表1](#zh-cn_topic_0108275448_table5046103815165)所示。

**表 1**  HDFS作为目的端时的作业参数

<a name="zh-cn_topic_0108275448_table5046103815165"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108275448_row585315215165"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0108275448_p1626397215165"><a name="zh-cn_topic_0108275448_p1626397215165"></a><a name="zh-cn_topic_0108275448_p1626397215165"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="55.00000000000001%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0108275448_p4231334915165"><a name="zh-cn_topic_0108275448_p4231334915165"></a><a name="zh-cn_topic_0108275448_p4231334915165"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0108275448_p482921015165"><a name="zh-cn_topic_0108275448_p482921015165"></a><a name="zh-cn_topic_0108275448_p482921015165"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108275448_row4012116315165"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275448_p2858877215165"><a name="zh-cn_topic_0108275448_p2858877215165"></a><a name="zh-cn_topic_0108275448_p2858877215165"></a>写入目录</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275448_p3398923015165"><a name="zh-cn_topic_0108275448_p3398923015165"></a><a name="zh-cn_topic_0108275448_p3398923015165"></a>写入数据到HDFS服务器的目录。</p>
<p id="zh-cn_topic_0108275442_p1210244910548"><a name="zh-cn_topic_0108275442_p1210244910548"></a><a name="zh-cn_topic_0108275442_p1210244910548"></a>该参数支持配置为时间宏变量，且一个路径名中可以有多个宏定义变量。使用时间宏变量和定时任务配合，可以实现定期同步新增数据，详细说明请参见<a href="使用时间宏变量完成增量同步.md">使用时间宏变量完成增量同步</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275448_p166427315165"><a name="zh-cn_topic_0108275448_p166427315165"></a><a name="zh-cn_topic_0108275448_p166427315165"></a>/user/output</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275448_row1497845915165"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275448_p529563715165"><a name="zh-cn_topic_0108275448_p529563715165"></a><a name="zh-cn_topic_0108275448_p529563715165"></a>文件格式</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108275448_p58390965143945"><a name="zh-cn_topic_0108275448_p58390965143945"></a><a name="zh-cn_topic_0108275448_p58390965143945"></a>写入后的文件格式，可选择以下文件格式：<a name="zh-cn_topic_0108275301_ul55756641143945"></a><a name="zh-cn_topic_0108275301_ul55756641143945"></a><ul id="zh-cn_topic_0108275301_ul55756641143945"><li>CSV格式：按CSV格式写入，适用于数据表到文件的迁移。</li><li>二进制格式：选择<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue13073035195648"><a name="zh-cn_topic_0108275301_parmvalue13073035195648"></a><a name="zh-cn_topic_0108275301_parmvalue13073035195648"></a>“二进制格式”</span>时不解析文件内容直接传输，CDM会原样写入文件，不改变原始文件格式，适用于文件到文件的迁移。</li></ul>
</div>
<p id="zh-cn_topic_0108275448_p5736095154452"><a name="zh-cn_topic_0108275448_p5736095154452"></a><a name="zh-cn_topic_0108275448_p5736095154452"></a>如果是文件类数据源（FTP/SFTP/NAS/HDFS/OBS）之间相互迁移数据，此处的<span class="parmname" id="zh-cn_topic_0108275301_parmname29778793154532"><a name="zh-cn_topic_0108275301_parmname29778793154532"></a><a name="zh-cn_topic_0108275301_parmname29778793154532"></a>“文件格式”</span>只能选择与源端的文件格式一致。</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275448_p3753014815165"><a name="zh-cn_topic_0108275448_p3753014815165"></a><a name="zh-cn_topic_0108275448_p3753014815165"></a>CSV格式</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275448_row17105247152948"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275448_p7164047103335"><a name="zh-cn_topic_0108275448_p7164047103335"></a><a name="zh-cn_topic_0108275448_p7164047103335"></a>重复文件处理方式</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108275448_p43416941103335"><a name="zh-cn_topic_0108275448_p43416941103335"></a><a name="zh-cn_topic_0108275448_p43416941103335"></a>只有文件名和文件大小都相同才会判定为重复文件。写入时如果出现文件重复，可选择如下处理方式：<a name="zh-cn_topic_0108275301_ul38524806103122"></a><a name="zh-cn_topic_0108275301_ul38524806103122"></a><ul id="zh-cn_topic_0108275301_ul38524806103122"><li>替换重复文件</li><li>跳过重复文件</li><li>停止任务</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275448_p39227948103335"><a name="zh-cn_topic_0108275448_p39227948103335"></a><a name="zh-cn_topic_0108275448_p39227948103335"></a>停止任务</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275448_row2317175816829"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275448_p5753610216847"><a name="zh-cn_topic_0108275448_p5753610216847"></a><a name="zh-cn_topic_0108275448_p5753610216847"></a>压缩格式</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.4.1.2 "><div class="p" id="zh-cn_topic_0108275448_p2991266716847"><a name="zh-cn_topic_0108275448_p2991266716847"></a><a name="zh-cn_topic_0108275448_p2991266716847"></a>写入文件后，选择对文件的压缩格式。支持以下压缩格式：<a name="zh-cn_topic_0108275448_ul77855316847"></a><a name="zh-cn_topic_0108275448_ul77855316847"></a><ul id="zh-cn_topic_0108275448_ul77855316847"><li>NONE：不压缩。</li><li>DEFLATE：压缩为DEFLATE格式。</li><li>GZIP：压缩为GZIP格式。</li><li>BZIP2：压缩为BZIP2格式。</li><li>LZ4：压缩为LZ4格式。</li><li>SNAPPY：压缩为SNAPPY格式。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275448_p5697647216847"><a name="zh-cn_topic_0108275448_p5697647216847"></a><a name="zh-cn_topic_0108275448_p5697647216847"></a>SNAPPY</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275448_row17596707153214"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275448_p19502615153235"><a name="zh-cn_topic_0108275448_p19502615153235"></a><a name="zh-cn_topic_0108275448_p19502615153235"></a>换行符</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275448_p57707849205028"><a name="zh-cn_topic_0108275448_p57707849205028"></a><a name="zh-cn_topic_0108275448_p57707849205028"></a>文件中的换行符，默认自动识别<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue20019196113242"><a name="zh-cn_topic_0108275301_parmvalue20019196113242"></a><a name="zh-cn_topic_0108275301_parmvalue20019196113242"></a>“\n”</span>、<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue34571243113250"><a name="zh-cn_topic_0108275301_parmvalue34571243113250"></a><a name="zh-cn_topic_0108275301_parmvalue34571243113250"></a>“\r”</span>或<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue1038974611337"><a name="zh-cn_topic_0108275301_parmvalue1038974611337"></a><a name="zh-cn_topic_0108275301_parmvalue1038974611337"></a>“\r\n”</span>。<span class="parmname" id="zh-cn_topic_0108275301_parmname23758818145740"><a name="zh-cn_topic_0108275301_parmname23758818145740"></a><a name="zh-cn_topic_0108275301_parmname23758818145740"></a>“文件格式”</span>为<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue46072507145830"><a name="zh-cn_topic_0108275301_parmvalue46072507145830"></a><a name="zh-cn_topic_0108275301_parmvalue46072507145830"></a>“二进制格式”</span>时该参数值无效。</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275448_p24750930153235"><a name="zh-cn_topic_0108275448_p24750930153235"></a><a name="zh-cn_topic_0108275448_p24750930153235"></a>\n</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275448_row41209902153231"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275448_p58252442153235"><a name="zh-cn_topic_0108275448_p58252442153235"></a><a name="zh-cn_topic_0108275448_p58252442153235"></a>字段分隔符</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275448_p36028355205028"><a name="zh-cn_topic_0108275448_p36028355205028"></a><a name="zh-cn_topic_0108275448_p36028355205028"></a>文件中的字段分隔符。<span class="parmname" id="zh-cn_topic_0108275301_parmname3855270114580"><a name="zh-cn_topic_0108275301_parmname3855270114580"></a><a name="zh-cn_topic_0108275301_parmname3855270114580"></a>“文件格式”</span>为<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue27349529145857"><a name="zh-cn_topic_0108275301_parmvalue27349529145857"></a><a name="zh-cn_topic_0108275301_parmvalue27349529145857"></a>“二进制格式”</span>时该参数值无效。</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275448_p9292827153235"><a name="zh-cn_topic_0108275448_p9292827153235"></a><a name="zh-cn_topic_0108275448_p9292827153235"></a>,</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275448_row9185716185910"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275448_p147801323132816"><a name="zh-cn_topic_0108275448_p147801323132816"></a><a name="zh-cn_topic_0108275448_p147801323132816"></a>使用包围符</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275448_p1210241263316"><a name="zh-cn_topic_0108275448_p1210241263316"></a><a name="zh-cn_topic_0108275448_p1210241263316"></a><span class="parmname" id="zh-cn_topic_0108275301_parmname111029121339"><a name="zh-cn_topic_0108275301_parmname111029121339"></a><a name="zh-cn_topic_0108275301_parmname111029121339"></a>“文件格式”</span>为<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue910281223312"><a name="zh-cn_topic_0108275301_parmvalue910281223312"></a><a name="zh-cn_topic_0108275301_parmvalue910281223312"></a>“CSV格式”</span>，才有该参数，用于将数据库的表迁移到文件系统的场景。</p>
<p id="zh-cn_topic_0108275448_p19249144319"><a name="zh-cn_topic_0108275448_p19249144319"></a><a name="zh-cn_topic_0108275448_p19249144319"></a>选择<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue13709134210325"><a name="zh-cn_topic_0108275301_parmvalue13709134210325"></a><a name="zh-cn_topic_0108275301_parmvalue13709134210325"></a>“是”</span>时，如果源端数据表中的某一个字段内容包含字段分隔符或换行符，写入目的端时CDM会使用双引号（"）作为包围符将该字段内容括起来，作为一个整体存储，避免其中的字段分隔符误将一个字段分隔成两个，或者换行符误将字段换行。例如：数据库中某字段为hello,world，使用包围符后，导出到CSV文件的时候数据为"hello,world"。</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275448_p778018234281"><a name="zh-cn_topic_0108275448_p778018234281"></a><a name="zh-cn_topic_0108275448_p778018234281"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275448_row9627105312214"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275448_p13851563214"><a name="zh-cn_topic_0108275448_p13851563214"></a><a name="zh-cn_topic_0108275448_p13851563214"></a>首行为标题行</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275448_p68171593216"><a name="zh-cn_topic_0108275448_p68171593216"></a><a name="zh-cn_topic_0108275448_p68171593216"></a><span class="parmname" id="zh-cn_topic_0108275301_parmname19396452103317"><a name="zh-cn_topic_0108275301_parmname19396452103317"></a><a name="zh-cn_topic_0108275301_parmname19396452103317"></a>“文件格式”</span>为<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue739785211338"><a name="zh-cn_topic_0108275301_parmvalue739785211338"></a><a name="zh-cn_topic_0108275301_parmvalue739785211338"></a>“CSV格式”</span>时才有该参数。在迁移表到CSV文件时，CDM默认是不迁移表的标题行，如果该参数选择<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue11024151389"><a name="zh-cn_topic_0108275301_parmvalue11024151389"></a><a name="zh-cn_topic_0108275301_parmvalue11024151389"></a>“是”</span>，CDM在才会将表的标题行数据写入文件。</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275448_p582155329"><a name="zh-cn_topic_0108275448_p582155329"></a><a name="zh-cn_topic_0108275448_p582155329"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275448_row139451454251"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275448_p596018814389"><a name="zh-cn_topic_0108275448_p596018814389"></a><a name="zh-cn_topic_0108275448_p596018814389"></a>写入到临时文件</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275448_p169603823818"><a name="zh-cn_topic_0108275448_p169603823818"></a><a name="zh-cn_topic_0108275448_p169603823818"></a>将二进制文件先写入到临时文件（临时文件以<span class="uicontrol" id="zh-cn_topic_0108275434_uicontrol1814221324816"><a name="zh-cn_topic_0108275434_uicontrol1814221324816"></a><a name="zh-cn_topic_0108275434_uicontrol1814221324816"></a>“.tmp”</span>作为后缀），迁移成功后，再进行rename或move操作，在目的端恢复文件。</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275448_p1194674515250"><a name="zh-cn_topic_0108275448_p1194674515250"></a><a name="zh-cn_topic_0108275448_p1194674515250"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275448_row18663102155916"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275448_p52821758161913"><a name="zh-cn_topic_0108275448_p52821758161913"></a><a name="zh-cn_topic_0108275448_p52821758161913"></a>作业成功标识文件</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275448_p2282115811910"><a name="zh-cn_topic_0108275448_p2282115811910"></a><a name="zh-cn_topic_0108275448_p2282115811910"></a>当作业执行成功时，会在写入目录下生成一个标识文件，文件名由用户指定。不指定时默认关闭该功能。</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275448_p192821858181918"><a name="zh-cn_topic_0108275448_p192821858181918"></a><a name="zh-cn_topic_0108275448_p192821858181918"></a>finish.txt</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275448_row16739255178"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275448_p1273915511715"><a name="zh-cn_topic_0108275448_p1273915511715"></a><a name="zh-cn_topic_0108275448_p1273915511715"></a>加密方式</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275448_p87391251172"><a name="zh-cn_topic_0108275448_p87391251172"></a><a name="zh-cn_topic_0108275448_p87391251172"></a><span class="parmname" id="zh-cn_topic_0108275448_parmname103132381818"><a name="zh-cn_topic_0108275448_parmname103132381818"></a><a name="zh-cn_topic_0108275448_parmname103132381818"></a>“文件格式”</span>选择<span class="parmvalue" id="zh-cn_topic_0108275448_parmvalue42720331181"><a name="zh-cn_topic_0108275448_parmvalue42720331181"></a><a name="zh-cn_topic_0108275448_parmvalue42720331181"></a>“二进制格式”</span>时，该参数才显示。</p>
<div class="p" id="zh-cn_topic_0108275448_p134714725211"><a name="zh-cn_topic_0108275448_p134714725211"></a><a name="zh-cn_topic_0108275448_p134714725211"></a>选择是否对写入的数据进行加密：<a name="zh-cn_topic_0108275448_ul363465719521"></a><a name="zh-cn_topic_0108275448_ul363465719521"></a><ul id="zh-cn_topic_0108275448_ul363465719521"><li>无：不加密，直接写入数据。</li><li>AES-256-GCM：使用长度为256byte的AES对称加密算法，目前加密算法只支持AES-256-GCM（NoPadding）。该参数在目的端为加密，在源端为解密。</li></ul>
</div>
<p id="zh-cn_topic_0108275448_p943615213200"><a name="zh-cn_topic_0108275448_p943615213200"></a><a name="zh-cn_topic_0108275448_p943615213200"></a>详细使用方法请参见<a href="迁移文件时加解密.md">迁移文件时加解密</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275448_p1173985171713"><a name="zh-cn_topic_0108275448_p1173985171713"></a><a name="zh-cn_topic_0108275448_p1173985171713"></a>AES-256-GCM</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275448_row16239201411176"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275448_p2560191135113"><a name="zh-cn_topic_0108275448_p2560191135113"></a><a name="zh-cn_topic_0108275448_p2560191135113"></a>数据加密密钥</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275448_p13560410513"><a name="zh-cn_topic_0108275448_p13560410513"></a><a name="zh-cn_topic_0108275448_p13560410513"></a><span class="parmname" id="zh-cn_topic_0108275301_parmname776612385559"><a name="zh-cn_topic_0108275301_parmname776612385559"></a><a name="zh-cn_topic_0108275301_parmname776612385559"></a>“加密方式”</span>选择<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue0767193814558"><a name="zh-cn_topic_0108275301_parmvalue0767193814558"></a><a name="zh-cn_topic_0108275301_parmvalue0767193814558"></a>“AES-256-GCM”</span>时显示该参数，密钥由长度64的十六进制数组成。</p>
<p id="zh-cn_topic_0108275448_p18430442724"><a name="zh-cn_topic_0108275448_p18430442724"></a><a name="zh-cn_topic_0108275448_p18430442724"></a>请您牢记这里配置的<span class="parmname" id="zh-cn_topic_0108275301_parmname035312613138"><a name="zh-cn_topic_0108275301_parmname035312613138"></a><a name="zh-cn_topic_0108275301_parmname035312613138"></a>“数据加密密钥”</span>，解密时的密钥与这里配置的必须一致。如果不一致系统不会报异常，只是解密出来的数据会错误。</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275448_p10560111155111"><a name="zh-cn_topic_0108275448_p10560111155111"></a><a name="zh-cn_topic_0108275448_p10560111155111"></a>DD0AE00DFECD78BF051BCFDA25BD4E320DB0A7AC75A1F3FC3D3C56A457DCDC1B</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275448_row8742102315171"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0108275448_p24773525117"><a name="zh-cn_topic_0108275448_p24773525117"></a><a name="zh-cn_topic_0108275448_p24773525117"></a>初始化向量</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0108275448_p24771354512"><a name="zh-cn_topic_0108275448_p24771354512"></a><a name="zh-cn_topic_0108275448_p24771354512"></a><span class="parmname" id="zh-cn_topic_0108275301_parmname9947565563"><a name="zh-cn_topic_0108275301_parmname9947565563"></a><a name="zh-cn_topic_0108275301_parmname9947565563"></a>“加密方式”</span>选择<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue179471468565"><a name="zh-cn_topic_0108275301_parmvalue179471468565"></a><a name="zh-cn_topic_0108275301_parmvalue179471468565"></a>“AES-256-GCM”</span>时显示该参数，初始化向量由长度32的十六进制数组成。</p>
<p id="zh-cn_topic_0108275448_p1645862617304"><a name="zh-cn_topic_0108275448_p1645862617304"></a><a name="zh-cn_topic_0108275448_p1645862617304"></a>请您牢记这里配置的<span class="parmname" id="zh-cn_topic_0108275301_parmname91651822122920"><a name="zh-cn_topic_0108275301_parmname91651822122920"></a><a name="zh-cn_topic_0108275301_parmname91651822122920"></a>“初始化向量”</span>，解密时的初始化向量与这里配置的必须一致。如果不一致系统不会报异常，只是解密出来的数据会错误。</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0108275448_p647775195111"><a name="zh-cn_topic_0108275448_p647775195111"></a><a name="zh-cn_topic_0108275448_p647775195111"></a>5C91687BA886EDCD12ACBC3FF19A3C3F</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：**   
>HDFS文件编码只能为“UTF-8“，故HDFS不支持设置文件编码类型。  

