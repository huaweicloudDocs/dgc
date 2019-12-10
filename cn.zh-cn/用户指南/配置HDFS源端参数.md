# 配置HDFS源端参数<a name="dayu_01_0049"></a>

作业中源连接为[配置HDFS连接](配置HDFS连接.md)时，即从MRS HDFS、FusionInsight HDFS、Apache HDFS导出数据时，源端作业参数如[表1](#zh-cn_topic_0108275442_table5046103815165)所示。

**表 1**  HDFS作为源端时的作业参数

<a name="zh-cn_topic_0108275442_table5046103815165"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108275442_row585315215165"><th class="cellrowborder" valign="top" width="17.349999999999998%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0108275442_p434331215165"><a name="zh-cn_topic_0108275442_p434331215165"></a><a name="zh-cn_topic_0108275442_p434331215165"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="19.27%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0108275442_p1626397215165"><a name="zh-cn_topic_0108275442_p1626397215165"></a><a name="zh-cn_topic_0108275442_p1626397215165"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="45.98%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0108275442_p4231334915165"><a name="zh-cn_topic_0108275442_p4231334915165"></a><a name="zh-cn_topic_0108275442_p4231334915165"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="17.4%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0108275442_p482921015165"><a name="zh-cn_topic_0108275442_p482921015165"></a><a name="zh-cn_topic_0108275442_p482921015165"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108275442_row4012116315165"><td class="cellrowborder" rowspan="2" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275442_p4930025215175"><a name="zh-cn_topic_0108275442_p4930025215175"></a><a name="zh-cn_topic_0108275442_p4930025215175"></a>基本参数</p>
</td>
<td class="cellrowborder" valign="top" width="19.27%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275442_p2858877215165"><a name="zh-cn_topic_0108275442_p2858877215165"></a><a name="zh-cn_topic_0108275442_p2858877215165"></a>源目录或文件</p>
</td>
<td class="cellrowborder" valign="top" width="45.98%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275442_p3398923015165"><a name="zh-cn_topic_0108275442_p3398923015165"></a><a name="zh-cn_topic_0108275442_p3398923015165"></a>待迁移数据的目录或单个文件路径。</p>
<p id="zh-cn_topic_0108275442_p1210244910548"><a name="zh-cn_topic_0108275442_p1210244910548"></a><a name="zh-cn_topic_0108275442_p1210244910548"></a>该参数支持配置为时间宏变量，且一个路径名中可以有多个宏定义变量。使用时间宏变量和定时任务配合，可以实现定期同步新增数据，详细说明请参见<a href="使用时间宏变量完成增量同步.md">使用时间宏变量完成增量同步</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="17.4%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108275442_p166427315165"><a name="zh-cn_topic_0108275442_p166427315165"></a><a name="zh-cn_topic_0108275442_p166427315165"></a>/user/cdm/</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275442_row1497845915165"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275442_p529563715165"><a name="zh-cn_topic_0108275442_p529563715165"></a><a name="zh-cn_topic_0108275442_p529563715165"></a>文件格式</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><div class="p" id="zh-cn_topic_0108275442_p27142413114140"><a name="zh-cn_topic_0108275442_p27142413114140"></a><a name="zh-cn_topic_0108275442_p27142413114140"></a>传输数据时所用的文件格式，可选择以下文件格式：<a name="zh-cn_topic_0108275442_ue5dec7869b79475f8f1e727e91bfc65e"></a><a name="zh-cn_topic_0108275442_ue5dec7869b79475f8f1e727e91bfc65e"></a><ul id="zh-cn_topic_0108275442_ue5dec7869b79475f8f1e727e91bfc65e"><li>CSV格式：以CSV格式解析源文件，用于迁移文件到数据表的场景。</li><li>二进制格式：选择<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue13073035195648"><a name="zh-cn_topic_0108275319_parmvalue13073035195648"></a><a name="zh-cn_topic_0108275319_parmvalue13073035195648"></a>“二进制格式”</span>时不解析文件内容直接传输，不要求文件格式必须为二进制。适用于文件到文件的原样复制。</li><li>Parquet格式：以Parquet格式解析源文件，用于HDFS数据导到表的场景。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275442_p3753014815165"><a name="zh-cn_topic_0108275442_p3753014815165"></a><a name="zh-cn_topic_0108275442_p3753014815165"></a>CSV格式</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275442_row3482998115165"><td class="cellrowborder" rowspan="15" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275442_p4617080315165"><a name="zh-cn_topic_0108275442_p4617080315165"></a><a name="zh-cn_topic_0108275442_p4617080315165"></a>高级属性</p>
</td>
<td class="cellrowborder" valign="top" width="19.27%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275442_p265625015165"><a name="zh-cn_topic_0108275442_p265625015165"></a><a name="zh-cn_topic_0108275442_p265625015165"></a>换行符</p>
</td>
<td class="cellrowborder" valign="top" width="45.98%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275442_p1382968715165"><a name="zh-cn_topic_0108275442_p1382968715165"></a><a name="zh-cn_topic_0108275442_p1382968715165"></a>文件中的换行符，默认自动识别<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue55807915142358"><a name="zh-cn_topic_0108275319_parmvalue55807915142358"></a><a name="zh-cn_topic_0108275319_parmvalue55807915142358"></a>“\n”</span>、<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue32509187142358"><a name="zh-cn_topic_0108275319_parmvalue32509187142358"></a><a name="zh-cn_topic_0108275319_parmvalue32509187142358"></a>“\r”</span>或<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue24147233142358"><a name="zh-cn_topic_0108275319_parmvalue24147233142358"></a><a name="zh-cn_topic_0108275319_parmvalue24147233142358"></a>“\r\n”</span>。当<span class="parmname" id="zh-cn_topic_0108275319_parmname48746474114843"><a name="zh-cn_topic_0108275319_parmname48746474114843"></a><a name="zh-cn_topic_0108275319_parmname48746474114843"></a>“文件格式”</span>选择为<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue19506594114819"><a name="zh-cn_topic_0108275319_parmvalue19506594114819"></a><a name="zh-cn_topic_0108275319_parmvalue19506594114819"></a>“CSV格式”</span>时，才有该参数。</p>
</td>
<td class="cellrowborder" valign="top" width="17.4%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108275442_p4854631115165"><a name="zh-cn_topic_0108275442_p4854631115165"></a><a name="zh-cn_topic_0108275442_p4854631115165"></a>\n</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275442_row3426361615165"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275442_p2388955115165"><a name="zh-cn_topic_0108275442_p2388955115165"></a><a name="zh-cn_topic_0108275442_p2388955115165"></a>字段分隔符</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275442_p5600551115165"><a name="zh-cn_topic_0108275442_p5600551115165"></a><a name="zh-cn_topic_0108275442_p5600551115165"></a>文件中的字段分隔符，使用Tab键作为分隔符请输入<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue6198888511118"><a name="zh-cn_topic_0108275319_parmvalue6198888511118"></a><a name="zh-cn_topic_0108275319_parmvalue6198888511118"></a>“\t”</span>。当<span class="parmname" id="zh-cn_topic_0108275319_parmname16895500142516"><a name="zh-cn_topic_0108275319_parmname16895500142516"></a><a name="zh-cn_topic_0108275319_parmname16895500142516"></a>“文件格式”</span>选择为<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue2853817145622"><a name="zh-cn_topic_0108275319_parmvalue2853817145622"></a><a name="zh-cn_topic_0108275319_parmvalue2853817145622"></a>“CSV格式”</span>时，才有该参数。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275442_p4015252715165"><a name="zh-cn_topic_0108275442_p4015252715165"></a><a name="zh-cn_topic_0108275442_p4015252715165"></a>,</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275442_row06816265114"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275442_p116811622519"><a name="zh-cn_topic_0108275442_p116811622519"></a><a name="zh-cn_topic_0108275442_p116811622519"></a>首行为标题行</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275442_p1468115213518"><a name="zh-cn_topic_0108275442_p1468115213518"></a><a name="zh-cn_topic_0108275442_p1468115213518"></a><span class="parmname" id="zh-cn_topic_0108275319_parmname32021984428"><a name="zh-cn_topic_0108275319_parmname32021984428"></a><a name="zh-cn_topic_0108275319_parmname32021984428"></a>“文件格式”</span>选择<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue4750111818424"><a name="zh-cn_topic_0108275319_parmvalue4750111818424"></a><a name="zh-cn_topic_0108275319_parmvalue4750111818424"></a>“CSV格式”</span>时才有该参数。在迁移CSV文件到表时，CDM默认是全部写入，如果该参数选择<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue11024151389"><a name="zh-cn_topic_0108275319_parmvalue11024151389"></a><a name="zh-cn_topic_0108275319_parmvalue11024151389"></a>“是”</span>，CDM会将CSV文件的第一行数据作为标题行，不写入目的端的表。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275442_p368113211517"><a name="zh-cn_topic_0108275442_p368113211517"></a><a name="zh-cn_topic_0108275442_p368113211517"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275442_row836779515165"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275442_p670282215165"><a name="zh-cn_topic_0108275442_p670282215165"></a><a name="zh-cn_topic_0108275442_p670282215165"></a>文件分割方式</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><div class="p" id="zh-cn_topic_0108275442_p1725054113534"><a name="zh-cn_topic_0108275442_p1725054113534"></a><a name="zh-cn_topic_0108275442_p1725054113534"></a>指定任务分片方式，选择按文件或文件大小进行分割。HDFS上的文件，如果在HDFS上已经分片，则HDFS每个分片视为一个文件。<a name="zh-cn_topic_0108275442_ul17679437141210"></a><a name="zh-cn_topic_0108275442_ul17679437141210"></a><ul id="zh-cn_topic_0108275442_ul17679437141210"><li>FILE：按文件数量进行分片。例如有10个文件，并在任务参数中指定<span class="parmname" id="zh-cn_topic_0108275442_parmname1679193710129"><a name="zh-cn_topic_0108275442_parmname1679193710129"></a><a name="zh-cn_topic_0108275442_parmname1679193710129"></a>“抽取并发数”</span>为<span class="parmvalue" id="zh-cn_topic_0108275442_parmvalue19679537121220"><a name="zh-cn_topic_0108275442_parmvalue19679537121220"></a><a name="zh-cn_topic_0108275442_parmvalue19679537121220"></a>“5”</span>，则每个分片2个文件。</li><li>SIZE：按文件大小分割。注意这里不会将文件做切分来实现均衡。例如：有10个文件，9个10M，1个200M，在并发任务数中指定<span class="parmname" id="zh-cn_topic_0108275442_parmname1067923717124"><a name="zh-cn_topic_0108275442_parmname1067923717124"></a><a name="zh-cn_topic_0108275442_parmname1067923717124"></a>“抽取并发数”</span>为<span class="parmvalue" id="zh-cn_topic_0108275442_parmvalue66793372126"><a name="zh-cn_topic_0108275442_parmvalue66793372126"></a><a name="zh-cn_topic_0108275442_parmvalue66793372126"></a>“2”</span>，则会分两个分片，一个处理9个10M的文件，一个处理1个200M的文件。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275442_p1024106015165"><a name="zh-cn_topic_0108275442_p1024106015165"></a><a name="zh-cn_topic_0108275442_p1024106015165"></a>FILE</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275442_row6330867615653"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275442_p2772909415653"><a name="zh-cn_topic_0108275442_p2772909415653"></a><a name="zh-cn_topic_0108275442_p2772909415653"></a>源文件处理方式</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><div class="p" id="zh-cn_topic_0108275442_p3146415715653"><a name="zh-cn_topic_0108275442_p3146415715653"></a><a name="zh-cn_topic_0108275442_p3146415715653"></a>作业执行成功后对源端文件的处理方式：<a name="zh-cn_topic_0108275319_ul7361215211443"></a><a name="zh-cn_topic_0108275319_ul7361215211443"></a><ul id="zh-cn_topic_0108275319_ul7361215211443"><li>重命名：作业执行成功后将源文件重命名，添加用户名和时间戳的后缀。</li><li>删除：作业执行成功后将源文件删除。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275442_p6556881715653"><a name="zh-cn_topic_0108275442_p6556881715653"></a><a name="zh-cn_topic_0108275442_p6556881715653"></a>重命名</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275442_row6041688715658"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275442_p6192965315658"><a name="zh-cn_topic_0108275442_p6192965315658"></a><a name="zh-cn_topic_0108275442_p6192965315658"></a>启动作业标识文件</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275442_p5024596315658"><a name="zh-cn_topic_0108275442_p5024596315658"></a><a name="zh-cn_topic_0108275442_p5024596315658"></a>选择是否开启作业标识文件的功能。当源端路径下存在启动作业的标识文件时才启动作业，否则会挂起等待一段时间，等待时长在下方<span class="parmname" id="zh-cn_topic_0108275319_parmname184551007590"><a name="zh-cn_topic_0108275319_parmname184551007590"></a><a name="zh-cn_topic_0108275319_parmname184551007590"></a>“等待时间”</span>中配置。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275442_p4339120215658"><a name="zh-cn_topic_0108275442_p4339120215658"></a><a name="zh-cn_topic_0108275442_p4339120215658"></a>ok.txt</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275442_row2506067615165"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275442_p25192287145116"><a name="zh-cn_topic_0108275442_p25192287145116"></a><a name="zh-cn_topic_0108275442_p25192287145116"></a>过滤类型</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><div class="p" id="zh-cn_topic_0108275442_p27309389145116"><a name="zh-cn_topic_0108275442_p27309389145116"></a><a name="zh-cn_topic_0108275442_p27309389145116"></a>选择过滤器的类型：<a name="dayu_01_0048_zh-cn_topic_0108275319_ul23048864142559"></a><a name="dayu_01_0048_zh-cn_topic_0108275319_ul23048864142559"></a><ul id="dayu_01_0048_zh-cn_topic_0108275319_ul23048864142559"><li>通配符：输入通配符作为过滤文件，满足过滤条件的路径或文件会被传输，具体使用方法可参见<a href="文件增量迁移.md#zh-cn_topic_0108275366_section1070082019442">文件/路径过滤器</a>。</li><li>时间过滤器：可以根据文件的修改时间，选择性的传输文件。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275442_p33228269145116"><a name="zh-cn_topic_0108275442_p33228269145116"></a><a name="zh-cn_topic_0108275442_p33228269145116"></a>通配符</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275442_row994336215165"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275442_p64217335145116"><a name="zh-cn_topic_0108275442_p64217335145116"></a><a name="zh-cn_topic_0108275442_p64217335145116"></a>路径过滤器</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275442_p34221671145116"><a name="zh-cn_topic_0108275442_p34221671145116"></a><a name="zh-cn_topic_0108275442_p34221671145116"></a><span class="parmname" id="zh-cn_topic_0108275319_parmname14340913362"><a name="zh-cn_topic_0108275319_parmname14340913362"></a><a name="zh-cn_topic_0108275319_parmname14340913362"></a>“过滤类型”</span>选择<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue15341983618"><a name="zh-cn_topic_0108275319_parmvalue15341983618"></a><a name="zh-cn_topic_0108275319_parmvalue15341983618"></a>“通配符”</span>时，用通配符过滤目录，符合过滤器规则的目录，允许进行迁移。支持配置多个路径，中间使用<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue5332191741811"><a name="zh-cn_topic_0108275319_parmvalue5332191741811"></a><a name="zh-cn_topic_0108275319_parmvalue5332191741811"></a>“,”</span>分隔。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275442_p20491984145116"><a name="zh-cn_topic_0108275442_p20491984145116"></a><a name="zh-cn_topic_0108275442_p20491984145116"></a>*input</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275442_row851377714512"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275442_p40488609145116"><a name="zh-cn_topic_0108275442_p40488609145116"></a><a name="zh-cn_topic_0108275442_p40488609145116"></a>文件过滤器</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275442_p58351869145116"><a name="zh-cn_topic_0108275442_p58351869145116"></a><a name="zh-cn_topic_0108275442_p58351869145116"></a><span class="parmname" id="zh-cn_topic_0108275319_parmname62691530113612"><a name="zh-cn_topic_0108275319_parmname62691530113612"></a><a name="zh-cn_topic_0108275319_parmname62691530113612"></a>“过滤类型”</span>选择<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue926953011362"><a name="zh-cn_topic_0108275319_parmvalue926953011362"></a><a name="zh-cn_topic_0108275319_parmvalue926953011362"></a>“通配符”</span>时，用通配符过滤目录下的文件，符合过滤器规则的文件，允许进行迁移。支持配置多个文件，中间使用<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue125501853131710"><a name="zh-cn_topic_0108275319_parmvalue125501853131710"></a><a name="zh-cn_topic_0108275319_parmvalue125501853131710"></a>“,”</span>分隔。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275442_p28880974145116"><a name="zh-cn_topic_0108275442_p28880974145116"></a><a name="zh-cn_topic_0108275442_p28880974145116"></a>*.csv</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275442_row8615115514527"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275442_p13831194733913"><a name="zh-cn_topic_0108275442_p13831194733913"></a><a name="zh-cn_topic_0108275442_p13831194733913"></a>起始时间</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275442_p18311447203911"><a name="zh-cn_topic_0108275442_p18311447203911"></a><a name="zh-cn_topic_0108275442_p18311447203911"></a><span class="parmname" id="zh-cn_topic_0108275319_parmname4237191913013"><a name="zh-cn_topic_0108275319_parmname4237191913013"></a><a name="zh-cn_topic_0108275319_parmname4237191913013"></a>“过滤类型”</span>选择<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue933016296308"><a name="zh-cn_topic_0108275319_parmvalue933016296308"></a><a name="zh-cn_topic_0108275319_parmvalue933016296308"></a>“时间过滤器”</span>时，可以指定一个时间值，当文件的修改时间大于该时间才会被传输，输入的时间格式需为<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue9313481341"><a name="zh-cn_topic_0108275319_parmvalue9313481341"></a><a name="zh-cn_topic_0108275319_parmvalue9313481341"></a>“yyyy-MM-dd HH:mm:ss”</span>。</p>
<p id="zh-cn_topic_0108275442_p12144111817144"><a name="zh-cn_topic_0108275442_p12144111817144"></a><a name="zh-cn_topic_0108275442_p12144111817144"></a>该参数支持配置为时间宏变量，例如<strong id="zh-cn_topic_0108275319_b97861314103"><a name="zh-cn_topic_0108275319_b97861314103"></a><a name="zh-cn_topic_0108275319_b97861314103"></a>${timestamp(dateformat(yyyy-MM-dd HH:mm:ss,-90,DAY))}</strong>表示：只迁移最近90天内的文件。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275442_p1683154713395"><a name="zh-cn_topic_0108275442_p1683154713395"></a><a name="zh-cn_topic_0108275442_p1683154713395"></a>2019-07-01 00:00:00</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275442_row1949013110145"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275442_p1149121141416"><a name="zh-cn_topic_0108275442_p1149121141416"></a><a name="zh-cn_topic_0108275442_p1149121141416"></a>终止时间</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275442_p34921611171416"><a name="zh-cn_topic_0108275442_p34921611171416"></a><a name="zh-cn_topic_0108275442_p34921611171416"></a><span class="parmname" id="zh-cn_topic_0108275319_parmname106751314209"><a name="zh-cn_topic_0108275319_parmname106751314209"></a><a name="zh-cn_topic_0108275319_parmname106751314209"></a>“过滤类型”</span>选择<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue13675131413012"><a name="zh-cn_topic_0108275319_parmvalue13675131413012"></a><a name="zh-cn_topic_0108275319_parmvalue13675131413012"></a>“时间过滤器”</span>时，可以指定一个时间值，当文件的修改时间小于该时间才会被传输，输入的时间格式需为<span class="parmvalue" id="zh-cn_topic_0108275319_parmvalue146759148017"><a name="zh-cn_topic_0108275319_parmvalue146759148017"></a><a name="zh-cn_topic_0108275319_parmvalue146759148017"></a>“yyyy-MM-dd HH:mm:ss”</span>。</p>
<p id="zh-cn_topic_0108275442_p13254806156"><a name="zh-cn_topic_0108275442_p13254806156"></a><a name="zh-cn_topic_0108275442_p13254806156"></a>该参数支持配置为时间宏变量，例如<strong id="zh-cn_topic_0108275319_b1521616538112"><a name="zh-cn_topic_0108275319_b1521616538112"></a><a name="zh-cn_topic_0108275319_b1521616538112"></a>${timestamp(dateformat(yyyy-MM-dd HH:mm:ss))}</strong>表示：只迁移修改时间为当前时间以前的文件。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275442_p8442749101515"><a name="zh-cn_topic_0108275442_p8442749101515"></a><a name="zh-cn_topic_0108275442_p8442749101515"></a>2019-07-30 00:00:00</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275442_row719361213207"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275442_p1719419128201"><a name="zh-cn_topic_0108275442_p1719419128201"></a><a name="zh-cn_topic_0108275442_p1719419128201"></a>创建快照</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275442_p17617269485"><a name="zh-cn_topic_0108275442_p17617269485"></a><a name="zh-cn_topic_0108275442_p17617269485"></a>如果选择<span class="parmvalue" id="zh-cn_topic_0108275442_parmvalue4617176154813"><a name="zh-cn_topic_0108275442_parmvalue4617176154813"></a><a name="zh-cn_topic_0108275442_parmvalue4617176154813"></a>“是”</span>，CDM读取HDFS系统上的文件时，会先对待迁移的源目录创建快照（不允许对单个文件创建快照），然后CDM迁移快照中的数据。</p>
<p id="zh-cn_topic_0108275442_p20194131216207"><a name="zh-cn_topic_0108275442_p20194131216207"></a><a name="zh-cn_topic_0108275442_p20194131216207"></a>需要HDFS系统的管理员权限才可以创建快照，CDM作业完成后，快照会被删除。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275442_p419411125208"><a name="zh-cn_topic_0108275442_p419411125208"></a><a name="zh-cn_topic_0108275442_p419411125208"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275442_row142015472296"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275442_p1273915511715"><a name="zh-cn_topic_0108275442_p1273915511715"></a><a name="zh-cn_topic_0108275442_p1273915511715"></a>加密方式</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275442_p87391251172"><a name="zh-cn_topic_0108275442_p87391251172"></a><a name="zh-cn_topic_0108275442_p87391251172"></a><span class="parmname" id="zh-cn_topic_0108275442_parmname103132381818"><a name="zh-cn_topic_0108275442_parmname103132381818"></a><a name="zh-cn_topic_0108275442_parmname103132381818"></a>“文件格式”</span>选择<span class="parmvalue" id="zh-cn_topic_0108275442_parmvalue42720331181"><a name="zh-cn_topic_0108275442_parmvalue42720331181"></a><a name="zh-cn_topic_0108275442_parmvalue42720331181"></a>“二进制格式”</span>时，该参数才显示。</p>
<div class="p" id="zh-cn_topic_0108275442_p943615213200"><a name="zh-cn_topic_0108275442_p943615213200"></a><a name="zh-cn_topic_0108275442_p943615213200"></a>如果源端数据是被加密过的，则CDM支持解密后再导出。这里选择是否对源端数据解密，以及选择解密算法：<a name="zh-cn_topic_0108275319_ul44410501486"></a><a name="zh-cn_topic_0108275319_ul44410501486"></a><ul id="zh-cn_topic_0108275319_ul44410501486"><li>无：不解密，直接导出。</li><li>AES-256-GCM：使用长度为256byte的AES对称加密算法，目前加密算法只支持AES-256-GCM（NoPadding）。该参数在目的端为加密，在源端为解密。</li></ul>
</div>
<p id="zh-cn_topic_0108275442_p1440312818259"><a name="zh-cn_topic_0108275442_p1440312818259"></a><a name="zh-cn_topic_0108275442_p1440312818259"></a>详细使用方法请参见<a href="迁移文件时加解密.md">迁移文件时加解密</a>。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275442_p1173985171713"><a name="zh-cn_topic_0108275442_p1173985171713"></a><a name="zh-cn_topic_0108275442_p1173985171713"></a>AES-256-GCM</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275442_row8357848162917"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275442_p2560191135113"><a name="zh-cn_topic_0108275442_p2560191135113"></a><a name="zh-cn_topic_0108275442_p2560191135113"></a>数据加密密钥</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275442_p13560410513"><a name="zh-cn_topic_0108275442_p13560410513"></a><a name="zh-cn_topic_0108275442_p13560410513"></a><span class="parmname" id="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmname776612385559"><a name="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmname776612385559"></a><a name="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmname776612385559"></a>“加密方式”</span>选择<span class="parmvalue" id="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmvalue0767193814558"><a name="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmvalue0767193814558"></a><a name="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmvalue0767193814558"></a>“AES-256-GCM”</span>时显示该参数，密钥由长度64的十六进制数组成，且必须与加密时配置的<span class="parmname" id="zh-cn_topic_0108275319_parmname48334346128"><a name="zh-cn_topic_0108275319_parmname48334346128"></a><a name="zh-cn_topic_0108275319_parmname48334346128"></a>“数据加密密钥”</span>一致。如果不一致系统不会报异常，只是解密出来的数据会错误。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275442_p10560111155111"><a name="zh-cn_topic_0108275442_p10560111155111"></a><a name="zh-cn_topic_0108275442_p10560111155111"></a>DD0AE00DFECD78BF051BCFDA25BD4E320DB0A7AC75A1F3FC3D3C56A457DCDC1B</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275442_row926318497295"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275442_p24773525117"><a name="zh-cn_topic_0108275442_p24773525117"></a><a name="zh-cn_topic_0108275442_p24773525117"></a>初始化向量</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275442_p24771354512"><a name="zh-cn_topic_0108275442_p24771354512"></a><a name="zh-cn_topic_0108275442_p24771354512"></a><span class="parmname" id="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmname9947565563"><a name="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmname9947565563"></a><a name="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmname9947565563"></a>“加密方式”</span>选择<span class="parmvalue" id="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmvalue179471468565"><a name="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmvalue179471468565"></a><a name="zh-cn_topic_0108275319_zh-cn_topic_0108275301_parmvalue179471468565"></a>“AES-256-GCM”</span>时显示该参数，初始化向量由长度32的十六进制数组成，且必须与加密时配置的<span class="parmname" id="zh-cn_topic_0108275319_parmname163755565172"><a name="zh-cn_topic_0108275319_parmname163755565172"></a><a name="zh-cn_topic_0108275319_parmname163755565172"></a>“初始化向量”</span>一致。如果不一致系统不会报异常，只是解密出来的数据会错误。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275442_p647775195111"><a name="zh-cn_topic_0108275442_p647775195111"></a><a name="zh-cn_topic_0108275442_p647775195111"></a>5C91687BA886EDCD12ACBC3FF19A3C3F</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：**   
>HDFS文件编码只能为“UTF-8“，故HDFS不支持设置文件编码类型。  

