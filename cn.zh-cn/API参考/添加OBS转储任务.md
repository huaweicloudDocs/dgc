# 添加OBS转储任务<a name="dis_02_0410"></a>

## 功能介绍<a name="section9940142115211"></a>

本接口用于添加OBS转储任务。

## 调试<a name="section49402210215"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=DIS&api=CreateObsTransferTask)中调试该接口。

## URI<a name="section69413212219"></a>

POST /v2/\{project\_id\}/streams/\{stream\_name\}/transfer-tasks

**表 1**  路径参数

<a name="table4942172116213"></a>
<table><thead align="left"><tr id="row194215211217"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p694312102110"><a name="p694312102110"></a><a name="p694312102110"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p199439219211"><a name="p199439219211"></a><a name="p199439219211"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p1994311217215"><a name="p1994311217215"></a><a name="p1994311217215"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p17943152142118"><a name="p17943152142118"></a><a name="p17943152142118"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1394222120214"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1594422102115"><a name="p1594422102115"></a><a name="p1594422102115"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p4944182112116"><a name="p4944182112116"></a><a name="p4944182112116"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p14944162115219"><a name="p14944162115219"></a><a name="p14944162115219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p394442113216"><a name="p394442113216"></a><a name="p394442113216"></a>项目ID。</p>
</td>
</tr>
<tr id="row15942122112210"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p20945122152115"><a name="p20945122152115"></a><a name="p20945122152115"></a>stream_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p11945152142110"><a name="p11945152142110"></a><a name="p11945152142110"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p694592113217"><a name="p694592113217"></a><a name="p694592113217"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p11945112110216"><a name="p11945112110216"></a><a name="p11945112110216"></a>已创建的通道名称。</p>
<p id="p13945112162112"><a name="p13945112162112"></a><a name="p13945112162112"></a>最大长度：<strong id="b14946221132119"><a name="b14946221132119"></a><a name="b14946221132119"></a>60</strong></p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section5946142115216"></a>

**表 2**  请求Header参数

<a name="HeaderParameter"></a>
<table><thead align="left"><tr id="row16946102117217"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p89471521142111"><a name="p89471521142111"></a><a name="p89471521142111"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p13947172122115"><a name="p13947172122115"></a><a name="p13947172122115"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p1594782182113"><a name="p1594782182113"></a><a name="p1594782182113"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p16948122122113"><a name="p16948122122113"></a><a name="p16948122122113"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row7946221192118"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p17948132112217"><a name="p17948132112217"></a><a name="p17948132112217"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p19481521172111"><a name="p19481521172111"></a><a name="p19481521172111"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p15948221122117"><a name="p15948221122117"></a><a name="p15948221122117"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p2948172162113"><a name="p2948172162113"></a><a name="p2948172162113"></a>用户Token。</p>
<p id="p2949921162113"><a name="p2949921162113"></a><a name="p2949921162113"></a>通过调用IAM服务获取用户Token接口获取（响应消息头中X-Subject-Token的值）。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  请求Body参数

