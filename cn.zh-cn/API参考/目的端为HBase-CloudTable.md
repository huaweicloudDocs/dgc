# 目的端为HBase/CloudTable<a name="dgc_02_0300"></a>

## JSON样例<a name="zh-cn_topic_0108272851_section33401108172339"></a>

```
"to-config-values": {
        "configs": [
          {
            "inputs": [
              {
                "name": "toJobConfig.table",
                "value": "rf_to"
              },
              {
                "name": "toJobConfig.storageType",
                "value": "PUTLIST"
              },
              {
                "name": "toJobConfig.columns",
                "value": "AA:AA&BB:BB&CC:CC&DD:DD"
              },
              {
                "name": "toJobConfig.rowKeyColumn",
                "value": "AA:AA"
              },
              {
                "name": "toJobConfig.isOverride",
                "value": "false"
              },
              {
                "name": "toJobConfig.isRowkeyRedundancy",
                "value": "false"
              },
              {
                "name": "toJobConfig.algorithm",
                "value": "NONE"
              },
              {
                "name": "toJobConfig.writeToWAL",
                "value": "true"
              },
              {
                "name": "toJobConfig.transType",
                "value": "false"
              }
            ],
            "name": "toJobConfig"
          }
        ]
      }
```

## 参数说明<a name="zh-cn_topic_0108272851_section48102183111156"></a>

