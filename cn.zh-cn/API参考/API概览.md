# API概览<a name="dgc_02_0007"></a>

DGC提供的接口为符合RESTful API设计规范的自研接口。通过DGC的自研接口，您可以完整使用DGC的所有功能。

**表 1**  批量数据迁移接口说明

<a name="table2232559154016"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108272809_rcbd6963cbf0e484f9ece7459bee48cd5"><th class="cellrowborder" valign="top" width="20.14%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0108272809_p51621169582"><a name="zh-cn_topic_0108272809_p51621169582"></a><a name="zh-cn_topic_0108272809_p51621169582"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="17.76%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0108272809_a5fcf863a5c724fb5bafc395df1b24239"><a name="zh-cn_topic_0108272809_a5fcf863a5c724fb5bafc395df1b24239"></a><a name="zh-cn_topic_0108272809_a5fcf863a5c724fb5bafc395df1b24239"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="30.740000000000002%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0108272809_a4ab9480388da4ec8bc0724d32edbe658"><a name="zh-cn_topic_0108272809_a4ab9480388da4ec8bc0724d32edbe658"></a><a name="zh-cn_topic_0108272809_a4ab9480388da4ec8bc0724d32edbe658"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="31.36%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0108272809_p3213161318486"><a name="zh-cn_topic_0108272809_p3213161318486"></a><a name="zh-cn_topic_0108272809_p3213161318486"></a>用户流量限制（单位时间内的单个用户请求次数上限）</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108272809_r831c9343c1b6412fbc5fa698fbd20a3a"><td class="cellrowborder" rowspan="7" valign="top" width="20.14%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272809_p101625616586"><a name="zh-cn_topic_0108272809_p101625616586"></a><a name="zh-cn_topic_0108272809_p101625616586"></a><a href="集群管理.md">集群管理API</a></p>
</td>
<td class="cellrowborder" valign="top" width="17.76%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272809_p668332715911"><a name="zh-cn_topic_0108272809_p668332715911"></a><a name="zh-cn_topic_0108272809_p668332715911"></a>创建集群</p>
</td>
<td class="cellrowborder" valign="top" width="30.740000000000002%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272809_p115416241412"><a name="zh-cn_topic_0108272809_p115416241412"></a><a name="zh-cn_topic_0108272809_p115416241412"></a>创建CDM集群。</p>
</td>
<td class="cellrowborder" valign="top" width="31.36%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108272809_p776418524518"><a name="zh-cn_topic_0108272809_p776418524518"></a><a name="zh-cn_topic_0108272809_p776418524518"></a>5次/min</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272809_row19328462591"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272809_p1732920655917"><a name="zh-cn_topic_0108272809_p1732920655917"></a><a name="zh-cn_topic_0108272809_p1732920655917"></a>查询集群列表</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272809_p1832918635912"><a name="zh-cn_topic_0108272809_p1832918635912"></a><a name="zh-cn_topic_0108272809_p1832918635912"></a>查询并显示集群列表。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272809_p147645519452"><a name="zh-cn_topic_0108272809_p147645519452"></a><a name="zh-cn_topic_0108272809_p147645519452"></a>120次/min</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272809_row1529814222599"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272809_p112981022115917"><a name="zh-cn_topic_0108272809_p112981022115917"></a><a name="zh-cn_topic_0108272809_p112981022115917"></a>查询集群详情</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272809_p11298922145910"><a name="zh-cn_topic_0108272809_p11298922145910"></a><a name="zh-cn_topic_0108272809_p11298922145910"></a>查询集群详情。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272809_p1499020612490"><a name="zh-cn_topic_0108272809_p1499020612490"></a><a name="zh-cn_topic_0108272809_p1499020612490"></a>120次/min</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272809_row943219171593"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272809_p6433171713594"><a name="zh-cn_topic_0108272809_p6433171713594"></a><a name="zh-cn_topic_0108272809_p6433171713594"></a>重启集群</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272809_p16433151795919"><a name="zh-cn_topic_0108272809_p16433151795919"></a><a name="zh-cn_topic_0108272809_p16433151795919"></a>重启CDM集群。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272809_p109331392494"><a name="zh-cn_topic_0108272809_p109331392494"></a><a name="zh-cn_topic_0108272809_p109331392494"></a>20次/min</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272809_row152842125591"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272809_p92848121599"><a name="zh-cn_topic_0108272809_p92848121599"></a><a name="zh-cn_topic_0108272809_p92848121599"></a>删除集群</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272809_p112848121597"><a name="zh-cn_topic_0108272809_p112848121597"></a><a name="zh-cn_topic_0108272809_p112848121597"></a>删除指定CDM集群。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272809_p133292114527"><a name="zh-cn_topic_0108272809_p133292114527"></a><a name="zh-cn_topic_0108272809_p133292114527"></a>20次/min</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272809_row2073712596209"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272809_p15737145972017"><a name="zh-cn_topic_0108272809_p15737145972017"></a><a name="zh-cn_topic_0108272809_p15737145972017"></a>停止集群</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272809_p18737145918206"><a name="zh-cn_topic_0108272809_p18737145918206"></a><a name="zh-cn_topic_0108272809_p18737145918206"></a>将指定CDM集群关机。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272809_p485062110529"><a name="zh-cn_topic_0108272809_p485062110529"></a><a name="zh-cn_topic_0108272809_p485062110529"></a>20次/min</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272809_row168001843142019"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272809_p6800443152012"><a name="zh-cn_topic_0108272809_p6800443152012"></a><a name="zh-cn_topic_0108272809_p6800443152012"></a>启动集群</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272809_p17800144342014"><a name="zh-cn_topic_0108272809_p17800144342014"></a><a name="zh-cn_topic_0108272809_p17800144342014"></a>开启指定CDM集群。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272809_p16445718104915"><a name="zh-cn_topic_0108272809_p16445718104915"></a><a name="zh-cn_topic_0108272809_p16445718104915"></a>20次/min</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272809_r97d9cdac29074b28a344a0d86496d90b"><td class="cellrowborder" rowspan="4" valign="top" width="20.14%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272809_p1416276115812"><a name="zh-cn_topic_0108272809_p1416276115812"></a><a name="zh-cn_topic_0108272809_p1416276115812"></a><a href="连接管理.md">连接管理API</a></p>
</td>
<td class="cellrowborder" valign="top" width="17.76%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272809_p1162520492612"><a name="zh-cn_topic_0108272809_p1162520492612"></a><a name="zh-cn_topic_0108272809_p1162520492612"></a>创建连接</p>
</td>
<td class="cellrowborder" valign="top" width="30.740000000000002%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272809_p11795717145"><a name="zh-cn_topic_0108272809_p11795717145"></a><a name="zh-cn_topic_0108272809_p11795717145"></a>连接指定的数据源。</p>
</td>
<td class="cellrowborder" valign="top" width="31.36%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108272809_p1440511523522"><a name="zh-cn_topic_0108272809_p1440511523522"></a><a name="zh-cn_topic_0108272809_p1440511523522"></a>120次/min</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272809_row1062594912611"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272809_p261419395124"><a name="zh-cn_topic_0108272809_p261419395124"></a><a name="zh-cn_topic_0108272809_p261419395124"></a>查询连接</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272809_p166251249865"><a name="zh-cn_topic_0108272809_p166251249865"></a><a name="zh-cn_topic_0108272809_p166251249865"></a>查询连接列表。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272809_p176211024195219"><a name="zh-cn_topic_0108272809_p176211024195219"></a><a name="zh-cn_topic_0108272809_p176211024195219"></a>120次/min</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272809_row1161483912128"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272809_p20912153551214"><a name="zh-cn_topic_0108272809_p20912153551214"></a><a name="zh-cn_topic_0108272809_p20912153551214"></a>修改连接</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272809_p1261453911123"><a name="zh-cn_topic_0108272809_p1261453911123"></a><a name="zh-cn_topic_0108272809_p1261453911123"></a>修改连接的参数。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272809_p1836122519524"><a name="zh-cn_topic_0108272809_p1836122519524"></a><a name="zh-cn_topic_0108272809_p1836122519524"></a>120次/min</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272809_row10912123512121"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272809_p1494103112124"><a name="zh-cn_topic_0108272809_p1494103112124"></a><a name="zh-cn_topic_0108272809_p1494103112124"></a>删除连接</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272809_p109138355127"><a name="zh-cn_topic_0108272809_p109138355127"></a><a name="zh-cn_topic_0108272809_p109138355127"></a>删除指定连接。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272809_p205291028145213"><a name="zh-cn_topic_0108272809_p205291028145213"></a><a name="zh-cn_topic_0108272809_p205291028145213"></a>120次/min</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272809_row25964459102952"><td class="cellrowborder" rowspan="9" valign="top" width="20.14%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272809_p22746401102952"><a name="zh-cn_topic_0108272809_p22746401102952"></a><a name="zh-cn_topic_0108272809_p22746401102952"></a><a href="作业管理.md">作业管理API</a></p>
</td>
<td class="cellrowborder" valign="top" width="17.76%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272809_p30519192102952"><a name="zh-cn_topic_0108272809_p30519192102952"></a><a name="zh-cn_topic_0108272809_p30519192102952"></a>指定集群创建作业</p>
</td>
<td class="cellrowborder" valign="top" width="30.740000000000002%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272809_p56135479102952"><a name="zh-cn_topic_0108272809_p56135479102952"></a><a name="zh-cn_topic_0108272809_p56135479102952"></a>在指定的CDM集群上创建数据迁移任务，作业不会启动。</p>
</td>
<td class="cellrowborder" valign="top" width="31.36%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108272809_p119611056105215"><a name="zh-cn_topic_0108272809_p119611056105215"></a><a name="zh-cn_topic_0108272809_p119611056105215"></a>1200次/min</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272809_row1172354525"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272809_p1572515419214"><a name="zh-cn_topic_0108272809_p1572515419214"></a><a name="zh-cn_topic_0108272809_p1572515419214"></a>随机集群创建作业并执行</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272809_p1372514529"><a name="zh-cn_topic_0108272809_p1372514529"></a><a name="zh-cn_topic_0108272809_p1372514529"></a>在指定的CDM集群列表中，随机选择一个开机状态的集群，在该集群中创建作业并执行作业。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272809_p46481657165215"><a name="zh-cn_topic_0108272809_p46481657165215"></a><a name="zh-cn_topic_0108272809_p46481657165215"></a>120次/min</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272809_row1576002410306"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272809_p5386732610306"><a name="zh-cn_topic_0108272809_p5386732610306"></a><a name="zh-cn_topic_0108272809_p5386732610306"></a>查询作业</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272809_p117731710306"><a name="zh-cn_topic_0108272809_p117731710306"></a><a name="zh-cn_topic_0108272809_p117731710306"></a>查询并显示作业列表。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272809_p969563695210"><a name="zh-cn_topic_0108272809_p969563695210"></a><a name="zh-cn_topic_0108272809_p969563695210"></a>120次/min</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272809_row1210575410309"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272809_p3607132810309"><a name="zh-cn_topic_0108272809_p3607132810309"></a><a name="zh-cn_topic_0108272809_p3607132810309"></a>修改作业</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272809_p3609642710309"><a name="zh-cn_topic_0108272809_p3609642710309"></a><a name="zh-cn_topic_0108272809_p3609642710309"></a>修改作业的参数。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272809_p7550137105215"><a name="zh-cn_topic_0108272809_p7550137105215"></a><a name="zh-cn_topic_0108272809_p7550137105215"></a>120次/min</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272809_row34472636103012"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272809_p18094461103012"><a name="zh-cn_topic_0108272809_p18094461103012"></a><a name="zh-cn_topic_0108272809_p18094461103012"></a>启动作业</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272809_p56365238103012"><a name="zh-cn_topic_0108272809_p56365238103012"></a><a name="zh-cn_topic_0108272809_p56365238103012"></a>启动数据迁移的任务。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272809_p34787017538"><a name="zh-cn_topic_0108272809_p34787017538"></a><a name="zh-cn_topic_0108272809_p34787017538"></a>1200次/min</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272809_row14941532103156"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272809_p52451665103156"><a name="zh-cn_topic_0108272809_p52451665103156"></a><a name="zh-cn_topic_0108272809_p52451665103156"></a>停止作业</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272809_p20726438103156"><a name="zh-cn_topic_0108272809_p20726438103156"></a><a name="zh-cn_topic_0108272809_p20726438103156"></a>停止运行中的作业。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272809_p16177115534"><a name="zh-cn_topic_0108272809_p16177115534"></a><a name="zh-cn_topic_0108272809_p16177115534"></a>1200次/min</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272809_row1744768310320"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272809_p5363966910320"><a name="zh-cn_topic_0108272809_p5363966910320"></a><a name="zh-cn_topic_0108272809_p5363966910320"></a>查询作业状态</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272809_p4984589410320"><a name="zh-cn_topic_0108272809_p4984589410320"></a><a name="zh-cn_topic_0108272809_p4984589410320"></a>查询并显示作业的运行状态。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272809_p639244219525"><a name="zh-cn_topic_0108272809_p639244219525"></a><a name="zh-cn_topic_0108272809_p639244219525"></a>120次/min</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272809_row3000249810324"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272809_p1609414910324"><a name="zh-cn_topic_0108272809_p1609414910324"></a><a name="zh-cn_topic_0108272809_p1609414910324"></a>查询作业执行历史</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272809_p2855767310324"><a name="zh-cn_topic_0108272809_p2855767310324"></a><a name="zh-cn_topic_0108272809_p2855767310324"></a>查询并显示作业执行的历史状态。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272809_p62911843145219"><a name="zh-cn_topic_0108272809_p62911843145219"></a><a name="zh-cn_topic_0108272809_p62911843145219"></a>120次/min</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272809_row1942734110327"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272809_p2305383310327"><a name="zh-cn_topic_0108272809_p2305383310327"></a><a name="zh-cn_topic_0108272809_p2305383310327"></a>删除作业</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272809_p5542115710327"><a name="zh-cn_topic_0108272809_p5542115710327"></a><a name="zh-cn_topic_0108272809_p5542115710327"></a>删除指定作业。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272809_p1593254310522"><a name="zh-cn_topic_0108272809_p1593254310522"></a><a name="zh-cn_topic_0108272809_p1593254310522"></a>120次/min</p>
</td>
</tr>
</tbody>
</table>