<a name="requestParameter"></a>
<table><thead align="left"><tr id="row8949132162113"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p295032116219"><a name="p295032116219"></a><a name="p295032116219"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p995042112217"><a name="p995042112217"></a><a name="p995042112217"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p495012219214"><a name="p495012219214"></a><a name="p495012219214"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p1595012118217"><a name="p1595012118217"></a><a name="p1595012118217"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row694919218216"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p995132132117"><a name="p995132132117"></a><a name="p995132132117"></a>destination_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p89511021112114"><a name="p89511021112114"></a><a name="p89511021112114"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p3951122192110"><a name="p3951122192110"></a><a name="p3951122192110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p895210213214"><a name="p895210213214"></a><a name="p895210213214"></a>转储任务类型。</p>
<a name="ul17952122112217"></a><a name="ul17952122112217"></a><ul id="ul17952122112217"><li>OBS：转储到OBS</li><li>MRS：转储到MRS</li><li>DLI：转储到DLI</li><li>DWS：转储到DWS</li></ul>
<p id="p7953521132118"><a name="p7953521132118"></a><a name="p7953521132118"></a>缺省值：<strong id="b10953112192119"><a name="b10953112192119"></a><a name="b10953112192119"></a>NOWHERE</strong></p>
<p id="p99537211216"><a name="p99537211216"></a><a name="p99537211216"></a>枚举值：</p>
<a name="ul795311212213"></a><a name="ul795311212213"></a><ul id="ul795311212213"><li><strong id="b11954172118211"><a name="b11954172118211"></a><a name="b11954172118211"></a>OBS</strong></li></ul>
</td>
</tr>
<tr id="row1594972142110"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p49541621102113"><a name="p49541621102113"></a><a name="p49541621102113"></a>obs_destination_descriptor</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p9954721122114"><a name="p9954721122114"></a><a name="p9954721122114"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p39545214212"><a name="p39545214212"></a><a name="p39545214212"></a><a href="#request_OBSDestinationDescriptorRequest">OBSDestinationDescriptorRequest</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p14955162116211"><a name="p14955162116211"></a><a name="p14955162116211"></a>转储目的地为OBS的参数列表。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  OBSDestinationDescriptorRequest

