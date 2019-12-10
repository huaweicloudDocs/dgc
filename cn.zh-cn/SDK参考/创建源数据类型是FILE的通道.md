# 创建源数据类型是FILE的通道<a name="dayu_06_0079"></a>

```
// 通道名称
char *pucStreamName = "myStream";
char *projectId = "d575b0b740e54221aeb9a165653b103d";
char *region = "southchina";
char *host = "XXX.XXX.XXX.XXX:XXX";
int ret = 0;
DISResponseInfo RspInfo = { 0 };
DISCreateStream *pstCreateStream = disMemAlloc(sizeof(DISCreateStream));
DISCreateStreamExpend *pstCreateStreamExpend = disMemAlloc(sizeof(DISCreateStreamExpend));

ObsDestinationDescriptor *pstObsDestinationDescriptor = disMemAlloc(sizeof(ObsDestinationDescriptor));
pstObsDestinationDescriptor->agencyName = "all";
pstObsDestinationDescriptor->obs_bucketPath = "obs-shawn";

pstCreateStreamExpend->dataType = DISDataTypeFile;
pstCreateStreamExpend->dataDuration = 3 * 24;
pstCreateStreamExpend->obsDestinationDescriptor = *pstObsDestinationDescriptor;

pstCreateStream->partitionCount = 10;
pstCreateStream->streamName = pucStreamName;
pstCreateStream->streamType = DISStreamTypeAdvanced;
pstCreateStream->pucReserved = pstCreateStreamExpend;

printf("===================%s Begin=======================\n", __FUNCTION__);
ret = CreateStream(host, projectId, region, pstCreateStream, &RspInfo);
if (ret != 0)
{
printf("Create Error: %d\r\n", ret);
printf("HttpResponseCode: %ld\r\n", RspInfo.HttpResponseCode);
printf("ErrorCode: %s\r\n", RspInfo.ErrorCode);
printf("ErrorDetail: %s\r\n", RspInfo.ErrorDetail);
}
else
{
printf("Create stream %s success\n", pstCreateStream->streamName);
printf("HttpResponseCode: %ld\r\n", RspInfo.HttpResponseCode);
}

disMemFree(pstCreateStream);
printf("===================%s End=======================\n", __FUNCTION__);
```

配置“DISCreateStream”对象之后，通过调用CreateStream的方法创建通道。

```
ret = CreateStream(host, projectId, region, pstCreateStream, &RspInfo);
```

## 运行结果<a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_section65958035"></a>

可以在控制台查看到类似如下信息：

```
Create stream myStream success
HttpResponseCode: 201
```

**表 1**  DISCreateStream的参数说明

