# 数据开发API错误码<a name="dgc_02_0313"></a>

错误响应消息格式如下：

\{

"error\_code":"DLF.1001",

"error\_msg":"The job not found"

\}

错误码如[表1](#zh-cn_topic_0181281370_table1456816221499)所示。

**表 1**  错误码

<a name="zh-cn_topic_0181281370_table1456816221499"></a>
<table><thead align="left"><tr id="zh-cn_topic_0181281370_row195688221391"><th class="cellrowborder" valign="top" width="9.080908090809082%" id="mcps1.2.6.1.1"><p id="p123056587241"><a name="p123056587241"></a><a name="p123056587241"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="14.361436143614362%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0181281370_p175681522991"><a name="zh-cn_topic_0181281370_p175681522991"></a><a name="zh-cn_topic_0181281370_p175681522991"></a>错误码</p>
</th>
<th class="cellrowborder" valign="top" width="23.03230323032303%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0181281370_p57237144301"><a name="zh-cn_topic_0181281370_p57237144301"></a><a name="zh-cn_topic_0181281370_p57237144301"></a>错误信息</p>
</th>
<th class="cellrowborder" valign="top" width="24.38243824382438%" id="mcps1.2.6.1.4"><p id="p11920316122211"><a name="p11920316122211"></a><a name="p11920316122211"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="29.14291429142914%" id="mcps1.2.6.1.5"><p id="p5834195222115"><a name="p5834195222115"></a><a name="p5834195222115"></a>处理措施</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0181281370_row25681622598"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p2306205862416"><a name="p2306205862416"></a><a name="p2306205862416"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p16724425390"><a name="zh-cn_topic_0181281370_p16724425390"></a><a name="zh-cn_topic_0181281370_p16724425390"></a>DLF.0100</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p157240253914"><a name="zh-cn_topic_0181281370_p157240253914"></a><a name="zh-cn_topic_0181281370_p157240253914"></a><span id="zh-cn_topic_0181281370_text606464029562"><a name="zh-cn_topic_0181281370_text606464029562"></a><a name="zh-cn_topic_0181281370_text606464029562"></a>作业</span>不存在。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p169200162226"><a name="p169200162226"></a><a name="p169200162226"></a><span id="text388554682514"><a name="text388554682514"></a><a name="text388554682514"></a>作业</span>不存在。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p13344174312218"><a name="p13344174312218"></a><a name="p13344174312218"></a>请检查作业是否存在。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row7568922290"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p1683152382611"><a name="p1683152382611"></a><a name="p1683152382611"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p58931058155515"><a name="zh-cn_topic_0181281370_p58931058155515"></a><a name="zh-cn_topic_0181281370_p58931058155515"></a>DLF.0101</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p67241225394"><a name="zh-cn_topic_0181281370_p67241225394"></a><a name="zh-cn_topic_0181281370_p67241225394"></a>作业配额已达上限。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p91538161266"><a name="p91538161266"></a><a name="p91538161266"></a>作业配额已达上限。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p1934414317211"><a name="p1934414317211"></a><a name="p1934414317211"></a>请申请作业配额。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row2568122595"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p11327142452617"><a name="p11327142452617"></a><a name="p11327142452617"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p61101119115611"><a name="zh-cn_topic_0181281370_p61101119115611"></a><a name="zh-cn_topic_0181281370_p61101119115611"></a>DLF.0102</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p1272413256918"><a name="zh-cn_topic_0181281370_p1272413256918"></a><a name="zh-cn_topic_0181281370_p1272413256918"></a>作业名称已经被其他作业占用。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p1153101613268"><a name="p1153101613268"></a><a name="p1153101613268"></a>作业名称已经被其他作业占用。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p73448436214"><a name="p73448436214"></a><a name="p73448436214"></a>请检查作业是否被占用。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row09568284911"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p63692514267"><a name="p63692514267"></a><a name="p63692514267"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p128149344918"><a name="zh-cn_topic_0181281370_p128149344918"></a><a name="zh-cn_topic_0181281370_p128149344918"></a>DLF.0136</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p1495672820911"><a name="zh-cn_topic_0181281370_p1495672820911"></a><a name="zh-cn_topic_0181281370_p1495672820911"></a>只有批作业才支持这个接口调用。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p815341618269"><a name="p815341618269"></a><a name="p815341618269"></a>只有批作业才支持这个接口调用。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p1734434312218"><a name="p1734434312218"></a><a name="p1734434312218"></a>请检查接口调用作业。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row1869574985"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p99747257267"><a name="p99747257267"></a><a name="p99747257267"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p146951342815"><a name="zh-cn_topic_0181281370_p146951342815"></a><a name="zh-cn_topic_0181281370_p146951342815"></a>DLF.0137</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p36969410810"><a name="zh-cn_topic_0181281370_p36969410810"></a><a name="zh-cn_topic_0181281370_p36969410810"></a>作业实例不存在。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p191538163264"><a name="p191538163264"></a><a name="p191538163264"></a>作业实例不存在。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p17344174332114"><a name="p17344174332114"></a><a name="p17344174332114"></a>请检查作业实例是否存在。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row116677620203"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p1511983072615"><a name="p1511983072615"></a><a name="p1511983072615"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p36676612204"><a name="zh-cn_topic_0181281370_p36676612204"></a><a name="zh-cn_topic_0181281370_p36676612204"></a>DLF.0201</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p1066706122017"><a name="zh-cn_topic_0181281370_p1066706122017"></a><a name="zh-cn_topic_0181281370_p1066706122017"></a>创建脚本失败。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p1315314166269"><a name="p1315314166269"></a><a name="p1315314166269"></a>创建脚本失败。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p4344743172118"><a name="p4344743172118"></a><a name="p4344743172118"></a>请检查脚本。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row20169135992016"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p111191930162612"><a name="p111191930162612"></a><a name="p111191930162612"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p1816914594207"><a name="zh-cn_topic_0181281370_p1816914594207"></a><a name="zh-cn_topic_0181281370_p1816914594207"></a>DLF.0202</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p716910593203"><a name="zh-cn_topic_0181281370_p716910593203"></a><a name="zh-cn_topic_0181281370_p716910593203"></a>脚本名称已经被其他脚本占用。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p7153121612261"><a name="p7153121612261"></a><a name="p7153121612261"></a>脚本名称已经被其他脚本占用。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p196605315293"><a name="p196605315293"></a><a name="p196605315293"></a>请检查脚本名称是否被占用。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row14799103522115"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p1011943014264"><a name="p1011943014264"></a><a name="p1011943014264"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p0358174852116"><a name="zh-cn_topic_0181281370_p0358174852116"></a><a name="zh-cn_topic_0181281370_p0358174852116"></a>DLF.0203</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p1779919353215"><a name="zh-cn_topic_0181281370_p1779919353215"></a><a name="zh-cn_topic_0181281370_p1779919353215"></a>修改脚本失败。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p31531616182615"><a name="p31531616182615"></a><a name="p31531616182615"></a>修改脚本失败。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p163449435210"><a name="p163449435210"></a><a name="p163449435210"></a>请检查脚本。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row10554710141818"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p5120183082611"><a name="p5120183082611"></a><a name="p5120183082611"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p1055481011189"><a name="zh-cn_topic_0181281370_p1055481011189"></a><a name="zh-cn_topic_0181281370_p1055481011189"></a>DLF.0802</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p35541910181816"><a name="zh-cn_topic_0181281370_p35541910181816"></a><a name="zh-cn_topic_0181281370_p35541910181816"></a>指定的参数没有配置。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p1915361672616"><a name="p1915361672616"></a><a name="p1915361672616"></a>指定的参数没有配置。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p834434382114"><a name="p834434382114"></a><a name="p834434382114"></a>请检查参数。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row10390237121812"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p101201730172619"><a name="p101201730172619"></a><a name="p101201730172619"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p166021441121813"><a name="zh-cn_topic_0181281370_p166021441121813"></a><a name="zh-cn_topic_0181281370_p166021441121813"></a>DLF.0803</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p1167648161817"><a name="zh-cn_topic_0181281370_p1167648161817"></a><a name="zh-cn_topic_0181281370_p1167648161817"></a>OBS路径不合法。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p1154111614265"><a name="p1154111614265"></a><a name="p1154111614265"></a>OBS路径不合法。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p1534454392113"><a name="p1534454392113"></a><a name="p1534454392113"></a>请检查OBS路径。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row429723411018"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p195101131182610"><a name="p195101131182610"></a><a name="p195101131182610"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p1790220491786"><a name="zh-cn_topic_0181281370_p1790220491786"></a><a name="zh-cn_topic_0181281370_p1790220491786"></a>DLF.0810</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p99328456810"><a name="zh-cn_topic_0181281370_p99328456810"></a><a name="zh-cn_topic_0181281370_p99328456810"></a>查询的系统任务不存在。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p015410167268"><a name="p015410167268"></a><a name="p015410167268"></a>查询的系统任务不存在。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p5344543112110"><a name="p5344543112110"></a><a name="p5344543112110"></a>请检查系统任务。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row298132718719"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p195105318268"><a name="p195105318268"></a><a name="p195105318268"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p89910277716"><a name="zh-cn_topic_0181281370_p89910277716"></a><a name="zh-cn_topic_0181281370_p89910277716"></a>DLF.0815</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p209910271379"><a name="zh-cn_topic_0181281370_p209910271379"></a><a name="zh-cn_topic_0181281370_p209910271379"></a>读取OBS文件失败。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p115411642616"><a name="p115411642616"></a><a name="p115411642616"></a>读取OBS文件失败。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p13441743152119"><a name="p13441743152119"></a><a name="p13441743152119"></a>请检查OBS文件。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row19932945484"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p8510183113266"><a name="p8510183113266"></a><a name="p8510183113266"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p8221162191318"><a name="zh-cn_topic_0181281370_p8221162191318"></a><a name="zh-cn_topic_0181281370_p8221162191318"></a>DLF.1006</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p41152307102"><a name="zh-cn_topic_0181281370_p41152307102"></a><a name="zh-cn_topic_0181281370_p41152307102"></a>作业的节点为空。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p61541716132610"><a name="p61541716132610"></a><a name="p61541716132610"></a>作业的节点为空。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p2344174311218"><a name="p2344174311218"></a><a name="p2344174311218"></a>请检查节点。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row9778121919142"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p2510173152615"><a name="p2510173152615"></a><a name="p2510173152615"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p15778121910144"><a name="zh-cn_topic_0181281370_p15778121910144"></a><a name="zh-cn_topic_0181281370_p15778121910144"></a>DLF.1242</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p9778121914141"><a name="zh-cn_topic_0181281370_p9778121914141"></a><a name="zh-cn_topic_0181281370_p9778121914141"></a>OBS桶不存在。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p515411165265"><a name="p515411165265"></a><a name="p515411165265"></a>OBS桶不存在。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p1174213723119"><a name="p1174213723119"></a><a name="p1174213723119"></a>请检查OBS桶。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row10759125122812"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p3510103113269"><a name="p3510103113269"></a><a name="p3510103113269"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p5759112518281"><a name="zh-cn_topic_0181281370_p5759112518281"></a><a name="zh-cn_topic_0181281370_p5759112518281"></a>DLF.3004</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p147591025172814"><a name="zh-cn_topic_0181281370_p147591025172814"></a><a name="zh-cn_topic_0181281370_p147591025172814"></a>作业名称不能为空。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p6154816142614"><a name="p6154816142614"></a><a name="p6154816142614"></a>作业名称不能为空。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p2344243122119"><a name="p2344243122119"></a><a name="p2344243122119"></a>请检查作业名称。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row135061024182919"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p825093342620"><a name="p825093342620"></a><a name="p825093342620"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p8506112402919"><a name="zh-cn_topic_0181281370_p8506112402919"></a><a name="zh-cn_topic_0181281370_p8506112402919"></a>DLF.3018</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p7507152402915"><a name="zh-cn_topic_0181281370_p7507152402915"></a><a name="zh-cn_topic_0181281370_p7507152402915"></a>作业名称不合法。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p1915481618262"><a name="p1915481618262"></a><a name="p1915481618262"></a>作业名称不合法。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p2344243132113"><a name="p2344243132113"></a><a name="p2344243132113"></a>请检查作业名称。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row153824392910"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p8250163322617"><a name="p8250163322617"></a><a name="p8250163322617"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p482374712917"><a name="zh-cn_topic_0181281370_p482374712917"></a><a name="zh-cn_topic_0181281370_p482374712917"></a>DLF.3025</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p12538144314290"><a name="zh-cn_topic_0181281370_p12538144314290"></a><a name="zh-cn_topic_0181281370_p12538144314290"></a>作业的调度参数不合法。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p161542163265"><a name="p161542163265"></a><a name="p161542163265"></a>作业的调度参数不合法。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p134410431212"><a name="p134410431212"></a><a name="p134410431212"></a>请检查调度参数。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row16206171863011"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p025015336269"><a name="p025015336269"></a><a name="p025015336269"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p92067186309"><a name="zh-cn_topic_0181281370_p92067186309"></a><a name="zh-cn_topic_0181281370_p92067186309"></a>DLF.3050</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p13206818163013"><a name="zh-cn_topic_0181281370_p13206818163013"></a><a name="zh-cn_topic_0181281370_p13206818163013"></a>作业的描述不合法。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p1115412167265"><a name="p1115412167265"></a><a name="p1115412167265"></a>作业的描述不合法。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p2034424319211"><a name="p2034424319211"></a><a name="p2034424319211"></a>请检查作业的描述。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row25811210516"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p18250533182611"><a name="p18250533182611"></a><a name="p18250533182611"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p11590122517"><a name="zh-cn_topic_0181281370_p11590122517"></a><a name="zh-cn_topic_0181281370_p11590122517"></a>DLF.6201</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p85971214520"><a name="zh-cn_topic_0181281370_p85971214520"></a><a name="zh-cn_topic_0181281370_p85971214520"></a>脚本不存在。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p31549164260"><a name="p31549164260"></a><a name="p31549164260"></a>脚本不存在。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p6344243182113"><a name="p6344243182113"></a><a name="p6344243182113"></a>请检查脚本。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row75769450516"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p152501733162618"><a name="p152501733162618"></a><a name="p152501733162618"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p5576144511514"><a name="zh-cn_topic_0181281370_p5576144511514"></a><a name="zh-cn_topic_0181281370_p5576144511514"></a>DLF.6205</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p155768451450"><a name="zh-cn_topic_0181281370_p155768451450"></a><a name="zh-cn_topic_0181281370_p155768451450"></a>脚本的执行实例不存在。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p201541016172610"><a name="p201541016172610"></a><a name="p201541016172610"></a>脚本的执行实例不存在。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p1098681193317"><a name="p1098681193317"></a><a name="p1098681193317"></a>请检查脚本的执行实例。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row1949019718164"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p356633511265"><a name="p356633511265"></a><a name="p356633511265"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p1150244518618"><a name="zh-cn_topic_0181281370_p1150244518618"></a><a name="zh-cn_topic_0181281370_p1150244518618"></a>DLF.6241</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p2050294518612"><a name="zh-cn_topic_0181281370_p2050294518612"></a><a name="zh-cn_topic_0181281370_p2050294518612"></a>查询的资源不存在。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p16154111642611"><a name="p16154111642611"></a><a name="p16154111642611"></a>查询的资源不存在。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p1339125103314"><a name="p1339125103314"></a><a name="p1339125103314"></a>请检查资源是否存在。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row11583182210916"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p556693510267"><a name="p556693510267"></a><a name="p556693510267"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p15654105013419"><a name="zh-cn_topic_0181281370_p15654105013419"></a><a name="zh-cn_topic_0181281370_p15654105013419"></a>DLF.6247</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p107401925698"><a name="zh-cn_topic_0181281370_p107401925698"></a><a name="zh-cn_topic_0181281370_p107401925698"></a>脚本类型没有指定。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p181541616112611"><a name="p181541616112611"></a><a name="p181541616112611"></a>脚本类型没有指定。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p034484342113"><a name="p034484342113"></a><a name="p034484342113"></a>请检查脚本类型。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row1550217451166"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p956663512263"><a name="p956663512263"></a><a name="p956663512263"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p124488412168"><a name="zh-cn_topic_0181281370_p124488412168"></a><a name="zh-cn_topic_0181281370_p124488412168"></a>DLF.6253</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p114472471617"><a name="zh-cn_topic_0181281370_p114472471617"></a><a name="zh-cn_topic_0181281370_p114472471617"></a>脚本配额已达上限。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p715491610267"><a name="p715491610267"></a><a name="p715491610267"></a>脚本配额已达上限。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p1836819853418"><a name="p1836819853418"></a><a name="p1836819853418"></a>请申请脚本配额。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row258315221097"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p1456617354269"><a name="p1456617354269"></a><a name="p1456617354269"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p823081119618"><a name="zh-cn_topic_0181281370_p823081119618"></a><a name="zh-cn_topic_0181281370_p823081119618"></a>DLF.6258</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p322910112069"><a name="zh-cn_topic_0181281370_p322910112069"></a><a name="zh-cn_topic_0181281370_p322910112069"></a>目录下有数据无法删除。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p6154116142617"><a name="p6154116142617"></a><a name="p6154116142617"></a>目录下有数据无法删除。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p1834520431219"><a name="p1834520431219"></a><a name="p1834520431219"></a>请先删除目录下数据。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row17861111981711"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p4566153513263"><a name="p4566153513263"></a><a name="p4566153513263"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p72241844172215"><a name="zh-cn_topic_0181281370_p72241844172215"></a><a name="zh-cn_topic_0181281370_p72241844172215"></a>DLF.6259</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p32253444229"><a name="zh-cn_topic_0181281370_p32253444229"></a><a name="zh-cn_topic_0181281370_p32253444229"></a>目录下已经存在同名的资源。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p2154131614267"><a name="p2154131614267"></a><a name="p2154131614267"></a>目录下已经存在同名的资源。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p13454432210"><a name="p13454432210"></a><a name="p13454432210"></a>请检查目录下是否存在同名的资源。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row317313616243"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p199417377264"><a name="p199417377264"></a><a name="p199417377264"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p61731864243"><a name="zh-cn_topic_0181281370_p61731864243"></a><a name="zh-cn_topic_0181281370_p61731864243"></a>DLF.6263</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p121731763249"><a name="zh-cn_topic_0181281370_p121731763249"></a><a name="zh-cn_topic_0181281370_p121731763249"></a>资源类型不合法。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p1015581642615"><a name="p1015581642615"></a><a name="p1015581642615"></a>资源类型不合法。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p103452436218"><a name="p103452436218"></a><a name="p103452436218"></a>请检查资源类型。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row129751044182412"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p1599414379264"><a name="p1599414379264"></a><a name="p1599414379264"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p20977124492418"><a name="zh-cn_topic_0181281370_p20977124492418"></a><a name="zh-cn_topic_0181281370_p20977124492418"></a>DLF.6264</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p199779447243"><a name="zh-cn_topic_0181281370_p199779447243"></a><a name="zh-cn_topic_0181281370_p199779447243"></a>资源文件所在的OBS路径不合法。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p1015541612617"><a name="p1015541612617"></a><a name="p1015541612617"></a>资源文件所在的OBS路径不合法。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p4345243112118"><a name="p4345243112118"></a><a name="p4345243112118"></a>请检查OBS路径。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row37601115142512"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p1899493772611"><a name="p1899493772611"></a><a name="p1899493772611"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p1376016158256"><a name="zh-cn_topic_0181281370_p1376016158256"></a><a name="zh-cn_topic_0181281370_p1376016158256"></a>DLF.6265</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p17760101552514"><a name="zh-cn_topic_0181281370_p17760101552514"></a><a name="zh-cn_topic_0181281370_p17760101552514"></a>资源描述不合法。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p131552166262"><a name="p131552166262"></a><a name="p131552166262"></a>资源描述不合法。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p18213912193617"><a name="p18213912193617"></a><a name="p18213912193617"></a>请检查资源描述。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row16387053123118"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p899433782614"><a name="p899433782614"></a><a name="p899433782614"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p8110125714317"><a name="zh-cn_topic_0181281370_p8110125714317"></a><a name="zh-cn_topic_0181281370_p8110125714317"></a>DLF.6271</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p73877536310"><a name="zh-cn_topic_0181281370_p73877536310"></a><a name="zh-cn_topic_0181281370_p73877536310"></a>每个用户只能创建一个DLI连接。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p3155216172617"><a name="p3155216172617"></a><a name="p3155216172617"></a>每个用户只能创建一个DLI连接。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p03452431213"><a name="p03452431213"></a><a name="p03452431213"></a>请检查DLI连接。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row9992101781112"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p129941237172614"><a name="p129941237172614"></a><a name="p129941237172614"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p1999221719113"><a name="zh-cn_topic_0181281370_p1999221719113"></a><a name="zh-cn_topic_0181281370_p1999221719113"></a>DLF.6309</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p999217177117"><a name="zh-cn_topic_0181281370_p999217177117"></a><a name="zh-cn_topic_0181281370_p999217177117"></a>连接名称已经在其他连接占用。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p6155616102612"><a name="p6155616102612"></a><a name="p6155616102612"></a>连接名称已经在其他连接占用。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p9345144342120"><a name="p9345144342120"></a><a name="p9345144342120"></a>请检查连接名称是否被其他连接占用。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row9750857101015"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p78260398265"><a name="p78260398265"></a><a name="p78260398265"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p37511657101014"><a name="zh-cn_topic_0181281370_p37511657101014"></a><a name="zh-cn_topic_0181281370_p37511657101014"></a>DLF.6322</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p375115577104"><a name="zh-cn_topic_0181281370_p375115577104"></a><a name="zh-cn_topic_0181281370_p375115577104"></a>数据连接不存在。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p7155616172615"><a name="p7155616172615"></a><a name="p7155616172615"></a>数据连接不存在。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p12345194332118"><a name="p12345194332118"></a><a name="p12345194332118"></a>请检查数据连接。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row106476173515"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p198261439162615"><a name="p198261439162615"></a><a name="p198261439162615"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p564712117354"><a name="zh-cn_topic_0181281370_p564712117354"></a><a name="zh-cn_topic_0181281370_p564712117354"></a>DLF.6323</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p764714115358"><a name="zh-cn_topic_0181281370_p764714115358"></a><a name="zh-cn_topic_0181281370_p764714115358"></a>连接类型不允许修改。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p1615561614269"><a name="p1615561614269"></a><a name="p1615561614269"></a>连接类型不允许修改。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p13768173110370"><a name="p13768173110370"></a><a name="p13768173110370"></a>请检查连接类型。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row6988556133214"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p178261439112613"><a name="p178261439112613"></a><a name="p178261439112613"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p1398582263210"><a name="zh-cn_topic_0181281370_p1398582263210"></a><a name="zh-cn_topic_0181281370_p1398582263210"></a>DLF.6416</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p29851223325"><a name="zh-cn_topic_0181281370_p29851223325"></a><a name="zh-cn_topic_0181281370_p29851223325"></a>集群已经被其他连接占用了。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p61551716102617"><a name="p61551716102617"></a><a name="p61551716102617"></a>集群已经被其他连接占用了。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p11739194914373"><a name="p11739194914373"></a><a name="p11739194914373"></a>请检查集群。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row013281012331"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p7826133932612"><a name="p7826133932612"></a><a name="p7826133932612"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p213210104331"><a name="zh-cn_topic_0181281370_p213210104331"></a><a name="zh-cn_topic_0181281370_p213210104331"></a>DLF.6418</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p0132101019335"><a name="zh-cn_topic_0181281370_p0132101019335"></a><a name="zh-cn_topic_0181281370_p0132101019335"></a>配置DWS集群名或者集群的访问地址、端口，两者二选一，不能都为空。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p7155181617264"><a name="p7155181617264"></a><a name="p7155181617264"></a>配置DWS集群名或者集群的访问地址、端口，两者二选一，不能都为空。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p0897259113711"><a name="p0897259113711"></a><a name="p0897259113711"></a>请检查集群DWS集群名或者集群的访问地址、端口。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281370_row2556123334615"><td class="cellrowborder" valign="top" width="9.080908090809082%" headers="mcps1.2.6.1.1 "><p id="p1582683919260"><a name="p1582683919260"></a><a name="p1582683919260"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="14.361436143614362%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0181281370_p1233618406466"><a name="zh-cn_topic_0181281370_p1233618406466"></a><a name="zh-cn_topic_0181281370_p1233618406466"></a>DLF.6888</p>
</td>
<td class="cellrowborder" valign="top" width="23.03230323032303%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0181281370_p13557103324614"><a name="zh-cn_topic_0181281370_p13557103324614"></a><a name="zh-cn_topic_0181281370_p13557103324614"></a>账户权限不合法。</p>
</td>
<td class="cellrowborder" valign="top" width="24.38243824382438%" headers="mcps1.2.6.1.4 "><p id="p4155151614263"><a name="p4155151614263"></a><a name="p4155151614263"></a>账户权限不合法。</p>
</td>
<td class="cellrowborder" valign="top" width="29.14291429142914%" headers="mcps1.2.6.1.5 "><p id="p985802812386"><a name="p985802812386"></a><a name="p985802812386"></a>请检查账户权限。</p>
</td>
</tr>
</tbody>
</table>