<a name="request_OBSDestinationDescriptorRequest"></a>
<table><thead align="left"><tr id="row1695662119213"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p17958172111215"><a name="p17958172111215"></a><a name="p17958172111215"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p179589211210"><a name="p179589211210"></a><a name="p179589211210"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p495820213217"><a name="p495820213217"></a><a name="p495820213217"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p595912217217"><a name="p595912217217"></a><a name="p595912217217"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row19956112112217"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p99591821132112"><a name="p99591821132112"></a><a name="p99591821132112"></a>task_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p6959102115214"><a name="p6959102115214"></a><a name="p6959102115214"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1795992117213"><a name="p1795992117213"></a><a name="p1795992117213"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p16960921182115"><a name="p16960921182115"></a><a name="p16960921182115"></a>转储任务的名称。  任务名称由英文字母、数字、中划线和下划线组成。长度为1～64个字符。</p>
</td>
</tr>
<tr id="row6956721152118"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p149601821132119"><a name="p149601821132119"></a><a name="p149601821132119"></a>agency_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p15960132162110"><a name="p15960132162110"></a><a name="p15960132162110"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1961122112218"><a name="p1961122112218"></a><a name="p1961122112218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1396112142113"><a name="p1396112142113"></a><a name="p1396112142113"></a>在统一身份认证服务(IAM)中创建委托的名称，DIS需要获取IAM委托信息去访问您指定的资源。创建委托的参数设置如下：</p>
<a name="ul99621721182120"></a><a name="ul99621721182120"></a><ul id="ul99621721182120"><li>委托类型：云服务</li><li>云服务：DIS</li><li>持续时间：永久</li><li>“所属区域”为“全局服务”，“项目”为“对象存储服务”对应的“策略”包含“Tenant Administrator”。 如果已经创建过委托，可以使用IAM服务提供的<a href="https://support.huaweicloud.com/api-iam/iam_12_0001.html" target="_blank" rel="noopener noreferrer">查询委托列表</a>接口，获取有效可用的委托名称。 取值范围：长度不超过64位，且不可配置为空。</li></ul>
<p id="p7963162116210"><a name="p7963162116210"></a><a name="p7963162116210"></a>如果有在Console控制台使用转储任务，会提示自动创建委托，自动创建的委托名称为：dis_admin_agency</p>
<p id="p59631121172118"><a name="p59631121172118"></a><a name="p59631121172118"></a>最大长度：<strong id="b14963142192118"><a name="b14963142192118"></a><a name="b14963142192118"></a>64</strong></p>
</td>
</tr>
<tr id="row9956821152119"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1896382111215"><a name="p1896382111215"></a><a name="p1896382111215"></a>deliver_time_interval</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p496332116213"><a name="p496332116213"></a><a name="p496332116213"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1896417218215"><a name="p1896417218215"></a><a name="p1896417218215"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1896432120215"><a name="p1896432120215"></a><a name="p1896432120215"></a>根据用户配置的时间，周期性的将数据导入OBS，若某个时间段内无数据，则此时间段不会生成打包文件。</p>
<p id="p159644215219"><a name="p159644215219"></a><a name="p159644215219"></a>取值范围：30～900</p>
<p id="p496452119214"><a name="p496452119214"></a><a name="p496452119214"></a>缺省值：300</p>
<p id="p796419214216"><a name="p796419214216"></a><a name="p796419214216"></a>单位：秒</p>
<p id="p79645217210"><a name="p79645217210"></a><a name="p79645217210"></a>最小值：<strong id="b1896492113214"><a name="b1896492113214"></a><a name="b1896492113214"></a>30</strong></p>
<p id="p1096432112119"><a name="p1096432112119"></a><a name="p1096432112119"></a>最大值：<strong id="b1596402113214"><a name="b1596402113214"></a><a name="b1596402113214"></a>900</strong></p>
<p id="p14964821182115"><a name="p14964821182115"></a><a name="p14964821182115"></a>缺省值：<strong id="b20965112115217"><a name="b20965112115217"></a><a name="b20965112115217"></a>300</strong></p>
</td>
</tr>
<tr id="row179561721152116"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1496502142110"><a name="p1496502142110"></a><a name="p1496502142110"></a>consumer_strategy</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p49651721202113"><a name="p49651721202113"></a><a name="p49651721202113"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p159679215213"><a name="p159679215213"></a><a name="p159679215213"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p16967192182110"><a name="p16967192182110"></a><a name="p16967192182110"></a>偏移量。</p>
<a name="ul109673214216"></a><a name="ul109673214216"></a><ul id="ul109673214216"><li>LATEST：最大偏移量，即获取最新的数据。</li><li>TRIM_HORIZON：最小偏移量，即读取最早的数据。</li></ul>
<p id="p12967192116218"><a name="p12967192116218"></a><a name="p12967192116218"></a>缺省值：LATEST</p>
<p id="p16968122112213"><a name="p16968122112213"></a><a name="p16968122112213"></a>缺省值：<strong id="b3968192112218"><a name="b3968192112218"></a><a name="b3968192112218"></a>LATEST</strong></p>
<p id="p1496815215219"><a name="p1496815215219"></a><a name="p1496815215219"></a>枚举值：</p>
<a name="ul59683213212"></a><a name="ul59683213212"></a><ul id="ul59683213212"><li><strong id="b596816214217"><a name="b596816214217"></a><a name="b596816214217"></a>LATEST</strong></li><li><strong id="b1896811216211"><a name="b1896811216211"></a><a name="b1896811216211"></a>TRIM_HORIZON</strong></li></ul>
</td>
</tr>
<tr id="row17956721182116"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p296819212216"><a name="p296819212216"></a><a name="p296819212216"></a>file_prefix</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p49691121112117"><a name="p49691121112117"></a><a name="p49691121112117"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p159703212219"><a name="p159703212219"></a><a name="p159703212219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p3970021112114"><a name="p3970021112114"></a><a name="p3970021112114"></a>在OBS中存储通道文件的自定义目录，多级目录可用“/”进行分隔，不可以“/”开头。</p>
<p id="p3971182110214"><a name="p3971182110214"></a><a name="p3971182110214"></a>取值范围：英文字母、数字、下划线和斜杠，最大长度为50个字符。</p>
<p id="p179711921152114"><a name="p179711921152114"></a><a name="p179711921152114"></a>默认配置为空。</p>
<p id="p397152119211"><a name="p397152119211"></a><a name="p397152119211"></a>最大长度：<strong id="b897112172114"><a name="b897112172114"></a><a name="b897112172114"></a>50</strong></p>
</td>
</tr>
<tr id="row99561421142119"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p7971132132116"><a name="p7971132132116"></a><a name="p7971132132116"></a>partition_format</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p9971172142114"><a name="p9971172142114"></a><a name="p9971172142114"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p15971112112218"><a name="p15971112112218"></a><a name="p15971112112218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p99721621182115"><a name="p99721621182115"></a><a name="p99721621182115"></a>将转储文件的生成时间使用“yyyy/MM/dd/HH/mm”格式生成分区字符串，用来定义写到OBS的Object文件所在的目录层次结构。</p>
<a name="ul89721721132116"></a><a name="ul89721721132116"></a><ul id="ul89721721132116"><li>N/A：置空，不使用日期时间目录。</li><li>yyyy：年</li><li>yyyy/MM：年/</li><li>yyyy/MM/dd：年/月/日</li><li>yyyy/MM/dd/HH：年/月/日/时</li><li>yyyy/MM/dd/HH/mm：年/月/日/时/分</li></ul>
<p id="p10974121102112"><a name="p10974121102112"></a><a name="p10974121102112"></a>例如：2017/11/10/14/49，目录结构就是“2017 &gt; 11 &gt; 10 &gt; 14 &gt; 49”，“2017”表示最外层文件夹。</p>
<p id="p16974921152113"><a name="p16974921152113"></a><a name="p16974921152113"></a>默认值：空</p>
<p id="p16974921122120"><a name="p16974921122120"></a><a name="p16974921122120"></a>说明：</p>
<p id="p1697422172114"><a name="p1697422172114"></a><a name="p1697422172114"></a>数据转储成功后，存储的目录结构为“obs_bucket_path/file_prefix/partition_format”。</p>
<p id="p89748213210"><a name="p89748213210"></a><a name="p89748213210"></a>枚举值：</p>
<a name="ul1897492114219"></a><a name="ul1897492114219"></a><ul id="ul1897492114219"><li><strong id="b13975142114217"><a name="b13975142114217"></a><a name="b13975142114217"></a>yyyy</strong></li><li><strong id="b209759212217"><a name="b209759212217"></a><a name="b209759212217"></a>yyyy/MM</strong></li><li><strong id="b15976192152119"><a name="b15976192152119"></a><a name="b15976192152119"></a>yyyy/MM/dd</strong></li><li><strong id="b297615212215"><a name="b297615212215"></a><a name="b297615212215"></a>yyyy/MM/dd/HH</strong></li><li><strong id="b797642115218"><a name="b797642115218"></a><a name="b797642115218"></a>yyyy/MM/dd/HH/mm</strong></li></ul>
</td>
</tr>
<tr id="row195722117217"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p797792112117"><a name="p797792112117"></a><a name="p797792112117"></a>obs_bucket_path</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p797722102111"><a name="p797722102111"></a><a name="p797722102111"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p297712114217"><a name="p297712114217"></a><a name="p297712114217"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p179771021162116"><a name="p179771021162116"></a><a name="p179771021162116"></a>存储该通道数据的OBS桶名称。</p>
</td>
</tr>
<tr id="row6957132116219"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p19979921162120"><a name="p19979921162120"></a><a name="p19979921162120"></a>destination_file_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1997972132119"><a name="p1997972132119"></a><a name="p1997972132119"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p18979132182110"><a name="p18979132182110"></a><a name="p18979132182110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p398082120217"><a name="p398082120217"></a><a name="p398082120217"></a>转储文件格式。</p>
<a name="ul10980152162118"></a><a name="ul10980152162118"></a><ul id="ul10980152162118"><li>text：转储目标格式为TEXT，缺省值</li><li>parquet：转储目标格式为Parquet</li><li>carbon：转储目标格式为Carbon</li></ul>
<p id="p998119217219"><a name="p998119217219"></a><a name="p998119217219"></a>说明：</p>
<p id="p6981421162117"><a name="p6981421162117"></a><a name="p6981421162117"></a>“源数据类型”为“JSON”，“转储服务类型”为“OBS”时才可选择“parquet”或“carbon”格式。</p>
<p id="p89811121152111"><a name="p89811121152111"></a><a name="p89811121152111"></a>缺省值：<strong id="b3981621202112"><a name="b3981621202112"></a><a name="b3981621202112"></a>text</strong></p>
<p id="p1598116217211"><a name="p1598116217211"></a><a name="p1598116217211"></a>枚举值：</p>
<a name="ul3982421112116"></a><a name="ul3982421112116"></a><ul id="ul3982421112116"><li><strong id="b7982192113219"><a name="b7982192113219"></a><a name="b7982192113219"></a>text</strong></li><li><strong id="b14982112117213"><a name="b14982112117213"></a><a name="b14982112117213"></a>parquet</strong></li><li><strong id="b1098222172114"><a name="b1098222172114"></a><a name="b1098222172114"></a>carbon</strong></li></ul>
</td>
</tr>
<tr id="row17957192120212"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p59822216215"><a name="p59822216215"></a><a name="p59822216215"></a>processing_schema</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p16983142192115"><a name="p16983142192115"></a><a name="p16983142192115"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p16983202110216"><a name="p16983202110216"></a><a name="p16983202110216"></a><a href="#request_ProcessingSchema">ProcessingSchema</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p109834214212"><a name="p109834214212"></a><a name="p109834214212"></a>根据源数据的时间戳和已配置的"partition_format"生成对应的转储时间目录。将源数据的时间戳使用“yyyy/MM/dd/HH/mm”格式生成分区字符串，用来定义写到OBS的Object文件所在的目录层次结构。</p>
</td>
</tr>
<tr id="row49572021192110"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1498518217213"><a name="p1498518217213"></a><a name="p1498518217213"></a>record_delimiter</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p16985102182118"><a name="p16985102182118"></a><a name="p16985102182118"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1986421132117"><a name="p1986421132117"></a><a name="p1986421132117"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p49865219213"><a name="p49865219213"></a><a name="p49865219213"></a>转储文件的记录分隔符，用于分隔写入转储文件的用户数据。</p>
<p id="p19986142152112"><a name="p19986142152112"></a><a name="p19986142152112"></a>取值范围：</p>
<a name="ul5986421142112"></a><a name="ul5986421142112"></a><ul id="ul5986421142112"><li>逗号 ","，默认值</li><li>分号 ";"</li><li>竖线 "|"</li><li>换行符 "\n"</li></ul>
<p id="p1498882113216"><a name="p1498882113216"></a><a name="p1498882113216"></a>缺省值：<strong id="b1298872112119"><a name="b1298872112119"></a><a name="b1298872112119"></a>\n</strong></p>
</td>
</tr>
</tbody>
</table>