<a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_table20074930"></a>
<table><thead align="left"><tr id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_row19390540"><th class="cellrowborder" valign="top" width="15.384615384615385%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p27129916"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p27129916"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p27129916"></a><strong id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b42842654"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b42842654"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b42842654"></a>名称</strong></p>
</th>
<th class="cellrowborder" valign="top" width="12.5%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p47702931"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p47702931"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p47702931"></a><strong id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b26673201"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b26673201"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b26673201"></a>是否必选</strong></p>
</th>
<th class="cellrowborder" valign="top" width="22.115384615384613%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p13045638"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p13045638"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p13045638"></a><strong id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b50301879"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b50301879"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b50301879"></a>类型</strong></p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p47920438"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p47920438"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p47920438"></a><strong id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b28630766"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b28630766"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b28630766"></a>说明</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_row37390672"><td class="cellrowborder" valign="top" width="15.384615384615385%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p8745607"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p8745607"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p8745607"></a>streamName</p>
</td>
<td class="cellrowborder" valign="top" width="12.5%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p37305595"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p37305595"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p37305595"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="22.115384615384613%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p1854355"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p1854355"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p1854355"></a>char *</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p15985080"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p15985080"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p15985080"></a>通道名称。</p>
<p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p9647994"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p9647994"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p9647994"></a>在用户发送或者接收实时数据时，需要指定通道名称，创建的通道名称不能重复。通道名称由字母、数字、下划线和中划线组成，长度为1～64字符。</p>
</td>
</tr>
<tr id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_row19723089"><td class="cellrowborder" valign="top" width="15.384615384615385%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p54066375"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p54066375"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p54066375"></a>streamType</p>
</td>
<td class="cellrowborder" valign="top" width="12.5%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p17300225"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p17300225"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p17300225"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="22.115384615384613%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p59140967"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p59140967"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p59140967"></a>enum DISStreamType</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p25689059"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p25689059"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p25689059"></a>通道类型。</p>
<p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p29874939"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p29874939"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p29874939"></a>取值范围：</p>
<a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_ul439002"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_ul439002"></a><ul id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_ul439002"><li>DISStreamTypeCommon：普通通道，表示1MB带宽。</li><li>DISStreamTypeAdvanced：高级通道，表示5MB带宽。</li></ul>
<p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p51597550"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p51597550"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p51597550"></a>缺省值：DISStreamTypeCommon。</p>
</td>
</tr>
<tr id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_row61724767"><td class="cellrowborder" valign="top" width="15.384615384615385%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p33650236"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p33650236"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p33650236"></a>partitionCount</p>
</td>
<td class="cellrowborder" valign="top" width="12.5%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p41314614"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p41314614"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p41314614"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="22.115384615384613%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p58149428"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p58149428"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p58149428"></a>long</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p12483231"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p12483231"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p12483231"></a>分区数。</p>
<p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p45240216"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p45240216"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p45240216"></a>分区是DIS数据通道的基本吞吐量单位。</p>
<p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p4508766"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p4508766"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p4508766"></a>通道类型有普通和高级两种选择（二选一），其对应的分区数取值范围不同。</p>
<a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_ul40578897"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_ul40578897"></a><ul id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_ul40578897"><li>普通通道的分区数取值范围：1～50的整数，每个租户默认可创建的分区总数最大为50。若该租户已创建“N”个普通分区，则本次最多可创建“50-N”个分区。</li><li>高级通道的分区数取值范围：1～10的整数，每个租户默认可创建的分区总数最大为10。若该租户已创建“N”个高级分区，则本次最多可创建“10-N”个分区。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_row54115834"><td class="cellrowborder" valign="top" width="15.384615384615385%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p21306406"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p21306406"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p21306406"></a>pucReserved</p>
</td>
<td class="cellrowborder" valign="top" width="12.5%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p48097351"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p48097351"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p48097351"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="22.115384615384613%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p3571397"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p3571397"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p3571397"></a>void *</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p20847751"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p20847751"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p20847751"></a>空指针，用于拓展请求体</p>
</td>
</tr>
</tbody>
</table>

**表 2**  DISCreateStreamExpend 的参数说明

