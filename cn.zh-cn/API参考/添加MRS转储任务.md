# 添加MRS转储任务<a name="CreateMrsTransferTask"></a>

## 功能介绍<a name="section1870412334329"></a>

本接口用于添加MRS转储任务。

## 调试<a name="section67095337325"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=DIS&api=CreateMrsTransferTask)中调试该接口。

## URI<a name="section871517332323"></a>

POST /v2/\{project\_id\}/streams/\{stream\_name\}/transfer-tasks

**表 1**  路径参数

<a name="table1272463323217"></a>
<table><thead align="left"><tr id="row972113334327"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p172615339326"><a name="p172615339326"></a><a name="p172615339326"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p77281833163217"><a name="p77281833163217"></a><a name="p77281833163217"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p97311033143212"><a name="p97311033143212"></a><a name="p97311033143212"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p13733533133210"><a name="p13733533133210"></a><a name="p13733533133210"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row10721103313329"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p147351033103220"><a name="p147351033103220"></a><a name="p147351033103220"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1073714334326"><a name="p1073714334326"></a><a name="p1073714334326"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p19739143313216"><a name="p19739143313216"></a><a name="p19739143313216"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1974143373218"><a name="p1974143373218"></a><a name="p1974143373218"></a>项目ID。</p>
</td>
</tr>
<tr id="row8721133133218"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1274320338325"><a name="p1274320338325"></a><a name="p1274320338325"></a>stream_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p4745633153215"><a name="p4745633153215"></a><a name="p4745633153215"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p137481333123215"><a name="p137481333123215"></a><a name="p137481333123215"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1375003393213"><a name="p1375003393213"></a><a name="p1375003393213"></a>已创建的通道名称。</p>
<p id="p1075353363213"><a name="p1075353363213"></a><a name="p1075353363213"></a>最大长度：<strong id="b8754833163213"><a name="b8754833163213"></a><a name="b8754833163213"></a>60</strong></p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section15756833153214"></a>

**表 2**  请求Header参数

<a name="HeaderParameter"></a>
<table><thead align="left"><tr id="row13759193316324"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p476310331320"><a name="p476310331320"></a><a name="p476310331320"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p37661433153215"><a name="p37661433153215"></a><a name="p37661433153215"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p127684337322"><a name="p127684337322"></a><a name="p127684337322"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p177073315322"><a name="p177073315322"></a><a name="p177073315322"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row177597332320"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1377212335325"><a name="p1377212335325"></a><a name="p1377212335325"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p20773133143216"><a name="p20773133143216"></a><a name="p20773133143216"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p3776163320321"><a name="p3776163320321"></a><a name="p3776163320321"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p7778233133210"><a name="p7778233133210"></a><a name="p7778233133210"></a>用户Token。</p>
<p id="p9780233113220"><a name="p9780233113220"></a><a name="p9780233113220"></a>通过调用IAM服务获取用户Token接口获取（响应消息头中X-Subject-Token的值）。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  请求Body参数

<a name="requestParameter"></a>
<table><thead align="left"><tr id="row197832338325"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p678683314326"><a name="p678683314326"></a><a name="p678683314326"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p4788433103217"><a name="p4788433103217"></a><a name="p4788433103217"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p1279163314325"><a name="p1279163314325"></a><a name="p1279163314325"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p1979363310324"><a name="p1979363310324"></a><a name="p1979363310324"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row07837339327"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p147971633183218"><a name="p147971633183218"></a><a name="p147971633183218"></a>destination_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p479903318329"><a name="p479903318329"></a><a name="p479903318329"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p188013330324"><a name="p188013330324"></a><a name="p188013330324"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p128035336328"><a name="p128035336328"></a><a name="p128035336328"></a>转储任务类型。</p>
<a name="ul680653323217"></a><a name="ul680653323217"></a><ul id="ul680653323217"><li>OBS：转储到OBS</li><li>MRS：转储到MRS</li><li>DLI：转储到DLI</li><li>DWS：转储到DWS</li></ul>
<p id="p138181533193219"><a name="p138181533193219"></a><a name="p138181533193219"></a>缺省值：<strong id="b6818103312325"><a name="b6818103312325"></a><a name="b6818103312325"></a>NOWHERE</strong></p>
<p id="p178191433153219"><a name="p178191433153219"></a><a name="p178191433153219"></a>枚举值：</p>
<a name="ul282183303220"></a><a name="ul282183303220"></a><ul id="ul282183303220"><li><strong id="b08231833103220"><a name="b08231833103220"></a><a name="b08231833103220"></a>MRS</strong></li></ul>
</td>
</tr>
<tr id="row1578319334328"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p4824133319323"><a name="p4824133319323"></a><a name="p4824133319323"></a>mrs_destination_descriptor</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p118262336324"><a name="p118262336324"></a><a name="p118262336324"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p128291533163210"><a name="p128291533163210"></a><a name="p128291533163210"></a><a href="#request_MRSDestinationDescriptorRequest">MRSDestinationDescriptorRequest</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p88311133133215"><a name="p88311133133215"></a><a name="p88311133133215"></a>转储目的地为MRS的参数列表。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  MRSDestinationDescriptorRequest

