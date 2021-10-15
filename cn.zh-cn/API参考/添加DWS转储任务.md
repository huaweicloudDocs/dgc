# 添加DWS转储任务<a name="CreateDwsTransferTask"></a>

## 功能介绍<a name="section9938202219211"></a>

本接口用于添加DWS转储任务。

## 调试<a name="section1093942292115"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=DIS&api=CreateDwsTransferTask)中调试该接口。

## URI<a name="section794012225216"></a>

POST /v2/\{project\_id\}/streams/\{stream\_name\}/transfer-tasks

**表 1**  路径参数

<a name="table5942222122119"></a>
<table><thead align="left"><tr id="row179419228218"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p99421222192114"><a name="p99421222192114"></a><a name="p99421222192114"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p7943322202116"><a name="p7943322202116"></a><a name="p7943322202116"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p794322212214"><a name="p794322212214"></a><a name="p794322212214"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p6943822102110"><a name="p6943822102110"></a><a name="p6943822102110"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row594182212114"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1944122192119"><a name="p1944122192119"></a><a name="p1944122192119"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p8944172218219"><a name="p8944172218219"></a><a name="p8944172218219"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p494512220214"><a name="p494512220214"></a><a name="p494512220214"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p3945162242116"><a name="p3945162242116"></a><a name="p3945162242116"></a>项目ID。</p>
</td>
</tr>
<tr id="row1994172252117"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p10945622172114"><a name="p10945622172114"></a><a name="p10945622172114"></a>stream_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p194672218216"><a name="p194672218216"></a><a name="p194672218216"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p19946182292120"><a name="p19946182292120"></a><a name="p19946182292120"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1194652214211"><a name="p1194652214211"></a><a name="p1194652214211"></a>已创建的通道名称。</p>
<p id="p149482022122119"><a name="p149482022122119"></a><a name="p149482022122119"></a>最大长度：<strong id="b1948182218215"><a name="b1948182218215"></a><a name="b1948182218215"></a>60</strong></p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section14949152202116"></a>

**表 2**  请求Header参数

<a name="HeaderParameter"></a>
<table><thead align="left"><tr id="row095002219213"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p189511122122111"><a name="p189511122122111"></a><a name="p189511122122111"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p5951622152117"><a name="p5951622152117"></a><a name="p5951622152117"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p6952162214213"><a name="p6952162214213"></a><a name="p6952162214213"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p395282214215"><a name="p395282214215"></a><a name="p395282214215"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row29501322182114"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1795302202114"><a name="p1795302202114"></a><a name="p1795302202114"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p11954122219216"><a name="p11954122219216"></a><a name="p11954122219216"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p39541422122116"><a name="p39541422122116"></a><a name="p39541422122116"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p4955422102120"><a name="p4955422102120"></a><a name="p4955422102120"></a>用户Token。</p>
<p id="p13955142219214"><a name="p13955142219214"></a><a name="p13955142219214"></a>通过调用IAM服务获取用户Token接口获取（响应消息头中X-Subject-Token的值）。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  请求Body参数

<a name="requestParameter"></a>
<table><thead align="left"><tr id="row1895612217212"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p295732252115"><a name="p295732252115"></a><a name="p295732252115"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p995832217215"><a name="p995832217215"></a><a name="p995832217215"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p13958102212215"><a name="p13958102212215"></a><a name="p13958102212215"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p1959162214210"><a name="p1959162214210"></a><a name="p1959162214210"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row79561822182112"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1795962222116"><a name="p1795962222116"></a><a name="p1795962222116"></a>destination_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1496016224215"><a name="p1496016224215"></a><a name="p1496016224215"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1961522102120"><a name="p1961522102120"></a><a name="p1961522102120"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p89619229215"><a name="p89619229215"></a><a name="p89619229215"></a>转储任务类型。</p>
<a name="ul14962202272111"></a><a name="ul14962202272111"></a><ul id="ul14962202272111"><li>OBS：转储到OBS</li><li>MRS：转储到MRS</li><li>DLI：转储到DLI</li><li>DWS：转储到DWS</li></ul>
<p id="p169644221213"><a name="p169644221213"></a><a name="p169644221213"></a>缺省值：<strong id="b11964112218212"><a name="b11964112218212"></a><a name="b11964112218212"></a>NOWHERE</strong></p>
<p id="p159658228216"><a name="p159658228216"></a><a name="p159658228216"></a>枚举值：</p>
<a name="ul89661722122115"></a><a name="ul89661722122115"></a><ul id="ul89661722122115"><li><strong id="b1296717223214"><a name="b1296717223214"></a><a name="b1296717223214"></a>DWS</strong></li></ul>
</td>
</tr>
<tr id="row119561122142114"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p496782219213"><a name="p496782219213"></a><a name="p496782219213"></a>dws_destination_descriptor</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p596842219217"><a name="p596842219217"></a><a name="p596842219217"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p109685225219"><a name="p109685225219"></a><a name="p109685225219"></a><a href="#request_DWSDestinationDescriptorRequest">DWSDestinationDescriptorRequest</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p18969102219219"><a name="p18969102219219"></a><a name="p18969102219219"></a>转储目的地为DWS的参数列表。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  DWSDestinationDescriptorRequest