**表 2**  实时数据接入接口说明

<a name="table5304152314427"></a>
<table><thead align="left"><tr id="row830412314216"><th class="cellrowborder" valign="top" width="17.080000000000002%" id="mcps1.2.3.1.1"><p id="p1430492364213"><a name="p1430492364213"></a><a name="p1430492364213"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="82.92%" id="mcps1.2.3.1.2"><p id="p13051238428"><a name="p13051238428"></a><a name="p13051238428"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row11305023134214"><td class="cellrowborder" valign="top" width="17.080000000000002%" headers="mcps1.2.3.1.1 "><p id="p5305112364216"><a name="p5305112364216"></a><a name="p5305112364216"></a><a href="通道管理.md">通道管理</a></p>
</td>
<td class="cellrowborder" valign="top" width="82.92%" headers="mcps1.2.3.1.2 "><p id="p5305123184216"><a name="p5305123184216"></a><a name="p5305123184216"></a>可实现通道创建、列表查询、删除、修改分区数量和更新信息，查询通道列表，查询通道详情等操作。</p>
</td>
</tr>
<tr id="row1730522319423"><td class="cellrowborder" valign="top" width="17.080000000000002%" headers="mcps1.2.3.1.1 "><p id="p17305112364210"><a name="p17305112364210"></a><a name="p17305112364210"></a><a href="App管理.md">App管理</a></p>
</td>
<td class="cellrowborder" valign="top" width="82.92%" headers="mcps1.2.3.1.2 "><p id="p143051523164216"><a name="p143051523164216"></a><a name="p143051523164216"></a>可实现APP的创建、查询、删除、查看APP详情和消费状态等操作。</p>
</td>
</tr>
<tr id="row6419125914458"><td class="cellrowborder" valign="top" width="17.080000000000002%" headers="mcps1.2.3.1.1 "><p id="p442025911454"><a name="p442025911454"></a><a name="p442025911454"></a><a href="Checkpoint管理.md">Checkpoint管理</a></p>
</td>
<td class="cellrowborder" valign="top" width="82.92%" headers="mcps1.2.3.1.2 "><p id="p1342020593452"><a name="p1342020593452"></a><a name="p1342020593452"></a>可实现Checkpoint的提交、查询、删除等操作。</p>
</td>
</tr>
<tr id="row9305182318422"><td class="cellrowborder" valign="top" width="17.080000000000002%" headers="mcps1.2.3.1.1 "><p id="p130592344215"><a name="p130592344215"></a><a name="p130592344215"></a><a href="数据管理.md">数据管理</a></p>
</td>
<td class="cellrowborder" valign="top" width="82.92%" headers="mcps1.2.3.1.2 "><p id="p830512394215"><a name="p830512394215"></a><a name="p830512394215"></a>可实现数据的上传、下载、获取游标等操作。</p>
</td>
</tr>
<tr id="row12305123164217"><td class="cellrowborder" valign="top" width="17.080000000000002%" headers="mcps1.2.3.1.1 "><p id="p130512394219"><a name="p130512394219"></a><a name="p130512394219"></a><a href="转储任务管理.md">转储任务管理</a></p>
</td>
<td class="cellrowborder" valign="top" width="82.92%" headers="mcps1.2.3.1.2 "><p id="p16305122394210"><a name="p16305122394210"></a><a name="p16305122394210"></a>可实现转储任务的添加、查询、删除、批量启动等操作 。</p>
</td>
</tr>
<tr id="row1349017387471"><td class="cellrowborder" valign="top" width="17.080000000000002%" headers="mcps1.2.3.1.1 "><p id="p19491538184716"><a name="p19491538184716"></a><a name="p19491538184716"></a><a href="监控管理.md">监控管理</a></p>
</td>
<td class="cellrowborder" valign="top" width="82.92%" headers="mcps1.2.3.1.2 "><p id="p549173810476"><a name="p549173810476"></a><a name="p549173810476"></a>可实现查询通道监控、查询分区监控操作。</p>
</td>
</tr>
<tr id="row538455113473"><td class="cellrowborder" valign="top" width="17.080000000000002%" headers="mcps1.2.3.1.1 "><p id="p5384135111478"><a name="p5384135111478"></a><a name="p5384135111478"></a><a href="标签管理.md">标签管理</a></p>
</td>
<td class="cellrowborder" valign="top" width="82.92%" headers="mcps1.2.3.1.2 "><p id="p1294556174816"><a name="p1294556174816"></a><a name="p1294556174816"></a>可实现标签的添加、查询、删除、批量处理等操作 。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  数据开发接口说明