<a name="request_MRSDestinationDescriptorRequest"></a>
<table><thead align="left"><tr id="row38331433153217"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p20838193317329"><a name="p20838193317329"></a><a name="p20838193317329"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p15840113313320"><a name="p15840113313320"></a><a name="p15840113313320"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p58421333123215"><a name="p58421333123215"></a><a name="p58421333123215"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p14844203314327"><a name="p14844203314327"></a><a name="p14844203314327"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row2083323383213"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p78462033123212"><a name="p78462033123212"></a><a name="p78462033123212"></a>task_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p0848153312327"><a name="p0848153312327"></a><a name="p0848153312327"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p985012332320"><a name="p985012332320"></a><a name="p985012332320"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1852153316322"><a name="p1852153316322"></a><a name="p1852153316322"></a>转储任务的名称。  任务名称由英文字母、数字、中划线和下划线组成。长度为1～64个字符。</p>
</td>
</tr>
<tr id="row19833193353215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p108541433133220"><a name="p108541433133220"></a><a name="p108541433133220"></a>agency_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p98561233133216"><a name="p98561233133216"></a><a name="p98561233133216"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p13858193323218"><a name="p13858193323218"></a><a name="p13858193323218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p11860193312323"><a name="p11860193312323"></a><a name="p11860193312323"></a>在统一身份认证服务(IAM)中创建委托的名称，DIS需要获取IAM委托信息去访问您指定的资源。创建委托的参数设置如下：</p>
<a name="ul1986283314326"></a><a name="ul1986283314326"></a><ul id="ul1986283314326"><li>委托类型：云服务</li><li>云服务：DIS</li><li>持续时间：永久</li><li>“所属区域”为“全局服务”，“项目”为“对象存储服务”对应的“策略”包含“Tenant Administrator”。 如果已经创建过委托，可以使用IAM服务提供的<a href="https://support.huaweicloud.com/api-iam/iam_12_0001.html" target="_blank" rel="noopener noreferrer">查询委托列表</a>接口，获取有效可用的委托名称。 取值范围：长度不超过64位，且不可配置为空。</li></ul>
<p id="p138731533113217"><a name="p138731533113217"></a><a name="p138731533113217"></a>如果有在Console控制台使用转储任务，会提示自动创建委托，自动创建的委托名称为：dis_admin_agency</p>
<p id="p1487419339324"><a name="p1487419339324"></a><a name="p1487419339324"></a>最大长度：<strong id="b11875833133214"><a name="b11875833133214"></a><a name="b11875833133214"></a>64</strong></p>
</td>
</tr>
<tr id="row6833103313216"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1287613317329"><a name="p1287613317329"></a><a name="p1287613317329"></a>deliver_time_interval</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p7878153373216"><a name="p7878153373216"></a><a name="p7878153373216"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p188073320321"><a name="p188073320321"></a><a name="p188073320321"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p14883733163219"><a name="p14883733163219"></a><a name="p14883733163219"></a>根据用户配置的时间，周期性的将数据导入OBS，若某个时间段内无数据，则此时间段不会生成打包文件。</p>
<p id="p138851733113218"><a name="p138851733113218"></a><a name="p138851733113218"></a>取值范围：30～900</p>
<p id="p208871233113210"><a name="p208871233113210"></a><a name="p208871233113210"></a>缺省值：300</p>
<p id="p688815332321"><a name="p688815332321"></a><a name="p688815332321"></a>单位：秒</p>
<p id="p889033312327"><a name="p889033312327"></a><a name="p889033312327"></a>最小值：<strong id="b2891433183220"><a name="b2891433183220"></a><a name="b2891433183220"></a>30</strong></p>
<p id="p1889273383216"><a name="p1889273383216"></a><a name="p1889273383216"></a>最大值：<strong id="b108931233203218"><a name="b108931233203218"></a><a name="b108931233203218"></a>900</strong></p>
<p id="p2894333173218"><a name="p2894333173218"></a><a name="p2894333173218"></a>缺省值：<strong id="b1689523303217"><a name="b1689523303217"></a><a name="b1689523303217"></a>300</strong></p>
</td>
</tr>
<tr id="row683323316325"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p128961833183214"><a name="p128961833183214"></a><a name="p128961833183214"></a>consumer_strategy</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p16899133163220"><a name="p16899133163220"></a><a name="p16899133163220"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p159005338326"><a name="p159005338326"></a><a name="p159005338326"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p19031533183219"><a name="p19031533183219"></a><a name="p19031533183219"></a>偏移量。</p>
<a name="ul9905113383216"></a><a name="ul9905113383216"></a><ul id="ul9905113383216"><li>LATEST：最大偏移量，即获取最新的数据。</li><li>TRIM_HORIZON：最小偏移量，即读取最早的数据。</li></ul>
<p id="p1190923310328"><a name="p1190923310328"></a><a name="p1190923310328"></a>缺省值：LATEST</p>
<p id="p691023373213"><a name="p691023373213"></a><a name="p691023373213"></a>缺省值：<strong id="b1791103373214"><a name="b1791103373214"></a><a name="b1791103373214"></a>LATEST</strong></p>
<p id="p109121633193215"><a name="p109121633193215"></a><a name="p109121633193215"></a>枚举值：</p>
<a name="ul1491463323212"></a><a name="ul1491463323212"></a><ul id="ul1491463323212"><li><strong id="b1491511336321"><a name="b1491511336321"></a><a name="b1491511336321"></a>LATEST</strong></li><li><strong id="b139181333103216"><a name="b139181333103216"></a><a name="b139181333103216"></a>TRIM_HORIZON</strong></li></ul>
</td>
</tr>
<tr id="row98333338325"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p2919163363219"><a name="p2919163363219"></a><a name="p2919163363219"></a>mrs_cluster_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1292120333325"><a name="p1292120333325"></a><a name="p1292120333325"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p189239333323"><a name="p189239333323"></a><a name="p189239333323"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p3925133163218"><a name="p3925133163218"></a><a name="p3925133163218"></a>存储该通道数据的MRS集群名称。</p>
<p id="p199271633123212"><a name="p199271633123212"></a><a name="p199271633123212"></a>说明：</p>
<p id="p13929833143215"><a name="p13929833143215"></a><a name="p13929833143215"></a>仅支持非Kerberos认证的MRS集群。</p>
</td>
</tr>
<tr id="row6834143343218"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p169316337327"><a name="p169316337327"></a><a name="p169316337327"></a>mrs_cluster_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p4933193353219"><a name="p4933193353219"></a><a name="p4933193353219"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p493515332323"><a name="p493515332323"></a><a name="p493515332323"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p19937103393218"><a name="p19937103393218"></a><a name="p19937103393218"></a>存储该通道数据的MRS集群ID。</p>
</td>
</tr>
<tr id="row18341233113213"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p494013383211"><a name="p494013383211"></a><a name="p494013383211"></a>mrs_hdfs_path</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p9941193313212"><a name="p9941193313212"></a><a name="p9941193313212"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p15943193323211"><a name="p15943193323211"></a><a name="p15943193323211"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p18946143303214"><a name="p18946143303214"></a><a name="p18946143303214"></a>存储该通道数据的MRS集群的HDFS路径。</p>
</td>
</tr>
<tr id="row18341333113216"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1894863333211"><a name="p1894863333211"></a><a name="p1894863333211"></a>file_prefix</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p15950123303217"><a name="p15950123303217"></a><a name="p15950123303217"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p79521633123214"><a name="p79521633123214"></a><a name="p79521633123214"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1595413317322"><a name="p1595413317322"></a><a name="p1595413317322"></a>临时存储该通道数据的OBS桶下的自定义目录，多级目录可用“/”进行分隔，不可以“/”开头。</p>
<p id="p1395763310328"><a name="p1395763310328"></a><a name="p1395763310328"></a>取值范围：英文字母、数字、下划线和斜杠，最大长度为50个字符。</p>
<p id="p1295820332329"><a name="p1295820332329"></a><a name="p1295820332329"></a>默认配置为空。</p>
</td>
</tr>
<tr id="row983412337322"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p796012334324"><a name="p796012334324"></a><a name="p796012334324"></a>hdfs_prefix_folder</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p19622338329"><a name="p19622338329"></a><a name="p19622338329"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p69641833203212"><a name="p69641833203212"></a><a name="p69641833203212"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1396743323213"><a name="p1396743323213"></a><a name="p1396743323213"></a>在MRS集群HDFS中存储通道文件的自定义目录，多级目录可用"/"进行分隔。</p>
<p id="p996963317325"><a name="p996963317325"></a><a name="p996963317325"></a>取值范围：0~50个字符。</p>
<p id="p2970103323214"><a name="p2970103323214"></a><a name="p2970103323214"></a>默认配置为空。</p>
</td>
</tr>
<tr id="row1483417331325"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p129721333113215"><a name="p129721333113215"></a><a name="p129721333113215"></a>obs_bucket_path</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1797453313327"><a name="p1797453313327"></a><a name="p1797453313327"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p0976193315321"><a name="p0976193315321"></a><a name="p0976193315321"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p8977233183211"><a name="p8977233183211"></a><a name="p8977233183211"></a>临时存储该通道数据的OBS桶名称。</p>
</td>
</tr>
<tr id="row15834733133215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p39804332328"><a name="p39804332328"></a><a name="p39804332328"></a>retry_duration</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p0982133316328"><a name="p0982133316328"></a><a name="p0982133316328"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1398419331325"><a name="p1398419331325"></a><a name="p1398419331325"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p16987153393210"><a name="p16987153393210"></a><a name="p16987153393210"></a>用户数据转储失败的失效重试时间。重试时间超过该配置项配置的值，则将转储失败的数据备份至“OBS桶/ file_prefix/mrs_error”目录下。</p>
<p id="p698813316326"><a name="p698813316326"></a><a name="p698813316326"></a>取值范围：0~7200。</p>
<p id="p2990143313327"><a name="p2990143313327"></a><a name="p2990143313327"></a>单位：秒。</p>
<p id="p4991133315327"><a name="p4991133315327"></a><a name="p4991133315327"></a>默认配置为1800。</p>
<p id="p3993193313212"><a name="p3993193313212"></a><a name="p3993193313212"></a>配置为“0”表示DIS服务不会在转储失败时进行重试。</p>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section19951433113217"></a>