<a name="request_DWSDestinationDescriptorRequest"></a>
<table><thead align="left"><tr id="row10971102272112"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p159731522102119"><a name="p159731522102119"></a><a name="p159731522102119"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p1997542215218"><a name="p1997542215218"></a><a name="p1997542215218"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p1697615220214"><a name="p1697615220214"></a><a name="p1697615220214"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p159762225210"><a name="p159762225210"></a><a name="p159762225210"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row197117228217"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p09761322202110"><a name="p09761322202110"></a><a name="p09761322202110"></a>task_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p7977322132119"><a name="p7977322132119"></a><a name="p7977322132119"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p14977182262110"><a name="p14977182262110"></a><a name="p14977182262110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p6978322112119"><a name="p6978322112119"></a><a name="p6978322112119"></a>转储任务的名称。  任务名称由英文字母、数字、中划线和下划线组成。长度为1～64个字符。</p>
</td>
</tr>
<tr id="row1397132222118"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p20978142272117"><a name="p20978142272117"></a><a name="p20978142272117"></a>agency_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1997912219213"><a name="p1997912219213"></a><a name="p1997912219213"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p17979142262115"><a name="p17979142262115"></a><a name="p17979142262115"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p10980142218211"><a name="p10980142218211"></a><a name="p10980142218211"></a>在统一身份认证服务(IAM)中创建委托的名称，DIS需要获取IAM委托信息去访问您指定的资源。创建委托的参数设置如下：</p>
<a name="ul698062213215"></a><a name="ul698062213215"></a><ul id="ul698062213215"><li>委托类型：云服务</li><li>云服务：DIS</li><li>持续时间：永久</li><li>“所属区域”为“全局服务”，“项目”为“对象存储服务”对应的“策略”包含“Tenant Administrator”。 如果已经创建过委托，可以使用IAM服务提供的<a href="https://support.huaweicloud.com/api-iam/iam_12_0001.html" target="_blank" rel="noopener noreferrer">查询委托列表</a>接口，获取有效可用的委托名称。 取值范围：长度不超过64位，且不可配置为空。</li></ul>
<p id="p17983182215216"><a name="p17983182215216"></a><a name="p17983182215216"></a>如果有在Console控制台使用转储任务，会提示自动创建委托，自动创建的委托名称为：dis_admin_agency</p>
<p id="p13983112217218"><a name="p13983112217218"></a><a name="p13983112217218"></a>最大长度：<strong id="b2983152282111"><a name="b2983152282111"></a><a name="b2983152282111"></a>64</strong></p>
</td>
</tr>
<tr id="row497112213210"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p3983192220215"><a name="p3983192220215"></a><a name="p3983192220215"></a>deliver_time_interval</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p498419222218"><a name="p498419222218"></a><a name="p498419222218"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p398452212113"><a name="p398452212113"></a><a name="p398452212113"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1985102222114"><a name="p1985102222114"></a><a name="p1985102222114"></a>根据用户配置的时间，周期性的将数据导入OBS，若某个时间段内无数据，则此时间段不会生成打包文件。</p>
<p id="p129854225218"><a name="p129854225218"></a><a name="p129854225218"></a>取值范围：30～900</p>
<p id="p19986162252118"><a name="p19986162252118"></a><a name="p19986162252118"></a>缺省值：300</p>
<p id="p11986202212218"><a name="p11986202212218"></a><a name="p11986202212218"></a>单位：秒</p>
<p id="p10986162212111"><a name="p10986162212111"></a><a name="p10986162212111"></a>最小值：<strong id="b1198712210217"><a name="b1198712210217"></a><a name="b1198712210217"></a>30</strong></p>
<p id="p14987142222113"><a name="p14987142222113"></a><a name="p14987142222113"></a>最大值：<strong id="b1987122122119"><a name="b1987122122119"></a><a name="b1987122122119"></a>900</strong></p>
<p id="p10987222142119"><a name="p10987222142119"></a><a name="p10987222142119"></a>缺省值：<strong id="b7987622142120"><a name="b7987622142120"></a><a name="b7987622142120"></a>300</strong></p>
</td>
</tr>
<tr id="row10971182220219"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1698816221212"><a name="p1698816221212"></a><a name="p1698816221212"></a>consumer_strategy</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p17988722132117"><a name="p17988722132117"></a><a name="p17988722132117"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p6989152216218"><a name="p6989152216218"></a><a name="p6989152216218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1898916226219"><a name="p1898916226219"></a><a name="p1898916226219"></a>偏移量。</p>
<a name="ul59901522202111"></a><a name="ul59901522202111"></a><ul id="ul59901522202111"><li>LATEST：最大偏移量，即获取最新的数据。</li><li>TRIM_HORIZON：最小偏移量，即读取最早的数据。</li></ul>
<p id="p15991622102110"><a name="p15991622102110"></a><a name="p15991622102110"></a>缺省值：LATEST</p>
<p id="p1999112218210"><a name="p1999112218210"></a><a name="p1999112218210"></a>缺省值：<strong id="b1991122212118"><a name="b1991122212118"></a><a name="b1991122212118"></a>LATEST</strong></p>
<p id="p1999142210214"><a name="p1999142210214"></a><a name="p1999142210214"></a>枚举值：</p>
<a name="ul49921222202119"></a><a name="ul49921222202119"></a><ul id="ul49921222202119"><li><strong id="b4992182219216"><a name="b4992182219216"></a><a name="b4992182219216"></a>LATEST</strong></li><li><strong id="b139931322142116"><a name="b139931322142116"></a><a name="b139931322142116"></a>TRIM_HORIZON</strong></li></ul>
</td>
</tr>
<tr id="row16971202212214"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p899322272110"><a name="p899322272110"></a><a name="p899322272110"></a>dws_cluster_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1299322210219"><a name="p1299322210219"></a><a name="p1299322210219"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p7994182217216"><a name="p7994182217216"></a><a name="p7994182217216"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1099472219212"><a name="p1099472219212"></a><a name="p1099472219212"></a>存储该通道数据的DWS集群名称。</p>
</td>
</tr>
<tr id="row6971322112113"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p139951622102111"><a name="p139951622102111"></a><a name="p139951622102111"></a>dws_cluster_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p11995422102119"><a name="p11995422102119"></a><a name="p11995422102119"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p15996102217218"><a name="p15996102217218"></a><a name="p15996102217218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p299622211213"><a name="p299622211213"></a><a name="p299622211213"></a>存储该通道数据的DWS集群ID。</p>
</td>
</tr>
<tr id="row1797216226214"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p799642222114"><a name="p799642222114"></a><a name="p799642222114"></a>dws_database_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p7997132212112"><a name="p7997132212112"></a><a name="p7997132212112"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1899822232117"><a name="p1899822232117"></a><a name="p1899822232117"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1199852219217"><a name="p1199852219217"></a><a name="p1199852219217"></a>存储该通道数据的DWS数据库名称。</p>
</td>
</tr>
<tr id="row69721322132114"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p499832213211"><a name="p499832213211"></a><a name="p499832213211"></a>dws_schema</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1899902218212"><a name="p1899902218212"></a><a name="p1899902218212"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p149992225219"><a name="p149992225219"></a><a name="p149992225219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p501223152117"><a name="p501223152117"></a><a name="p501223152117"></a>存储该通道数据的DWS数据库模式。</p>
</td>
</tr>
<tr id="row14972162202112"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p00192314218"><a name="p00192314218"></a><a name="p00192314218"></a>dws_table_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p31112362117"><a name="p31112362117"></a><a name="p31112362117"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1011723122110"><a name="p1011723122110"></a><a name="p1011723122110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p131202342114"><a name="p131202342114"></a><a name="p131202342114"></a>存储该通道数据的DWS数据库模式下的数据表。</p>
</td>
</tr>
<tr id="row13972152212118"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p182423102116"><a name="p182423102116"></a><a name="p182423102116"></a>dws_delimiter</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p10262316215"><a name="p10262316215"></a><a name="p10262316215"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1231238217"><a name="p1231238217"></a><a name="p1231238217"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p73023182119"><a name="p73023182119"></a><a name="p73023182119"></a>用户数据的字段分隔符，根据此分隔符分隔用户数据插入DWS数据表的相应列。</p>
<p id="p1841723112117"><a name="p1841723112117"></a><a name="p1841723112117"></a>取值范围：“，”、“；”和“|”三种字符中的一个。</p>
</td>
</tr>
<tr id="row497242217219"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p14422320212"><a name="p14422320212"></a><a name="p14422320212"></a>user_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p8511233214"><a name="p8511233214"></a><a name="p8511233214"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p205323132115"><a name="p205323132115"></a><a name="p205323132115"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p65223202114"><a name="p65223202114"></a><a name="p65223202114"></a>存储该通道数据的DWS数据库的用户名。</p>
</td>
</tr>
<tr id="row197212225218"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p146923142110"><a name="p146923142110"></a><a name="p146923142110"></a>user_password</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p461623102120"><a name="p461623102120"></a><a name="p461623102120"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p3642318216"><a name="p3642318216"></a><a name="p3642318216"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p0792317218"><a name="p0792317218"></a><a name="p0792317218"></a>存储该通道数据的DWS数据库的密码。</p>
</td>
</tr>
<tr id="row297242215219"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p47202382115"><a name="p47202382115"></a><a name="p47202382115"></a>kms_user_key_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p48142332117"><a name="p48142332117"></a><a name="p48142332117"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1789233214"><a name="p1789233214"></a><a name="p1789233214"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p199182382114"><a name="p199182382114"></a><a name="p199182382114"></a>用户在密钥管理服务（简称KMS）创建的用户主密钥名称，用于加密存储DWS数据库的密码。</p>
</td>
</tr>
<tr id="row0972822162113"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p59523182113"><a name="p59523182113"></a><a name="p59523182113"></a>kms_user_key_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p191423202117"><a name="p191423202117"></a><a name="p191423202117"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p10103237217"><a name="p10103237217"></a><a name="p10103237217"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1810423182111"><a name="p1810423182111"></a><a name="p1810423182111"></a>用户在密钥管理服务（简称KMS）创建的用户主密钥ID，用于加密存储DWS数据库的密码。</p>
</td>
</tr>
<tr id="row3972922142116"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p11111023172120"><a name="p11111023172120"></a><a name="p11111023172120"></a>obs_bucket_path</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p171114236211"><a name="p171114236211"></a><a name="p171114236211"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p51172382112"><a name="p51172382112"></a><a name="p51172382112"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1312102362117"><a name="p1312102362117"></a><a name="p1312102362117"></a>临时存储该通道数据的OBS桶名称。</p>
</td>
</tr>
<tr id="row1997272212112"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p41419236211"><a name="p41419236211"></a><a name="p41419236211"></a>file_prefix</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p9159238214"><a name="p9159238214"></a><a name="p9159238214"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p2161023192119"><a name="p2161023192119"></a><a name="p2161023192119"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p21615237213"><a name="p21615237213"></a><a name="p21615237213"></a>临时存储该通道数据的OBS桶下的自定义目录，多级目录可用“/”进行分隔，不可以“/”开头。</p>
<p id="p1316112315215"><a name="p1316112315215"></a><a name="p1316112315215"></a>取值范围：英文字母、数字、下划线和斜杠，最大长度为50个字符。</p>
<p id="p417172372117"><a name="p417172372117"></a><a name="p417172372117"></a>默认配置为空。</p>
</td>
</tr>
<tr id="row9972422182111"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p117122362119"><a name="p117122362119"></a><a name="p117122362119"></a>retry_duration</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p7178235213"><a name="p7178235213"></a><a name="p7178235213"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1218112352117"><a name="p1218112352117"></a><a name="p1218112352117"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p141810233217"><a name="p141810233217"></a><a name="p141810233217"></a>用户数据导入DWS集群失败的重试失效时间。超出此配置项配置的时间，转储DWS失败的数据将备份至“OBS桶/ file_prefix/dws_error”目录下。</p>
<p id="p818023112113"><a name="p818023112113"></a><a name="p818023112113"></a>取值范围： 0～7200</p>
<p id="p121932312118"><a name="p121932312118"></a><a name="p121932312118"></a>单位：秒</p>
<p id="p13191123152117"><a name="p13191123152117"></a><a name="p13191123152117"></a>默认配置为1800。</p>
</td>
</tr>
<tr id="row997216226213"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p13191123102119"><a name="p13191123102119"></a><a name="p13191123102119"></a>dws_table_columns</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p6201234213"><a name="p6201234213"></a><a name="p6201234213"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p11201023112111"><a name="p11201023112111"></a><a name="p11201023112111"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p120162332119"><a name="p120162332119"></a><a name="p120162332119"></a>指定要转储到DWS表中的列，为null或者为空则默认全列。比如“c1,c2”表示将Schema中c1和c2这两列转储到DWS。</p>
<p id="p221182311210"><a name="p221182311210"></a><a name="p221182311210"></a>默认为空。</p>
</td>
</tr>
<tr id="row397219226211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p112132302114"><a name="p112132302114"></a><a name="p112132302114"></a>options</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1322132312214"><a name="p1322132312214"></a><a name="p1322132312214"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p12242392114"><a name="p12242392114"></a><a name="p12242392114"></a><a href="#request_Options">Options</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p62311233212"><a name="p62311233212"></a><a name="p62311233212"></a>DWS容错性选项（用于指定外表数据的各类参数）。</p>
</td>
</tr>
</tbody>
</table>

