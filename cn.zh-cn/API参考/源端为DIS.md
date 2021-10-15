# 源端为DIS<a name="dgc_02_0291"></a>

## JSON样例<a name="zh-cn_topic_0108272853_section33401108172339"></a>

```
"from-config-values": {
          "configs": [
              {
                  "inputs": [
                      {
                         "name": "fromJobConfig.streamName",
                         "value": "cdm"
                      },
                      {
                         "name": "fromJobConfig.disConsumerStrategy",
                         "value": "FROM_LAST_STOP"
                      },
                      {
                         "name": "fromJobConfig.isPermanency",
                         "value": "true"
                      },
                      {
                         "name": "fromJobConfig.maxPollRecords",
                         "value": "100"
                      },
                      {
                         "name": "fromJobConfig.shardId",
                         "value": "0"
                      },
                      {
                         "name": "fromJobConfig.separator",
                         "value": ","
                      }
                  ],
                  "name": "fromJobConfig"
              }
          ]
      }
```

## 参数说明<a name="zh-cn_topic_0108272853_section28186120174818"></a>

<a name="zh-cn_topic_0108272853_table13922888141527"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108272853_row229143141527"><th class="cellrowborder" valign="top" width="22.66%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272853_p66756185141527"><a name="zh-cn_topic_0108272853_p66756185141527"></a><a name="zh-cn_topic_0108272853_p66756185141527"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="19.78%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272853_p38541938141527"><a name="zh-cn_topic_0108272853_p38541938141527"></a><a name="zh-cn_topic_0108272853_p38541938141527"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.05%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272853_p34889279141527"><a name="zh-cn_topic_0108272853_p34889279141527"></a><a name="zh-cn_topic_0108272853_p34889279141527"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="40.510000000000005%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272853_p7459369141527"><a name="zh-cn_topic_0108272853_p7459369141527"></a><a name="zh-cn_topic_0108272853_p7459369141527"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108272853_row62628929141527"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272853_p18560626141527"><a name="zh-cn_topic_0108272853_p18560626141527"></a><a name="zh-cn_topic_0108272853_p18560626141527"></a>fromJobConfig.streamName</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272853_p27015713141527"><a name="zh-cn_topic_0108272853_p27015713141527"></a><a name="zh-cn_topic_0108272853_p27015713141527"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272853_p50167516142856"><a name="zh-cn_topic_0108272853_p50167516142856"></a><a name="zh-cn_topic_0108272853_p50167516142856"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272853_p32605071143018"><a name="zh-cn_topic_0108272853_p32605071143018"></a><a name="zh-cn_topic_0108272853_p32605071143018"></a>DIS的通道名。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272853_row42094113141527"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272853_p26789449141527"><a name="zh-cn_topic_0108272853_p26789449141527"></a><a name="zh-cn_topic_0108272853_p26789449141527"></a>fromJobConfig.disConsumerStrategy</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272853_p22461756141527"><a name="zh-cn_topic_0108272853_p22461756141527"></a><a name="zh-cn_topic_0108272853_p22461756141527"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272853_p7462956141527"><a name="zh-cn_topic_0108272853_p7462956141527"></a><a name="zh-cn_topic_0108272853_p7462956141527"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272853_p1561824172319"><a name="zh-cn_topic_0108272853_p1561824172319"></a><a name="zh-cn_topic_0108272853_p1561824172319"></a>设置从DIS拉取数据时的初始偏移量：</p>
<a name="zh-cn_topic_0108272853_ul4823568317828"></a><a name="zh-cn_topic_0108272853_ul4823568317828"></a><ul id="zh-cn_topic_0108272853_ul4823568317828"><li>LATEST：最大偏移量，即最新的数据。</li><li>FROM_LAST_STOP：从上次停止处继续拉取。</li><li>EARLIEST：最小偏移量，即最早的数据。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0108272853_row8336449141527"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272853_p29681527141527"><a name="zh-cn_topic_0108272853_p29681527141527"></a><a name="zh-cn_topic_0108272853_p29681527141527"></a>fromJobConfig.isPermanency</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272853_p55393515141527"><a name="zh-cn_topic_0108272853_p55393515141527"></a><a name="zh-cn_topic_0108272853_p55393515141527"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272853_p8057768172040"><a name="zh-cn_topic_0108272853_p8057768172040"></a><a name="zh-cn_topic_0108272853_p8057768172040"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272853_p31296545154541"><a name="zh-cn_topic_0108272853_p31296545154541"></a><a name="zh-cn_topic_0108272853_p31296545154541"></a>是否永久运行。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272853_row3034171115124"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272853_p3395516415124"><a name="zh-cn_topic_0108272853_p3395516415124"></a><a name="zh-cn_topic_0108272853_p3395516415124"></a>fromJobConfig.maxPollRecords</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272853_p6601372415124"><a name="zh-cn_topic_0108272853_p6601372415124"></a><a name="zh-cn_topic_0108272853_p6601372415124"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272853_p4551140015124"><a name="zh-cn_topic_0108272853_p4551140015124"></a><a name="zh-cn_topic_0108272853_p4551140015124"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272853_p6254480915124"><a name="zh-cn_topic_0108272853_p6254480915124"></a><a name="zh-cn_topic_0108272853_p6254480915124"></a>每次向DIS请求数据限制最大请求记录数。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272853_row4065400315124"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272853_p2824781215124"><a name="zh-cn_topic_0108272853_p2824781215124"></a><a name="zh-cn_topic_0108272853_p2824781215124"></a>fromJobConfig.shardId</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272853_p637144815124"><a name="zh-cn_topic_0108272853_p637144815124"></a><a name="zh-cn_topic_0108272853_p637144815124"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272853_p4632524315124"><a name="zh-cn_topic_0108272853_p4632524315124"></a><a name="zh-cn_topic_0108272853_p4632524315124"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272853_p6135724015124"><a name="zh-cn_topic_0108272853_p6135724015124"></a><a name="zh-cn_topic_0108272853_p6135724015124"></a>DIS分区ID，该参数支持输入多个分区ID，使用<span class="parmvalue" id="zh-cn_topic_0108272853_parmvalue158181995417"><a name="zh-cn_topic_0108272853_parmvalue158181995417"></a><a name="zh-cn_topic_0108272853_parmvalue158181995417"></a>“,”</span>分隔。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272853_row177282453112"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272853_p17565527611"><a name="zh-cn_topic_0108272853_p17565527611"></a><a name="zh-cn_topic_0108272853_p17565527611"></a>fromJobConfig.dataFormat</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272853_p165651821569"><a name="zh-cn_topic_0108272853_p165651821569"></a><a name="zh-cn_topic_0108272853_p165651821569"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272853_p3565025614"><a name="zh-cn_topic_0108272853_p3565025614"></a><a name="zh-cn_topic_0108272853_p3565025614"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272853_p111321138622"><a name="zh-cn_topic_0108272853_p111321138622"></a><a name="zh-cn_topic_0108272853_p111321138622"></a>解析数据时使用的格式：</p>
<a name="zh-cn_topic_0108272853_ul59573391929"></a><a name="zh-cn_topic_0108272853_ul59573391929"></a><ul id="zh-cn_topic_0108272853_ul59573391929"><li>BINARY：适用于文件迁移场景，不解析数据内容原样传输。</li><li>CSV：以CSV格式解析源数据。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0108272853_row4268185173352"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272853_p10178715173352"><a name="zh-cn_topic_0108272853_p10178715173352"></a><a name="zh-cn_topic_0108272853_p10178715173352"></a>fromJobConfig.separator</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272853_p19169610173352"><a name="zh-cn_topic_0108272853_p19169610173352"></a><a name="zh-cn_topic_0108272853_p19169610173352"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272853_p9234573173352"><a name="zh-cn_topic_0108272853_p9234573173352"></a><a name="zh-cn_topic_0108272853_p9234573173352"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272853_p9802957173352"><a name="zh-cn_topic_0108272853_p9802957173352"></a><a name="zh-cn_topic_0108272853_p9802957173352"></a>字段分隔符。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272853_row8201182620484"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272853_p2020117268481"><a name="zh-cn_topic_0108272853_p2020117268481"></a><a name="zh-cn_topic_0108272853_p2020117268481"></a>fromJobConfig.appName</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272853_p13201126194815"><a name="zh-cn_topic_0108272853_p13201126194815"></a><a name="zh-cn_topic_0108272853_p13201126194815"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272853_p1420162613485"><a name="zh-cn_topic_0108272853_p1420162613485"></a><a name="zh-cn_topic_0108272853_p1420162613485"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272853_p32011926114812"><a name="zh-cn_topic_0108272853_p32011926114812"></a><a name="zh-cn_topic_0108272853_p32011926114812"></a>用户数据消费程序的唯一标识符。</p>
</td>
</tr>
</tbody>
</table>

