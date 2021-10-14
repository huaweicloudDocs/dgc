# DGC使用简介<a name="dgc_01_0007"></a>

数据湖治理中心DGC是具有数据全生命周期管理、智能数据管理能力的一站式治理运营平台，支持行业知识库智能化建设，支持大数据存储、大数据计算分析引擎等数据底座，帮助企业快速构建从数据接入到数据分析的端到端智能数据系统，消除数据孤岛，统一数据标准，加快数据变现，实现数字化转型。

## 使用DGC的用户<a name="section43921341113716"></a>

根据人员的职能进行划分，使用DGC的用户主要可以分为以下四类。四类角色具有不同的DGC权限，详情请参见[DGC权限列表](https://support.huaweicloud.com/productdesc-dgc/dgc_07_013.html)章节。

-   **管理员**

    面向熟悉业务并具有管理、决策、审核权限的管理人员。管理员具有除创建工作空间之外的其他所有DGC权限，包括开发者权限、审核人员权限、工作空间管理、数据资产管理、配置管理等权限。例如，在规范设计、数据服务模块中，审核人员可以对开发人员发布的数据模型、API等数据对象进行审核，把好质量关。

-   **开发者**

    面向数据建模师、熟悉脚本开发的开发人员。DGC为开发者提供了从管理中心、规范设计、数据集成、数据开发、数据质量、数据资产到数据服务的端到端开发和运营流程，帮助您快速、简单且高效地构建一个智能数据系统。

    数据系统构建完成后，其他开发人员就可以通过SDK的方式调用DGC提供的数据服务API进行数据分析。

    开发者具有除审核人员权限、工作空间及其成员管理等少数权限以外的大部分DGC权限。

-   **运维者**

    面向运维人员。运维者主要具有查看详细信息、运维调度、资源监控等权限。DGC的数据资产360度全链路可视化，数据质量可检验，数据使用可控、可追溯，帮助运维人员实现端到端的作业调度和监控，从数据采集到数据消费运维一条龙服务。

-   **访客**

    访客仅具备只读权限，可以查看详细信息。


## DGC使用流程简介<a name="section937732811212"></a>

DGC典型的端到端开发流程如下图所示：

**图 1**  DGC使用流程<a name="zh-cn_topic_0262779560_fig1392611412814"></a>  
![](figures/DGC使用流程.png "DGC使用流程")

使用DGC平台，通常包括以下步骤：

**表 1**  DGC全流程开发

<a name="table131731252131219"></a>
<table><thead align="left"><tr id="row15174155213125"><th class="cellrowborder" valign="top" width="18.45815418458154%" id="mcps1.2.5.1.1"><p id="p1730191810136"><a name="p1730191810136"></a><a name="p1730191810136"></a>主流程</p>
</th>
<th class="cellrowborder" valign="top" width="41.4058594140586%" id="mcps1.2.5.1.2"><p id="p562892914489"><a name="p562892914489"></a><a name="p562892914489"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="16.52834716528347%" id="mcps1.2.5.1.3"><p id="p2174205271213"><a name="p2174205271213"></a><a name="p2174205271213"></a>子任务</p>
</th>
<th class="cellrowborder" valign="top" width="23.607639236076395%" id="mcps1.2.5.1.4"><p id="p917425218125"><a name="p917425218125"></a><a name="p917425218125"></a>操作指导</p>
</th>
</tr>
</thead>
<tbody><tr id="row1456331035312"><td class="cellrowborder" rowspan="4" valign="top" width="18.45815418458154%" headers="mcps1.2.5.1.1 "><p id="p16892627141417"><a name="p16892627141417"></a><a name="p16892627141417"></a>使用前的准备</p>
</td>
<td class="cellrowborder" valign="top" width="41.4058594140586%" headers="mcps1.2.5.1.2 "><p id="p14628132913484"><a name="p14628132913484"></a><a name="p14628132913484"></a>如果您是第一次使用<span id="text171526335323"><a name="text171526335323"></a><a name="text171526335323"></a>DGC</span>，需要先完成<span id="text853025518181"><a name="text853025518181"></a><a name="text853025518181"></a>注册</span>华为云帐号、<span id="text38751336198"><a name="text38751336198"></a><a name="text38751336198"></a>购买</span><span id="text940193815323"><a name="text940193815323"></a><a name="text940193815323"></a>DGC</span>实例、创建工作空间、创建用户并授予<span id="text12878183913214"><a name="text12878183913214"></a><a name="text12878183913214"></a>DGC</span>权限、添加工作空间成员和角色等一系列操作。</p>
</td>
<td class="cellrowborder" valign="top" width="16.52834716528347%" headers="mcps1.2.5.1.3 "><p id="p18666915164912"><a name="p18666915164912"></a><a name="p18666915164912"></a>准备工作</p>
</td>
<td class="cellrowborder" valign="top" width="23.607639236076395%" headers="mcps1.2.5.1.4 "><p id="p11564141045315"><a name="p11564141045315"></a><a name="p11564141045315"></a><a href="使用DGC前的准备.md#section485519219101">DGC准备工作</a></p>
</td>
</tr>
<tr id="row13662152114170"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="p4668421959"><a name="p4668421959"></a><a name="p4668421959"></a>获取数据源的连接地址等信息，并确保数据源所在的主机和华为云网络互通。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p17668521159"><a name="p17668521159"></a><a name="p17668521159"></a>准备数据源</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="p366842652"><a name="p366842652"></a><a name="p366842652"></a><a href="使用DGC前的准备.md#section104811741192013">准备数据源</a></p>
</td>
</tr>
<tr id="row151252519188"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="p134432015141210"><a name="p134432015141210"></a><a name="p134432015141210"></a>根据业务场景选择符合需求的云服务作为数据湖，用于存储原始数据和数据治理过程中的数据，并进行数据开发、治理和运营。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p1551517954"><a name="p1551517954"></a><a name="p1551517954"></a>准备数据湖</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="p1515271255"><a name="p1515271255"></a><a name="p1515271255"></a><a href="使用DGC前的准备.md#section19482194142011">准备数据湖</a></p>
</td>
</tr>
<tr id="row17174185211125"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="p662962911486"><a name="p662962911486"></a><a name="p662962911486"></a>根据自身的业务特点和源数据类型，进行数据存储与分析系统的选型，选取合适的云服务用于存储源数据并进行数据查询和分析。然后，创建该云服务相应的数据连接。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p8666715124914"><a name="p8666715124914"></a><a name="p8666715124914"></a>创建数据连接</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="p9926173019435"><a name="p9926173019435"></a><a name="p9926173019435"></a><a href="创建数据连接.md">创建数据连接</a></p>
</td>
</tr>
<tr id="row1017416527122"><td class="cellrowborder" valign="top" width="18.45815418458154%" headers="mcps1.2.5.1.1 "><p id="p7548152218151"><a name="p7548152218151"></a><a name="p7548152218151"></a>数据集成（批量数据迁移）</p>
</td>
<td class="cellrowborder" valign="top" width="41.4058594140586%" headers="mcps1.2.5.1.2 "><p id="p1786911508476"><a name="p1786911508476"></a><a name="p1786911508476"></a>通过<span id="text1574164363217"><a name="text1574164363217"></a><a name="text1574164363217"></a>DGC</span>平台将源数据上传或者接入到云上。</p>
<p id="p102441698522"><a name="p102441698522"></a><a name="p102441698522"></a>批量数据迁移提供同构/异构数据源之间批量数据迁移的服务，支持自建和云上的文件系统，关系数据库，数据仓库，NoSQL，大数据云服务，对象存储等数据源。</p>
</td>
<td class="cellrowborder" valign="top" width="16.52834716528347%" headers="mcps1.2.5.1.3 "><p id="p155631014851"><a name="p155631014851"></a><a name="p155631014851"></a>批量数据迁移</p>
</td>
<td class="cellrowborder" valign="top" width="23.607639236076395%" headers="mcps1.2.5.1.4 "><p id="p1128213481854"><a name="p1128213481854"></a><a name="p1128213481854"></a><a href="支持的数据源.md">支持的数据源</a></p>
<p id="p1262317115385"><a name="p1262317115385"></a><a name="p1262317115385"></a><a href="创建集群.md">创建集群</a></p>
<p id="p596205813612"><a name="p596205813612"></a><a name="p596205813612"></a><a href="创建连接.md">创建连接</a></p>
<p id="p10795153111713"><a name="p10795153111713"></a><a name="p10795153111713"></a><a href="创建作业.md">创建作业</a></p>
</td>
</tr>
<tr id="row1399813106420"><td class="cellrowborder" valign="top" width="18.45815418458154%" headers="mcps1.2.5.1.1 "><p id="p19384653175114"><a name="p19384653175114"></a><a name="p19384653175114"></a>数据集成（实时数据接入）</p>
</td>
<td class="cellrowborder" valign="top" width="41.4058594140586%" headers="mcps1.2.5.1.2 "><p id="p530372116523"><a name="p530372116523"></a><a name="p530372116523"></a>通过<span id="text203037214529"><a name="text203037214529"></a><a name="text203037214529"></a>DGC</span>平台将源数据上传或者接入到云上。</p>
<p id="p167582515527"><a name="p167582515527"></a><a name="p167582515527"></a>实时数据接入可以将云下的实时数据接入到云服务中。</p>
</td>
<td class="cellrowborder" valign="top" width="16.52834716528347%" headers="mcps1.2.5.1.3 "><p id="p153401916456"><a name="p153401916456"></a><a name="p153401916456"></a>实时数据接入</p>
</td>
<td class="cellrowborder" valign="top" width="23.607639236076395%" headers="mcps1.2.5.1.4 "><p id="dgc_01_0007_p189987108413"><a name="dgc_01_0007_p189987108413"></a><a name="dgc_01_0007_p189987108413"></a><a href="实时数据接入快速入门.md#section12577139103116">按需计费方式购买实时数据接入的增量包</a></p>
<p id="p49375011101"><a name="p49375011101"></a><a name="p49375011101"></a><a href="实时数据接入快速入门.md">实时数据接入快速入门</a></p>
</td>
</tr>
<tr id="row10465165318372"><td class="cellrowborder" valign="top" width="18.45815418458154%" headers="mcps1.2.5.1.1 "><p id="p2465953203719"><a name="p2465953203719"></a><a name="p2465953203719"></a>数据资产采集</p>
</td>
<td class="cellrowborder" valign="top" width="41.4058594140586%" headers="mcps1.2.5.1.2 "><p id="p1136911633413"><a name="p1136911633413"></a><a name="p1136911633413"></a>为了在<span id="text55751944163213"><a name="text55751944163213"></a><a name="text55751944163213"></a>DGC</span>平台中对迁移到云上的原始数据层进行管理和监控，先对其元数据进行采集并监控。</p>
</td>
<td class="cellrowborder" valign="top" width="16.52834716528347%" headers="mcps1.2.5.1.3 "><p id="p4369196123418"><a name="p4369196123418"></a><a name="p4369196123418"></a>元数据采集</p>
</td>
<td class="cellrowborder" valign="top" width="23.607639236076395%" headers="mcps1.2.5.1.4 "><p id="p173691062346"><a name="p173691062346"></a><a name="p173691062346"></a><a href="元数据采集.md">元数据采集</a></p>
</td>
</tr>
<tr id="row820133914351"><td class="cellrowborder" rowspan="7" valign="top" width="18.45815418458154%" headers="mcps1.2.5.1.1 "><p id="p42083993519"><a name="p42083993519"></a><a name="p42083993519"></a>规范设计</p>
</td>
<td class="cellrowborder" rowspan="7" valign="top" width="41.4058594140586%" headers="mcps1.2.5.1.2 "><p id="p1699641143814"><a name="p1699641143814"></a><a name="p1699641143814"></a>规范设计以关系建模、维度建模理论支撑实现规范化、可视化、标准化数据模型开发，定位于数据治理流程设计落地阶段，输出成果用于指导开发人员实践落地数据治理方法论。</p>
<p id="p20932545173616"><a name="p20932545173616"></a><a name="p20932545173616"></a>根据业务需求设计关系模型、维度模型，在规范设计模块中，一步一步建立模型中的对象，例如维度、事实表、指标、汇总表等。</p>
</td>
<td class="cellrowborder" valign="top" width="16.52834716528347%" headers="mcps1.2.5.1.3 "><p id="p129321145143614"><a name="p129321145143614"></a><a name="p129321145143614"></a>规范设计实施流程</p>
</td>
<td class="cellrowborder" valign="top" width="23.607639236076395%" headers="mcps1.2.5.1.4 "><p id="p14906325103611"><a name="p14906325103611"></a><a name="p14906325103611"></a><a href="数据规范使用流程.md">数据规范使用流程</a></p>
</td>
</tr>
<tr id="row421810157363"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="p373513206367"><a name="p373513206367"></a><a name="p373513206367"></a>添加审核人</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p1573612204369"><a name="p1573612204369"></a><a name="p1573612204369"></a><a href="添加审核人.md#zh-cn_topic_0190201557_section128061611164613">添加审核人</a></p>
</td>
</tr>
<tr id="row993085711353"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="p1193294514361"><a name="p1193294514361"></a><a name="p1193294514361"></a>主题设计</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p1093234515369"><a name="p1093234515369"></a><a name="p1093234515369"></a><a href="主题设计.md">主题设计</a></p>
</td>
</tr>
<tr id="row04039115367"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="p2093234514365"><a name="p2093234514365"></a><a name="p2093234514365"></a>码表管理</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p15932545163611"><a name="p15932545163611"></a><a name="p15932545163611"></a><a href="新建码表.md">新建码表</a></p>
</td>
</tr>
<tr id="row174203453616"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="p15932945103610"><a name="p15932945103610"></a><a name="p15932945103610"></a>制定数据标准</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p1393274510362"><a name="p1393274510362"></a><a name="p1393274510362"></a><a href="新建数据标准.md">新建数据标准</a></p>
</td>
</tr>
<tr id="row399886362"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="p6932204563610"><a name="p6932204563610"></a><a name="p6932204563610"></a>关系建模</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p18932174518366"><a name="p18932174518366"></a><a name="p18932174518366"></a><a href="关系建模.md">关系建模</a></p>
</td>
</tr>
<tr id="row12162711113618"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="p18932145133618"><a name="p18932145133618"></a><a name="p18932145133618"></a>维度建模</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p6783410175615"><a name="p6783410175615"></a><a name="p6783410175615"></a><a href="维度建模.md">维度建模</a></p>
</td>
</tr>
<tr id="row1666715816395"><td class="cellrowborder" rowspan="4" valign="top" width="18.45815418458154%" headers="mcps1.2.5.1.1 "><p id="p96670811398"><a name="p96670811398"></a><a name="p96670811398"></a>数据开发</p>
</td>
<td class="cellrowborder" rowspan="4" valign="top" width="41.4058594140586%" headers="mcps1.2.5.1.2 "><p id="p4667158163912"><a name="p4667158163912"></a><a name="p4667158163912"></a>可管理多种大数据服务，提供一站式的大数据开发环境。</p>
<p id="p3963256215128"><a name="p3963256215128"></a><a name="p3963256215128"></a>使用<span id="text151877469328"><a name="text151877469328"></a><a name="text151877469328"></a>DGC</span>数据开发，用户可进行数据管理、数据集成、脚本开发、作业开发、作业调度、运维监控等操作，轻松完成整个数据的处理分析流程。</p>
</td>
<td class="cellrowborder" valign="top" width="16.52834716528347%" headers="mcps1.2.5.1.3 "><p id="p20667689395"><a name="p20667689395"></a><a name="p20667689395"></a>数据管理</p>
</td>
<td class="cellrowborder" valign="top" width="23.607639236076395%" headers="mcps1.2.5.1.4 "><p id="p966718203917"><a name="p966718203917"></a><a name="p966718203917"></a><a href="数据管理.md">数据管理</a></p>
</td>
</tr>
<tr id="row11175185281217"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="p46665157492"><a name="p46665157492"></a><a name="p46665157492"></a>脚本开发</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p14157901386"><a name="p14157901386"></a><a name="p14157901386"></a><a href="脚本开发.md">脚本开发</a></p>
</td>
</tr>
<tr id="row438118613100"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="p1221163201119"><a name="p1221163201119"></a><a name="p1221163201119"></a>作业开发</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p338166141010"><a name="p338166141010"></a><a name="p338166141010"></a><a href="作业开发.md">作业开发</a></p>
</td>
</tr>
<tr id="row200141463911"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="p1101014103915"><a name="p1101014103915"></a><a name="p1101014103915"></a>运维调度</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p30151420398"><a name="p30151420398"></a><a name="p30151420398"></a><a href="运维调度.md">运维调度</a></p>
</td>
</tr>
<tr id="row91757521121"><td class="cellrowborder" rowspan="2" valign="top" width="18.45815418458154%" headers="mcps1.2.5.1.1 "><p id="p18102154211510"><a name="p18102154211510"></a><a name="p18102154211510"></a>数据质量监控</p>
</td>
<td class="cellrowborder" rowspan="2" valign="top" width="41.4058594140586%" headers="mcps1.2.5.1.2 "><p id="p1689361711417"><a name="p1689361711417"></a><a name="p1689361711417"></a>对业务指标和数据指标进行监控。您可从完整性、有效性、及时性、一致性、准确性、唯一性六个维度进行单列、跨列、跨行和跨表的分析。支持数据的清洗和标准化，能够根据数据标准自动生成清洗和标准化的质量规则。支持周期性的监控和清洗。</p>
</td>
<td class="cellrowborder" valign="top" width="16.52834716528347%" headers="mcps1.2.5.1.3 "><p id="p14666191554916"><a name="p14666191554916"></a><a name="p14666191554916"></a>业务指标监控</p>
</td>
<td class="cellrowborder" valign="top" width="23.607639236076395%" headers="mcps1.2.5.1.4 "><p id="p8395655171014"><a name="p8395655171014"></a><a name="p8395655171014"></a><a href="新建指标.md">新建指标</a></p>
<p id="p11894205714101"><a name="p11894205714101"></a><a name="p11894205714101"></a><a href="新建规则.md">新建规则</a></p>
<p id="p16838155981015"><a name="p16838155981015"></a><a name="p16838155981015"></a><a href="新建业务场景.md">新建业务场景</a></p>
</td>
</tr>
<tr id="row317391381311"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="p11738133134"><a name="p11738133134"></a><a name="p11738133134"></a>数据质量监控</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p890711151120"><a name="p890711151120"></a><a name="p890711151120"></a><a href="新建规则模板.md">新建规则模板</a></p>
<p id="p656314421112"><a name="p656314421112"></a><a name="p656314421112"></a><a href="新建质量作业.md">新建质量作业</a></p>
<p id="p1249212621111"><a name="p1249212621111"></a><a name="p1249212621111"></a><a href="新建对账作业.md">新建对账作业</a></p>
</td>
</tr>
<tr id="row1175952191216"><td class="cellrowborder" valign="top" width="18.45815418458154%" headers="mcps1.2.5.1.1 "><p id="p1230271881319"><a name="p1230271881319"></a><a name="p1230271881319"></a>数据资产管理</p>
</td>
<td class="cellrowborder" valign="top" width="41.4058594140586%" headers="mcps1.2.5.1.2 "><p id="p17505131103914"><a name="p17505131103914"></a><a name="p17505131103914"></a>在<span id="text1025117136333"><a name="text1025117136333"></a><a name="text1025117136333"></a>DGC</span>数据资产模块中，您可以查看数据地图，还可以对数据资产进行数据权限管理。</p>
</td>
<td class="cellrowborder" valign="top" width="16.52834716528347%" headers="mcps1.2.5.1.3 "><p id="p18666111516493"><a name="p18666111516493"></a><a name="p18666111516493"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="23.607639236076395%" headers="mcps1.2.5.1.4 "><p id="p8355621143918"><a name="p8355621143918"></a><a name="p8355621143918"></a><a href="数据地图.md">数据地图</a></p>
<p id="p1275758164016"><a name="p1275758164016"></a><a name="p1275758164016"></a><a href="数据权限.md">数据权限</a></p>
</td>
</tr>
<tr id="row16175135213125"><td class="cellrowborder" rowspan="2" valign="top" width="18.45815418458154%" headers="mcps1.2.5.1.1 "><p id="p596917971610"><a name="p596917971610"></a><a name="p596917971610"></a>数据服务API开发</p>
</td>
<td class="cellrowborder" rowspan="2" valign="top" width="41.4058594140586%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0179716868_p144281149208"><a name="zh-cn_topic_0179716868_p144281149208"></a><a name="zh-cn_topic_0179716868_p144281149208"></a>统一管理对内对外的API服务，提供快速将数据表生成数据API的能力，同时支持将现有的API快速注册到数据服务平台以统一管理和发布。</p>
</td>
<td class="cellrowborder" valign="top" width="16.52834716528347%" headers="mcps1.2.5.1.3 "><p id="p1766617155495"><a name="p1766617155495"></a><a name="p1766617155495"></a>开发API</p>
</td>
<td class="cellrowborder" valign="top" width="23.607639236076395%" headers="mcps1.2.5.1.4 "><p id="p8175552111215"><a name="p8175552111215"></a><a name="p8175552111215"></a><a href="准备工作-9.md">准备工作</a></p>
<p id="p1587616505279"><a name="p1587616505279"></a><a name="p1587616505279"></a><a href="创建API.md">创建API</a></p>
<p id="p1877135015271"><a name="p1877135015271"></a><a name="p1877135015271"></a><a href="调试API.md">调试API</a></p>
<p id="p78771650202719"><a name="p78771650202719"></a><a name="p78771650202719"></a><a href="发布API.md">发布API</a></p>
<p id="p1857619580413"><a name="p1857619580413"></a><a name="p1857619580413"></a><a href="管理API.md">管理API</a></p>
<p id="p39931219425"><a name="p39931219425"></a><a name="p39931219425"></a><a href="流量控制.md">流量控制</a></p>
</td>
</tr>
<tr id="row16249320151713"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="p15250122015178"><a name="p15250122015178"></a><a name="p15250122015178"></a>调用API</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="p1782275012178"><a name="p1782275012178"></a><a name="p1782275012178"></a><a href="调用API.md">调用API</a></p>
</td>
</tr>
</tbody>
</table>