**表 5**  Options

<a name="request_Options"></a>
<table><thead align="left"><tr id="row1824192352116"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p1425123152112"><a name="p1425123152112"></a><a name="p1425123152112"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p172652310213"><a name="p172652310213"></a><a name="p172652310213"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p11263232211"><a name="p11263232211"></a><a name="p11263232211"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p4274234219"><a name="p4274234219"></a><a name="p4274234219"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row124523162112"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p132782311216"><a name="p132782311216"></a><a name="p132782311216"></a>fill_missing_fields</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1528623102115"><a name="p1528623102115"></a><a name="p1528623102115"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p6281523192110"><a name="p6281523192110"></a><a name="p6281523192110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p729112317216"><a name="p729112317216"></a><a name="p729112317216"></a>数据入库时，数据源文件中某行的最后一个字段缺失时，请选择是直接将字段设为Null，还是在错误表中报错提示。</p>
<p id="p132916231217"><a name="p132916231217"></a><a name="p132916231217"></a>取值范围：</p>
<a name="ul11305239217"></a><a name="ul11305239217"></a><ul id="ul11305239217"><li>true/on</li><li>false/off</li></ul>
<p id="p3310230212"><a name="p3310230212"></a><a name="p3310230212"></a>缺省值：false/off</p>
<p id="p163102312213"><a name="p163102312213"></a><a name="p163102312213"></a>枚举值：</p>
<a name="ul193112313213"></a><a name="ul193112313213"></a><ul id="ul193112313213"><li><strong id="b7329234215"><a name="b7329234215"></a><a name="b7329234215"></a>true/on</strong></li><li><strong id="b732723192117"><a name="b732723192117"></a><a name="b732723192117"></a>false/off</strong></li></ul>
</td>
</tr>
<tr id="row13244236215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p183202392113"><a name="p183202392113"></a><a name="p183202392113"></a>ignore_extra_data</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1333182362112"><a name="p1333182362112"></a><a name="p1333182362112"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p9331323112113"><a name="p9331323112113"></a><a name="p9331323112113"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p434122312111"><a name="p434122312111"></a><a name="p434122312111"></a>数据源文件中的字段比外表定义列数多时，是否忽略多出的列。该参数只在数据导入过程中使用。</p>
<p id="p2035162352116"><a name="p2035162352116"></a><a name="p2035162352116"></a>取值范围：</p>
<a name="ul1635182332115"></a><a name="ul1635182332115"></a><ul id="ul1635182332115"><li>true/on</li><li>false/off</li></ul>
<p id="p11361234214"><a name="p11361234214"></a><a name="p11361234214"></a>缺省值：false/off</p>
<p id="p133652372117"><a name="p133652372117"></a><a name="p133652372117"></a>枚举值：</p>
<a name="ul1637172372112"></a><a name="ul1637172372112"></a><ul id="ul1637172372112"><li><strong id="b1537162372110"><a name="b1537162372110"></a><a name="b1537162372110"></a>true/on</strong></li><li><strong id="b123762372113"><a name="b123762372113"></a><a name="b123762372113"></a>false/off</strong></li></ul>
</td>
</tr>
<tr id="row182462362117"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p2381323152110"><a name="p2381323152110"></a><a name="p2381323152110"></a>compatible_illegal_chars</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1038923122114"><a name="p1038923122114"></a><a name="p1038923122114"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1039723152119"><a name="p1039723152119"></a><a name="p1039723152119"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p34020235212"><a name="p34020235212"></a><a name="p34020235212"></a>导入非法字符容错参数。是将非法字符按照转换规则转换后入库，还是报错中止导入。</p>
<p id="p18401923112110"><a name="p18401923112110"></a><a name="p18401923112110"></a>取值范围：</p>
<a name="ul1940122319219"></a><a name="ul1940122319219"></a><ul id="ul1940122319219"><li>true/on</li><li>false/off</li></ul>
<p id="p441162372111"><a name="p441162372111"></a><a name="p441162372111"></a>缺省值：false/off</p>
<p id="p1947852311211"><a name="p1947852311211"></a><a name="p1947852311211"></a>枚举值：</p>
<a name="ul1847852372114"></a><a name="ul1847852372114"></a><ul id="ul1847852372114"><li><strong id="b14478102316211"><a name="b14478102316211"></a><a name="b14478102316211"></a>true/on</strong></li><li><strong id="b2047817236211"><a name="b2047817236211"></a><a name="b2047817236211"></a>false/off</strong></li></ul>
</td>
</tr>
<tr id="row524723132112"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p047815232211"><a name="p047815232211"></a><a name="p047815232211"></a>reject_limit</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1747872319213"><a name="p1747872319213"></a><a name="p1747872319213"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p184781223162120"><a name="p184781223162120"></a><a name="p184781223162120"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p18479132310212"><a name="p18479132310212"></a><a name="p18479132310212"></a>指定本次数据导入允许出现的数据格式错误个数，当导入过程中出现的数据格式错误未达到限定值时，本次数据导入可以成功。</p>
<p id="p24798231219"><a name="p24798231219"></a><a name="p24798231219"></a>取值范围：</p>
<a name="ul17479723102111"></a><a name="ul17479723102111"></a><ul id="ul17479723102111"><li>整型值</li><li>unlimited（无限制）</li></ul>
<p id="p54804235219"><a name="p54804235219"></a><a name="p54804235219"></a>缺省值为0，有错误信息立即返回。</p>
</td>
</tr>
<tr id="row82422372119"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p448042322114"><a name="p448042322114"></a><a name="p448042322114"></a>error_table_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p10480172312213"><a name="p10480172312213"></a><a name="p10480172312213"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1248092312116"><a name="p1248092312116"></a><a name="p1248092312116"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p648052342113"><a name="p648052342113"></a><a name="p648052342113"></a>用于记录数据格式错误信息的错误表表名。并行导入结束后查询此错误信息表，能够获取详细的错误信息。</p>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section44801823192117"></a>

