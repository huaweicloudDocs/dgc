# 源端为Kafka<a name="dgc_02_0292"></a>

## JSON样例<a name="zh-cn_topic_0108272821_section33401108172339"></a>

```
"from-config-values": {
           "configs": [
               {
                   "inputs": [
                       {
                       "name": "fromJobConfig.topicsList",
                       "value": "est1,est2"
                       },
                       {
                       "name": "fromJobConfig.kafkaConsumerStrategy",
                       "value": "EARLIEST"
                       },
                       {
                       "name": "fromJobConfig.isPermanency",
                       "value": "true"
                       }
                   ],
                   "name": "fromJobConfig"
               }
           ]
       }
```

## 参数说明<a name="zh-cn_topic_0108272821_section61808073174843"></a>

<a name="zh-cn_topic_0108272821_table13922888141527"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108272821_row229143141527"><th class="cellrowborder" valign="top" width="22.66%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272821_p66756185141527"><a name="zh-cn_topic_0108272821_p66756185141527"></a><a name="zh-cn_topic_0108272821_p66756185141527"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="19.78%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272821_p38541938141527"><a name="zh-cn_topic_0108272821_p38541938141527"></a><a name="zh-cn_topic_0108272821_p38541938141527"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.05%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272821_p34889279141527"><a name="zh-cn_topic_0108272821_p34889279141527"></a><a name="zh-cn_topic_0108272821_p34889279141527"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="40.510000000000005%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272821_p7459369141527"><a name="zh-cn_topic_0108272821_p7459369141527"></a><a name="zh-cn_topic_0108272821_p7459369141527"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108272821_row62628929141527"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272821_p18560626141527"><a name="zh-cn_topic_0108272821_p18560626141527"></a><a name="zh-cn_topic_0108272821_p18560626141527"></a>fromJobConfig.topicsList</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272821_p27015713141527"><a name="zh-cn_topic_0108272821_p27015713141527"></a><a name="zh-cn_topic_0108272821_p27015713141527"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272821_p50167516142856"><a name="zh-cn_topic_0108272821_p50167516142856"></a><a name="zh-cn_topic_0108272821_p50167516142856"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272821_p32605071143018"><a name="zh-cn_topic_0108272821_p32605071143018"></a><a name="zh-cn_topic_0108272821_p32605071143018"></a>Kafka topic列表，可以为多个topic，以<span class="uicontrol" id="zh-cn_topic_0108272821_uicontrol3658879321040"><a name="zh-cn_topic_0108272821_uicontrol3658879321040"></a><a name="zh-cn_topic_0108272821_uicontrol3658879321040"></a>“,”</span>作为分隔符。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272821_row42094113141527"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272821_p26789449141527"><a name="zh-cn_topic_0108272821_p26789449141527"></a><a name="zh-cn_topic_0108272821_p26789449141527"></a>fromJobConfig.kafkaConsumerStrategy</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272821_p22461756141527"><a name="zh-cn_topic_0108272821_p22461756141527"></a><a name="zh-cn_topic_0108272821_p22461756141527"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272821_p7462956141527"><a name="zh-cn_topic_0108272821_p7462956141527"></a><a name="zh-cn_topic_0108272821_p7462956141527"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272821_p1561824172319"><a name="zh-cn_topic_0108272821_p1561824172319"></a><a name="zh-cn_topic_0108272821_p1561824172319"></a>从Kafka拉取数据时的初始偏移量设置：</p>
<a name="zh-cn_topic_0108272821_ul4823568317828"></a><a name="zh-cn_topic_0108272821_ul4823568317828"></a><ul id="zh-cn_topic_0108272821_ul4823568317828"><li>LATEST：最大偏移量，即最新的数据。</li><li>EARLIEST：最小偏移量，即最老的数据。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0108272821_row8336449141527"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272821_p29681527141527"><a name="zh-cn_topic_0108272821_p29681527141527"></a><a name="zh-cn_topic_0108272821_p29681527141527"></a>fromJobConfig.isPermanency</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272821_p55393515141527"><a name="zh-cn_topic_0108272821_p55393515141527"></a><a name="zh-cn_topic_0108272821_p55393515141527"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272821_p8057768172040"><a name="zh-cn_topic_0108272821_p8057768172040"></a><a name="zh-cn_topic_0108272821_p8057768172040"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272821_p31296545154541"><a name="zh-cn_topic_0108272821_p31296545154541"></a><a name="zh-cn_topic_0108272821_p31296545154541"></a>是否永久运行。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272821_row14054899103013"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272821_p64705066103013"><a name="zh-cn_topic_0108272821_p64705066103013"></a><a name="zh-cn_topic_0108272821_p64705066103013"></a>fromJobConfig.groupId</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272821_p6618956103013"><a name="zh-cn_topic_0108272821_p6618956103013"></a><a name="zh-cn_topic_0108272821_p6618956103013"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272821_p66373443103013"><a name="zh-cn_topic_0108272821_p66373443103013"></a><a name="zh-cn_topic_0108272821_p66373443103013"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272821_p1638011885013"><a name="zh-cn_topic_0108272821_p1638011885013"></a><a name="zh-cn_topic_0108272821_p1638011885013"></a>用户指定消费组ID。</p>
<p id="zh-cn_topic_0108272821_p1114017325017"><a name="zh-cn_topic_0108272821_p1114017325017"></a><a name="zh-cn_topic_0108272821_p1114017325017"></a>如果是从DMS Kafka导出数据，专享版请任意输入，标准版请输入有效的消费组ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272821_row55656218613"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272821_p17565527611"><a name="zh-cn_topic_0108272821_p17565527611"></a><a name="zh-cn_topic_0108272821_p17565527611"></a>fromJobConfig.dataFormat</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272821_p165651821569"><a name="zh-cn_topic_0108272821_p165651821569"></a><a name="zh-cn_topic_0108272821_p165651821569"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272821_p3565025614"><a name="zh-cn_topic_0108272821_p3565025614"></a><a name="zh-cn_topic_0108272821_p3565025614"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272821_p111321138622"><a name="zh-cn_topic_0108272821_p111321138622"></a><a name="zh-cn_topic_0108272821_p111321138622"></a>解析数据时使用的格式：</p>
<a name="zh-cn_topic_0108272821_ul59573391929"></a><a name="zh-cn_topic_0108272821_ul59573391929"></a><ul id="zh-cn_topic_0108272821_ul59573391929"><li>BINARY：适用于文件迁移场景，不解析数据内容原样传输。</li><li>CSV：以CSV格式解析源数据。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0108272821_row3034171115124"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272821_p3395516415124"><a name="zh-cn_topic_0108272821_p3395516415124"></a><a name="zh-cn_topic_0108272821_p3395516415124"></a>fromJobConfig.maxPollRecords</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272821_p6601372415124"><a name="zh-cn_topic_0108272821_p6601372415124"></a><a name="zh-cn_topic_0108272821_p6601372415124"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272821_p4551140015124"><a name="zh-cn_topic_0108272821_p4551140015124"></a><a name="zh-cn_topic_0108272821_p4551140015124"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272821_p6254480915124"><a name="zh-cn_topic_0108272821_p6254480915124"></a><a name="zh-cn_topic_0108272821_p6254480915124"></a>每次向Kafka请求数据限制最大请求记录数。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272821_row4065400315124"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272821_p2824781215124"><a name="zh-cn_topic_0108272821_p2824781215124"></a><a name="zh-cn_topic_0108272821_p2824781215124"></a>fromJobConfig.maxPollInterval</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272821_p637144815124"><a name="zh-cn_topic_0108272821_p637144815124"></a><a name="zh-cn_topic_0108272821_p637144815124"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272821_p4632524315124"><a name="zh-cn_topic_0108272821_p4632524315124"></a><a name="zh-cn_topic_0108272821_p4632524315124"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272821_p6135724015124"><a name="zh-cn_topic_0108272821_p6135724015124"></a><a name="zh-cn_topic_0108272821_p6135724015124"></a>每次poll之间的最大时间间隔。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272821_row4268185173352"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272821_p10178715173352"><a name="zh-cn_topic_0108272821_p10178715173352"></a><a name="zh-cn_topic_0108272821_p10178715173352"></a>fromJobConfig.separator</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272821_p19169610173352"><a name="zh-cn_topic_0108272821_p19169610173352"></a><a name="zh-cn_topic_0108272821_p19169610173352"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272821_p9234573173352"><a name="zh-cn_topic_0108272821_p9234573173352"></a><a name="zh-cn_topic_0108272821_p9234573173352"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272821_p9802957173352"><a name="zh-cn_topic_0108272821_p9802957173352"></a><a name="zh-cn_topic_0108272821_p9802957173352"></a>字段分隔符。</p>
</td>
</tr>
</tbody>
</table>

