# 添加DLI转储任务<a name="CreateDliTransferTask"></a>

## 功能介绍<a name="section168071639143212"></a>

本接口用于添加DLI转储任务。

## 调试<a name="section8811143916327"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=DIS&api=CreateDliTransferTask)中调试该接口。

## URI<a name="section081753983213"></a>

POST /v2/\{project\_id\}/streams/\{stream\_name\}/transfer-tasks

**表 1**  路径参数

<a name="table19826163923214"></a>
<table><thead align="left"><tr id="row1982333913211"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p182893973213"><a name="p182893973213"></a><a name="p182893973213"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p983163903216"><a name="p983163903216"></a><a name="p983163903216"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p683363916326"><a name="p683363916326"></a><a name="p683363916326"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p1783517393327"><a name="p1783517393327"></a><a name="p1783517393327"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row882353913213"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1983723917325"><a name="p1983723917325"></a><a name="p1983723917325"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p138401539153210"><a name="p138401539153210"></a><a name="p138401539153210"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p3842163923218"><a name="p3842163923218"></a><a name="p3842163923218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p28453398323"><a name="p28453398323"></a><a name="p28453398323"></a>项目ID。</p>
</td>
</tr>
<tr id="row1082303917326"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p684815398323"><a name="p684815398323"></a><a name="p684815398323"></a>stream_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p158511239153218"><a name="p158511239153218"></a><a name="p158511239153218"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p68531839153213"><a name="p68531839153213"></a><a name="p68531839153213"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p985543993219"><a name="p985543993219"></a><a name="p985543993219"></a>已创建的通道名称。</p>
<p id="p2085810399326"><a name="p2085810399326"></a><a name="p2085810399326"></a>最大长度：<strong id="b16859193993215"><a name="b16859193993215"></a><a name="b16859193993215"></a>60</strong></p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section1386217398329"></a>

**表 2**  请求Header参数

<a name="HeaderParameter"></a>
<table><thead align="left"><tr id="row148659399328"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p20868163919324"><a name="p20868163919324"></a><a name="p20868163919324"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p8871239123215"><a name="p8871239123215"></a><a name="p8871239123215"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p1587373919321"><a name="p1587373919321"></a><a name="p1587373919321"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p48759397324"><a name="p48759397324"></a><a name="p48759397324"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row7865839153215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p8878203918321"><a name="p8878203918321"></a><a name="p8878203918321"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p118811139163219"><a name="p118811139163219"></a><a name="p118811139163219"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p148831339193214"><a name="p148831339193214"></a><a name="p148831339193214"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p0885133914325"><a name="p0885133914325"></a><a name="p0885133914325"></a>用户Token。</p>
<p id="p12887113913323"><a name="p12887113913323"></a><a name="p12887113913323"></a>通过调用IAM服务获取用户Token接口获取（响应消息头中X-Subject-Token的值）。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  请求Body参数

<a name="requestParameter"></a>
<table><thead align="left"><tr id="row2088943918321"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p12892153915322"><a name="p12892153915322"></a><a name="p12892153915322"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p1289512393328"><a name="p1289512393328"></a><a name="p1289512393328"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p138981539153216"><a name="p138981539153216"></a><a name="p138981539153216"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p159001439113211"><a name="p159001439113211"></a><a name="p159001439113211"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row68892399321"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1890243913212"><a name="p1890243913212"></a><a name="p1890243913212"></a>destination_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p5904939193218"><a name="p5904939193218"></a><a name="p5904939193218"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1090619395326"><a name="p1090619395326"></a><a name="p1090619395326"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1390883919321"><a name="p1390883919321"></a><a name="p1390883919321"></a>转储任务类型。</p>
<a name="ul1391173912329"></a><a name="ul1391173912329"></a><ul id="ul1391173912329"><li>OBS：转储到OBS</li><li>MRS：转储到MRS</li><li>DLI：转储到DLI</li><li>DWS：转储到DWS</li></ul>
<p id="p1492615393329"><a name="p1492615393329"></a><a name="p1492615393329"></a>缺省值：<strong id="b19927173912325"><a name="b19927173912325"></a><a name="b19927173912325"></a>NOWHERE</strong></p>
<p id="p15928123914325"><a name="p15928123914325"></a><a name="p15928123914325"></a>枚举值：</p>
<a name="ul2930173963214"></a><a name="ul2930173963214"></a><ul id="ul2930173963214"><li><strong id="b0933183983220"><a name="b0933183983220"></a><a name="b0933183983220"></a>DLI</strong></li></ul>
</td>
</tr>
<tr id="row788913943218"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p59341439163217"><a name="p59341439163217"></a><a name="p59341439163217"></a>dli_destination_descriptor</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p15936103993210"><a name="p15936103993210"></a><a name="p15936103993210"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p693910399322"><a name="p693910399322"></a><a name="p693910399322"></a><a href="#request_DliDestinationDescriptorRequest">DliDestinationDescriptorRequest</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p794293918326"><a name="p794293918326"></a><a name="p794293918326"></a>转储目的地为DLI的参数列表。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  DliDestinationDescriptorRequest