<a name="zh-cn_topic_0108272851_table13922888141527"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108272851_row229143141527"><th class="cellrowborder" valign="top" width="22.657734226577343%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272851_p66756185141527"><a name="zh-cn_topic_0108272851_p66756185141527"></a><a name="zh-cn_topic_0108272851_p66756185141527"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="19.96800319968003%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272851_p38541938141527"><a name="zh-cn_topic_0108272851_p38541938141527"></a><a name="zh-cn_topic_0108272851_p38541938141527"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.23827617238276%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272851_p34889279141527"><a name="zh-cn_topic_0108272851_p34889279141527"></a><a name="zh-cn_topic_0108272851_p34889279141527"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="40.135986401359865%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272851_p7459369141527"><a name="zh-cn_topic_0108272851_p7459369141527"></a><a name="zh-cn_topic_0108272851_p7459369141527"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108272851_row62628929141527"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272851_p29098284165959"><a name="zh-cn_topic_0108272851_p29098284165959"></a><a name="zh-cn_topic_0108272851_p29098284165959"></a>toJobConfig.table</p>
</td>
<td class="cellrowborder" valign="top" width="19.96800319968003%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272851_p27015713141527"><a name="zh-cn_topic_0108272851_p27015713141527"></a><a name="zh-cn_topic_0108272851_p27015713141527"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272851_p50167516142856"><a name="zh-cn_topic_0108272851_p50167516142856"></a><a name="zh-cn_topic_0108272851_p50167516142856"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.135986401359865%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272851_p2430205141527"><a name="zh-cn_topic_0108272851_p2430205141527"></a><a name="zh-cn_topic_0108272851_p2430205141527"></a>写入数据的表名，例如：<span class="parmvalue" id="zh-cn_topic_0108272851_parmvalue15419570101029"><a name="zh-cn_topic_0108272851_parmvalue15419570101029"></a><a name="zh-cn_topic_0108272851_parmvalue15419570101029"></a>“TBL_EXAMPLE”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272851_row64475722155949"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272851_p32328561155955"><a name="zh-cn_topic_0108272851_p32328561155955"></a><a name="zh-cn_topic_0108272851_p32328561155955"></a>toJobConfig.storageType</p>
</td>
<td class="cellrowborder" valign="top" width="19.96800319968003%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272851_p1367823155955"><a name="zh-cn_topic_0108272851_p1367823155955"></a><a name="zh-cn_topic_0108272851_p1367823155955"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272851_p43684849155955"><a name="zh-cn_topic_0108272851_p43684849155955"></a><a name="zh-cn_topic_0108272851_p43684849155955"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="40.135986401359865%" headers="mcps1.1.5.1.4 "><div class="p" id="zh-cn_topic_0108272851_p52791884154748"><a name="zh-cn_topic_0108272851_p52791884154748"></a><a name="zh-cn_topic_0108272851_p52791884154748"></a>将数据写入到HBase表中的方法：<a name="zh-cn_topic_0108272851_ul54155538155037"></a><a name="zh-cn_topic_0108272851_ul54155538155037"></a><ul id="zh-cn_topic_0108272851_ul54155538155037"><li>BULKLOAD：推荐使用BULKLOAD模式，提高加载性能。</li><li>PUTLIST：只有数据量很小的时候推荐用PUTLIST模式。</li></ul>
</div>
</td>
</tr>
<tr id="zh-cn_topic_0108272851_row1211632319404"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272851_p29681527141527"><a name="zh-cn_topic_0108272851_p29681527141527"></a><a name="zh-cn_topic_0108272851_p29681527141527"></a>toJobConfig.columns</p>
</td>
<td class="cellrowborder" valign="top" width="19.96800319968003%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272851_p55393515141527"><a name="zh-cn_topic_0108272851_p55393515141527"></a><a name="zh-cn_topic_0108272851_p55393515141527"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272851_p57689731141527"><a name="zh-cn_topic_0108272851_p57689731141527"></a><a name="zh-cn_topic_0108272851_p57689731141527"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.135986401359865%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272851_p42356648141527"><a name="zh-cn_topic_0108272851_p42356648141527"></a><a name="zh-cn_topic_0108272851_p42356648141527"></a>需要抽取数据的列，列号之间使用<span class="parmvalue" id="zh-cn_topic_0108272851_parmvalue23649168101043"><a name="zh-cn_topic_0108272851_parmvalue23649168101043"></a><a name="zh-cn_topic_0108272851_parmvalue23649168101043"></a>“&amp;”</span>分割，列族与列之间用<span class="parmvalue" id="zh-cn_topic_0108272851_parmvalue8963984101051"><a name="zh-cn_topic_0108272851_parmvalue8963984101051"></a><a name="zh-cn_topic_0108272851_parmvalue8963984101051"></a>“:”</span>分隔，例如：<span class="parmvalue" id="zh-cn_topic_0108272851_parmvalue5164117810112"><a name="zh-cn_topic_0108272851_parmvalue5164117810112"></a><a name="zh-cn_topic_0108272851_parmvalue5164117810112"></a>“cf1:c1&amp;cf2:c2”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272851_row5807461019222"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272851_p642293319222"><a name="zh-cn_topic_0108272851_p642293319222"></a><a name="zh-cn_topic_0108272851_p642293319222"></a>toJobConfig.rowKeyColumn</p>
</td>
<td class="cellrowborder" valign="top" width="19.96800319968003%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272851_p5049560219222"><a name="zh-cn_topic_0108272851_p5049560219222"></a><a name="zh-cn_topic_0108272851_p5049560219222"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272851_p6361195119222"><a name="zh-cn_topic_0108272851_p6361195119222"></a><a name="zh-cn_topic_0108272851_p6361195119222"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.135986401359865%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272851_p5229438819222"><a name="zh-cn_topic_0108272851_p5229438819222"></a><a name="zh-cn_topic_0108272851_p5229438819222"></a>作为rowkey的列，列号之间使用<span class="parmvalue" id="zh-cn_topic_0108272851_parmvalue20031956101139"><a name="zh-cn_topic_0108272851_parmvalue20031956101139"></a><a name="zh-cn_topic_0108272851_parmvalue20031956101139"></a>“&amp;”</span>分割，列族与列之间用<span class="parmvalue" id="zh-cn_topic_0108272851_parmvalue10476847101148"><a name="zh-cn_topic_0108272851_parmvalue10476847101148"></a><a name="zh-cn_topic_0108272851_parmvalue10476847101148"></a>“:”</span>分隔，例如：<span class="parmvalue" id="zh-cn_topic_0108272851_parmvalue61920664101158"><a name="zh-cn_topic_0108272851_parmvalue61920664101158"></a><a name="zh-cn_topic_0108272851_parmvalue61920664101158"></a>“cf1:c1&amp;cf2:c2”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272851_row45367709192212"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272851_p50905776192212"><a name="zh-cn_topic_0108272851_p50905776192212"></a><a name="zh-cn_topic_0108272851_p50905776192212"></a>toJobConfig.isOverride</p>
</td>
<td class="cellrowborder" valign="top" width="19.96800319968003%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272851_p29727229192212"><a name="zh-cn_topic_0108272851_p29727229192212"></a><a name="zh-cn_topic_0108272851_p29727229192212"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272851_p59095338192212"><a name="zh-cn_topic_0108272851_p59095338192212"></a><a name="zh-cn_topic_0108272851_p59095338192212"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="40.135986401359865%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272851_p21993055192212"><a name="zh-cn_topic_0108272851_p21993055192212"></a><a name="zh-cn_topic_0108272851_p21993055192212"></a>使用BULKLOAD方式导入数据时，是否清空数据，例如：<span class="parmvalue" id="zh-cn_topic_0108272851_parmvalue13848598101223"><a name="zh-cn_topic_0108272851_parmvalue13848598101223"></a><a name="zh-cn_topic_0108272851_parmvalue13848598101223"></a>“true”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272851_row44180181192225"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272851_p21824946192225"><a name="zh-cn_topic_0108272851_p21824946192225"></a><a name="zh-cn_topic_0108272851_p21824946192225"></a>toJobConfig.delimiter</p>
</td>
<td class="cellrowborder" valign="top" width="19.96800319968003%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272851_p22990191192225"><a name="zh-cn_topic_0108272851_p22990191192225"></a><a name="zh-cn_topic_0108272851_p22990191192225"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272851_p50266164192225"><a name="zh-cn_topic_0108272851_p50266164192225"></a><a name="zh-cn_topic_0108272851_p50266164192225"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.135986401359865%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272851_p45027498192225"><a name="zh-cn_topic_0108272851_p45027498192225"></a><a name="zh-cn_topic_0108272851_p45027498192225"></a>当选取多个列做rowkey时，连接多列的分隔符，例如：<span class="parmvalue" id="zh-cn_topic_0108272851_parmvalue52352021101248"><a name="zh-cn_topic_0108272851_parmvalue52352021101248"></a><a name="zh-cn_topic_0108272851_parmvalue52352021101248"></a>“|”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272851_row40951843151814"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272851_p28764986151814"><a name="zh-cn_topic_0108272851_p28764986151814"></a><a name="zh-cn_topic_0108272851_p28764986151814"></a>toJobConfig.isRowkeyRedundancy</p>
</td>
<td class="cellrowborder" valign="top" width="19.96800319968003%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272851_p48262521151814"><a name="zh-cn_topic_0108272851_p48262521151814"></a><a name="zh-cn_topic_0108272851_p48262521151814"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272851_p16950153151814"><a name="zh-cn_topic_0108272851_p16950153151814"></a><a name="zh-cn_topic_0108272851_p16950153151814"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="40.135986401359865%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272851_p30785170151814"><a name="zh-cn_topic_0108272851_p30785170151814"></a><a name="zh-cn_topic_0108272851_p30785170151814"></a>是否将选做Rowkey的数据同时写入HBase的列。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272851_row870435217434"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272851_p1770415524430"><a name="zh-cn_topic_0108272851_p1770415524430"></a><a name="zh-cn_topic_0108272851_p1770415524430"></a>toJobConfig.algorithm</p>
</td>
<td class="cellrowborder" valign="top" width="19.96800319968003%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272851_p3704155284317"><a name="zh-cn_topic_0108272851_p3704155284317"></a><a name="zh-cn_topic_0108272851_p3704155284317"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272851_p1704752114317"><a name="zh-cn_topic_0108272851_p1704752114317"></a><a name="zh-cn_topic_0108272851_p1704752114317"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="40.135986401359865%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272851_p1870405219437"><a name="zh-cn_topic_0108272851_p1870405219437"></a><a name="zh-cn_topic_0108272851_p1870405219437"></a>创建新HBase表时采用的压缩算法，支持SNAPPY和GZ算法，默认为<span class="parmvalue" id="zh-cn_topic_0108272851_parmvalue293717481586"><a name="zh-cn_topic_0108272851_parmvalue293717481586"></a><a name="zh-cn_topic_0108272851_parmvalue293717481586"></a>“NONE”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272851_row98514123112"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272851_p12850133114"><a name="zh-cn_topic_0108272851_p12850133114"></a><a name="zh-cn_topic_0108272851_p12850133114"></a>toJobConfig.writeToWAL</p>
</td>
<td class="cellrowborder" valign="top" width="19.96800319968003%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272851_p585617317"><a name="zh-cn_topic_0108272851_p585617317"></a><a name="zh-cn_topic_0108272851_p585617317"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272851_p1291535313115"><a name="zh-cn_topic_0108272851_p1291535313115"></a><a name="zh-cn_topic_0108272851_p1291535313115"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="40.135986401359865%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272851_p791673125616"><a name="zh-cn_topic_0108272851_p791673125616"></a><a name="zh-cn_topic_0108272851_p791673125616"></a>选择是否开启HBase的预写日志机制（WAL，Write Ahead Log）。</p>
<a name="zh-cn_topic_0108272851_ul1899132517107"></a><a name="zh-cn_topic_0108272851_ul1899132517107"></a><ul id="zh-cn_topic_0108272851_ul1899132517107"><li>是：开启后如果出现HBase服务器宕机，则可以从WAL中回放执行之前没有完成的操作。</li><li>否：关闭时能提升写入性能，但如果HBase服务器宕机可能会造成数据丢失。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0108272851_row1253573222917"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272851_p05351632182912"><a name="zh-cn_topic_0108272851_p05351632182912"></a><a name="zh-cn_topic_0108272851_p05351632182912"></a>toJobConfig.transType</p>
</td>
<td class="cellrowborder" valign="top" width="19.96800319968003%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272851_p1535163262915"><a name="zh-cn_topic_0108272851_p1535163262915"></a><a name="zh-cn_topic_0108272851_p1535163262915"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272851_p953563272917"><a name="zh-cn_topic_0108272851_p953563272917"></a><a name="zh-cn_topic_0108272851_p953563272917"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="40.135986401359865%" headers="mcps1.1.5.1.4 "><a name="zh-cn_topic_0108272851_ul4509123194219"></a><a name="zh-cn_topic_0108272851_ul4509123194219"></a><ul id="zh-cn_topic_0108272851_ul4509123194219"><li>true：源端数据库中的Short、Int、Long、Float、Double、Decimal类型列的数据，会转换为Byte[]数组（二进制）写入HBase，其他类型的按字符串写入。如果这几种类型中，有合并做rowkey的，就依然当字符串写入。<p id="zh-cn_topic_0108272851_p12731115251120"><a name="zh-cn_topic_0108272851_p12731115251120"></a><a name="zh-cn_topic_0108272851_p12731115251120"></a>该功能作用是：降低存储占用空间，存储更高效；特定场景下rowkey分布更均匀。</p>
</li><li>false：源端数据库中所有类型的数据，都会按照字符串写入HBase。</li></ul>
</td>
</tr>
</tbody>
</table>