<a name="zh-cn_topic_0181281314_table3537164813475"></a>
<table><thead align="left"><tr id="zh-cn_topic_0181281314_row3537154813475"><th class="cellrowborder" valign="top" width="17.080000000000002%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0181281314_p7538144814714"><a name="zh-cn_topic_0181281314_p7538144814714"></a><a name="zh-cn_topic_0181281314_p7538144814714"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="82.92%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0181281314_p5538104834711"><a name="zh-cn_topic_0181281314_p5538104834711"></a><a name="zh-cn_topic_0181281314_p5538104834711"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0181281314_row65381348194716"><td class="cellrowborder" valign="top" width="17.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0181281314_p25381148174716"><a name="zh-cn_topic_0181281314_p25381148174716"></a><a name="zh-cn_topic_0181281314_p25381148174716"></a><a href="连接管理API.md">连接管理API</a></p>
</td>
<td class="cellrowborder" valign="top" width="82.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0181281314_p145381548194717"><a name="zh-cn_topic_0181281314_p145381548194717"></a><a name="zh-cn_topic_0181281314_p145381548194717"></a>可实现创建、编辑、删除、导入和导出连接，查询连接列表，查询连接详情等操作。对应用户指南手册的“数据开发 &gt; 数据管理 &gt; 创建数据连接”操作。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281314_row6538144810473"><td class="cellrowborder" valign="top" width="17.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0181281314_p1753824844710"><a name="zh-cn_topic_0181281314_p1753824844710"></a><a name="zh-cn_topic_0181281314_p1753824844710"></a><a href="脚本开发API.md">脚本开发API</a></p>
</td>
<td class="cellrowborder" valign="top" width="82.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0181281314_p053884834718"><a name="zh-cn_topic_0181281314_p053884834718"></a><a name="zh-cn_topic_0181281314_p053884834718"></a>可实现创建、查询、修改、删除、执行脚本等操作。对应用户指南手册的“数据开发 &gt; 脚本开发”操作。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281314_row1453815486472"><td class="cellrowborder" valign="top" width="17.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0181281314_p1153884812475"><a name="zh-cn_topic_0181281314_p1153884812475"></a><a name="zh-cn_topic_0181281314_p1153884812475"></a><a href="资源管理API.md">资源管理API</a></p>
</td>
<td class="cellrowborder" valign="top" width="82.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0181281314_p10538448154717"><a name="zh-cn_topic_0181281314_p10538448154717"></a><a name="zh-cn_topic_0181281314_p10538448154717"></a>可实现创建、查询、修改资源等操作。对应用户指南手册的“数据开发 &gt; 配置管理 &gt; 管理资源”操作。</p>
</td>
</tr>
<tr id="zh-cn_topic_0181281314_row175381848114710"><td class="cellrowborder" valign="top" width="17.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0181281314_p1753874816477"><a name="zh-cn_topic_0181281314_p1753874816477"></a><a name="zh-cn_topic_0181281314_p1753874816477"></a><a href="作业开发API.md">作业开发API</a></p>
</td>
<td class="cellrowborder" valign="top" width="82.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0181281314_p2053884813479"><a name="zh-cn_topic_0181281314_p2053884813479"></a><a name="zh-cn_topic_0181281314_p2053884813479"></a>可实现创建、编辑、删除、导入导出作业，查询作业列表，查询作业详情等操作 。对应用户指南手册的“数据开发 &gt; 作业开发”操作。</p>
</td>
</tr>
</tbody>
</table>

