# 配置OBS目的端参数<a name="dayu_01_0062"></a>

作业中目的连接为[配置OBS连接](配置OBS连接.md)时，即导入数据到云服务OBS时，目的端作业参数如[表1](#zh-cn_topic_0108275301_table31823995163953)所示。

高级属性里的参数为可选参数，默认隐藏，单击界面上的“显示高级属性“后显示。

**表 1**  OBS作为目的端时的作业参数

<a name="zh-cn_topic_0108275301_table31823995163953"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108275301_row18653487163953"><th class="cellrowborder" valign="top" width="17.349999999999998%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0108275301_p2993976910371"><a name="zh-cn_topic_0108275301_p2993976910371"></a><a name="zh-cn_topic_0108275301_p2993976910371"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="19.46%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0108275301_p15314298163953"><a name="zh-cn_topic_0108275301_p15314298163953"></a><a name="zh-cn_topic_0108275301_p15314298163953"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="42.78%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0108275301_p32498630163953"><a name="zh-cn_topic_0108275301_p32498630163953"></a><a name="zh-cn_topic_0108275301_p32498630163953"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="20.41%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0108275301_p15143370163953"><a name="zh-cn_topic_0108275301_p15143370163953"></a><a name="zh-cn_topic_0108275301_p15143370163953"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108275301_row34313000163953"><td class="cellrowborder" rowspan="4" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275301_p52608321103750"><a name="zh-cn_topic_0108275301_p52608321103750"></a><a name="zh-cn_topic_0108275301_p52608321103750"></a>基本参数</p>
</td>
<td class="cellrowborder" valign="top" width="19.46%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275301_p46804376161524"><a name="zh-cn_topic_0108275301_p46804376161524"></a><a name="zh-cn_topic_0108275301_p46804376161524"></a>桶名</p>
</td>
<td class="cellrowborder" valign="top" width="42.78%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275301_p46074171163953"><a name="zh-cn_topic_0108275301_p46074171163953"></a><a name="zh-cn_topic_0108275301_p46074171163953"></a>写入数据的OBS桶名。</p>
</td>
<td class="cellrowborder" valign="top" width="20.41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108275301_p41020337163953"><a name="zh-cn_topic_0108275301_p41020337163953"></a><a name="zh-cn_topic_0108275301_p41020337163953"></a>bucket_2</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275301_row1928353163953"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275301_p28108739161524"><a name="zh-cn_topic_0108275301_p28108739161524"></a><a name="zh-cn_topic_0108275301_p28108739161524"></a>写入目录</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275301_p49679878163953"><a name="zh-cn_topic_0108275301_p49679878163953"></a><a name="zh-cn_topic_0108275301_p49679878163953"></a>写入数据到OBS服务器的目录，目录前面不加<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue64710778143642"><a name="zh-cn_topic_0108275301_parmvalue64710778143642"></a><a name="zh-cn_topic_0108275301_parmvalue64710778143642"></a>“/”</span>。</p>
<p id="zh-cn_topic_0108275442_p1210244910548"><a name="zh-cn_topic_0108275442_p1210244910548"></a><a name="zh-cn_topic_0108275442_p1210244910548"></a>该参数支持配置为时间宏变量，且一个路径名中可以有多个宏定义变量。使用时间宏变量和定时任务配合，可以实现定期同步新增数据，详细说明请参见<a href="使用时间宏变量完成增量同步.md">使用时间宏变量完成增量同步</a>。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275301_p64647157163953"><a name="zh-cn_topic_0108275301_p64647157163953"></a><a name="zh-cn_topic_0108275301_p64647157163953"></a>directory/</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275301_row11687830163953"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275301_p23518636161524"><a name="zh-cn_topic_0108275301_p23518636161524"></a><a name="zh-cn_topic_0108275301_p23518636161524"></a>文件格式</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><div class="p" id="zh-cn_topic_0108275301_p58390965143945"><a name="zh-cn_topic_0108275301_p58390965143945"></a><a name="zh-cn_topic_0108275301_p58390965143945"></a>写入后的文件格式，可选择以下文件格式：<a name="zh-cn_topic_0108275301_ul55756641143945"></a><a name="zh-cn_topic_0108275301_ul55756641143945"></a><ul id="zh-cn_topic_0108275301_ul55756641143945"><li>CSV格式：按CSV格式写入，适用于数据表到文件的迁移。</li><li>二进制格式：选择<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue13073035195648"><a name="zh-cn_topic_0108275301_parmvalue13073035195648"></a><a name="zh-cn_topic_0108275301_parmvalue13073035195648"></a>“二进制格式”</span>时不解析文件内容直接传输，CDM会原样写入文件，不改变原始文件格式，适用于文件到文件的迁移。</li></ul>
</div>
<a name="zh-cn_topic_0108275301_ul16363950154915"></a><a name="zh-cn_topic_0108275301_ul16363950154915"></a><ul id="zh-cn_topic_0108275301_ul16363950154915"><li>CarbonData格式：按CarbonData格式写入，适用于数据表到文件的迁移。</li></ul>
<p id="zh-cn_topic_0108275301_p5736095154452"><a name="zh-cn_topic_0108275301_p5736095154452"></a><a name="zh-cn_topic_0108275301_p5736095154452"></a>如果是文件类数据源（FTP/SFTP/NAS/HDFS/OBS）之间相互迁移数据，此处的<span class="parmname" id="zh-cn_topic_0108275301_parmname29778793154532"><a name="zh-cn_topic_0108275301_parmname29778793154532"></a><a name="zh-cn_topic_0108275301_parmname29778793154532"></a>“文件格式”</span>只能选择与源端的文件格式一致。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275301_p50683068163953"><a name="zh-cn_topic_0108275301_p50683068163953"></a><a name="zh-cn_topic_0108275301_p50683068163953"></a>CSV格式</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275301_row33602446102911"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275301_p13031414102911"><a name="zh-cn_topic_0108275301_p13031414102911"></a><a name="zh-cn_topic_0108275301_p13031414102911"></a>重复文件处理方式</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><div class="p" id="zh-cn_topic_0108275301_p48911576102911"><a name="zh-cn_topic_0108275301_p48911576102911"></a><a name="zh-cn_topic_0108275301_p48911576102911"></a>只有文件名和文件大小都相同才会判定为重复文件。写入时如果出现文件重复，可选择如下处理方式：<a name="zh-cn_topic_0108275301_ul38524806103122"></a><a name="zh-cn_topic_0108275301_ul38524806103122"></a><ul id="zh-cn_topic_0108275301_ul38524806103122"><li>替换重复文件</li><li>跳过重复文件</li><li>停止任务</li></ul>
</div>
<p id="zh-cn_topic_0108275301_p1212309585"><a name="zh-cn_topic_0108275301_p1212309585"></a><a name="zh-cn_topic_0108275301_p1212309585"></a>具体使用方法请参见<a href="文件增量迁移.md#zh-cn_topic_0108275366_section1265543752816">跳过重复文件</a>。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275301_p2414735102911"><a name="zh-cn_topic_0108275301_p2414735102911"></a><a name="zh-cn_topic_0108275301_p2414735102911"></a>跳过重复文件</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275301_row168768506410"><td class="cellrowborder" rowspan="19" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275301_p5876650545"><a name="zh-cn_topic_0108275301_p5876650545"></a><a name="zh-cn_topic_0108275301_p5876650545"></a>高级属性</p>
</td>
<td class="cellrowborder" valign="top" width="19.46%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275301_p118762050344"><a name="zh-cn_topic_0108275301_p118762050344"></a><a name="zh-cn_topic_0108275301_p118762050344"></a>加密方式</p>
</td>
<td class="cellrowborder" valign="top" width="42.78%" headers="mcps1.2.5.1.3 "><div class="p" id="zh-cn_topic_0108275301_p268631112373"><a name="zh-cn_topic_0108275301_p268631112373"></a><a name="zh-cn_topic_0108275301_p268631112373"></a>选择是否对上传的数据进行加密，以及加密方式：<a name="zh-cn_topic_0108275301_ul193603764111"></a><a name="zh-cn_topic_0108275301_ul193603764111"></a><ul id="zh-cn_topic_0108275301_ul193603764111"><li>无：不加密，直接写入数据。</li><li>KMS：使用数据加密服务中的KMS进行加密。如果启用KMS加密则无法进行数据的MD5校验。</li><li>AES-256-GCM：使用长度为256byte的AES对称加密算法，目前加密算法只支持AES-256-GCM（NoPadding）。该参数在目的端为加密，在源端为解密。</li></ul>
</div>
<p id="zh-cn_topic_0108275301_p647742212504"><a name="zh-cn_topic_0108275301_p647742212504"></a><a name="zh-cn_topic_0108275301_p647742212504"></a>详细使用方法请参见<a href="迁移文件时加解密.md">迁移文件时加解密</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="20.41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108275301_p168764505413"><a name="zh-cn_topic_0108275301_p168764505413"></a><a name="zh-cn_topic_0108275301_p168764505413"></a>KMS</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275301_row169871402061"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275301_p189871808614"><a name="zh-cn_topic_0108275301_p189871808614"></a><a name="zh-cn_topic_0108275301_p189871808614"></a>KMS ID</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275301_p124381309114"><a name="zh-cn_topic_0108275301_p124381309114"></a><a name="zh-cn_topic_0108275301_p124381309114"></a>写入文件时加密使用的密钥，<span class="parmname" id="zh-cn_topic_0108275301_parmname204378018111"><a name="zh-cn_topic_0108275301_parmname204378018111"></a><a name="zh-cn_topic_0108275301_parmname204378018111"></a>“加密方式”</span>选择<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue1743810012114"><a name="zh-cn_topic_0108275301_parmvalue1743810012114"></a><a name="zh-cn_topic_0108275301_parmvalue1743810012114"></a>“KMS”</span>时显示该参数。单击输入框后面的<a name="zh-cn_topic_0108275301_image514169183517"></a><a name="zh-cn_topic_0108275301_image514169183517"></a><span><img id="zh-cn_topic_0108275301_image514169183517" src="figures/点选按钮.png"></span>，可以直接选择在数据加密服务中已创建好的KMS密钥。</p>
<a name="zh-cn_topic_0108275301_ul1564184121119"></a><a name="zh-cn_topic_0108275301_ul1564184121119"></a><ul id="zh-cn_topic_0108275301_ul1564184121119"><li>当使用与CDM集群相同项目下的KMS密钥时，不需要修改下面的<span class="parmname" id="zh-cn_topic_0108275301_parmname52363183237"><a name="zh-cn_topic_0108275301_parmname52363183237"></a><a name="zh-cn_topic_0108275301_parmname52363183237"></a>“项目ID”</span>参数。</li><li>当用户使用其它项目下的KMS密钥时，需要修改下面的<span class="parmname" id="zh-cn_topic_0108275301_parmname73725389427"><a name="zh-cn_topic_0108275301_parmname73725389427"></a><a name="zh-cn_topic_0108275301_parmname73725389427"></a>“项目ID”</span>参数。</li></ul>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275301_p990948669"><a name="zh-cn_topic_0108275301_p990948669"></a><a name="zh-cn_topic_0108275301_p990948669"></a>53440ccb-3e73-4700-98b5-71ff5476e621</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275301_row21403316717"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275301_p41715339717"><a name="zh-cn_topic_0108275301_p41715339717"></a><a name="zh-cn_topic_0108275301_p41715339717"></a>项目ID</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275301_p18101134914317"><a name="zh-cn_topic_0108275301_p18101134914317"></a><a name="zh-cn_topic_0108275301_p18101134914317"></a>KMS ID所属的项目ID，该参数默认值为当前CDM集群所属的项目ID。</p>
<a name="zh-cn_topic_0108275301_ul11109174919434"></a><a name="zh-cn_topic_0108275301_ul11109174919434"></a><ul id="zh-cn_topic_0108275301_ul11109174919434"><li>当<span class="parmname" id="zh-cn_topic_0108275301_parmname1710911499430"><a name="zh-cn_topic_0108275301_parmname1710911499430"></a><a name="zh-cn_topic_0108275301_parmname1710911499430"></a>“KMS ID”</span>与CDM集群在同一个项目下时，这里的<span class="parmname" id="zh-cn_topic_0108275301_parmname810994914318"><a name="zh-cn_topic_0108275301_parmname810994914318"></a><a name="zh-cn_topic_0108275301_parmname810994914318"></a>“项目ID”</span>保持默认即可。</li><li>当<span class="parmname" id="zh-cn_topic_0108275301_parmname610994944319"><a name="zh-cn_topic_0108275301_parmname610994944319"></a><a name="zh-cn_topic_0108275301_parmname610994944319"></a>“KMS ID”</span>使用的是其它项目下的KMS ID时，这里需要修改为KMS所属的项目ID。</li></ul>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275301_p91715337717"><a name="zh-cn_topic_0108275301_p91715337717"></a><a name="zh-cn_topic_0108275301_p91715337717"></a>9bd7c4bd54e5417198f9591bef07ae67</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275301_row11559818514"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275301_p2560191135113"><a name="zh-cn_topic_0108275301_p2560191135113"></a><a name="zh-cn_topic_0108275301_p2560191135113"></a>数据加密密钥</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275301_p13560410513"><a name="zh-cn_topic_0108275301_p13560410513"></a><a name="zh-cn_topic_0108275301_p13560410513"></a><span class="parmname" id="zh-cn_topic_0108275301_parmname776612385559"><a name="zh-cn_topic_0108275301_parmname776612385559"></a><a name="zh-cn_topic_0108275301_parmname776612385559"></a>“加密方式”</span>选择<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue0767193814558"><a name="zh-cn_topic_0108275301_parmvalue0767193814558"></a><a name="zh-cn_topic_0108275301_parmvalue0767193814558"></a>“AES-256-GCM”</span>时显示该参数，密钥由长度64的十六进制数组成。</p>
<p id="zh-cn_topic_0108275301_p18430442724"><a name="zh-cn_topic_0108275301_p18430442724"></a><a name="zh-cn_topic_0108275301_p18430442724"></a>请您牢记这里配置的<span class="parmname" id="zh-cn_topic_0108275301_parmname035312613138"><a name="zh-cn_topic_0108275301_parmname035312613138"></a><a name="zh-cn_topic_0108275301_parmname035312613138"></a>“数据加密密钥”</span>，解密时的密钥与这里配置的必须一致。如果不一致系统不会报异常，只是解密出来的数据会错误。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275301_p10560111155111"><a name="zh-cn_topic_0108275301_p10560111155111"></a><a name="zh-cn_topic_0108275301_p10560111155111"></a>DD0AE00DFECD78BF051BCFDA25BD4E320DB0A7AC75A1F3FC3D3C56A457DCDC1B</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275301_row114771518519"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275301_p24773525117"><a name="zh-cn_topic_0108275301_p24773525117"></a><a name="zh-cn_topic_0108275301_p24773525117"></a>初始化向量</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275301_p24771354512"><a name="zh-cn_topic_0108275301_p24771354512"></a><a name="zh-cn_topic_0108275301_p24771354512"></a><span class="parmname" id="zh-cn_topic_0108275301_parmname9947565563"><a name="zh-cn_topic_0108275301_parmname9947565563"></a><a name="zh-cn_topic_0108275301_parmname9947565563"></a>“加密方式”</span>选择<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue179471468565"><a name="zh-cn_topic_0108275301_parmvalue179471468565"></a><a name="zh-cn_topic_0108275301_parmvalue179471468565"></a>“AES-256-GCM”</span>时显示该参数，初始化向量由长度32的十六进制数组成。</p>
<p id="zh-cn_topic_0108275301_p51641322122914"><a name="zh-cn_topic_0108275301_p51641322122914"></a><a name="zh-cn_topic_0108275301_p51641322122914"></a>请您牢记这里配置的<span class="parmname" id="zh-cn_topic_0108275301_parmname91651822122920"><a name="zh-cn_topic_0108275301_parmname91651822122920"></a><a name="zh-cn_topic_0108275301_parmname91651822122920"></a>“初始化向量”</span>，解密时的初始化向量与这里配置的必须一致。如果不一致系统不会报异常，只是解密出来的数据会错误。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275301_p647775195111"><a name="zh-cn_topic_0108275301_p647775195111"></a><a name="zh-cn_topic_0108275301_p647775195111"></a>5C91687BA886EDCD12ACBC3FF19A3C3F</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275301_row654017329411"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275301_p1754014324418"><a name="zh-cn_topic_0108275301_p1754014324418"></a><a name="zh-cn_topic_0108275301_p1754014324418"></a>复制Content-Type属性</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275301_p18177191318566"><a name="zh-cn_topic_0108275301_p18177191318566"></a><a name="zh-cn_topic_0108275301_p18177191318566"></a><span class="parmname" id="zh-cn_topic_0108275301_parmname41779138565"><a name="zh-cn_topic_0108275301_parmname41779138565"></a><a name="zh-cn_topic_0108275301_parmname41779138565"></a>“文件格式”</span>为<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue917751375617"><a name="zh-cn_topic_0108275301_parmvalue917751375617"></a><a name="zh-cn_topic_0108275301_parmvalue917751375617"></a>“二进制”</span>，且源端、目的端都为对象存储时，才有该参数。</p>
<p id="zh-cn_topic_0108275301_p014919221606"><a name="zh-cn_topic_0108275301_p014919221606"></a><a name="zh-cn_topic_0108275301_p014919221606"></a>选择<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue514910221608"><a name="zh-cn_topic_0108275301_parmvalue514910221608"></a><a name="zh-cn_topic_0108275301_parmvalue514910221608"></a>“是”</span>后，迁移对象文件时会复制源文件的Content-Type属性，主要用于静态网站的迁移场景。</p>
<p id="zh-cn_topic_0108275301_p9540193215413"><a name="zh-cn_topic_0108275301_p9540193215413"></a><a name="zh-cn_topic_0108275301_p9540193215413"></a>归档存储的桶不支持设置Content-Type属性，所以如果开启了该参数，目的端选择写入的桶时，必须选择非归档存储的桶。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275301_p25401432204120"><a name="zh-cn_topic_0108275301_p25401432204120"></a><a name="zh-cn_topic_0108275301_p25401432204120"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275301_row4164236716479"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275301_p5746360161524"><a name="zh-cn_topic_0108275301_p5746360161524"></a><a name="zh-cn_topic_0108275301_p5746360161524"></a>换行符</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275301_p1538732316479"><a name="zh-cn_topic_0108275301_p1538732316479"></a><a name="zh-cn_topic_0108275301_p1538732316479"></a>文件中的换行符，默认自动识别<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue20019196113242"><a name="zh-cn_topic_0108275301_parmvalue20019196113242"></a><a name="zh-cn_topic_0108275301_parmvalue20019196113242"></a>“\n”</span>、<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue34571243113250"><a name="zh-cn_topic_0108275301_parmvalue34571243113250"></a><a name="zh-cn_topic_0108275301_parmvalue34571243113250"></a>“\r”</span>或<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue1038974611337"><a name="zh-cn_topic_0108275301_parmvalue1038974611337"></a><a name="zh-cn_topic_0108275301_parmvalue1038974611337"></a>“\r\n”</span>。<span class="parmname" id="zh-cn_topic_0108275301_parmname23758818145740"><a name="zh-cn_topic_0108275301_parmname23758818145740"></a><a name="zh-cn_topic_0108275301_parmname23758818145740"></a>“文件格式”</span>为<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue46072507145830"><a name="zh-cn_topic_0108275301_parmvalue46072507145830"></a><a name="zh-cn_topic_0108275301_parmvalue46072507145830"></a>“二进制格式”</span>时该参数值无效。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275301_p3841367016479"><a name="zh-cn_topic_0108275301_p3841367016479"></a><a name="zh-cn_topic_0108275301_p3841367016479"></a>\n</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275301_row52292662164713"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275301_p3584363161524"><a name="zh-cn_topic_0108275301_p3584363161524"></a><a name="zh-cn_topic_0108275301_p3584363161524"></a>字段分隔符</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275301_p31647034164713"><a name="zh-cn_topic_0108275301_p31647034164713"></a><a name="zh-cn_topic_0108275301_p31647034164713"></a>文件中的字段分隔符。<span class="parmname" id="zh-cn_topic_0108275301_parmname3855270114580"><a name="zh-cn_topic_0108275301_parmname3855270114580"></a><a name="zh-cn_topic_0108275301_parmname3855270114580"></a>“文件格式”</span>为<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue27349529145857"><a name="zh-cn_topic_0108275301_parmvalue27349529145857"></a><a name="zh-cn_topic_0108275301_parmvalue27349529145857"></a>“二进制格式”</span>时该参数值无效。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275301_p13273001164713"><a name="zh-cn_topic_0108275301_p13273001164713"></a><a name="zh-cn_topic_0108275301_p13273001164713"></a>,</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275301_row679211194911"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275301_p1848919333580"><a name="zh-cn_topic_0108275301_p1848919333580"></a><a name="zh-cn_topic_0108275301_p1848919333580"></a>写入文件大小</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275301_p34895339587"><a name="zh-cn_topic_0108275301_p34895339587"></a><a name="zh-cn_topic_0108275301_p34895339587"></a>源端为数据库时该参数才显示，支持按大小分成多个文件存储，避免导出的文件过大，单位为MB。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275301_p9489113313583"><a name="zh-cn_topic_0108275301_p9489113313583"></a><a name="zh-cn_topic_0108275301_p9489113313583"></a>1024</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275301_row779218329215"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275301_p12792153216220"><a name="zh-cn_topic_0108275301_p12792153216220"></a><a name="zh-cn_topic_0108275301_p12792153216220"></a>校验MD5值</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275301_p315803203318"><a name="zh-cn_topic_0108275301_p315803203318"></a><a name="zh-cn_topic_0108275301_p315803203318"></a>使用<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue315812322337"><a name="zh-cn_topic_0108275301_parmvalue315812322337"></a><a name="zh-cn_topic_0108275301_parmvalue315812322337"></a>“二进制格式”</span>传输文件时，才能校验MD5值。选择校验MD5值时，无法使用KMS加密。</p>
<p id="zh-cn_topic_0108275301_p187921432029"><a name="zh-cn_topic_0108275301_p187921432029"></a><a name="zh-cn_topic_0108275301_p187921432029"></a>计算源文件的MD5值，并与OBS返回的MD5值进行校验。如果源端已经存在MD5文件，则直接读取源端的MD5文件与OBS返回的MD5值进行校验，具体请参见<a href="MD5校验文件一致性.md">MD5校验文件一致性</a>。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275301_p10792103211219"><a name="zh-cn_topic_0108275301_p10792103211219"></a><a name="zh-cn_topic_0108275301_p10792103211219"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275301_row111227419319"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275301_p612218412318"><a name="zh-cn_topic_0108275301_p612218412318"></a><a name="zh-cn_topic_0108275301_p612218412318"></a>记录校验结果</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275301_p14122114117312"><a name="zh-cn_topic_0108275301_p14122114117312"></a><a name="zh-cn_topic_0108275301_p14122114117312"></a>当选择校验MD5值时，可以选择是否记录校验结果。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275301_p151371941535"><a name="zh-cn_topic_0108275301_p151371941535"></a><a name="zh-cn_topic_0108275301_p151371941535"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275301_row164221301947"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275301_p1442210010419"><a name="zh-cn_topic_0108275301_p1442210010419"></a><a name="zh-cn_topic_0108275301_p1442210010419"></a>校验结果写入连接</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275301_p24225018412"><a name="zh-cn_topic_0108275301_p24225018412"></a><a name="zh-cn_topic_0108275301_p24225018412"></a>可以指定任意一个OBS连接，将MD5校验结果写入该连接的桶下。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275301_p4422901141"><a name="zh-cn_topic_0108275301_p4422901141"></a><a name="zh-cn_topic_0108275301_p4422901141"></a>obslink</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275301_row1773402110414"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275301_p1575111211945"><a name="zh-cn_topic_0108275301_p1575111211945"></a><a name="zh-cn_topic_0108275301_p1575111211945"></a>OBS桶</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275301_p5751921745"><a name="zh-cn_topic_0108275301_p5751921745"></a><a name="zh-cn_topic_0108275301_p5751921745"></a>写入MD5校验结果的OBS桶。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275301_p0751152117414"><a name="zh-cn_topic_0108275301_p0751152117414"></a><a name="zh-cn_topic_0108275301_p0751152117414"></a>cdm05</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275301_row17765240941"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275301_p57650401547"><a name="zh-cn_topic_0108275301_p57650401547"></a><a name="zh-cn_topic_0108275301_p57650401547"></a>写入目录</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275301_p16765184013417"><a name="zh-cn_topic_0108275301_p16765184013417"></a><a name="zh-cn_topic_0108275301_p16765184013417"></a>写入MD5校验结果的目录。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275301_p107655405411"><a name="zh-cn_topic_0108275301_p107655405411"></a><a name="zh-cn_topic_0108275301_p107655405411"></a>/md5/</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275301_row20619738164716"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275301_p59975518161524"><a name="zh-cn_topic_0108275301_p59975518161524"></a><a name="zh-cn_topic_0108275301_p59975518161524"></a>编码类型</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275301_p61741608164716"><a name="zh-cn_topic_0108275301_p61741608164716"></a><a name="zh-cn_topic_0108275301_p61741608164716"></a>文件编码类型，例如：<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue4971784420504"><a name="zh-cn_topic_0108275301_parmvalue4971784420504"></a><a name="zh-cn_topic_0108275301_parmvalue4971784420504"></a>“UTF-8”</span>或<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue61358620504"><a name="zh-cn_topic_0108275301_parmvalue61358620504"></a><a name="zh-cn_topic_0108275301_parmvalue61358620504"></a>“GBK”</span>。<span class="parmname" id="zh-cn_topic_0108275301_parmname66615771145817"><a name="zh-cn_topic_0108275301_parmname66615771145817"></a><a name="zh-cn_topic_0108275301_parmname66615771145817"></a>“文件格式”</span>为<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue52502287145839"><a name="zh-cn_topic_0108275301_parmvalue52502287145839"></a><a name="zh-cn_topic_0108275301_parmvalue52502287145839"></a>“二进制格式”</span>时该参数值无效。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275301_p35014356164716"><a name="zh-cn_topic_0108275301_p35014356164716"></a><a name="zh-cn_topic_0108275301_p35014356164716"></a>GBK</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275301_row1178013239283"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275301_p147801323132816"><a name="zh-cn_topic_0108275301_p147801323132816"></a><a name="zh-cn_topic_0108275301_p147801323132816"></a>使用包围符</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275301_p1210241263316"><a name="zh-cn_topic_0108275301_p1210241263316"></a><a name="zh-cn_topic_0108275301_p1210241263316"></a><span class="parmname" id="zh-cn_topic_0108275301_parmname111029121339"><a name="zh-cn_topic_0108275301_parmname111029121339"></a><a name="zh-cn_topic_0108275301_parmname111029121339"></a>“文件格式”</span>为<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue910281223312"><a name="zh-cn_topic_0108275301_parmvalue910281223312"></a><a name="zh-cn_topic_0108275301_parmvalue910281223312"></a>“CSV格式”</span>，才有该参数，用于将数据库的表迁移到文件系统的场景。</p>
<p id="zh-cn_topic_0108275301_p19249144319"><a name="zh-cn_topic_0108275301_p19249144319"></a><a name="zh-cn_topic_0108275301_p19249144319"></a>选择<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue13709134210325"><a name="zh-cn_topic_0108275301_parmvalue13709134210325"></a><a name="zh-cn_topic_0108275301_parmvalue13709134210325"></a>“是”</span>时，如果源端数据表中的某一个字段内容包含字段分隔符或换行符，写入目的端时CDM会使用双引号（"）作为包围符将该字段内容括起来，作为一个整体存储，避免其中的字段分隔符误将一个字段分隔成两个，或者换行符误将字段换行。例如：数据库中某字段为hello,world，使用包围符后，导出到CSV文件的时候数据为"hello,world"。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275301_p778018234281"><a name="zh-cn_topic_0108275301_p778018234281"></a><a name="zh-cn_topic_0108275301_p778018234281"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275301_row196815113218"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275301_p13851563214"><a name="zh-cn_topic_0108275301_p13851563214"></a><a name="zh-cn_topic_0108275301_p13851563214"></a>首行为标题行</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275301_p68171593216"><a name="zh-cn_topic_0108275301_p68171593216"></a><a name="zh-cn_topic_0108275301_p68171593216"></a><span class="parmname" id="zh-cn_topic_0108275301_parmname19396452103317"><a name="zh-cn_topic_0108275301_parmname19396452103317"></a><a name="zh-cn_topic_0108275301_parmname19396452103317"></a>“文件格式”</span>为<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue739785211338"><a name="zh-cn_topic_0108275301_parmvalue739785211338"></a><a name="zh-cn_topic_0108275301_parmvalue739785211338"></a>“CSV格式”</span>时才有该参数。在迁移表到CSV文件时，CDM默认是不迁移表的标题行，如果该参数选择<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue11024151389"><a name="zh-cn_topic_0108275301_parmvalue11024151389"></a><a name="zh-cn_topic_0108275301_parmvalue11024151389"></a>“是”</span>，CDM在才会将表的标题行数据写入文件。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275301_p582155329"><a name="zh-cn_topic_0108275301_p582155329"></a><a name="zh-cn_topic_0108275301_p582155329"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275301_row162821858141920"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275301_p52821758161913"><a name="zh-cn_topic_0108275301_p52821758161913"></a><a name="zh-cn_topic_0108275301_p52821758161913"></a>作业成功标识文件</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275301_p2282115811910"><a name="zh-cn_topic_0108275301_p2282115811910"></a><a name="zh-cn_topic_0108275301_p2282115811910"></a>当作业执行成功时，会在写入目录下生成一个标识文件，文件名由用户指定。不指定时默认关闭该功能。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275301_p192821858181918"><a name="zh-cn_topic_0108275301_p192821858181918"></a><a name="zh-cn_topic_0108275301_p192821858181918"></a>finish.txt</p>
</td>
</tr>
<tr id="zh-cn_topic_0108275301_row69170353619"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108275301_p49174351862"><a name="zh-cn_topic_0108275301_p49174351862"></a><a name="zh-cn_topic_0108275301_p49174351862"></a>自定义文件名</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108275301_p991718356610"><a name="zh-cn_topic_0108275301_p991718356610"></a><a name="zh-cn_topic_0108275301_p991718356610"></a>从关系型数据库导出数据到OBS，且<span class="parmname" id="zh-cn_topic_0108275301_parmname15585735103412"><a name="zh-cn_topic_0108275301_parmname15585735103412"></a><a name="zh-cn_topic_0108275301_parmname15585735103412"></a>“文件格式”</span>为<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue78218403514"><a name="zh-cn_topic_0108275301_parmvalue78218403514"></a><a name="zh-cn_topic_0108275301_parmvalue78218403514"></a>“CSV格式”</span>时，才有该参数。</p>
<div class="p" id="zh-cn_topic_0108275301_p12170261354"><a name="zh-cn_topic_0108275301_p12170261354"></a><a name="zh-cn_topic_0108275301_p12170261354"></a>用户可以通过该参数自定义OBS端生成的文件名，支持以下自定义方式：<a name="zh-cn_topic_0108275301_ul16382063436"></a><a name="zh-cn_topic_0108275301_ul16382063436"></a><ul id="zh-cn_topic_0108275301_ul16382063436"><li>字符串，支持特殊字符。例如<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue1436324044418"><a name="zh-cn_topic_0108275301_parmvalue1436324044418"></a><a name="zh-cn_topic_0108275301_parmvalue1436324044418"></a>“cdm#”</span>，则生成的文件名为<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue8596161012451"><a name="zh-cn_topic_0108275301_parmvalue8596161012451"></a><a name="zh-cn_topic_0108275301_parmvalue8596161012451"></a>“cdm#.csv”</span>。</li><li>时间宏，例如<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue3630134255018"><a name="zh-cn_topic_0108275301_parmvalue3630134255018"></a><a name="zh-cn_topic_0108275301_parmvalue3630134255018"></a>“${timestamp()}”</span>，则生成的文件名为<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue935517108536"><a name="zh-cn_topic_0108275301_parmvalue935517108536"></a><a name="zh-cn_topic_0108275301_parmvalue935517108536"></a>“1554108737.csv”</span>。</li><li>表名宏，例如<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue138891113545"><a name="zh-cn_topic_0108275301_parmvalue138891113545"></a><a name="zh-cn_topic_0108275301_parmvalue138891113545"></a>“${tableName}”</span>，则生成的文件名为<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue16429112975711"><a name="zh-cn_topic_0108275301_parmvalue16429112975711"></a><a name="zh-cn_topic_0108275301_parmvalue16429112975711"></a>“sqltabname.csv”</span>。</li><li>版本宏，例如<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue106082049604"><a name="zh-cn_topic_0108275301_parmvalue106082049604"></a><a name="zh-cn_topic_0108275301_parmvalue106082049604"></a>“${version}”</span>，则生成的文件名为<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue823014816320"><a name="zh-cn_topic_0108275301_parmvalue823014816320"></a><a name="zh-cn_topic_0108275301_parmvalue823014816320"></a>“v1.csv”</span>。</li><li>字符串和宏（时间宏/表名宏/版本宏）任意组合，例如<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue113932657"><a name="zh-cn_topic_0108275301_parmvalue113932657"></a><a name="zh-cn_topic_0108275301_parmvalue113932657"></a>“cdm#${timestamp()}_${version}”</span>，则生成的文件名为<span class="parmvalue" id="zh-cn_topic_0108275301_parmvalue714712878"><a name="zh-cn_topic_0108275301_parmvalue714712878"></a><a name="zh-cn_topic_0108275301_parmvalue714712878"></a>“cdm#1554108737_v1.csv”</span>。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108275301_p59171435463"><a name="zh-cn_topic_0108275301_p59171435463"></a><a name="zh-cn_topic_0108275301_p59171435463"></a>cdm</p>
</td>
</tr>
</tbody>
</table>