<a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_table31407785"></a>
<table><thead align="left"><tr id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_row12715278"><th class="cellrowborder" valign="top" width="18.269230769230766%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p23304563"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p23304563"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p23304563"></a><strong id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b8414476"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b8414476"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b8414476"></a>名称</strong></p>
</th>
<th class="cellrowborder" valign="top" width="10.576923076923077%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p10483995"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p10483995"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p10483995"></a><strong id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b27247099"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b27247099"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b27247099"></a>是否必选</strong></p>
</th>
<th class="cellrowborder" valign="top" width="23.076923076923077%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p59531373"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p59531373"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p59531373"></a><strong id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b66020315"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b66020315"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b66020315"></a>类型</strong></p>
</th>
<th class="cellrowborder" valign="top" width="48.07692307692307%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p46045275"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p46045275"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p46045275"></a><strong id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b11754296"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b11754296"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b11754296"></a>说明</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_row12573920"><td class="cellrowborder" valign="top" width="18.269230769230766%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p11854613"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p11854613"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p11854613"></a>dataDuration</p>
</td>
<td class="cellrowborder" valign="top" width="10.576923076923077%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p20699582"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p20699582"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p20699582"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="23.076923076923077%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p66053444"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p66053444"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p66053444"></a>long</p>
</td>
<td class="cellrowborder" valign="top" width="48.07692307692307%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p48728718"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p48728718"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p48728718"></a>数据保留时长。</p>
<p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p35905280"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p35905280"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p35905280"></a>取值范围：<em id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_i54712068"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_i54712068"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_i54712068"></a>N</em>*24，N的取值为1~7的整数。</p>
<p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p22646572"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p22646572"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p22646572"></a>单位：小时。</p>
<p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p2492560"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p2492560"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p2492560"></a>缺省值：24。</p>
<p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p22433040"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p22433040"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p22433040"></a>空表示使用缺省值。</p>
</td>
</tr>
<tr id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_row570775"><td class="cellrowborder" valign="top" width="18.269230769230766%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p46232835"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p46232835"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p46232835"></a>dataType</p>
</td>
<td class="cellrowborder" valign="top" width="10.576923076923077%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p53872188"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p53872188"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p53872188"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="23.076923076923077%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p1571113"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p1571113"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p1571113"></a>enum DISDataType</p>
</td>
<td class="cellrowborder" valign="top" width="48.07692307692307%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p60151347"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p60151347"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p60151347"></a>源数据类型。</p>
<p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p4491214"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p4491214"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p4491214"></a>取值范围：</p>
<a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_ul40420929"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_ul40420929"></a><ul id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_ul40420929"><li>DISDataTypeBlob：存储在数据库管理系统中的一组二进制数据。</li><li>DISDataTypeJson：一种开放的文件格式，以易读的文字为基础，用来传输由属性值或者序列性的值组成的数据对象。</li><li>DISDataTypeCsv：纯文本形式存储的表格数据，分隔符默认采用逗号。</li><li>DISDataTypeFile：源数据为文件。</li></ul>
<p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p21610982"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p21610982"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p21610982"></a>缺省值：DISDataTypeBlob。</p>
</td>
</tr>
<tr id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_row60281111"><td class="cellrowborder" valign="top" width="18.269230769230766%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p50931783"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p50931783"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p50931783"></a>obsDestinationDescriptor</p>
</td>
<td class="cellrowborder" valign="top" width="10.576923076923077%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p31833731"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p31833731"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p31833731"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="23.076923076923077%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p28395444"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p28395444"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p28395444"></a>Struct ObsDestinationDescriptor</p>
</td>
<td class="cellrowborder" valign="top" width="48.07692307692307%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p18329666"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p18329666"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p18329666"></a>转储目的地为OBS的参数列表。暂时不支持同时转储至多个目的地。</p>
<p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p30749271"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p30749271"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p30749271"></a>缺省值：空。</p>
<p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p8307988"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p8307988"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p8307988"></a>配置为空表示数据不转储到OBS。</p>
<p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p7663035"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p7663035"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p7663035"></a><strong id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b1858451"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b1858451"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b1858451"></a>说明：</strong></p>
<p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p16726062"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p16726062"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p16726062"></a>此参数，仅“源数据类型”为“FILE”时呈现且需要配置。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  Struct ObsDestinationDescriptor参数说明