<a name="request_DliDestinationDescriptorRequest"></a>
<table><thead align="left"><tr id="row194713395322"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p195114399328"><a name="p195114399328"></a><a name="p195114399328"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p12953739153217"><a name="p12953739153217"></a><a name="p12953739153217"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p10955193963214"><a name="p10955193963214"></a><a name="p10955193963214"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p9958203918326"><a name="p9958203918326"></a><a name="p9958203918326"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1094753919322"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p296053943216"><a name="p296053943216"></a><a name="p296053943216"></a>task_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p13962113943215"><a name="p13962113943215"></a><a name="p13962113943215"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p14964193917321"><a name="p14964193917321"></a><a name="p14964193917321"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p5967103913215"><a name="p5967103913215"></a><a name="p5967103913215"></a>转储任务的名称。  任务名称由英文字母、数字、中划线和下划线组成。长度为1～64个字符。</p>
</td>
</tr>
<tr id="row794743914322"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p10969139153219"><a name="p10969139153219"></a><a name="p10969139153219"></a>agency_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p17971239193210"><a name="p17971239193210"></a><a name="p17971239193210"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p6974203943218"><a name="p6974203943218"></a><a name="p6974203943218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p39771539173213"><a name="p39771539173213"></a><a name="p39771539173213"></a>在统一身份认证服务(IAM)中创建委托的名称，DIS需要获取IAM委托信息去访问您指定的资源。创建委托的参数设置如下：</p>
<a name="ul19980239193220"></a><a name="ul19980239193220"></a><ul id="ul19980239193220"><li>委托类型：云服务</li><li>云服务：DIS</li><li>持续时间：永久</li><li>“所属区域”为“全局服务”，“项目”为“对象存储服务”对应的“策略”包含“Tenant Administrator”。 如果已经创建过委托，可以使用IAM服务提供的<a href="https://support.huaweicloud.com/api-iam/iam_12_0001.html" target="_blank" rel="noopener noreferrer">查询委托列表</a>接口，获取有效可用的委托名称。 取值范围：长度不超过64位，且不可配置为空。</li></ul>
<p id="p199143917327"><a name="p199143917327"></a><a name="p199143917327"></a>如果有在Console控制台使用转储任务，会提示自动创建委托，自动创建的委托名称为：dis_admin_agency</p>
<p id="p17993639133213"><a name="p17993639133213"></a><a name="p17993639133213"></a>最大长度：<strong id="b6994103913320"><a name="b6994103913320"></a><a name="b6994103913320"></a>64</strong></p>
</td>
</tr>
<tr id="row09473392324"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p999623918326"><a name="p999623918326"></a><a name="p999623918326"></a>deliver_time_interval</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p14998113903214"><a name="p14998113903214"></a><a name="p14998113903214"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1518405326"><a name="p1518405326"></a><a name="p1518405326"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1541040153211"><a name="p1541040153211"></a><a name="p1541040153211"></a>根据用户配置的时间，周期性的将数据导入OBS，若某个时间段内无数据，则此时间段不会生成打包文件。</p>
<p id="p5718400325"><a name="p5718400325"></a><a name="p5718400325"></a>取值范围：30～900</p>
<p id="p189114012323"><a name="p189114012323"></a><a name="p189114012323"></a>缺省值：300</p>
<p id="p131020409326"><a name="p131020409326"></a><a name="p131020409326"></a>单位：秒</p>
<p id="p21384083220"><a name="p21384083220"></a><a name="p21384083220"></a>最小值：<strong id="b91484053218"><a name="b91484053218"></a><a name="b91484053218"></a>30</strong></p>
<p id="p1916184018326"><a name="p1916184018326"></a><a name="p1916184018326"></a>最大值：<strong id="b1317164093220"><a name="b1317164093220"></a><a name="b1317164093220"></a>900</strong></p>
<p id="p618154018322"><a name="p618154018322"></a><a name="p618154018322"></a>缺省值：<strong id="b319144015325"><a name="b319144015325"></a><a name="b319144015325"></a>300</strong></p>
</td>
</tr>
<tr id="row109476393320"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p18212040153219"><a name="p18212040153219"></a><a name="p18212040153219"></a>consumer_strategy</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1923164073219"><a name="p1923164073219"></a><a name="p1923164073219"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p10261040163218"><a name="p10261040163218"></a><a name="p10261040163218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1630184016322"><a name="p1630184016322"></a><a name="p1630184016322"></a>偏移量。</p>
<a name="ul232114018327"></a><a name="ul232114018327"></a><ul id="ul232114018327"><li>LATEST：最大偏移量，即获取最新的数据。</li><li>TRIM_HORIZON：最小偏移量，即读取最早的数据。</li></ul>
<p id="p0361401320"><a name="p0361401320"></a><a name="p0361401320"></a>缺省值：LATEST</p>
<p id="p638540123220"><a name="p638540123220"></a><a name="p638540123220"></a>缺省值：<strong id="b10400403323"><a name="b10400403323"></a><a name="b10400403323"></a>LATEST</strong></p>
<p id="p841104023213"><a name="p841104023213"></a><a name="p841104023213"></a>枚举值：</p>
<a name="ul7431040133218"></a><a name="ul7431040133218"></a><ul id="ul7431040133218"><li><strong id="b154504033211"><a name="b154504033211"></a><a name="b154504033211"></a>LATEST</strong></li><li><strong id="b148144011329"><a name="b148144011329"></a><a name="b148144011329"></a>TRIM_HORIZON</strong></li></ul>
</td>
</tr>
<tr id="row4947133910327"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p135017407327"><a name="p135017407327"></a><a name="p135017407327"></a>dli_database_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p195214063219"><a name="p195214063219"></a><a name="p195214063219"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p17541940103216"><a name="p17541940103216"></a><a name="p17541940103216"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p35744043220"><a name="p35744043220"></a><a name="p35744043220"></a>存储该通道数据的DLI数据库名称。</p>
</td>
</tr>
<tr id="row29471139143214"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p160164023213"><a name="p160164023213"></a><a name="p160164023213"></a>dli_table_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p362840113216"><a name="p362840113216"></a><a name="p362840113216"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p196514015329"><a name="p196514015329"></a><a name="p196514015329"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1469194023211"><a name="p1469194023211"></a><a name="p1469194023211"></a>存储该通道数据的DLI表名称。</p>
<p id="p271184093215"><a name="p271184093215"></a><a name="p271184093215"></a>说明：</p>
<p id="p1173114010326"><a name="p1173114010326"></a><a name="p1173114010326"></a>仅支持数据位置为DLI的表，且用户需具有该表的插入权限。</p>
</td>
</tr>
<tr id="row20947183913320"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p47516405325"><a name="p47516405325"></a><a name="p47516405325"></a>obs_bucket_path</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p978144093211"><a name="p978144093211"></a><a name="p978144093211"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p18111408322"><a name="p18111408322"></a><a name="p18111408322"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p984194013210"><a name="p984194013210"></a><a name="p984194013210"></a>临时存储该通道数据的OBS桶名称。</p>
</td>
</tr>
<tr id="row0948639163213"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p11861640133220"><a name="p11861640133220"></a><a name="p11861640133220"></a>file_prefix</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p168864063211"><a name="p168864063211"></a><a name="p168864063211"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p19115407327"><a name="p19115407327"></a><a name="p19115407327"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p79519401326"><a name="p79519401326"></a><a name="p79519401326"></a>临时存储该通道数据的OBS桶下的自定义目录，多级目录可用“/”进行分隔，不可以“/”开头。</p>
<p id="p1497340113211"><a name="p1497340113211"></a><a name="p1497340113211"></a>取值范围：英文字母、数字、下划线和斜杠，最大长度为50个字符。</p>
<p id="p1299134018327"><a name="p1299134018327"></a><a name="p1299134018327"></a>默认配置为空。</p>
</td>
</tr>
<tr id="row2948123910325"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p0101340123215"><a name="p0101340123215"></a><a name="p0101340123215"></a>retry_duration</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p810434016323"><a name="p810434016323"></a><a name="p810434016323"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p121071640143219"><a name="p121071640143219"></a><a name="p121071640143219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p21108408329"><a name="p21108408329"></a><a name="p21108408329"></a>用户数据导入DLI失败的失效重试时间。重试时间超过该配置项配置的值，则将转储失败的数据备份至“OBS桶/ file_prefix/dli_error”目录下。 取值范围：0~7200。 单位：秒。 默认配置为1800。 配置为“0”表示DIS服务不会在转储失败时进行重试。</p>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section4112540143216"></a>

无

## 请求示例<a name="section16117144023210"></a>

无

## 响应示例<a name="section8122840133215"></a>

无

## 状态码<a name="section81261340173216"></a>

<a name="status_code"></a>
<table><thead align="left"><tr id="row112913407326"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p51311940173210"><a name="p51311940173210"></a><a name="p51311940173210"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p513319404328"><a name="p513319404328"></a><a name="p513319404328"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1912954012329"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p11135440153210"><a name="p11135440153210"></a><a name="p11135440153210"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p16138440113213"><a name="p16138440113213"></a><a name="p16138440113213"></a>正常返回</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section1414054011325"></a>

请参见[错误码](错误码.md)。