无

## 请求示例<a name="section5481823182112"></a>

添加DWS转储任务

```
POST https://{Endpoint}/v2/{project_id}/streams/{stream_name}/transfer-tasks

{
  "destination_type" : "DWS",
  "dws_destination_descriptor" : {
    "task_name" : "dwstask",
    "consumer_strategy" : "LATEST",
    "agency_name" : "dis_admin_agency",
    "dws_cluster_name" : "dwscluster",
    "dws_cluster_id" : "f82dc227-3691-47eb-bca7-e7851f509b2a",
    "dws_database_name" : "postgres",
    "dws_schema" : "dbadmin",
    "dws_table_name" : "dwstablename",
    "dws_delimiter" : "",
    "user_name" : "dbadmin",
    "user_password" : "userpassword",
    "kms_user_key_name" : "kmskey",
    "kms_user_key_id" : "1e759f06-9188-4d21-afab-a75e57c04d2b",
    "obs_bucket_path" : "obsbucket",
    "file_prefix" : "",
    "deliver_time_interval" : 60,
    "retry_duration" : 1800,
    "options" : {
      "fill_missing_fields" : "false",
      "ignore_extra_data" : "false",
      "compatible_illegal_chars" : "false"
    }
  }
}
```

## 响应示例<a name="section204851923152110"></a>

无

## 状态码<a name="section20485132322113"></a>

<a name="status_code"></a>
<table><thead align="left"><tr id="row125562342119"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p1348672332117"><a name="p1348672332117"></a><a name="p1348672332117"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p048632362113"><a name="p048632362113"></a><a name="p048632362113"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row17554232214"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p1486112312111"><a name="p1486112312111"></a><a name="p1486112312111"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p04867234212"><a name="p04867234212"></a><a name="p04867234212"></a>正常返回</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section84868235219"></a>

请参见[错误码](错误码.md)。