<a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_table46595510"></a>
<table><thead align="left"><tr id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_row34717793"><th class="cellrowborder" valign="top" width="21.43%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p60677888"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p60677888"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p60677888"></a><strong id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b9230088"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b9230088"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b9230088"></a>名称</strong></p>
</th>
<th class="cellrowborder" valign="top" width="11.219999999999999%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p9439626"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p9439626"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p9439626"></a><strong id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b17847776"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b17847776"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b17847776"></a>是否必选</strong></p>
</th>
<th class="cellrowborder" valign="top" width="14.29%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p36383728"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p36383728"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p36383728"></a><strong id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b59018101"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b59018101"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b59018101"></a>类型</strong></p>
</th>
<th class="cellrowborder" valign="top" width="53.059999999999995%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p15736877"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p15736877"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p15736877"></a><strong id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b7414170"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b7414170"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b7414170"></a>说明</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_row63676932"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p57557895"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p57557895"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p57557895"></a>agencyName</p>
</td>
<td class="cellrowborder" valign="top" width="11.219999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p31677898"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p31677898"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p31677898"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p15772917"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p15772917"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p15772917"></a>char *</p>
</td>
<td class="cellrowborder" valign="top" width="53.059999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p2537905"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p2537905"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p2537905"></a>在IAM中创建委托的名称，DIS需要获取IAM委托信息去访问您指定的资源。创建委托的参数设置如下：</p>
<a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_ul22841149"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_ul22841149"></a><ul id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_ul22841149"><li>委托类型：云服务</li><li>云服务：DIS</li><li>持续时间：永久</li><li>“所属区域”为“全局服务”，“项目”为“对象存储服务”对应的“策略”包含“Tenant Administrator”。</li></ul>
<p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p60173144"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p60173144"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p60173144"></a>取值范围：长度不超过64位，且不可配置为空。</p>
</td>
</tr>
<tr id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_row4687385"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p44133910"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p44133910"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p44133910"></a>obsBucketPath</p>
</td>
<td class="cellrowborder" valign="top" width="11.219999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p18076976"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p18076976"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p18076976"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p54948942"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p54948942"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p54948942"></a>char *</p>
</td>
<td class="cellrowborder" valign="top" width="53.059999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p21679321"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p21679321"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p21679321"></a>存储该通道数据的OBS桶名称。</p>
</td>
</tr>
<tr id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_row60896162"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p33642107"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p33642107"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p33642107"></a>pucReserved</p>
</td>
<td class="cellrowborder" valign="top" width="11.219999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p40656116"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p40656116"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p40656116"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p4811061"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p4811061"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p4811061"></a>void *</p>
</td>
<td class="cellrowborder" valign="top" width="53.059999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p54151655"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p54151655"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p54151655"></a>空指针，用于拓展结构</p>
</td>
</tr>
</tbody>
</table>

**表 4**  DISResponseInfo响应参数说明

<a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_table14684604"></a>
<table><thead align="left"><tr id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_row45399024"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p53442317"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p53442317"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p53442317"></a><strong id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b11218807"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b11218807"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b11218807"></a>参数名</strong></p>
</th>
<th class="cellrowborder" valign="top" width="26%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p36308168"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p36308168"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p36308168"></a><strong id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b58338056"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b58338056"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b58338056"></a>类型</strong></p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p27762102"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p27762102"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p27762102"></a><strong id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b48532334"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b48532334"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_b48532334"></a>说明</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_row38805013"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p56198311"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p56198311"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p56198311"></a>HttpResponseCode</p>
</td>
<td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p55769358"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p55769358"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p55769358"></a>long</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p21024178"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p21024178"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p21024178"></a><a href="https://support.huaweicloud.com/api-dis/dis_02_0021.html" target="_blank" rel="noopener noreferrer">错误码</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_row25236858"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p30919631"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p30919631"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p30919631"></a>ErrorCode</p>
</td>
<td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p21462168"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p21462168"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p21462168"></a>Char[32]</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p60714046"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p60714046"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p60714046"></a><a href="https://support.huaweicloud.com/api-dis/dis_02_0022.html" target="_blank" rel="noopener noreferrer">状态码</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_row18890664"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p53748798"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p53748798"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p53748798"></a>ErrorDetail</p>
</td>
<td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p58685418"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p58685418"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p58685418"></a>Char[526]</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p55898385"><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p55898385"></a><a name="zh-cn_topic_0131160810_zh-cn_topic_0131140744_p55898385"></a>错误响应消息体</p>
</td>
</tr>
</tbody>
</table>

