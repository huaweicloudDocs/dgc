# 配置FTP/SFTP/NAS/SFS目的端参数<a name="dayu_01_0067"></a>

作业中目的连接为[配置FTP/SFTP连接](配置FTP-SFTP连接.md)或[配置NAS/SFS连接](配置NAS-SFS连接.md)时，目的端作业参数如[表1](#zh-cn_topic_0108275434_table5046103815165)所示。

**表 1**  FTP/SFTP/NAS/SFS作为目的端时的作业参数

<a name="zh-cn_topic_0108275434_table5046103815165"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108275434_row585315215165"><th class="cellrowborder" valign="top" width="16.03%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0108275434_p434331215165"><a name="zh-cn_topic_0108275434_p434331215165"></a><a name="zh-cn_topic_0108275434_p434331215165"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="20.4%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0108275434_p1626397215165"><a name="zh-cn_topic_0108275434_p1626397215165"></a><a name="zh-cn_topic_0108275434_p1626397215165"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="46.17%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0108275434_p4231334915165"><a name="zh-cn_topic_0108275434_p4231334915165"></a><a name="zh-cn_topic_0108275434_p4231334915165"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="17.4%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0108275434_p482921015165"><a name="zh-cn_topic_0108275434_p482921015165"></a><a name="zh-cn_topic_0108275434_p482921015165"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108275434_row4012116315165"><td class="cellrowborder" rowspan="3" valign="top" width="16.03%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275434_p4930025215175"><a name="zh-cn_topic_0108275434_p4930025215175"></a><a name="zh-cn_topic_0108275434_p4930025215175"></a>基本参数</p>
</td>
<td class="cellrowborder" valign="top" width="20.4%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275434_p2858877215165"><a name="zh-cn_topic_0108275434_p2858877215165"></a><a name="zh-cn_topic_0108275434_p2858877215165"></a>写入目录</p>
</td>
<td class="cellrowborder" valign="top" width="46.17%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275434_p3398923015165"><a name="zh-cn_topic_0108275434_p3398923015165"></a><a name="zh-cn_topic_0108275434_p3398923015165"></a>写入数据的目录。</p>
<p id="zh-cn_topic_0108275442_p1210244910548"><a name="zh-cn_topic_0108275442_p1210244910548"></a><a name="zh-cn_topic_0108275442_p1210244910548"></a>该参数支持配置为时间宏变量，且一个路径名中可以有多个宏定义变量。使用时间宏变量和定时任务配合，可以实现定期同步新增数据，详细说明请参见<a href="使用时间宏变量完成增量同步.md">使用时间宏变量完成增量同步</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="17.4%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108275434_p166427315165"><a name="zh-cn_topic_0108275434_p166427315165"></a><a name="zh-cn_topic_0108275434_p166427315165"></a>/opt/ftp/</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275434_row1497845915165"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275434_p529563715165"><a name="zh-cn_topic_0108275434_p529563715165"></a><a name="zh-cn_topic_0108275434_p529563715165"></a>文件格式</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><div class="p" id="zh-cn_topic_0108275434_p4648068715203"><a name="zh-cn_topic_0108275434_p4648068715203"></a><a name="zh-cn_topic_0108275434_p4648068715203"></a>写入后的文件格式，可选择以下文件格式：<a name="zh-cn_topic_0108275301_ul55756641143945"></a><a name="zh-cn_topic_0108275301_ul55756641143945"></a><ul id="zh-cn_topic_0108275301_ul55756641143945"><li>CSV格式：按CSV格式写入，适用于数据表到文件的迁移。</li><li>二进制格式：选择<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue13073035195648"><a name="zh-cn_topic_0108275301_parmvalue13073035195648"></a><a name="zh-cn_topic_0108275301_parmvalue13073035195648"></a>“二进制格式”</span>时不解析文件内容直接传输，CDM会原样写入文件，不改变原始文件格式，适用于文件到文件的迁移。</li></ul>
</div>
<p id="zh-cn_topic_0108275434_p4369273215203"><a name="zh-cn_topic_0108275434_p4369273215203"></a><a name="zh-cn_topic_0108275434_p4369273215203"></a>如果是文件类数据源（FTP/SFTP/NAS/HDFS/OBS）之间相互迁移数据，此处的<span class="parmname" id="zh-cn_topic_0108275301_parmname29778793154532"><a name="zh-cn_topic_0108275301_parmname29778793154532"></a><a name="zh-cn_topic_0108275301_parmname29778793154532"></a>“文件格式”</span>只能选择与源端的文件格式一致。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275434_p3753014815165"><a name="zh-cn_topic_0108275434_p3753014815165"></a><a name="zh-cn_topic_0108275434_p3753014815165"></a>CSV格式</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275434_row6530734103243"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275434_p44698576103257"><a name="zh-cn_topic_0108275434_p44698576103257"></a><a name="zh-cn_topic_0108275434_p44698576103257"></a>重复文件处理方式</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><div class="p" id="zh-cn_topic_0108275434_p63814919103257"><a name="zh-cn_topic_0108275434_p63814919103257"></a><a name="zh-cn_topic_0108275434_p63814919103257"></a>只有文件名和文件大小都相同才会判定为重复文件。写入时如果出现文件重复，可选择如下处理方式：<a name="zh-cn_topic_0108275301_ul38524806103122"></a><a name="zh-cn_topic_0108275301_ul38524806103122"></a><ul id="zh-cn_topic_0108275301_ul38524806103122"><li>替换重复文件</li><li>跳过重复文件</li><li>停止任务</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275434_p64851000103257"><a name="zh-cn_topic_0108275434_p64851000103257"></a><a name="zh-cn_topic_0108275434_p64851000103257"></a>跳过重复文件</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275434_row3482998115165"><td class="cellrowborder" rowspan="13" valign="top" width="16.03%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275434_p59649567161429"><a name="zh-cn_topic_0108275434_p59649567161429"></a><a name="zh-cn_topic_0108275434_p59649567161429"></a>高级属性</p>
</td>
<td class="cellrowborder" valign="top" width="20.4%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275434_p265625015165"><a name="zh-cn_topic_0108275434_p265625015165"></a><a name="zh-cn_topic_0108275434_p265625015165"></a>换行符</p>
</td>
<td class="cellrowborder" valign="top" width="46.17%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275434_p4684560152026"><a name="zh-cn_topic_0108275434_p4684560152026"></a><a name="zh-cn_topic_0108275434_p4684560152026"></a>文件中的换行符，默认自动识别<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue20019196113242"><a name="zh-cn_topic_0108275301_parmvalue20019196113242"></a><a name="zh-cn_topic_0108275301_parmvalue20019196113242"></a>“\n”</span>、<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue34571243113250"><a name="zh-cn_topic_0108275301_parmvalue34571243113250"></a><a name="zh-cn_topic_0108275301_parmvalue34571243113250"></a>“\r”</span>或<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue1038974611337"><a name="zh-cn_topic_0108275301_parmvalue1038974611337"></a><a name="zh-cn_topic_0108275301_parmvalue1038974611337"></a>“\r\n”</span>。<span class="parmname" id="zh-cn_topic_0108275301_parmname23758818145740"><a name="zh-cn_topic_0108275301_parmname23758818145740"></a><a name="zh-cn_topic_0108275301_parmname23758818145740"></a>“文件格式”</span>为<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue46072507145830"><a name="zh-cn_topic_0108275301_parmvalue46072507145830"></a><a name="zh-cn_topic_0108275301_parmvalue46072507145830"></a>“二进制格式”</span>时该参数值无效。</p>
</td>
<td class="cellrowborder" valign="top" width="17.4%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108275434_p4854631115165"><a name="zh-cn_topic_0108275434_p4854631115165"></a><a name="zh-cn_topic_0108275434_p4854631115165"></a>\n</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275434_row3426361615165"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275434_p2388955115165"><a name="zh-cn_topic_0108275434_p2388955115165"></a><a name="zh-cn_topic_0108275434_p2388955115165"></a>字段分隔符</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275434_p3174568152026"><a name="zh-cn_topic_0108275434_p3174568152026"></a><a name="zh-cn_topic_0108275434_p3174568152026"></a>文件中的字段分隔符。<span class="parmname" id="zh-cn_topic_0108275301_parmname3855270114580"><a name="zh-cn_topic_0108275301_parmname3855270114580"></a><a name="zh-cn_topic_0108275301_parmname3855270114580"></a>“文件格式”</span>为<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue27349529145857"><a name="zh-cn_topic_0108275301_parmvalue27349529145857"></a><a name="zh-cn_topic_0108275301_parmvalue27349529145857"></a>“二进制格式”</span>时该参数值无效。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275434_p4015252715165"><a name="zh-cn_topic_0108275434_p4015252715165"></a><a name="zh-cn_topic_0108275434_p4015252715165"></a>,</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275434_row1351311581494"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275434_p1848919333580"><a name="zh-cn_topic_0108275434_p1848919333580"></a><a name="zh-cn_topic_0108275434_p1848919333580"></a>写入文件大小</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275434_p34895339587"><a name="zh-cn_topic_0108275434_p34895339587"></a><a name="zh-cn_topic_0108275434_p34895339587"></a>源端为数据库时该参数才显示，支持按大小分成多个文件存储，避免导出的文件过大，单位为MB。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275434_p9489113313583"><a name="zh-cn_topic_0108275434_p9489113313583"></a><a name="zh-cn_topic_0108275434_p9489113313583"></a>1024</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275434_row135659916647"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275434_p5093321916739"><a name="zh-cn_topic_0108275434_p5093321916739"></a><a name="zh-cn_topic_0108275434_p5093321916739"></a>编码类型</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275434_p1356036720516"><a name="zh-cn_topic_0108275434_p1356036720516"></a><a name="zh-cn_topic_0108275434_p1356036720516"></a>文件编码类型，例如：<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue4971784420504"><a name="zh-cn_topic_0108275301_parmvalue4971784420504"></a><a name="zh-cn_topic_0108275301_parmvalue4971784420504"></a>“UTF-8”</span>或<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue61358620504"><a name="zh-cn_topic_0108275301_parmvalue61358620504"></a><a name="zh-cn_topic_0108275301_parmvalue61358620504"></a>“GBK”</span>。<span class="parmname" id="zh-cn_topic_0108275301_parmname66615771145817"><a name="zh-cn_topic_0108275301_parmname66615771145817"></a><a name="zh-cn_topic_0108275301_parmname66615771145817"></a>“文件格式”</span>为<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue52502287145839"><a name="zh-cn_topic_0108275301_parmvalue52502287145839"></a><a name="zh-cn_topic_0108275301_parmvalue52502287145839"></a>“二进制格式”</span>时该参数值无效。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275434_p227755916647"><a name="zh-cn_topic_0108275434_p227755916647"></a><a name="zh-cn_topic_0108275434_p227755916647"></a>GBK</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275434_row195520317337"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275434_p15557312333"><a name="zh-cn_topic_0108275434_p15557312333"></a><a name="zh-cn_topic_0108275434_p15557312333"></a>使用包围符</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275434_p1055163133310"><a name="zh-cn_topic_0108275434_p1055163133310"></a><a name="zh-cn_topic_0108275434_p1055163133310"></a><span class="parmname" id="zh-cn_topic_0108275301_parmname111029121339"><a name="zh-cn_topic_0108275301_parmname111029121339"></a><a name="zh-cn_topic_0108275301_parmname111029121339"></a>“文件格式”</span>为<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue910281223312"><a name="zh-cn_topic_0108275301_parmvalue910281223312"></a><a name="zh-cn_topic_0108275301_parmvalue910281223312"></a>“CSV格式”</span>，才有该参数，用于将数据库的表迁移到文件系统的场景。</p>
<p id="zh-cn_topic_0108275434_p136507120342"><a name="zh-cn_topic_0108275434_p136507120342"></a><a name="zh-cn_topic_0108275434_p136507120342"></a>选择<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue13709134210325"><a name="zh-cn_topic_0108275301_parmvalue13709134210325"></a><a name="zh-cn_topic_0108275301_parmvalue13709134210325"></a>“是”</span>时，如果源端数据表中的某一个字段内容包含字段分隔符或换行符，写入目的端时CDM会使用双引号（"）作为包围符将该字段内容括起来，作为一个整体存储，避免其中的字段分隔符误将一个字段分隔成两个，或者换行符误将字段换行。例如：数据库中某字段为hello,world，使用包围符后，导出到CSV文件的时候数据为"hello,world"。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275434_p0551431183320"><a name="zh-cn_topic_0108275434_p0551431183320"></a><a name="zh-cn_topic_0108275434_p0551431183320"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275434_row12960118143814"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275434_p596018814389"><a name="zh-cn_topic_0108275434_p596018814389"></a><a name="zh-cn_topic_0108275434_p596018814389"></a>写入到临时文件</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275434_p169603823818"><a name="zh-cn_topic_0108275434_p169603823818"></a><a name="zh-cn_topic_0108275434_p169603823818"></a>将二进制文件先写入到临时文件（临时文件以<span class="uicontrol" id="zh-cn_topic_0108275434_uicontrol1814221324816"><a name="zh-cn_topic_0108275434_uicontrol1814221324816"></a><a name="zh-cn_topic_0108275434_uicontrol1814221324816"></a>“.tmp”</span>作为后缀），迁移成功后，再进行rename或move操作，在目的端恢复文件。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275434_p10960489386"><a name="zh-cn_topic_0108275434_p10960489386"></a><a name="zh-cn_topic_0108275434_p10960489386"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275434_row4164141523814"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275434_p1016418153386"><a name="zh-cn_topic_0108275434_p1016418153386"></a><a name="zh-cn_topic_0108275434_p1016418153386"></a>生成文件MD5值</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275434_p53601941494"><a name="zh-cn_topic_0108275434_p53601941494"></a><a name="zh-cn_topic_0108275434_p53601941494"></a>源端为文件系统（OBS/FTP/SFTP/NAS/HDFS），目的端为FTP/SFP/NAS，且文件格式为<span class="parmvalue" id="zh-cn_topic_0108275434_parmvalue03601240499"><a name="zh-cn_topic_0108275434_parmvalue03601240499"></a><a name="zh-cn_topic_0108275434_parmvalue03601240499"></a>“二进制”</span>时，才有该参数。</p>
<p id="zh-cn_topic_0108275434_p18361106194911"><a name="zh-cn_topic_0108275434_p18361106194911"></a><a name="zh-cn_topic_0108275434_p18361106194911"></a>对每个传输的文件都生成一个MD5值，并将该值记录在一个新文件中（新文件以<span class="uicontrol" id="zh-cn_topic_0108275434_uicontrol78827455013"><a name="zh-cn_topic_0108275434_uicontrol78827455013"></a><a name="zh-cn_topic_0108275434_uicontrol78827455013"></a>“.md5”</span>作为后缀），且可以指定MD5值生成的目录。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275434_p416413158385"><a name="zh-cn_topic_0108275434_p416413158385"></a><a name="zh-cn_topic_0108275434_p416413158385"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275434_row6698164342313"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275434_p116986439239"><a name="zh-cn_topic_0108275434_p116986439239"></a><a name="zh-cn_topic_0108275434_p116986439239"></a>MD5值写入的目录</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275434_p1698134317233"><a name="zh-cn_topic_0108275434_p1698134317233"></a><a name="zh-cn_topic_0108275434_p1698134317233"></a>自定义MD5值写入的目录。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275434_p66981543172312"><a name="zh-cn_topic_0108275434_p66981543172312"></a><a name="zh-cn_topic_0108275434_p66981543172312"></a>/md5</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275434_row1142412103255"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275434_p13851563214"><a name="zh-cn_topic_0108275434_p13851563214"></a><a name="zh-cn_topic_0108275434_p13851563214"></a>首行为标题行</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275434_p68171593216"><a name="zh-cn_topic_0108275434_p68171593216"></a><a name="zh-cn_topic_0108275434_p68171593216"></a><span class="parmname" id="zh-cn_topic_0108275301_parmname19396452103317"><a name="zh-cn_topic_0108275301_parmname19396452103317"></a><a name="zh-cn_topic_0108275301_parmname19396452103317"></a>“文件格式”</span>为<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue739785211338"><a name="zh-cn_topic_0108275301_parmvalue739785211338"></a><a name="zh-cn_topic_0108275301_parmvalue739785211338"></a>“CSV格式”</span>时才有该参数。在迁移表到CSV文件时，CDM默认是不迁移表的标题行，如果该参数选择<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue11024151389"><a name="zh-cn_topic_0108275301_parmvalue11024151389"></a><a name="zh-cn_topic_0108275301_parmvalue11024151389"></a>“是”</span>，CDM在才会将表的标题行数据写入文件。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275434_p582155329"><a name="zh-cn_topic_0108275434_p582155329"></a><a name="zh-cn_topic_0108275434_p582155329"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275434_row6168132121513"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275434_p916842118158"><a name="zh-cn_topic_0108275434_p916842118158"></a><a name="zh-cn_topic_0108275434_p916842118158"></a>作业成功标识文件</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275434_p12168921151518"><a name="zh-cn_topic_0108275434_p12168921151518"></a><a name="zh-cn_topic_0108275434_p12168921151518"></a>当作业执行成功时，会在写入目录下生成一个标识文件，文件名由用户指定。不指定时默认关闭该功能。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275434_p192821858181918"><a name="zh-cn_topic_0108275434_p192821858181918"></a><a name="zh-cn_topic_0108275434_p192821858181918"></a>finish.txt</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275434_row19725102919247"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275434_p1273915511715"><a name="zh-cn_topic_0108275434_p1273915511715"></a><a name="zh-cn_topic_0108275434_p1273915511715"></a>加密方式</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><div class="p" id="zh-cn_topic_0108275434_p1155816444583"><a name="zh-cn_topic_0108275434_p1155816444583"></a><a name="zh-cn_topic_0108275434_p1155816444583"></a>选择是否对写入的数据进行加密：<a name="zh-cn_topic_0108275448_ul363465719521"></a><a name="zh-cn_topic_0108275448_ul363465719521"></a><ul id="zh-cn_topic_0108275448_ul363465719521"><li>无：不加密，直接写入数据。</li><li>AES-256-GCM：使用长度为256byte的AES对称加密算法，目前加密算法只支持AES-256-GCM（NoPadding）。该参数在目的端为加密，在源端为解密。</li></ul>
</div>
<p id="zh-cn_topic_0108275442_p1440312818259"><a name="zh-cn_topic_0108275442_p1440312818259"></a><a name="zh-cn_topic_0108275442_p1440312818259"></a>详细使用方法请参见<a href="迁移文件时加解密.md">迁移文件时加解密</a>。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275434_p1173985171713"><a name="zh-cn_topic_0108275434_p1173985171713"></a><a name="zh-cn_topic_0108275434_p1173985171713"></a>AES-256-GCM</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275434_row18953123242417"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275434_p2560191135113"><a name="zh-cn_topic_0108275434_p2560191135113"></a><a name="zh-cn_topic_0108275434_p2560191135113"></a>数据加密密钥</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275434_p13560410513"><a name="zh-cn_topic_0108275434_p13560410513"></a><a name="zh-cn_topic_0108275434_p13560410513"></a><span class="parmname" id="zh-cn_topic_0108275301_parmname776612385559"><a name="zh-cn_topic_0108275301_parmname776612385559"></a><a name="zh-cn_topic_0108275301_parmname776612385559"></a>“加密方式”</span>选择<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue0767193814558"><a name="zh-cn_topic_0108275301_parmvalue0767193814558"></a><a name="zh-cn_topic_0108275301_parmvalue0767193814558"></a>“AES-256-GCM”</span>时显示该参数，密钥由长度64的十六进制数组成。</p>
<p id="zh-cn_topic_0108275434_p18430442724"><a name="zh-cn_topic_0108275434_p18430442724"></a><a name="zh-cn_topic_0108275434_p18430442724"></a>请您牢记这里配置的<span class="parmname" id="zh-cn_topic_0108275301_parmname035312613138"><a name="zh-cn_topic_0108275301_parmname035312613138"></a><a name="zh-cn_topic_0108275301_parmname035312613138"></a>“数据加密密钥”</span>，解密时的密钥与这里配置的必须一致。如果不一致系统不会报异常，只是解密出来的数据会错误。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275434_p10560111155111"><a name="zh-cn_topic_0108275434_p10560111155111"></a><a name="zh-cn_topic_0108275434_p10560111155111"></a>DD0AE00DFECD78BF051BCFDA25BD4E320DB0A7AC75A1F3FC3D3C56A457DCDC1B</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275434_row13991143515249"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275434_p24773525117"><a name="zh-cn_topic_0108275434_p24773525117"></a><a name="zh-cn_topic_0108275434_p24773525117"></a>初始化向量</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275434_p24771354512"><a name="zh-cn_topic_0108275434_p24771354512"></a><a name="zh-cn_topic_0108275434_p24771354512"></a><span class="parmname" id="zh-cn_topic_0108275301_parmname9947565563"><a name="zh-cn_topic_0108275301_parmname9947565563"></a><a name="zh-cn_topic_0108275301_parmname9947565563"></a>“加密方式”</span>选择<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue179471468565"><a name="zh-cn_topic_0108275301_parmvalue179471468565"></a><a name="zh-cn_topic_0108275301_parmvalue179471468565"></a>“AES-256-GCM”</span>时显示该参数，初始化向量由长度32的十六进制数组成。</p>
<p id="zh-cn_topic_0108275434_p1645862617304"><a name="zh-cn_topic_0108275434_p1645862617304"></a><a name="zh-cn_topic_0108275434_p1645862617304"></a>请您牢记这里配置的<span class="parmname" id="zh-cn_topic_0108275301_parmname91651822122920"><a name="zh-cn_topic_0108275301_parmname91651822122920"></a><a name="zh-cn_topic_0108275301_parmname91651822122920"></a>“初始化向量”</span>，解密时的初始化向量与这里配置的必须一致。如果不一致系统不会报异常，只是解密出来的数据会错误。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275434_p647775195111"><a name="zh-cn_topic_0108275434_p647775195111"></a><a name="zh-cn_topic_0108275434_p647775195111"></a>5C91687BA886EDCD12ACBC3FF19A3C3F</p>
</td>
</tr>
</tbody>
</table>