**表 5**  ProcessingSchema

<a name="request_ProcessingSchema"></a>
<table><thead align="left"><tr id="row79891211214"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p1199112114210"><a name="p1199112114210"></a><a name="p1199112114210"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p1399212217213"><a name="p1399212217213"></a><a name="p1399212217213"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p17992122112119"><a name="p17992122112119"></a><a name="p17992122112119"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p1099352122119"><a name="p1099352122119"></a><a name="p1099352122119"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row398982119212"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p399322117212"><a name="p399322117212"></a><a name="p399322117212"></a>timestamp_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1993192117213"><a name="p1993192117213"></a><a name="p1993192117213"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p189943215219"><a name="p189943215219"></a><a name="p189943215219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1699413215216"><a name="p1699413215216"></a><a name="p1699413215216"></a>源数据时间戳的属性名称。</p>
</td>
</tr>
<tr id="row599062119213"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p189941821142120"><a name="p189941821142120"></a><a name="p189941821142120"></a>timestamp_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p599416210219"><a name="p599416210219"></a><a name="p599416210219"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1099419215210"><a name="p1099419215210"></a><a name="p1099419215210"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p14994152132115"><a name="p14994152132115"></a><a name="p14994152132115"></a>源数据时间戳的类型。</p>
<a name="ul9995162152116"></a><a name="ul9995162152116"></a><ul id="ul9995162152116"><li>String</li><li>Timestamp：Long类型的13位时间戳</li></ul>
</td>
</tr>
<tr id="row1599052119218"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p13996182132119"><a name="p13996182132119"></a><a name="p13996182132119"></a>timestamp_format</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p6996152113215"><a name="p6996152113215"></a><a name="p6996152113215"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p49961421162111"><a name="p49961421162111"></a><a name="p49961421162111"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p399642114212"><a name="p399642114212"></a><a name="p399642114212"></a>源数据时间戳的类型为String时必选，用于根据时间戳格式生成OBS的时间目录。</p>
<p id="p17997921102117"><a name="p17997921102117"></a><a name="p17997921102117"></a>取值范围：</p>
<a name="ul49971321162113"></a><a name="ul49971321162113"></a><ul id="ul49971321162113"><li>yyyy/MM/dd HH:mm:ss</li><li>MM/dd/yyyy HH:mm:ss</li><li>dd/MM/yyyy HH:mm:ss</li><li>yyyy-MM-dd HH:mm:ss</li><li>MM-dd-yyyy HH:mm:ss</li><li>dd-MM-yyyy HH:mm:ss</li></ul>
<p id="p199812118219"><a name="p199812118219"></a><a name="p199812118219"></a>枚举值：</p>
<a name="ul79981021132120"></a><a name="ul79981021132120"></a><ul id="ul79981021132120"><li><strong id="b5999172113215"><a name="b5999172113215"></a><a name="b5999172113215"></a>yyyy/MM/dd HH:mm:ss</strong></li><li><strong id="b89997219211"><a name="b89997219211"></a><a name="b89997219211"></a>MM/dd/yyyy HH:mm:ss</strong></li><li><strong id="b1199912114219"><a name="b1199912114219"></a><a name="b1199912114219"></a>dd/MM/yyyy HH:mm:ss</strong></li><li><strong id="b799919212215"><a name="b799919212215"></a><a name="b799919212215"></a>yyyy-MM-dd HH:mm:ss</strong></li><li><strong id="b1399962142111"><a name="b1399962142111"></a><a name="b1399962142111"></a>MM-dd-yyyy HH:mm:ss</strong></li><li><strong id="b19991212217"><a name="b19991212217"></a><a name="b19991212217"></a>dd-MM-yyyy HH:mm:ss</strong></li></ul>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section11999421162114"></a>

