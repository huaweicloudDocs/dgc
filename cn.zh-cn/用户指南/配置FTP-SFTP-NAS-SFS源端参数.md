# 配置FTP/SFTP/NAS/SFS源端参数<a name="dayu_01_0052"></a>

作业中源连接为[配置FTP/SFTP连接](配置FTP-SFTP连接.md)或[配置NAS/SFS连接](配置NAS-SFS连接.md)时，源端作业参数如[表1](#zh-cn_topic_0108275374_table5046103815165)所示。

高级属性里的参数为可选参数，默认隐藏，单击界面上的“显示高级属性“后显示。

**表 1**  FTP/SFTP/NAS/SFS作为源端时的作业参数

<a name="zh-cn_topic_0108275374_table5046103815165"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108275374_row585315215165"><th class="cellrowborder" valign="top" width="17.349999999999998%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0108275374_p434331215165"><a name="zh-cn_topic_0108275374_p434331215165"></a><a name="zh-cn_topic_0108275374_p434331215165"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="19.650000000000002%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0108275374_p1626397215165"><a name="zh-cn_topic_0108275374_p1626397215165"></a><a name="zh-cn_topic_0108275374_p1626397215165"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="45.6%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0108275374_p4231334915165"><a name="zh-cn_topic_0108275374_p4231334915165"></a><a name="zh-cn_topic_0108275374_p4231334915165"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="17.4%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0108275374_p482921015165"><a name="zh-cn_topic_0108275374_p482921015165"></a><a name="zh-cn_topic_0108275374_p482921015165"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108275374_row4012116315165"><td class="cellrowborder" rowspan="4" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275374_p4930025215175"><a name="zh-cn_topic_0108275374_p4930025215175"></a><a name="zh-cn_topic_0108275374_p4930025215175"></a>基本参数</p>
</td>
<td class="cellrowborder" valign="top" width="19.650000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275374_p2858877215165"><a name="zh-cn_topic_0108275374_p2858877215165"></a><a name="zh-cn_topic_0108275374_p2858877215165"></a>源目录或文件</p>
</td>
<td class="cellrowborder" valign="top" width="45.6%" headers="mcps1.2.5.1.3 "><p id="p175671619462"><a name="p175671619462"></a><a name="p175671619462"></a>待迁移数据的目录或单个文件路径。文件路径支持输入多个文件（最多50个），默认以<span class="parmvalue" id="dayu_01_0048_zh-cn_topic_0108275319_parmvalue164501515620"><a name="dayu_01_0048_zh-cn_topic_0108275319_parmvalue164501515620"></a><a name="dayu_01_0048_zh-cn_topic_0108275319_parmvalue164501515620"></a>“|”</span>分隔，也可以自定义文件分隔符，具体请参见<a href="文件列表迁移.md">文件列表迁移</a>。</p>
<p id="zh-cn_topic_0108275442_p1210244910548"><a name="zh-cn_topic_0108275442_p1210244910548"></a><a name="zh-cn_topic_0108275442_p1210244910548"></a>该参数支持配置为时间宏变量，且一个路径名中可以有多个宏定义变量。使用时间宏变量和定时任务配合，可以实现定期同步新增数据，详细说明请参见<a href="使用时间宏变量完成增量同步.md">使用时间宏变量完成增量同步</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="17.4%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108275374_p166427315165"><a name="zh-cn_topic_0108275374_p166427315165"></a><a name="zh-cn_topic_0108275374_p166427315165"></a>/ftp/a.csv|/ftp/b.txt</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275374_row1497845915165"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275374_p529563715165"><a name="zh-cn_topic_0108275374_p529563715165"></a><a name="zh-cn_topic_0108275374_p529563715165"></a>文件格式</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><div class="p" id="zh-cn_topic_0108275374_p27142413114140"><a name="zh-cn_topic_0108275374_p27142413114140"></a><a name="zh-cn_topic_0108275374_p27142413114140"></a>指CDM以哪种格式解析数据，可选择以下格式：<a name="zh-cn_topic_0108275319_ul41690379112856"></a><a name="zh-cn_topic_0108275319_ul41690379112856"></a><ul id="zh-cn_topic_0108275319_ul41690379112856"><li>CSV格式：以CSV格式解析源文件，用于迁移文件到数据表的场景。</li><li>二进制格式：选择<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue13073035195648"><a name="zh-cn_topic_0108275319_parmvalue13073035195648"></a><a name="zh-cn_topic_0108275319_parmvalue13073035195648"></a>“二进制格式”</span>时不解析文件内容直接传输，不要求文件格式必须为二进制。适用于文件到文件的原样复制。</li><li>JSON格式：以JSON格式解析源文件，一般都是用于迁移文件到数据表的场景。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275374_p3753014815165"><a name="zh-cn_topic_0108275374_p3753014815165"></a><a name="zh-cn_topic_0108275374_p3753014815165"></a>CSV格式</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275374_row8316154014433"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275374_p631674094316"><a name="zh-cn_topic_0108275374_p631674094316"></a><a name="zh-cn_topic_0108275374_p631674094316"></a>JSON类型</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275374_p231620409435"><a name="zh-cn_topic_0108275374_p231620409435"></a><a name="zh-cn_topic_0108275374_p231620409435"></a>当<span class="parmname" id="zh-cn_topic_0108275319_parmname148454530418"><a name="zh-cn_topic_0108275319_parmname148454530418"></a><a name="zh-cn_topic_0108275319_parmname148454530418"></a>“文件格式”</span>选择为<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue2845135334115"><a name="zh-cn_topic_0108275319_parmvalue2845135334115"></a><a name="zh-cn_topic_0108275319_parmvalue2845135334115"></a>“JSON格式”</span>时，才有该参数。JSON文件中存储的JSON对象的类型，可以选择<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue10971153720423"><a name="zh-cn_topic_0108275319_parmvalue10971153720423"></a><a name="zh-cn_topic_0108275319_parmvalue10971153720423"></a>“JSON对象”</span>或<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue171891642104212"><a name="zh-cn_topic_0108275319_parmvalue171891642104212"></a><a name="zh-cn_topic_0108275319_parmvalue171891642104212"></a>“JSON数组”</span>。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275374_p10316340104318"><a name="zh-cn_topic_0108275374_p10316340104318"></a><a name="zh-cn_topic_0108275374_p10316340104318"></a>JSON对象</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275374_row45435898151424"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275374_p7358643151424"><a name="zh-cn_topic_0108275374_p7358643151424"></a><a name="zh-cn_topic_0108275374_p7358643151424"></a>记录节点</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275374_p59179226151424"><a name="zh-cn_topic_0108275374_p59179226151424"></a><a name="zh-cn_topic_0108275374_p59179226151424"></a>当<span class="parmname" id="zh-cn_topic_0108275319_parmname63369917145142"><a name="zh-cn_topic_0108275319_parmname63369917145142"></a><a name="zh-cn_topic_0108275319_parmname63369917145142"></a>“文件格式”</span>选择为<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue32689672145142"><a name="zh-cn_topic_0108275319_parmvalue32689672145142"></a><a name="zh-cn_topic_0108275319_parmvalue32689672145142"></a>“JSON格式”</span>时，才有该参数。对该JSON节点下的数据进行解析，如果该节点对应的数据为JSON数组，那么系统会以同一模式从该数组中提取数据。多层嵌套的JSON节点以字符<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue4745445093348"><a name="zh-cn_topic_0108275319_parmvalue4745445093348"></a><a name="zh-cn_topic_0108275319_parmvalue4745445093348"></a>“.”</span>分割。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275374_p28788030151424"><a name="zh-cn_topic_0108275374_p28788030151424"></a><a name="zh-cn_topic_0108275374_p28788030151424"></a>data.list</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275374_row3482998115165"><td class="cellrowborder" rowspan="22" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275374_p4617080315165"><a name="zh-cn_topic_0108275374_p4617080315165"></a><a name="zh-cn_topic_0108275374_p4617080315165"></a>高级属性</p>
</td>
<td class="cellrowborder" valign="top" width="19.650000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275374_p265625015165"><a name="zh-cn_topic_0108275374_p265625015165"></a><a name="zh-cn_topic_0108275374_p265625015165"></a>换行符</p>
</td>
<td class="cellrowborder" valign="top" width="45.6%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275374_p540226144442"><a name="zh-cn_topic_0108275374_p540226144442"></a><a name="zh-cn_topic_0108275374_p540226144442"></a>文件中的换行符，默认自动识别<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue55807915142358"><a name="zh-cn_topic_0108275319_parmvalue55807915142358"></a><a name="zh-cn_topic_0108275319_parmvalue55807915142358"></a>“\n”</span>、<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue32509187142358"><a name="zh-cn_topic_0108275319_parmvalue32509187142358"></a><a name="zh-cn_topic_0108275319_parmvalue32509187142358"></a>“\r”</span>或<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue24147233142358"><a name="zh-cn_topic_0108275319_parmvalue24147233142358"></a><a name="zh-cn_topic_0108275319_parmvalue24147233142358"></a>“\r\n”</span>。当<span class="parmname" id="zh-cn_topic_0108275319_parmname48746474114843"><a name="zh-cn_topic_0108275319_parmname48746474114843"></a><a name="zh-cn_topic_0108275319_parmname48746474114843"></a>“文件格式”</span>选择为<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue19506594114819"><a name="zh-cn_topic_0108275319_parmvalue19506594114819"></a><a name="zh-cn_topic_0108275319_parmvalue19506594114819"></a>“CSV格式”</span>时，才有该参数。</p>
</td>
<td class="cellrowborder" valign="top" width="17.4%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108275374_p4854631115165"><a name="zh-cn_topic_0108275374_p4854631115165"></a><a name="zh-cn_topic_0108275374_p4854631115165"></a>\n</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275374_row3426361615165"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275374_p2388955115165"><a name="zh-cn_topic_0108275374_p2388955115165"></a><a name="zh-cn_topic_0108275374_p2388955115165"></a>字段分隔符</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275374_p10609498144442"><a name="zh-cn_topic_0108275374_p10609498144442"></a><a name="zh-cn_topic_0108275374_p10609498144442"></a>文件中的字段分隔符，使用Tab键作为分隔符请输入<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue6198888511118"><a name="zh-cn_topic_0108275319_parmvalue6198888511118"></a><a name="zh-cn_topic_0108275319_parmvalue6198888511118"></a>“\t”</span>。当<span class="parmname" id="zh-cn_topic_0108275319_parmname16895500142516"><a name="zh-cn_topic_0108275319_parmname16895500142516"></a><a name="zh-cn_topic_0108275319_parmname16895500142516"></a>“文件格式”</span>选择为<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue2853817145622"><a name="zh-cn_topic_0108275319_parmvalue2853817145622"></a><a name="zh-cn_topic_0108275319_parmvalue2853817145622"></a>“CSV格式”</span>时，才有该参数。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275374_p4015252715165"><a name="zh-cn_topic_0108275374_p4015252715165"></a><a name="zh-cn_topic_0108275374_p4015252715165"></a>,</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275374_row134341011524"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275374_p243161005210"><a name="zh-cn_topic_0108275374_p243161005210"></a><a name="zh-cn_topic_0108275374_p243161005210"></a>使用包围符</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275374_p743121065218"><a name="zh-cn_topic_0108275374_p743121065218"></a><a name="zh-cn_topic_0108275374_p743121065218"></a>选择<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue1512517923819"><a name="zh-cn_topic_0108275319_parmvalue1512517923819"></a><a name="zh-cn_topic_0108275319_parmvalue1512517923819"></a>“是”</span>时，包围符内的字段分隔符会被视为字符串值的一部分，目前CDM默认的包围符为："。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275374_p164319103522"><a name="zh-cn_topic_0108275374_p164319103522"></a><a name="zh-cn_topic_0108275374_p164319103522"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275374_row67089727154335"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275374_p65558825154335"><a name="zh-cn_topic_0108275374_p65558825154335"></a><a name="zh-cn_topic_0108275374_p65558825154335"></a>使用正则表达式分隔字段</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275374_p8664599154335"><a name="zh-cn_topic_0108275374_p8664599154335"></a><a name="zh-cn_topic_0108275374_p8664599154335"></a>选择是否使用正则表达式分隔字段，选择<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue64732363153745"><a name="zh-cn_topic_0108275319_parmvalue64732363153745"></a><a name="zh-cn_topic_0108275319_parmvalue64732363153745"></a>“是”</span>时，<span class="parmname" id="zh-cn_topic_0108275319_parmname5144246815383"><a name="zh-cn_topic_0108275319_parmname5144246815383"></a><a name="zh-cn_topic_0108275319_parmname5144246815383"></a>“字段分隔符”</span>参数无效。当<span class="parmname" id="zh-cn_topic_0108275319_parmname23895818153637"><a name="zh-cn_topic_0108275319_parmname23895818153637"></a><a name="zh-cn_topic_0108275319_parmname23895818153637"></a>“文件格式”</span>选择为<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue56513111153637"><a name="zh-cn_topic_0108275319_parmvalue56513111153637"></a><a name="zh-cn_topic_0108275319_parmvalue56513111153637"></a>“CSV格式”</span>时，才有该参数。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275374_p30743922154335"><a name="zh-cn_topic_0108275374_p30743922154335"></a><a name="zh-cn_topic_0108275374_p30743922154335"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275374_row43686683154343"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275374_p48960438154343"><a name="zh-cn_topic_0108275374_p48960438154343"></a><a name="zh-cn_topic_0108275374_p48960438154343"></a>正则表达式</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p19995153644613"><a name="p19995153644613"></a><a name="p19995153644613"></a>分隔字段的正则表达式，正则表达式写法请参考<a href="正则表达式分隔半结构化文本.md">正则表达式分隔半结构化文本</a>。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275374_p46411857154343"><a name="zh-cn_topic_0108275374_p46411857154343"></a><a name="zh-cn_topic_0108275374_p46411857154343"></a>^(\d.*\d) (\w*) \[(.*)\] ([\w\.]*) (\w.*).*</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275374_row15301324194018"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275374_p101860576360"><a name="zh-cn_topic_0108275374_p101860576360"></a><a name="zh-cn_topic_0108275374_p101860576360"></a>首行为标题行</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275374_p23062415408"><a name="zh-cn_topic_0108275374_p23062415408"></a><a name="zh-cn_topic_0108275374_p23062415408"></a><span class="parmname" id="zh-cn_topic_0108275319_parmname32021984428"><a name="zh-cn_topic_0108275319_parmname32021984428"></a><a name="zh-cn_topic_0108275319_parmname32021984428"></a>“文件格式”</span>选择<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue4750111818424"><a name="zh-cn_topic_0108275319_parmvalue4750111818424"></a><a name="zh-cn_topic_0108275319_parmvalue4750111818424"></a>“CSV格式”</span>时才有该参数。在迁移CSV文件到表时，CDM默认是全部写入，如果该参数选择<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue11024151389"><a name="zh-cn_topic_0108275319_parmvalue11024151389"></a><a name="zh-cn_topic_0108275319_parmvalue11024151389"></a>“是”</span>，CDM会将CSV文件的第一行数据作为标题行，不写入目的端的表。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275374_p1630112484014"><a name="zh-cn_topic_0108275374_p1630112484014"></a><a name="zh-cn_topic_0108275374_p1630112484014"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275374_row135659916647"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275374_p5093321916739"><a name="zh-cn_topic_0108275374_p5093321916739"></a><a name="zh-cn_topic_0108275374_p5093321916739"></a>编码类型</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275374_p3195010716739"><a name="zh-cn_topic_0108275374_p3195010716739"></a><a name="zh-cn_topic_0108275374_p3195010716739"></a>文件编码类型，例如：<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue17149399142526"><a name="zh-cn_topic_0108275319_parmvalue17149399142526"></a><a name="zh-cn_topic_0108275319_parmvalue17149399142526"></a>“UTF-8”</span>或<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue20126867142526"><a name="zh-cn_topic_0108275319_parmvalue20126867142526"></a><a name="zh-cn_topic_0108275319_parmvalue20126867142526"></a>“GBK”</span>。只有文本文件可以设置编码类型，当<span class="parmname" id="zh-cn_topic_0108275319_parmname25778748142537"><a name="zh-cn_topic_0108275319_parmname25778748142537"></a><a name="zh-cn_topic_0108275319_parmname25778748142537"></a>“文件格式”</span>选择为<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue13285685144950"><a name="zh-cn_topic_0108275319_parmvalue13285685144950"></a><a name="zh-cn_topic_0108275319_parmvalue13285685144950"></a>“二进制格式”</span>时，该参数值无效。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275374_p227755916647"><a name="zh-cn_topic_0108275374_p227755916647"></a><a name="zh-cn_topic_0108275374_p227755916647"></a>UTF-8</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275374_row60426972154540"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275374_p62746533154540"><a name="zh-cn_topic_0108275374_p62746533154540"></a><a name="zh-cn_topic_0108275374_p62746533154540"></a>压缩格式</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><div class="p" id="zh-cn_topic_0108275374_p49304374154540"><a name="zh-cn_topic_0108275374_p49304374154540"></a><a name="zh-cn_topic_0108275374_p49304374154540"></a>当<span class="parmname" id="zh-cn_topic_0108275319_parmname44390303154156"><a name="zh-cn_topic_0108275319_parmname44390303154156"></a><a name="zh-cn_topic_0108275319_parmname44390303154156"></a>“文件格式”</span>为<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue63968411154156"><a name="zh-cn_topic_0108275319_parmvalue63968411154156"></a><a name="zh-cn_topic_0108275319_parmvalue63968411154156"></a>“CSV格式”</span>或<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue38844792154156"><a name="zh-cn_topic_0108275319_parmvalue38844792154156"></a><a name="zh-cn_topic_0108275319_parmvalue38844792154156"></a>“JSON格式”</span>时该参数才显示。选择对应压缩格式的源文件：<a name="zh-cn_topic_0108275319_ul2275301315423"></a><a name="zh-cn_topic_0108275319_ul2275301315423"></a><ul id="zh-cn_topic_0108275319_ul2275301315423"><li>NONE：表示传输所有格式的文件。</li><li>GZIP：表示只传输GZIP格式的文件。</li><li>ZIP：表示只传输ZIP格式的文件。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275374_p34231352154540"><a name="zh-cn_topic_0108275374_p34231352154540"></a><a name="zh-cn_topic_0108275374_p34231352154540"></a>NONE</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275374_row28716199151311"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275374_p44310779151311"><a name="zh-cn_topic_0108275374_p44310779151311"></a><a name="zh-cn_topic_0108275374_p44310779151311"></a>源文件处理方式</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><div class="p" id="zh-cn_topic_0108275374_p32403376151311"><a name="zh-cn_topic_0108275374_p32403376151311"></a><a name="zh-cn_topic_0108275374_p32403376151311"></a>作业执行成功后对源端文件的处理方式：<a name="zh-cn_topic_0108275319_ul7361215211443"></a><a name="zh-cn_topic_0108275319_ul7361215211443"></a><ul id="zh-cn_topic_0108275319_ul7361215211443"><li>重命名：作业执行成功后将源文件重命名，添加用户名和时间戳的后缀。</li><li>删除：作业执行成功后将源文件删除。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275374_p7427822151311"><a name="zh-cn_topic_0108275374_p7427822151311"></a><a name="zh-cn_topic_0108275374_p7427822151311"></a>重命名</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275374_row23261995151316"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275374_p5173423151316"><a name="zh-cn_topic_0108275374_p5173423151316"></a><a name="zh-cn_topic_0108275374_p5173423151316"></a>启动作业标识文件</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275374_p16394112151316"><a name="zh-cn_topic_0108275374_p16394112151316"></a><a name="zh-cn_topic_0108275374_p16394112151316"></a>选择是否开启作业标识文件的功能。当源端路径下存在启动作业的标识文件时才启动作业，否则会挂起等待一段时间，等待时长在下方<span class="parmname" id="zh-cn_topic_0108275319_parmname184551007590"><a name="zh-cn_topic_0108275319_parmname184551007590"></a><a name="zh-cn_topic_0108275319_parmname184551007590"></a>“等待时间”</span>中配置。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275374_p768792312910"><a name="zh-cn_topic_0108275374_p768792312910"></a><a name="zh-cn_topic_0108275374_p768792312910"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275374_row1417117101198"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275374_p7528205145616"><a name="zh-cn_topic_0108275374_p7528205145616"></a><a name="zh-cn_topic_0108275374_p7528205145616"></a>标识文件名</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275374_p952895115563"><a name="zh-cn_topic_0108275374_p952895115563"></a><a name="zh-cn_topic_0108275374_p952895115563"></a>选择开启作业标识文件的功能时，需要指定启动作业的标识文件名。指定文件后，只有在源端路径下存在该文件的情况下才会运行任务。该文件本身不会被迁移。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275374_p52854661151316"><a name="zh-cn_topic_0108275374_p52854661151316"></a><a name="zh-cn_topic_0108275374_p52854661151316"></a>ok.txt</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275374_row13171131315919"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275374_p245210975717"><a name="zh-cn_topic_0108275374_p245210975717"></a><a name="zh-cn_topic_0108275374_p245210975717"></a>等待时间</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275374_p15247819764"><a name="zh-cn_topic_0108275374_p15247819764"></a><a name="zh-cn_topic_0108275374_p15247819764"></a>选择开启作业标识文件的功能时，如果源路径下不存在启动作业的标识文件，作业挂机等待的时长，当超时后任务会失败。</p>
<p id="zh-cn_topic_0108275374_p149111137114"><a name="zh-cn_topic_0108275374_p149111137114"></a><a name="zh-cn_topic_0108275374_p149111137114"></a>等待时间设置为0时，当源端路径下不存在标识文件，任务会立即失败。</p>
<p id="zh-cn_topic_0108275374_p104529915719"><a name="zh-cn_topic_0108275374_p104529915719"></a><a name="zh-cn_topic_0108275374_p104529915719"></a>单位：秒。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275374_p121711413496"><a name="zh-cn_topic_0108275374_p121711413496"></a><a name="zh-cn_topic_0108275374_p121711413496"></a>10</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275374_row4933843102615"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275374_p581315631913"><a name="zh-cn_topic_0108275374_p581315631913"></a><a name="zh-cn_topic_0108275374_p581315631913"></a>文件分隔符</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275374_p59331143162617"><a name="zh-cn_topic_0108275374_p59331143162617"></a><a name="zh-cn_topic_0108275374_p59331143162617"></a><span class="parmname" id="zh-cn_topic_0108275319_parmname1411185092217"><a name="zh-cn_topic_0108275319_parmname1411185092217"></a><a name="zh-cn_topic_0108275319_parmname1411185092217"></a>“源目录或文件”</span>参数中如果输入的是多个文件路径，CDM使用这里配置的文件分隔符来区分各个文件，默认为|。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275374_p139331943172612"><a name="zh-cn_topic_0108275374_p139331943172612"></a><a name="zh-cn_topic_0108275374_p139331943172612"></a>|</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275374_row2506067615165"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275374_p19345321161328"><a name="zh-cn_topic_0108275374_p19345321161328"></a><a name="zh-cn_topic_0108275374_p19345321161328"></a>过滤类型</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><div class="p" id="p39433188478"><a name="p39433188478"></a><a name="p39433188478"></a>选择过滤器的类型：<a name="dayu_01_0048_zh-cn_topic_0108275319_ul23048864142559"></a><a name="dayu_01_0048_zh-cn_topic_0108275319_ul23048864142559"></a><ul id="dayu_01_0048_zh-cn_topic_0108275319_ul23048864142559"><li>通配符：输入通配符作为过滤文件，满足过滤条件的路径或文件会被传输，具体使用方法可参见<a href="文件增量迁移.md#zh-cn_topic_0108275366_section1070082019442">文件/路径过滤器</a>。</li><li>时间过滤器：可以根据文件的修改时间，选择性的传输文件。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275374_p48778339161328"><a name="zh-cn_topic_0108275374_p48778339161328"></a><a name="zh-cn_topic_0108275374_p48778339161328"></a>通配符</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275374_row994336215165"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275374_p58820566161328"><a name="zh-cn_topic_0108275374_p58820566161328"></a><a name="zh-cn_topic_0108275374_p58820566161328"></a>路径过滤器</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275374_p4672372415942"><a name="zh-cn_topic_0108275374_p4672372415942"></a><a name="zh-cn_topic_0108275374_p4672372415942"></a><span class="parmname" id="zh-cn_topic_0108275319_parmname14340913362"><a name="zh-cn_topic_0108275319_parmname14340913362"></a><a name="zh-cn_topic_0108275319_parmname14340913362"></a>“过滤类型”</span>选择<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue15341983618"><a name="zh-cn_topic_0108275319_parmvalue15341983618"></a><a name="zh-cn_topic_0108275319_parmvalue15341983618"></a>“通配符”</span>时，用通配符过滤目录，符合过滤器规则的目录，允许进行迁移。支持配置多个路径，中间使用<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue5332191741811"><a name="zh-cn_topic_0108275319_parmvalue5332191741811"></a><a name="zh-cn_topic_0108275319_parmvalue5332191741811"></a>“,”</span>分隔。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275374_p45766974161328"><a name="zh-cn_topic_0108275374_p45766974161328"></a><a name="zh-cn_topic_0108275374_p45766974161328"></a>*input,*out</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275374_row56738186161317"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275374_p11018662161328"><a name="zh-cn_topic_0108275374_p11018662161328"></a><a name="zh-cn_topic_0108275374_p11018662161328"></a>文件过滤器</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275374_p3740142115942"><a name="zh-cn_topic_0108275374_p3740142115942"></a><a name="zh-cn_topic_0108275374_p3740142115942"></a><span class="parmname" id="zh-cn_topic_0108275319_parmname62691530113612"><a name="zh-cn_topic_0108275319_parmname62691530113612"></a><a name="zh-cn_topic_0108275319_parmname62691530113612"></a>“过滤类型”</span>选择<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue926953011362"><a name="zh-cn_topic_0108275319_parmvalue926953011362"></a><a name="zh-cn_topic_0108275319_parmvalue926953011362"></a>“通配符”</span>时，用通配符过滤目录下的文件，符合过滤器规则的文件，允许进行迁移。支持配置多个文件，中间使用<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue125501853131710"><a name="zh-cn_topic_0108275319_parmvalue125501853131710"></a><a name="zh-cn_topic_0108275319_parmvalue125501853131710"></a>“,”</span>分隔。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275374_p17196199161328"><a name="zh-cn_topic_0108275374_p17196199161328"></a><a name="zh-cn_topic_0108275374_p17196199161328"></a>*.csv</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275374_row1783111475398"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275374_p13831194733913"><a name="zh-cn_topic_0108275374_p13831194733913"></a><a name="zh-cn_topic_0108275374_p13831194733913"></a>起始时间</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275374_p18311447203911"><a name="zh-cn_topic_0108275374_p18311447203911"></a><a name="zh-cn_topic_0108275374_p18311447203911"></a><span class="parmname" id="zh-cn_topic_0108275319_parmname4237191913013"><a name="zh-cn_topic_0108275319_parmname4237191913013"></a><a name="zh-cn_topic_0108275319_parmname4237191913013"></a>“过滤类型”</span>选择<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue933016296308"><a name="zh-cn_topic_0108275319_parmvalue933016296308"></a><a name="zh-cn_topic_0108275319_parmvalue933016296308"></a>“时间过滤器”</span>时，可以指定一个时间值，当文件的修改时间大于该时间才会被传输，输入的时间格式需为<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue9313481341"><a name="zh-cn_topic_0108275319_parmvalue9313481341"></a><a name="zh-cn_topic_0108275319_parmvalue9313481341"></a>“yyyy-MM-dd HH:mm:ss”</span>。</p>
<p id="zh-cn_topic_0108275374_p12144111817144"><a name="zh-cn_topic_0108275374_p12144111817144"></a><a name="zh-cn_topic_0108275374_p12144111817144"></a>该参数支持配置为时间宏变量，例如<strong id="zh-cn_topic_0108275319_b97861314103"><a name="zh-cn_topic_0108275319_b97861314103"></a><a name="zh-cn_topic_0108275319_b97861314103"></a>${timestamp(dateformat(yyyy-MM-dd HH:mm:ss,-90,DAY))}</strong>表示：只迁移最近90天内的文件。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275374_p1683154713395"><a name="zh-cn_topic_0108275374_p1683154713395"></a><a name="zh-cn_topic_0108275374_p1683154713395"></a>2019-07-01 00:00:00</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275374_row050332521619"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275374_p1149121141416"><a name="zh-cn_topic_0108275374_p1149121141416"></a><a name="zh-cn_topic_0108275374_p1149121141416"></a>终止时间</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275374_p34921611171416"><a name="zh-cn_topic_0108275374_p34921611171416"></a><a name="zh-cn_topic_0108275374_p34921611171416"></a><span class="parmname" id="zh-cn_topic_0108275319_parmname106751314209"><a name="zh-cn_topic_0108275319_parmname106751314209"></a><a name="zh-cn_topic_0108275319_parmname106751314209"></a>“过滤类型”</span>选择<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue13675131413012"><a name="zh-cn_topic_0108275319_parmvalue13675131413012"></a><a name="zh-cn_topic_0108275319_parmvalue13675131413012"></a>“时间过滤器”</span>时，可以指定一个时间值，当文件的修改时间小于该时间才会被传输，输入的时间格式需为<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue146759148017"><a name="zh-cn_topic_0108275319_parmvalue146759148017"></a><a name="zh-cn_topic_0108275319_parmvalue146759148017"></a>“yyyy-MM-dd HH:mm:ss”</span>。</p>
<p id="zh-cn_topic_0108275374_p13254806156"><a name="zh-cn_topic_0108275374_p13254806156"></a><a name="zh-cn_topic_0108275374_p13254806156"></a>该参数支持配置为时间宏变量，例如<strong id="zh-cn_topic_0108275319_b1521616538112"><a name="zh-cn_topic_0108275319_b1521616538112"></a><a name="zh-cn_topic_0108275319_b1521616538112"></a>${timestamp(dateformat(yyyy-MM-dd HH:mm:ss))}</strong>表示：只迁移修改时间为当前时间以前的文件。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275374_p8442749101515"><a name="zh-cn_topic_0108275374_p8442749101515"></a><a name="zh-cn_topic_0108275374_p8442749101515"></a>2019-07-30 00:00:00</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275374_row983741015300"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275374_p1273915511715"><a name="zh-cn_topic_0108275374_p1273915511715"></a><a name="zh-cn_topic_0108275374_p1273915511715"></a>加密方式</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><div class="p" id="zh-cn_topic_0108275374_p943615213200"><a name="zh-cn_topic_0108275374_p943615213200"></a><a name="zh-cn_topic_0108275374_p943615213200"></a>如果源端数据是被加密过的，则CDM支持解密后再导出。这里选择是否对源端数据解密，以及选择解密算法：<a name="zh-cn_topic_0108275319_ul44410501486"></a><a name="zh-cn_topic_0108275319_ul44410501486"></a><ul id="zh-cn_topic_0108275319_ul44410501486"><li>无：不解密，直接导出。</li><li>AES-256-GCM：使用长度为256byte的AES对称加密算法，目前加密算法只支持AES-256-GCM（NoPadding）。该参数在目的端为加密，在源端为解密。</li></ul>
</div>
<p id="zh-cn_topic_0108275442_p1440312818259"><a name="zh-cn_topic_0108275442_p1440312818259"></a><a name="zh-cn_topic_0108275442_p1440312818259"></a>详细使用方法请参见<a href="迁移文件时加解密.md">迁移文件时加解密</a>。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275374_p1173985171713"><a name="zh-cn_topic_0108275374_p1173985171713"></a><a name="zh-cn_topic_0108275374_p1173985171713"></a>AES-256-GCM</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275374_row83531811183015"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275374_p2560191135113"><a name="zh-cn_topic_0108275374_p2560191135113"></a><a name="zh-cn_topic_0108275374_p2560191135113"></a>数据加密密钥</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275374_p13560410513"><a name="zh-cn_topic_0108275374_p13560410513"></a><a name="zh-cn_topic_0108275374_p13560410513"></a><span class="parmname" id="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmname776612385559"><a name="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmname776612385559"></a><a name="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmname776612385559"></a>“加密方式”</span>选择<span class="parmvalue" id="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmvalue0767193814558"><a name="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmvalue0767193814558"></a><a name="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmvalue0767193814558"></a>“AES-256-GCM”</span>时显示该参数，密钥由长度64的十六进制数组成，且必须与加密时配置的<span class="parmname" id="zh-cn_topic_0108275319_parmname48334346128"><a name="zh-cn_topic_0108275319_parmname48334346128"></a><a name="zh-cn_topic_0108275319_parmname48334346128"></a>“数据加密密钥”</span>一致。如果不一致系统不会报异常，只是解密出来的数据会错误。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275374_p10560111155111"><a name="zh-cn_topic_0108275374_p10560111155111"></a><a name="zh-cn_topic_0108275374_p10560111155111"></a>DD0AE00DFECD78BF051BCFDA25BD4E320DB0A7AC75A1F3FC3D3C56A457DCDC1B</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275374_row691415116301"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275374_p24773525117"><a name="zh-cn_topic_0108275374_p24773525117"></a><a name="zh-cn_topic_0108275374_p24773525117"></a>初始化向量</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275374_p24771354512"><a name="zh-cn_topic_0108275374_p24771354512"></a><a name="zh-cn_topic_0108275374_p24771354512"></a><span class="parmname" id="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmname9947565563"><a name="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmname9947565563"></a><a name="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmname9947565563"></a>“加密方式”</span>选择<span class="parmvalue" id="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmvalue179471468565"><a name="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmvalue179471468565"></a><a name="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmvalue179471468565"></a>“AES-256-GCM”</span>时显示该参数，初始化向量由长度32的十六进制数组成，且必须与加密时配置的<span class="parmname" id="zh-cn_topic_0108275319_parmname163755565172"><a name="zh-cn_topic_0108275319_parmname163755565172"></a><a name="zh-cn_topic_0108275319_parmname163755565172"></a>“初始化向量”</span>一致。如果不一致系统不会报异常，只是解密出来的数据会错误。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275374_p647775195111"><a name="zh-cn_topic_0108275374_p647775195111"></a><a name="zh-cn_topic_0108275374_p647775195111"></a>5C91687BA886EDCD12ACBC3FF19A3C3F</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275374_row56771133321"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275374_p116778319321"><a name="zh-cn_topic_0108275374_p116778319321"></a><a name="zh-cn_topic_0108275374_p116778319321"></a>MD5文件名后缀</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p1929618329481"><a name="p1929618329481"></a><a name="p1929618329481"></a>校验CDM抽取的文件，是否与源文件一致，详细请参见<a href="MD5校验文件一致性.md">MD5校验文件一致性</a>。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275374_p267718319321"><a name="zh-cn_topic_0108275374_p267718319321"></a><a name="zh-cn_topic_0108275374_p267718319321"></a>.md5</p>
</td>
</tr>
</tbody>
</table>

