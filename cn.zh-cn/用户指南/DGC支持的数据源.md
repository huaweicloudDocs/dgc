# DGC支持的数据源<a name="dgc_01_0005"></a>

在使用DGC前，您需要根据业务场景选择符合需求的云服务或数据仓库作为数据湖，用于存储原始数据和数据治理过程中的数据，并进行数据开发、服务和运营。DGC集成了丰富的数据引擎，支持对接如DLI、DWS、MRS Hive等云上数据湖与数据库云服务，也支持对接企业传统数据库，例如MySQL、PostgreSQL等。

## DGC支持的数据源<a name="section1818582902919"></a>

DGC支持的数据源可分为“数据集成组件支持的数据源”和“DGC其他组件支持的数据源”。

-   数据集成组件支持的数据源。数据集成组件需要集成源数据到数据湖中，因此支持的数据源范围更广。

    批量数据迁移支持的数据源请参见[批量数据迁移支持的数据源](支持的数据源.md)。注意，如需在批量数据迁移中使用这些数据源，请先在批量数据迁移中创建对应的数据连接，这些数据连接仅限于在批量数据迁移模块中使用。

    实时数据接入支持的数据源，请参见[实时数据接入支持的数据源](实时数据接入支持的数据源.md)。

-   DGC其他组件支持的数据源，即为DGC所支持的数据湖底座。

    其他组件支持的数据源如[表1](#table157791731112911)所示，数据源的介绍请参见[数据源简介](#section83131942185515)。注意，如需在其他组件中使用这些数据源，请先前往DGC管理中心控制台创建数据连接，这些数据连接不能在批量数据迁移模块中使用。


**表 1**  DGC其他组件支持的数据源

<a name="table157791731112911"></a>
<table><thead align="left"><tr id="row67794318296"><th class="cellrowborder" valign="top" width="25.65256525652565%" id="mcps1.2.9.1.1"><p id="p677914311295"><a name="p677914311295"></a><a name="p677914311295"></a>数据源类型</p>
</th>
<th class="cellrowborder" valign="top" width="10.79107910791079%" id="mcps1.2.9.1.2"><p id="p12780331172915"><a name="p12780331172915"></a><a name="p12780331172915"></a>管理中心</p>
</th>
<th class="cellrowborder" valign="top" width="10.461046104610459%" id="mcps1.2.9.1.3"><p id="p7780193182919"><a name="p7780193182919"></a><a name="p7780193182919"></a>规范设计</p>
</th>
<th class="cellrowborder" valign="top" width="10.66106610661066%" id="mcps1.2.9.1.4"><p id="p17802316298"><a name="p17802316298"></a><a name="p17802316298"></a>数据开发</p>
</th>
<th class="cellrowborder" valign="top" width="10.351035103510348%" id="mcps1.2.9.1.5"><p id="p378010310293"><a name="p378010310293"></a><a name="p378010310293"></a>数据资产</p>
</th>
<th class="cellrowborder" valign="top" width="10.97109710971097%" id="mcps1.2.9.1.6"><p id="p107802318295"><a name="p107802318295"></a><a name="p107802318295"></a>数据质量</p>
</th>
<th class="cellrowborder" valign="top" width="10.66106610661066%" id="mcps1.2.9.1.7"><p id="p10780193182915"><a name="p10780193182915"></a><a name="p10780193182915"></a>数据服务</p>
</th>
<th class="cellrowborder" valign="top" width="10.451045104510449%" id="mcps1.2.9.1.8"><p id="p1878023122918"><a name="p1878023122918"></a><a name="p1878023122918"></a>数据安全</p>
</th>
</tr>
</thead>
<tbody><tr id="row1478093115290"><td class="cellrowborder" valign="top" width="25.65256525652565%" headers="mcps1.2.9.1.1 "><p id="p678053114297"><a name="p678053114297"></a><a name="p678053114297"></a>数据仓库服务（DWS）</p>
</td>
<td class="cellrowborder" valign="top" width="10.79107910791079%" headers="mcps1.2.9.1.2 "><p id="p17801331102918"><a name="p17801331102918"></a><a name="p17801331102918"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.461046104610459%" headers="mcps1.2.9.1.3 "><p id="p4780031182917"><a name="p4780031182917"></a><a name="p4780031182917"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.66106610661066%" headers="mcps1.2.9.1.4 "><p id="p178073114296"><a name="p178073114296"></a><a name="p178073114296"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.351035103510348%" headers="mcps1.2.9.1.5 "><p id="p1878013314297"><a name="p1878013314297"></a><a name="p1878013314297"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.97109710971097%" headers="mcps1.2.9.1.6 "><p id="p878063102914"><a name="p878063102914"></a><a name="p878063102914"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.66106610661066%" headers="mcps1.2.9.1.7 "><p id="p1778083114293"><a name="p1778083114293"></a><a name="p1778083114293"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.451045104510449%" headers="mcps1.2.9.1.8 "><p id="p10780931102913"><a name="p10780931102913"></a><a name="p10780931102913"></a>√</p>
</td>
</tr>
<tr id="row13780103113293"><td class="cellrowborder" valign="top" width="25.65256525652565%" headers="mcps1.2.9.1.1 "><p id="p47801931172911"><a name="p47801931172911"></a><a name="p47801931172911"></a>数据湖探索（DLI）</p>
</td>
<td class="cellrowborder" valign="top" width="10.79107910791079%" headers="mcps1.2.9.1.2 "><p id="p2780173162913"><a name="p2780173162913"></a><a name="p2780173162913"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.461046104610459%" headers="mcps1.2.9.1.3 "><p id="p6780163112919"><a name="p6780163112919"></a><a name="p6780163112919"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.66106610661066%" headers="mcps1.2.9.1.4 "><p id="p278093114294"><a name="p278093114294"></a><a name="p278093114294"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.351035103510348%" headers="mcps1.2.9.1.5 "><p id="p578013112910"><a name="p578013112910"></a><a name="p578013112910"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.97109710971097%" headers="mcps1.2.9.1.6 "><p id="p117806312290"><a name="p117806312290"></a><a name="p117806312290"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.66106610661066%" headers="mcps1.2.9.1.7 "><p id="p137801631112913"><a name="p137801631112913"></a><a name="p137801631112913"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.451045104510449%" headers="mcps1.2.9.1.8 "><p id="p137805313298"><a name="p137805313298"></a><a name="p137805313298"></a>√</p>
</td>
</tr>
<tr id="row97805317296"><td class="cellrowborder" valign="top" width="25.65256525652565%" headers="mcps1.2.9.1.1 "><p id="p137801331112919"><a name="p137801331112919"></a><a name="p137801331112919"></a>MapReduce服务（MRS HBase）</p>
</td>
<td class="cellrowborder" valign="top" width="10.79107910791079%" headers="mcps1.2.9.1.2 "><p id="p778083122914"><a name="p778083122914"></a><a name="p778083122914"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.461046104610459%" headers="mcps1.2.9.1.3 "><p id="p3780153142915"><a name="p3780153142915"></a><a name="p3780153142915"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.66106610661066%" headers="mcps1.2.9.1.4 "><p id="p16780331192911"><a name="p16780331192911"></a><a name="p16780331192911"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.351035103510348%" headers="mcps1.2.9.1.5 "><p id="p5780631162920"><a name="p5780631162920"></a><a name="p5780631162920"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.97109710971097%" headers="mcps1.2.9.1.6 "><p id="p27801131162910"><a name="p27801131162910"></a><a name="p27801131162910"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.66106610661066%" headers="mcps1.2.9.1.7 "><p id="p278033112915"><a name="p278033112915"></a><a name="p278033112915"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.451045104510449%" headers="mcps1.2.9.1.8 "><p id="p1778011316293"><a name="p1778011316293"></a><a name="p1778011316293"></a>×</p>
</td>
</tr>
<tr id="row97806314294"><td class="cellrowborder" valign="top" width="25.65256525652565%" headers="mcps1.2.9.1.1 "><p id="p17780123132920"><a name="p17780123132920"></a><a name="p17780123132920"></a>MapReduce服务（MRS Hive）</p>
</td>
<td class="cellrowborder" valign="top" width="10.79107910791079%" headers="mcps1.2.9.1.2 "><p id="p1778013122916"><a name="p1778013122916"></a><a name="p1778013122916"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.461046104610459%" headers="mcps1.2.9.1.3 "><p id="p3780183172911"><a name="p3780183172911"></a><a name="p3780183172911"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.66106610661066%" headers="mcps1.2.9.1.4 "><p id="p187802317292"><a name="p187802317292"></a><a name="p187802317292"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.351035103510348%" headers="mcps1.2.9.1.5 "><p id="p9780203114296"><a name="p9780203114296"></a><a name="p9780203114296"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.97109710971097%" headers="mcps1.2.9.1.6 "><p id="p2780531152911"><a name="p2780531152911"></a><a name="p2780531152911"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.66106610661066%" headers="mcps1.2.9.1.7 "><p id="p678023111296"><a name="p678023111296"></a><a name="p678023111296"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.451045104510449%" headers="mcps1.2.9.1.8 "><p id="p17780143119299"><a name="p17780143119299"></a><a name="p17780143119299"></a>√</p>
</td>
</tr>
<tr id="row15780431192920"><td class="cellrowborder" valign="top" width="25.65256525652565%" headers="mcps1.2.9.1.1 "><p id="p0780163118298"><a name="p0780163118298"></a><a name="p0780163118298"></a>MapReduce服务（MRS Kafka）</p>
</td>
<td class="cellrowborder" valign="top" width="10.79107910791079%" headers="mcps1.2.9.1.2 "><p id="p15780731192916"><a name="p15780731192916"></a><a name="p15780731192916"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.461046104610459%" headers="mcps1.2.9.1.3 "><p id="p16780113115298"><a name="p16780113115298"></a><a name="p16780113115298"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.66106610661066%" headers="mcps1.2.9.1.4 "><p id="p18780731192915"><a name="p18780731192915"></a><a name="p18780731192915"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.351035103510348%" headers="mcps1.2.9.1.5 "><p id="p13780143142911"><a name="p13780143142911"></a><a name="p13780143142911"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.97109710971097%" headers="mcps1.2.9.1.6 "><p id="p127801631132911"><a name="p127801631132911"></a><a name="p127801631132911"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.66106610661066%" headers="mcps1.2.9.1.7 "><p id="p6780193110298"><a name="p6780193110298"></a><a name="p6780193110298"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.451045104510449%" headers="mcps1.2.9.1.8 "><p id="p10780831162914"><a name="p10780831162914"></a><a name="p10780831162914"></a>×</p>
</td>
</tr>
<tr id="row18780113116291"><td class="cellrowborder" valign="top" width="25.65256525652565%" headers="mcps1.2.9.1.1 "><p id="p478014316297"><a name="p478014316297"></a><a name="p478014316297"></a>MapReduce服务（MRS Ranger）</p>
</td>
<td class="cellrowborder" valign="top" width="10.79107910791079%" headers="mcps1.2.9.1.2 "><p id="p117801731142914"><a name="p117801731142914"></a><a name="p117801731142914"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.461046104610459%" headers="mcps1.2.9.1.3 "><p id="p1278093112291"><a name="p1278093112291"></a><a name="p1278093112291"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.66106610661066%" headers="mcps1.2.9.1.4 "><p id="p378018317290"><a name="p378018317290"></a><a name="p378018317290"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.351035103510348%" headers="mcps1.2.9.1.5 "><p id="p14780331142915"><a name="p14780331142915"></a><a name="p14780331142915"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.97109710971097%" headers="mcps1.2.9.1.6 "><p id="p27802031112910"><a name="p27802031112910"></a><a name="p27802031112910"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.66106610661066%" headers="mcps1.2.9.1.7 "><p id="p207809311293"><a name="p207809311293"></a><a name="p207809311293"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.451045104510449%" headers="mcps1.2.9.1.8 "><p id="p157800319293"><a name="p157800319293"></a><a name="p157800319293"></a>√</p>
</td>
</tr>
<tr id="row18780143152916"><td class="cellrowborder" valign="top" width="25.65256525652565%" headers="mcps1.2.9.1.1 "><p id="p14780331162918"><a name="p14780331162918"></a><a name="p14780331162918"></a>MySQL（待下线）</p>
</td>
<td class="cellrowborder" valign="top" width="10.79107910791079%" headers="mcps1.2.9.1.2 "><p id="p9780193115299"><a name="p9780193115299"></a><a name="p9780193115299"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.461046104610459%" headers="mcps1.2.9.1.3 "><p id="p378023112910"><a name="p378023112910"></a><a name="p378023112910"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.66106610661066%" headers="mcps1.2.9.1.4 "><p id="p3780153111298"><a name="p3780153111298"></a><a name="p3780153111298"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.351035103510348%" headers="mcps1.2.9.1.5 "><p id="p278023182910"><a name="p278023182910"></a><a name="p278023182910"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.97109710971097%" headers="mcps1.2.9.1.6 "><p id="p12780731202911"><a name="p12780731202911"></a><a name="p12780731202911"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.66106610661066%" headers="mcps1.2.9.1.7 "><p id="p17801431142911"><a name="p17801431142911"></a><a name="p17801431142911"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.451045104510449%" headers="mcps1.2.9.1.8 "><p id="p13780731132919"><a name="p13780731132919"></a><a name="p13780731132919"></a>×</p>
</td>
</tr>
<tr id="row127801331192914"><td class="cellrowborder" valign="top" width="25.65256525652565%" headers="mcps1.2.9.1.1 "><p id="p147802031112913"><a name="p147802031112913"></a><a name="p147802031112913"></a>Oracle</p>
</td>
<td class="cellrowborder" valign="top" width="10.79107910791079%" headers="mcps1.2.9.1.2 "><p id="p97811431202915"><a name="p97811431202915"></a><a name="p97811431202915"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.461046104610459%" headers="mcps1.2.9.1.3 "><p id="p978163115293"><a name="p978163115293"></a><a name="p978163115293"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.66106610661066%" headers="mcps1.2.9.1.4 "><p id="p2781103112290"><a name="p2781103112290"></a><a name="p2781103112290"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.351035103510348%" headers="mcps1.2.9.1.5 "><p id="p1078117318293"><a name="p1078117318293"></a><a name="p1078117318293"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.97109710971097%" headers="mcps1.2.9.1.6 "><p id="p19781203192914"><a name="p19781203192914"></a><a name="p19781203192914"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.66106610661066%" headers="mcps1.2.9.1.7 "><p id="p078143172920"><a name="p078143172920"></a><a name="p078143172920"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.451045104510449%" headers="mcps1.2.9.1.8 "><p id="p1478193110296"><a name="p1478193110296"></a><a name="p1478193110296"></a>×</p>
</td>
</tr>
<tr id="row278153119291"><td class="cellrowborder" valign="top" width="25.65256525652565%" headers="mcps1.2.9.1.1 "><p id="p178173172917"><a name="p178173172917"></a><a name="p178173172917"></a>MapReduce服务（MRS Spark）</p>
</td>
<td class="cellrowborder" valign="top" width="10.79107910791079%" headers="mcps1.2.9.1.2 "><p id="p2781103162915"><a name="p2781103162915"></a><a name="p2781103162915"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.461046104610459%" headers="mcps1.2.9.1.3 "><p id="p1778163162916"><a name="p1778163162916"></a><a name="p1778163162916"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.66106610661066%" headers="mcps1.2.9.1.4 "><p id="p12781173162918"><a name="p12781173162918"></a><a name="p12781173162918"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.351035103510348%" headers="mcps1.2.9.1.5 "><p id="p778153118293"><a name="p778153118293"></a><a name="p778153118293"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.97109710971097%" headers="mcps1.2.9.1.6 "><p id="p18781331152915"><a name="p18781331152915"></a><a name="p18781331152915"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.66106610661066%" headers="mcps1.2.9.1.7 "><p id="p4781123152914"><a name="p4781123152914"></a><a name="p4781123152914"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.451045104510449%" headers="mcps1.2.9.1.8 "><p id="p12781113120297"><a name="p12781113120297"></a><a name="p12781113120297"></a>×</p>
</td>
</tr>
<tr id="row078112312295"><td class="cellrowborder" valign="top" width="25.65256525652565%" headers="mcps1.2.9.1.1 "><p id="p9781153110292"><a name="p9781153110292"></a><a name="p9781153110292"></a>云数据库 RDS</p>
</td>
<td class="cellrowborder" valign="top" width="10.79107910791079%" headers="mcps1.2.9.1.2 "><p id="p078183132910"><a name="p078183132910"></a><a name="p078183132910"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.461046104610459%" headers="mcps1.2.9.1.3 "><p id="p2781153192911"><a name="p2781153192911"></a><a name="p2781153192911"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.66106610661066%" headers="mcps1.2.9.1.4 "><p id="p578133114293"><a name="p578133114293"></a><a name="p578133114293"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.351035103510348%" headers="mcps1.2.9.1.5 "><p id="p187811331112918"><a name="p187811331112918"></a><a name="p187811331112918"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.97109710971097%" headers="mcps1.2.9.1.6 "><p id="p17781173132914"><a name="p17781173132914"></a><a name="p17781173132914"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.66106610661066%" headers="mcps1.2.9.1.7 "><p id="p578123117299"><a name="p578123117299"></a><a name="p578123117299"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.451045104510449%" headers="mcps1.2.9.1.8 "><p id="p167811231102912"><a name="p167811231102912"></a><a name="p167811231102912"></a>×</p>
</td>
</tr>
<tr id="row1678193122916"><td class="cellrowborder" valign="top" width="25.65256525652565%" headers="mcps1.2.9.1.1 "><p id="p87811931182916"><a name="p87811931182916"></a><a name="p87811931182916"></a>实时数据接入 DIS</p>
</td>
<td class="cellrowborder" valign="top" width="10.79107910791079%" headers="mcps1.2.9.1.2 "><p id="p6781331122912"><a name="p6781331122912"></a><a name="p6781331122912"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.461046104610459%" headers="mcps1.2.9.1.3 "><p id="p1178173102913"><a name="p1178173102913"></a><a name="p1178173102913"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.66106610661066%" headers="mcps1.2.9.1.4 "><p id="p97811631152911"><a name="p97811631152911"></a><a name="p97811631152911"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.351035103510348%" headers="mcps1.2.9.1.5 "><p id="p1378114314299"><a name="p1378114314299"></a><a name="p1378114314299"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.97109710971097%" headers="mcps1.2.9.1.6 "><p id="p078173142918"><a name="p078173142918"></a><a name="p078173142918"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.66106610661066%" headers="mcps1.2.9.1.7 "><p id="p57812311299"><a name="p57812311299"></a><a name="p57812311299"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.451045104510449%" headers="mcps1.2.9.1.8 "><p id="p778183182912"><a name="p778183182912"></a><a name="p778183182912"></a>×</p>
</td>
</tr>
<tr id="row15781831132916"><td class="cellrowborder" valign="top" width="25.65256525652565%" headers="mcps1.2.9.1.1 "><p id="p10781193192918"><a name="p10781193192918"></a><a name="p10781193192918"></a>主机连接</p>
</td>
<td class="cellrowborder" valign="top" width="10.79107910791079%" headers="mcps1.2.9.1.2 "><p id="p137812316291"><a name="p137812316291"></a><a name="p137812316291"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.461046104610459%" headers="mcps1.2.9.1.3 "><p id="p147811831142911"><a name="p147811831142911"></a><a name="p147811831142911"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.66106610661066%" headers="mcps1.2.9.1.4 "><p id="p3781163102918"><a name="p3781163102918"></a><a name="p3781163102918"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.351035103510348%" headers="mcps1.2.9.1.5 "><p id="p2781731202910"><a name="p2781731202910"></a><a name="p2781731202910"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.97109710971097%" headers="mcps1.2.9.1.6 "><p id="p578183182914"><a name="p578183182914"></a><a name="p578183182914"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.66106610661066%" headers="mcps1.2.9.1.7 "><p id="p1678119314292"><a name="p1678119314292"></a><a name="p1678119314292"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.451045104510449%" headers="mcps1.2.9.1.8 "><p id="p14781103162911"><a name="p14781103162911"></a><a name="p14781103162911"></a>×</p>
</td>
</tr>
<tr id="row8781173132916"><td class="cellrowborder" valign="top" width="25.65256525652565%" headers="mcps1.2.9.1.1 "><p id="p1478103112295"><a name="p1478103112295"></a><a name="p1478103112295"></a>MapReduce服务（MRS Presto）</p>
</td>
<td class="cellrowborder" valign="top" width="10.79107910791079%" headers="mcps1.2.9.1.2 "><p id="p1778123115296"><a name="p1778123115296"></a><a name="p1778123115296"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.461046104610459%" headers="mcps1.2.9.1.3 "><p id="p1478111318299"><a name="p1478111318299"></a><a name="p1478111318299"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.66106610661066%" headers="mcps1.2.9.1.4 "><p id="p13781123192910"><a name="p13781123192910"></a><a name="p13781123192910"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.351035103510348%" headers="mcps1.2.9.1.5 "><p id="p5781183152917"><a name="p5781183152917"></a><a name="p5781183152917"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.97109710971097%" headers="mcps1.2.9.1.6 "><p id="p117814313297"><a name="p117814313297"></a><a name="p117814313297"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="10.66106610661066%" headers="mcps1.2.9.1.7 "><p id="p1781193111296"><a name="p1781193111296"></a><a name="p1781193111296"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="10.451045104510449%" headers="mcps1.2.9.1.8 "><p id="p19781531112911"><a name="p19781531112911"></a><a name="p19781531112911"></a>×</p>
</td>
</tr>
</tbody>
</table>

除了上表中列出的需要在管理中心创建数据连接的数据源外，数据资产组件还支持采集以下数据源的元数据：

-   CSS（云搜索服务）
-   GES（图引擎服务）
-   OBS（对象存储服务）

## 数据源简介<a name="section83131942185515"></a>

**表 2**  数据源简介

<a name="table3323716565"></a>
<table><thead align="left"><tr id="row153235116568"><th class="cellrowborder" valign="top" width="33.300000000000004%" id="mcps1.2.3.1.1"><p id="p1132315110567"><a name="p1132315110567"></a><a name="p1132315110567"></a>数据源类型</p>
</th>
<th class="cellrowborder" valign="top" width="66.7%" id="mcps1.2.3.1.2"><p id="p103236105619"><a name="p103236105619"></a><a name="p103236105619"></a>简介</p>
</th>
</tr>
</thead>
<tbody><tr id="row133243175614"><td class="cellrowborder" valign="top" width="33.300000000000004%" headers="mcps1.2.3.1.1 "><p id="p113246116563"><a name="p113246116563"></a><a name="p113246116563"></a>数据仓库服务（DWS）</p>
</td>
<td class="cellrowborder" valign="top" width="66.7%" headers="mcps1.2.3.1.2 "><p id="p2324616561"><a name="p2324616561"></a><a name="p2324616561"></a>华为云DWS是基于Shared-nothing分布式架构，具备MPP大规模并行处理引擎，兼容标准ANSI SQL 99和SQL 2003，同时兼容PostgreSQL/Oracle数据库生态，为各行业PB级海量大数据分析提供有竞争力的解决方案。</p>
</td>
</tr>
<tr id="row03247125619"><td class="cellrowborder" valign="top" width="33.300000000000004%" headers="mcps1.2.3.1.1 "><p id="p1532412195617"><a name="p1532412195617"></a><a name="p1532412195617"></a>数据湖探索（DLI）</p>
</td>
<td class="cellrowborder" valign="top" width="66.7%" headers="mcps1.2.3.1.2 "><p id="p1532415125616"><a name="p1532415125616"></a><a name="p1532415125616"></a>华为云DLI是完全兼容Apache Spark和Apache Flink生态，实现批流一体的Serverless大数据计算分析服务。DLI支持多模引擎，企业仅需使用SQL或程序就可轻松完成异构数据源的批处理、流处理、内存计算、机器学习等，挖掘和探索数据价值。</p>
</td>
</tr>
<tr id="row93240120563"><td class="cellrowborder" valign="top" width="33.300000000000004%" headers="mcps1.2.3.1.1 "><p id="p143241619563"><a name="p143241619563"></a><a name="p143241619563"></a>MapReduce服务（MRS HBase）</p>
</td>
<td class="cellrowborder" valign="top" width="66.7%" headers="mcps1.2.3.1.2 "><p id="p1324219569"><a name="p1324219569"></a><a name="p1324219569"></a>HBase是一个开源的、面向列（Column-Oriented）、适合存储海量非结构化数据或半结构化数据的、具备高可靠性、高性能、可灵活扩展伸缩的、支持实时数据读写的分布式存储系统。</p>
<p id="p12324131185610"><a name="p12324131185610"></a><a name="p12324131185610"></a>使用MRS HBase可实现海量数据存储，并实现毫秒级数据查询。选择MRS HBase可以实现物流数据毫秒级实时入库更新，并支持百万级时序数据查询分析。</p>
</td>
</tr>
<tr id="row1532401185618"><td class="cellrowborder" valign="top" width="33.300000000000004%" headers="mcps1.2.3.1.1 "><p id="p832481165618"><a name="p832481165618"></a><a name="p832481165618"></a>MapReduce服务（MRS Hive）</p>
</td>
<td class="cellrowborder" valign="top" width="66.7%" headers="mcps1.2.3.1.2 "><p id="p53241145617"><a name="p53241145617"></a><a name="p53241145617"></a>Hive是一种可以存储、查询和分析存储在 Hadoop 中的大规模数据的机制。Hive定义了简单的类 SQL 查询语言，称为HiveQL，它允许熟悉SQL的用户查询数据。</p>
<p id="p1324412563"><a name="p1324412563"></a><a name="p1324412563"></a>使用MRS Hive可实现TB/PB级的数据分析，快速将线下Hadoop大数据平台（CDH、HDP等）迁移上云，业务迁移 “0”中断，业务代码 “0”改动。</p>
</td>
</tr>
<tr id="row193249111567"><td class="cellrowborder" valign="top" width="33.300000000000004%" headers="mcps1.2.3.1.1 "><p id="p1132412165613"><a name="p1132412165613"></a><a name="p1132412165613"></a>MapReduce服务（MRS Kafka）</p>
</td>
<td class="cellrowborder" valign="top" width="66.7%" headers="mcps1.2.3.1.2 "><p id="p1232411110561"><a name="p1232411110561"></a><a name="p1232411110561"></a>华为云MapReduce服务可提供专属MRS Kafka集群。Kafka是一个分布式的、分区的、多副本的消息发布-订阅系统，它提供了类似于JMS的特性，但在设计上完全不同，它具有消息持久化、高吞吐、分布式、多客户端支持、实时等特性，适用于离线和在线的消息消费，如常规的消息收集、网站活性跟踪、聚合统计系统运营数据（监控数据）、日志收集等大量数据的互联网服务的数据收集场景。</p>
</td>
</tr>
<tr id="row3518131945619"><td class="cellrowborder" valign="top" width="33.300000000000004%" headers="mcps1.2.3.1.1 "><p id="p3518419195615"><a name="p3518419195615"></a><a name="p3518419195615"></a>MapReduce服务（MRS Ranger）</p>
</td>
<td class="cellrowborder" valign="top" width="66.7%" headers="mcps1.2.3.1.2 "><p id="p11518121910567"><a name="p11518121910567"></a><a name="p11518121910567"></a>Ranger提供一个集中式安全管理框架，提供统一授权和统一审计能力。它可以对整个Hadoop生态中如HDFS、Hive、HBase、Kafka、Storm等进行细粒度的数据访问控制。用户可以利用Ranger提供的前端WebUI控制台通过配置相关策略来控制用户对这些组件的访问权限 。</p>
</td>
</tr>
<tr id="row193249110564"><td class="cellrowborder" valign="top" width="33.300000000000004%" headers="mcps1.2.3.1.1 "><p id="p1332415117569"><a name="p1332415117569"></a><a name="p1332415117569"></a>MySQL（待下线）</p>
</td>
<td class="cellrowborder" valign="top" width="66.7%" headers="mcps1.2.3.1.2 "><p id="p1332415112566"><a name="p1332415112566"></a><a name="p1332415112566"></a>MySQL是目前最受欢迎的开源数据库之一，其性能卓越，架构成熟稳定，支持流行应用程序，适用于多领域多行业，支持各种WEB应用，成本低，中小企业首选。</p>
</td>
</tr>
<tr id="row1399063515515"><td class="cellrowborder" valign="top" width="33.300000000000004%" headers="mcps1.2.3.1.1 "><p id="p10990935135520"><a name="p10990935135520"></a><a name="p10990935135520"></a>ORACLE</p>
</td>
<td class="cellrowborder" valign="top" width="66.7%" headers="mcps1.2.3.1.2 "><p id="p11576051726"><a name="p11576051726"></a><a name="p11576051726"></a>ORACLE数据库系统是以分布式数据库为核心的一组软件产品，是目前最流行的客户/服务器(CLIENT/SERVER)或B/S体系结构的数据库之一。</p>
<p id="p0990183513555"><a name="p0990183513555"></a><a name="p0990183513555"></a>ORACLE数据库是目前世界上使用最为广泛的数据库管理系统，作为一个通用的数据库系统，它具有完整的数据管理功能；作为一个关系数据库，它是一个完备关系的产品；作为分布式数据库它实现了分布式处理功能。</p>
</td>
</tr>
<tr id="row103254185617"><td class="cellrowborder" valign="top" width="33.300000000000004%" headers="mcps1.2.3.1.1 "><p id="p9325191125615"><a name="p9325191125615"></a><a name="p9325191125615"></a>MapReduce服务（MRS Spark）</p>
</td>
<td class="cellrowborder" valign="top" width="66.7%" headers="mcps1.2.3.1.2 "><p id="p332514112568"><a name="p332514112568"></a><a name="p332514112568"></a>Spark是一个开源的，并行数据处理框架，能够帮助用户简单的开发快速、统一的大数据应用，对数据进行协处理、流式处理、交互式分析等等。</p>
<p id="p532519175615"><a name="p532519175615"></a><a name="p532519175615"></a>Spark提供了一个快速的计算、写入以及交互式查询的框架。相比于Hadoop，Spark拥有明显的性能优势。Spark提供类似SQL的Spark SQL语言操作结构化数据。</p>
</td>
</tr>
<tr id="row103250118563"><td class="cellrowborder" valign="top" width="33.300000000000004%" headers="mcps1.2.3.1.1 "><p id="p6325161135619"><a name="p6325161135619"></a><a name="p6325161135619"></a>云数据库 RDS</p>
</td>
<td class="cellrowborder" valign="top" width="66.7%" headers="mcps1.2.3.1.2 "><p id="p685818353325"><a name="p685818353325"></a><a name="p685818353325"></a>华为云RDS是一种基于云计算平台的即开即用、稳定可靠、弹性伸缩、便捷管理的在线关系型数据库服务。</p>
<p id="p10325161105615"><a name="p10325161105615"></a><a name="p10325161105615"></a>注意，<span id="text142207259556"><a name="text142207259556"></a><a name="text142207259556"></a>DGC</span>平台目前仅支持RDS中的MySQL和PostgreSQL数据库。</p>
</td>
</tr>
<tr id="row1232551195616"><td class="cellrowborder" valign="top" width="33.300000000000004%" headers="mcps1.2.3.1.1 "><p id="p183259110561"><a name="p183259110561"></a><a name="p183259110561"></a>实时数据接入 DIS</p>
</td>
<td class="cellrowborder" valign="top" width="66.7%" headers="mcps1.2.3.1.2 "><p id="p132511115569"><a name="p132511115569"></a><a name="p132511115569"></a>使用实时数据接入通道，可实现跨空间作业调度。若使用数据通道连接，可以向其他帐号的DIS通道发送消息；若不使用，仅能给本帐号下所有region的通道发送消息。</p>
</td>
</tr>
<tr id="row93253118565"><td class="cellrowborder" valign="top" width="33.300000000000004%" headers="mcps1.2.3.1.1 "><p id="p432513155618"><a name="p432513155618"></a><a name="p432513155618"></a>主机连接</p>
</td>
<td class="cellrowborder" valign="top" width="66.7%" headers="mcps1.2.3.1.2 "><p id="p16325614563"><a name="p16325614563"></a><a name="p16325614563"></a>通过主机连接，用户可以在<span id="text0729226115514"><a name="text0729226115514"></a><a name="text0729226115514"></a>DGC</span>数据开发中连接到指定的主机，通过脚本开发和作业开发在主机上执行Shell脚本。主机连接保存连接某个主机的连接信息，当主机的连接信息有变化时，只需在主机连接管理中编辑修改，而不需要到具体的脚本或作业中逐一修改。</p>
</td>
</tr>
<tr id="row129881928115611"><td class="cellrowborder" valign="top" width="33.300000000000004%" headers="mcps1.2.3.1.1 "><p id="p26044285218"><a name="p26044285218"></a><a name="p26044285218"></a>MapReduce服务（MRS Presto）</p>
</td>
<td class="cellrowborder" valign="top" width="66.7%" headers="mcps1.2.3.1.2 "><p id="p953491201"><a name="p953491201"></a><a name="p953491201"></a>Presto是一个开源的用户交互式分析查询的SQL查询引擎，用于针对各种大小的数据源进行交互式分析查询。其主要应用于海量结构化数据/半结构化数据分析、海量多维数据聚合/报表、ETL、Ad-Hoc查询等场景。</p>
<p id="p195317913017"><a name="p195317913017"></a><a name="p195317913017"></a>Presto允许查询的数据源包括Hadoop分布式文件系统（HDFS），Hive，HBase，Cassandra，关系数据库甚至专有数据存储。一个Presto查询可以组合不同数据源，执行跨数据源的数据分析。</p>
</td>
</tr>
</tbody>
</table>