无

## 请求示例<a name="section199991133193217"></a>

添加MRS转储任务

```
POST https://{Endpoint}/v2/{project_id}/streams/{stream_name}/transfer-tasks

{
  "destination_type" : "MRS",
  "mrs_destination_descriptor" : {
    "task_name" : "mrstask",
    "consumer_strategy" : "LATEST",
    "agency_name" : "dis_admin_agency",
    "destination_file_type" : "text",
    "mrs_cluster_id" : "f8123fa6-99f1-4ed9-83f4-c827c7277d41",
    "mrs_cluster_name" : "mrscluster",
    "mrs_hdfs_path" : "/user",
    "obs_bucket_path" : "obsbucket",
    "file_prefix" : "",
    "hdfs_prefix_folder" : "",
    "deliver_time_interval" : 30,
    "retry_duration" : 1800
  }
}
```

## 响应示例<a name="section64033493213"></a>

无

## 状态码<a name="section645153417323"></a>

<a name="status_code"></a>
<table><thead align="left"><tr id="row6487347322"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p851113412323"><a name="p851113412323"></a><a name="p851113412323"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p2521234133213"><a name="p2521234133213"></a><a name="p2521234133213"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row194993463218"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p05420341329"><a name="p05420341329"></a><a name="p05420341329"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p3561234153212"><a name="p3561234153212"></a><a name="p3561234153212"></a>正常返回</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section11581834143219"></a>

请参见[错误码](错误码.md)。