无

## 请求示例<a name="section16052272119"></a>

-   添加OBS转储任务

    ```
    POST https://{Endpoint}/v2/{project_id}/streams/{stream_name}/transfer-tasks
    
    {
      "destination_type" : "OBS",
      "obs_destination_descriptor" : {
        "task_name" : "newtask",
        "consumer_strategy" : "LATEST",
        "agency_name" : "dis_admin_agency",
        "destination_file_type" : "text",
        "obs_bucket_path" : "obsbucket",
        "file_prefix" : "",
        "partition_format" : "yyyy/MM/dd/HH/mm",
        "record_delimiter" : "|",
        "deliver_time_interval" : 30
      }
    }
    ```

-   添加OBS转储任务（转储文件格式是parquet）

    ```
    POST https://{Endpoint}/v2/{project_id}/streams/{stream_name}/transfer-tasks
    
    {
      "destination_type" : "OBS",
      "obs_destination_descriptor" : {
        "task_name" : "newtask",
        "consumer_strategy" : "LATEST",
        "agency_name" : "dis_admin_agency",
        "destination_file_type" : "parquet",
        "obs_bucket_path" : "obsbucket",
        "file_prefix" : "",
        "partition_format" : "yyyy/MM/dd/HH/mm",
        "record_delimiter" : "|",
        "deliver_time_interval" : 30
      }
    }
    ```


## 响应示例<a name="section132215225213"></a>

无

## 状态码<a name="section7322102272117"></a>

<a name="status_code"></a>
<table><thead align="left"><tr id="row13510222219"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p183221522112113"><a name="p183221522112113"></a><a name="p183221522112113"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p432232211210"><a name="p432232211210"></a><a name="p432232211210"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row7582217217"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p9322322172116"><a name="p9322322172116"></a><a name="p9322322172116"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p19322522142118"><a name="p19322522142118"></a><a name="p19322522142118"></a>正常返回</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section0323322142114"></a>

请参见[错误码](错误码.md)。

