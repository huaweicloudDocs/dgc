# 源端为HDFS<a name="dgc_02_0284"></a>

## JSON样例<a name="zh-cn_topic_0108272787_section33401108172339"></a>

```
"from-config-values": {
        "configs": [
          {
            "inputs": [
              {
                "name": "fromJobConfig.inputDirectory",
                "value": "/hdfsfrom/from_hdfs_est.csv"
              },
              {
                "name": "fromJobConfig.inputFormat",
                "value": "CSV_FILE"
              },
              {
                "name": "fromJobConfig.columnList",
                "value": "1"
              },
              {
                "name": "fromJobConfig.jsonType",
                "value": "JSON_OBJECT"
              },
              {
                "name": "fromJobConfig.fieldSeparator",
                "value": ","
              },
              {
                "name": "fromJobConfig.quoteChar",
                "value": "false"
              },
              {
                "name": "fromJobConfig.regexSeparator",
                "value": "false"
              },
              {
                "name": "fromJobConfig.firstRowAsHeader",
                "value": "false"
              },
              {
                "name": "fromJobConfig.encodeType",
                "value": "UTF-8"
              },
              {
                "name": "fromJobConfig.fromCompression",
                "value": "NONE"
              },
              {
                "name": "fromJobConfig.compressedFileSuffix",
                "value": "*"
              },
              {
                "name": "fromJobConfig.splitType",
                "value": "FILE"
              },
              {
                "name": "fromJobConfig.fromFileOpType",
                "value": "DO_NOTHING"
              },
              {
                "name": "fromJobConfig.useMarkerFile",
                "value": "false"
              },
              {
                "name": "fromJobConfig.fileSeparator",
                "value": "|"
              },
              {
                "name": "fromJobConfig.filterType",
                "value": "NONE"
              }
            ],
            "name": "fromJobConfig"
          }
        ]
      }
```

## 参数说明<a name="zh-cn_topic_0108272787_section32183847173555"></a>

-   HDFS作业参数说明

    <a name="zh-cn_topic_0108272787_table13922888141527"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0108272787_row229143141527"><th class="cellrowborder" valign="top" width="22.657734226577343%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272787_p16670181995619"><a name="zh-cn_topic_0108272787_p16670181995619"></a><a name="zh-cn_topic_0108272787_p16670181995619"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.96800319968003%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272787_p1867361912566"><a name="zh-cn_topic_0108272787_p1867361912566"></a><a name="zh-cn_topic_0108272787_p1867361912566"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.23827617238276%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272787_p3674171925614"><a name="zh-cn_topic_0108272787_p3674171925614"></a><a name="zh-cn_topic_0108272787_p3674171925614"></a>类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="40.135986401359865%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272787_p8677131955612"><a name="zh-cn_topic_0108272787_p8677131955612"></a><a name="zh-cn_topic_0108272787_p8677131955612"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0108272787_row62628929141527"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272787_p18560626141527"><a name="zh-cn_topic_0108272787_p18560626141527"></a><a name="zh-cn_topic_0108272787_p18560626141527"></a>fromJobConfig.inputDirectory</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.96800319968003%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272787_p27015713141527"><a name="zh-cn_topic_0108272787_p27015713141527"></a><a name="zh-cn_topic_0108272787_p27015713141527"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272787_p50167516142856"><a name="zh-cn_topic_0108272787_p50167516142856"></a><a name="zh-cn_topic_0108272787_p50167516142856"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.135986401359865%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272787_p2430205141527"><a name="zh-cn_topic_0108272787_p2430205141527"></a><a name="zh-cn_topic_0108272787_p2430205141527"></a>待抽取数据的路径，例如：<span class="parmvalue" id="zh-cn_topic_0108272787_parmvalue4700711494936"><a name="zh-cn_topic_0108272787_parmvalue4700711494936"></a><a name="zh-cn_topic_0108272787_parmvalue4700711494936"></a>“/data_dir”</span>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272787_row42094113141527"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272787_p26789449141527"><a name="zh-cn_topic_0108272787_p26789449141527"></a><a name="zh-cn_topic_0108272787_p26789449141527"></a>fromJobConfig.inputFormat</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.96800319968003%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272787_p22461756141527"><a name="zh-cn_topic_0108272787_p22461756141527"></a><a name="zh-cn_topic_0108272787_p22461756141527"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272787_p7462956141527"><a name="zh-cn_topic_0108272787_p7462956141527"></a><a name="zh-cn_topic_0108272787_p7462956141527"></a>枚举</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.135986401359865%" headers="mcps1.1.5.1.4 "><div class="p" id="zh-cn_topic_0108272787_p38464865164333"><a name="zh-cn_topic_0108272787_p38464865164333"></a><a name="zh-cn_topic_0108272787_p38464865164333"></a>传输数据时所用的文件格式，目前支持以下文件格式：<a name="zh-cn_topic_0108272787_u5620b8a5e51e4cf8b56d59790c671ce3"></a><a name="zh-cn_topic_0108272787_u5620b8a5e51e4cf8b56d59790c671ce3"></a><ul id="zh-cn_topic_0108272787_u5620b8a5e51e4cf8b56d59790c671ce3"><li>CSV_FILE：CSV格式。</li><li>PARQUET_FILE：PARQUET格式。</li><li>BINARY_FILE：二进制格式。</li></ul>
    </div>
    <p id="zh-cn_topic_0108272787_p12369546164333"><a name="zh-cn_topic_0108272787_p12369546164333"></a><a name="zh-cn_topic_0108272787_p12369546164333"></a>当选择<span class="parmvalue" id="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue4805818695742"><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue4805818695742"></a><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue4805818695742"></a>“BINARY_FILE”</span>时，目的端也必须为文件系统。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272787_row8336449141527"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272787_p29681527141527"><a name="zh-cn_topic_0108272787_p29681527141527"></a><a name="zh-cn_topic_0108272787_p29681527141527"></a>fromJobConfig.columnList</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.96800319968003%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272787_p55393515141527"><a name="zh-cn_topic_0108272787_p55393515141527"></a><a name="zh-cn_topic_0108272787_p55393515141527"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272787_p57689731141527"><a name="zh-cn_topic_0108272787_p57689731141527"></a><a name="zh-cn_topic_0108272787_p57689731141527"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.135986401359865%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272787_p37985002193940"><a name="zh-cn_topic_0108272787_p37985002193940"></a><a name="zh-cn_topic_0108272787_p37985002193940"></a>需要抽取的列号，列号之间使用<span class="parmvalue" id="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue36226019586"><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue36226019586"></a><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue36226019586"></a>“&amp;”</span>分割，并由小到大排序，例如：<span class="parmvalue" id="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue6416671195818"><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue6416671195818"></a><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue6416671195818"></a>“1&amp;3&amp;5”</span>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272787_row3034171115124"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272787_p3395516415124"><a name="zh-cn_topic_0108272787_p3395516415124"></a><a name="zh-cn_topic_0108272787_p3395516415124"></a>fromJobConfig.lineSeparator</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.96800319968003%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272787_p6601372415124"><a name="zh-cn_topic_0108272787_p6601372415124"></a><a name="zh-cn_topic_0108272787_p6601372415124"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272787_p4551140015124"><a name="zh-cn_topic_0108272787_p4551140015124"></a><a name="zh-cn_topic_0108272787_p4551140015124"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.135986401359865%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272787_p5480229817929"><a name="zh-cn_topic_0108272787_p5480229817929"></a><a name="zh-cn_topic_0108272787_p5480229817929"></a>换行符，当文件格式为<span class="parmvalue" id="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue5573206395833"><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue5573206395833"></a><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue5573206395833"></a>“CSV_FILE”</span>时此参数有效，默认值为：<span class="parmvalue" id="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue1131293795837"><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue1131293795837"></a><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue1131293795837"></a>“\r\n”</span>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272787_row4065400315124"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272787_p2824781215124"><a name="zh-cn_topic_0108272787_p2824781215124"></a><a name="zh-cn_topic_0108272787_p2824781215124"></a>fromJobConfig.fieldSeparator</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.96800319968003%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272787_p637144815124"><a name="zh-cn_topic_0108272787_p637144815124"></a><a name="zh-cn_topic_0108272787_p637144815124"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272787_p4632524315124"><a name="zh-cn_topic_0108272787_p4632524315124"></a><a name="zh-cn_topic_0108272787_p4632524315124"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.135986401359865%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272787_p3152061417929"><a name="zh-cn_topic_0108272787_p3152061417929"></a><a name="zh-cn_topic_0108272787_p3152061417929"></a>字段分隔符，当文件格式为<span class="parmvalue" id="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue3066733595853"><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue3066733595853"></a><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue3066733595853"></a>“CSV_FILE”</span>时此参数有效，默认值为：<span class="parmvalue" id="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue1399095795859"><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue1399095795859"></a><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue1399095795859"></a>“,”</span>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272787_row46472373171014"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272787_p66009299193940"><a name="zh-cn_topic_0108272787_p66009299193940"></a><a name="zh-cn_topic_0108272787_p66009299193940"></a>fromJobConfig.encodeType</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.96800319968003%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272787_p45152983193940"><a name="zh-cn_topic_0108272787_p45152983193940"></a><a name="zh-cn_topic_0108272787_p45152983193940"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272787_p33513000193940"><a name="zh-cn_topic_0108272787_p33513000193940"></a><a name="zh-cn_topic_0108272787_p33513000193940"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.135986401359865%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272787_p30198445193940"><a name="zh-cn_topic_0108272787_p30198445193940"></a><a name="zh-cn_topic_0108272787_p30198445193940"></a>编码类型，例如：<span class="parmvalue" id="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue4489407595918"><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue4489407595918"></a><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue4489407595918"></a>“UTF_8”</span>或<span class="parmvalue" id="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue3309953795922"><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue3309953795922"></a><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue3309953795922"></a>“GBK”</span>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272787_row17517103911525"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272787_p1482152417486"><a name="zh-cn_topic_0108272787_p1482152417486"></a><a name="zh-cn_topic_0108272787_p1482152417486"></a>fromJobConfig.firstRowAsHeader</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.96800319968003%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272787_p3517133955220"><a name="zh-cn_topic_0108272787_p3517133955220"></a><a name="zh-cn_topic_0108272787_p3517133955220"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272787_p15171739145218"><a name="zh-cn_topic_0108272787_p15171739145218"></a><a name="zh-cn_topic_0108272787_p15171739145218"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.135986401359865%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272787_p20517239185219"><a name="zh-cn_topic_0108272787_p20517239185219"></a><a name="zh-cn_topic_0108272787_p20517239185219"></a>是否默认首行为标题行，当文件格式为<span class="parmvalue" id="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue1467312083111"><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue1467312083111"></a><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue1467312083111"></a>“CSV_FILE”</span>时此参数有效。在迁移CSV文件到表时，CDM默认是全部写入，当该参数选择<span class="parmvalue" id="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue11024151389"><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue11024151389"></a><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue11024151389"></a>“true”</span>时，CDM会将CSV文件的第一行数据作为标题行，不写入目的端的表。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272787_row6246161713307"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272787_p12247121733015"><a name="zh-cn_topic_0108272787_p12247121733015"></a><a name="zh-cn_topic_0108272787_p12247121733015"></a>fromJobConfig.fromCompression</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.96800319968003%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272787_p52478177306"><a name="zh-cn_topic_0108272787_p52478177306"></a><a name="zh-cn_topic_0108272787_p52478177306"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272787_p46668477103023"><a name="zh-cn_topic_0108272787_p46668477103023"></a><a name="zh-cn_topic_0108272787_p46668477103023"></a>枚举</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.135986401359865%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272787_p22050281103023"><a name="zh-cn_topic_0108272787_p22050281103023"></a><a name="zh-cn_topic_0108272787_p22050281103023"></a>压缩格式，表示选择只传输对应压缩格式的源文件。<span class="parmvalue" id="zh-cn_topic_0108272787_parmvalue39996941103332"><a name="zh-cn_topic_0108272787_parmvalue39996941103332"></a><a name="zh-cn_topic_0108272787_parmvalue39996941103332"></a>“NONE”</span>表示传输所有格式的文件。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272787_row41911953165237"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272787_p38366493193940"><a name="zh-cn_topic_0108272787_p38366493193940"></a><a name="zh-cn_topic_0108272787_p38366493193940"></a>fromJobConfig.splitType</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.96800319968003%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272787_p20678213193940"><a name="zh-cn_topic_0108272787_p20678213193940"></a><a name="zh-cn_topic_0108272787_p20678213193940"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272787_p64322533193940"><a name="zh-cn_topic_0108272787_p64322533193940"></a><a name="zh-cn_topic_0108272787_p64322533193940"></a>枚举</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.135986401359865%" headers="mcps1.1.5.1.4 "><div class="p" id="zh-cn_topic_0108272787_p1725054113534"><a name="zh-cn_topic_0108272787_p1725054113534"></a><a name="zh-cn_topic_0108272787_p1725054113534"></a>指定任务分片方式，选择按文件或文件大小进行分割。HDFS上的文件，如果在HDFS上已经分片，则HDFS每个分片视为一个文件。<a name="zh-cn_topic_0108272787_ul17679437141210"></a><a name="zh-cn_topic_0108272787_ul17679437141210"></a><ul id="zh-cn_topic_0108272787_ul17679437141210"><li>FILE：按文件数量进行分片。例如有10个文件，并在任务参数中指定<span class="parmname" id="zh-cn_topic_0108272787_parmname1358017585120"><a name="zh-cn_topic_0108272787_parmname1358017585120"></a><a name="zh-cn_topic_0108272787_parmname1358017585120"></a>“throttlingConfig.numExtractors”</span>（抽取并发数）为<span class="parmvalue" id="zh-cn_topic_0108272787_parmvalue19679537121220"><a name="zh-cn_topic_0108272787_parmvalue19679537121220"></a><a name="zh-cn_topic_0108272787_parmvalue19679537121220"></a>“5”</span>，则每个分片2个文件。</li><li>SIZE：按文件大小分割。注意这里不会将文件做切分来实现均衡。例如：有10个文件，9个10M，1个200M，在并发任务数中指定<span class="parmname" id="zh-cn_topic_0108272787_parmname1142720241137"><a name="zh-cn_topic_0108272787_parmname1142720241137"></a><a name="zh-cn_topic_0108272787_parmname1142720241137"></a>“throttlingConfig.numExtractors”</span>（抽取并发数）为<span class="parmvalue" id="zh-cn_topic_0108272787_parmvalue66793372126"><a name="zh-cn_topic_0108272787_parmvalue66793372126"></a><a name="zh-cn_topic_0108272787_parmvalue66793372126"></a>“2”</span>，则会分两个分片，一个处理9个10M的文件，一个处理1个200M的文件。</li></ul>
    </div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272787_row19998202812370"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272787_p6998828133713"><a name="zh-cn_topic_0108272787_p6998828133713"></a><a name="zh-cn_topic_0108272787_p6998828133713"></a>fromJobConfig.fromFileOpType</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.96800319968003%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272787_p199987287376"><a name="zh-cn_topic_0108272787_p199987287376"></a><a name="zh-cn_topic_0108272787_p199987287376"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272787_p6998142810373"><a name="zh-cn_topic_0108272787_p6998142810373"></a><a name="zh-cn_topic_0108272787_p6998142810373"></a>枚举</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.135986401359865%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272787_p999812281378"><a name="zh-cn_topic_0108272787_p999812281378"></a><a name="zh-cn_topic_0108272787_p999812281378"></a>源文件处理方式，作业完成后对源端文件的操作，支持重命名或删除源端文件。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272787_row35215953910"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272787_p11521793391"><a name="zh-cn_topic_0108272787_p11521793391"></a><a name="zh-cn_topic_0108272787_p11521793391"></a>fromJobConfig.markerFile</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.96800319968003%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272787_p63489546171234"><a name="zh-cn_topic_0108272787_p63489546171234"></a><a name="zh-cn_topic_0108272787_p63489546171234"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272787_p42379607171234"><a name="zh-cn_topic_0108272787_p42379607171234"></a><a name="zh-cn_topic_0108272787_p42379607171234"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.135986401359865%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272787_p10196161171234"><a name="zh-cn_topic_0108272787_p10196161171234"></a><a name="zh-cn_topic_0108272787_p10196161171234"></a>启动作业的标识文件名。指定文件后，只有在源端路径下存在该文件的情况下才会运行任务，不指定时默认不启用该功能，例如：<span class="filepath" id="zh-cn_topic_0108272787_zh-cn_topic_0108272831_filepath47013227185444"><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_filepath47013227185444"></a><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_filepath47013227185444"></a>“ok.txt”</span>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272787_row696792714011"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272787_p36206523193940"><a name="zh-cn_topic_0108272787_p36206523193940"></a><a name="zh-cn_topic_0108272787_p36206523193940"></a>fromJobConfig.filterType</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.96800319968003%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272787_p47047254193940"><a name="zh-cn_topic_0108272787_p47047254193940"></a><a name="zh-cn_topic_0108272787_p47047254193940"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272787_p52731205193940"><a name="zh-cn_topic_0108272787_p52731205193940"></a><a name="zh-cn_topic_0108272787_p52731205193940"></a>枚举</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.135986401359865%" headers="mcps1.1.5.1.4 "><div class="p" id="zh-cn_topic_0108272787_p43369201193940"><a name="zh-cn_topic_0108272787_p43369201193940"></a><a name="zh-cn_topic_0108272787_p43369201193940"></a>选择过滤器类型：<a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_ul32827929185645"></a><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_ul32827929185645"></a><ul id="zh-cn_topic_0108272787_zh-cn_topic_0108272831_ul32827929185645"><li>WILDCARD：输入通配符作为过滤文件，满足过滤条件的路径或文件会被传输。</li><li>TIME：时间过滤器，当文件的修改时间晚于输入的时间时，该文件才会被传输。</li></ul>
    </div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272787_row7813105174114"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272787_p34862062193940"><a name="zh-cn_topic_0108272787_p34862062193940"></a><a name="zh-cn_topic_0108272787_p34862062193940"></a>fromJobConfig.pathFilter</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.96800319968003%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272787_p5254812193940"><a name="zh-cn_topic_0108272787_p5254812193940"></a><a name="zh-cn_topic_0108272787_p5254812193940"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272787_p22986638193940"><a name="zh-cn_topic_0108272787_p22986638193940"></a><a name="zh-cn_topic_0108272787_p22986638193940"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.135986401359865%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272787_p49978413193940"><a name="zh-cn_topic_0108272787_p49978413193940"></a><a name="zh-cn_topic_0108272787_p49978413193940"></a>路径过滤器，过滤类型为通配符时配置，用于过滤文件目录，例如：<span class="uicontrol" id="zh-cn_topic_0108272787_zh-cn_topic_0108272831_uicontrol66669561185917"><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_uicontrol66669561185917"></a><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_uicontrol66669561185917"></a>“*input”</span>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272787_row16113153914405"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272787_p14461072193940"><a name="zh-cn_topic_0108272787_p14461072193940"></a><a name="zh-cn_topic_0108272787_p14461072193940"></a>fromJobConfig.fileFilter</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.96800319968003%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272787_p30496164193940"><a name="zh-cn_topic_0108272787_p30496164193940"></a><a name="zh-cn_topic_0108272787_p30496164193940"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272787_p54270213193940"><a name="zh-cn_topic_0108272787_p54270213193940"></a><a name="zh-cn_topic_0108272787_p54270213193940"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.135986401359865%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272787_p33811098193940"><a name="zh-cn_topic_0108272787_p33811098193940"></a><a name="zh-cn_topic_0108272787_p33811098193940"></a>文件过滤器，过滤类型为通配符时配置，用于过滤目录下的文件，支持配置多个文件，中间使用<span class="parmvalue" id="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue125501853131710"><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue125501853131710"></a><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmvalue125501853131710"></a>“,”</span>分隔，例如：<span class="uicontrol" id="zh-cn_topic_0108272787_zh-cn_topic_0108272831_uicontrol4491163718912"><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_uicontrol4491163718912"></a><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_uicontrol4491163718912"></a>“*.csv,*.txt”</span>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272787_row1711597141"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272787_p101771547152117"><a name="zh-cn_topic_0108272787_p101771547152117"></a><a name="zh-cn_topic_0108272787_p101771547152117"></a>fromJobConfig.startTime</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.96800319968003%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272787_p574033312314"><a name="zh-cn_topic_0108272787_p574033312314"></a><a name="zh-cn_topic_0108272787_p574033312314"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272787_p1085074720811"><a name="zh-cn_topic_0108272787_p1085074720811"></a><a name="zh-cn_topic_0108272787_p1085074720811"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.135986401359865%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272787_p18311447203911"><a name="zh-cn_topic_0108272787_p18311447203911"></a><a name="zh-cn_topic_0108272787_p18311447203911"></a><span class="parmname" id="zh-cn_topic_0108272787_zh-cn_topic_0108275319_parmname4237191913013"><a name="zh-cn_topic_0108272787_zh-cn_topic_0108275319_parmname4237191913013"></a><a name="zh-cn_topic_0108272787_zh-cn_topic_0108275319_parmname4237191913013"></a>“过滤类型”</span>选择<span class="parmvalue" id="zh-cn_topic_0108272787_zh-cn_topic_0108275319_parmvalue933016296308"><a name="zh-cn_topic_0108272787_zh-cn_topic_0108275319_parmvalue933016296308"></a><a name="zh-cn_topic_0108272787_zh-cn_topic_0108275319_parmvalue933016296308"></a>“时间过滤器”</span>时，可以指定一个时间值，当文件的修改时间大于该时间才会被传输，输入的时间格式需为<span class="parmvalue" id="zh-cn_topic_0108272787_zh-cn_topic_0108275319_parmvalue9313481341"><a name="zh-cn_topic_0108272787_zh-cn_topic_0108275319_parmvalue9313481341"></a><a name="zh-cn_topic_0108272787_zh-cn_topic_0108275319_parmvalue9313481341"></a>“yyyy-MM-dd HH:mm:ss”</span>。</p>
    <p id="zh-cn_topic_0108272787_p12144111817144"><a name="zh-cn_topic_0108272787_p12144111817144"></a><a name="zh-cn_topic_0108272787_p12144111817144"></a>该参数支持配置为时间宏变量，例如<strong id="zh-cn_topic_0108272787_zh-cn_topic_0108275319_b97861314103"><a name="zh-cn_topic_0108272787_zh-cn_topic_0108275319_b97861314103"></a><a name="zh-cn_topic_0108272787_zh-cn_topic_0108275319_b97861314103"></a>${timestamp(dateformat(yyyy-MM-dd HH:mm:ss,-90,DAY))}</strong>表示：只迁移最近90天内的文件。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272787_row9604124014240"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272787_p2076744121718"><a name="zh-cn_topic_0108272787_p2076744121718"></a><a name="zh-cn_topic_0108272787_p2076744121718"></a>fromJobConfig.endTime</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.96800319968003%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272787_p176712419173"><a name="zh-cn_topic_0108272787_p176712419173"></a><a name="zh-cn_topic_0108272787_p176712419173"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272787_p155977520229"><a name="zh-cn_topic_0108272787_p155977520229"></a><a name="zh-cn_topic_0108272787_p155977520229"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.135986401359865%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272787_p34921611171416"><a name="zh-cn_topic_0108272787_p34921611171416"></a><a name="zh-cn_topic_0108272787_p34921611171416"></a><span class="parmname" id="zh-cn_topic_0108272787_zh-cn_topic_0108275319_parmname106751314209"><a name="zh-cn_topic_0108272787_zh-cn_topic_0108275319_parmname106751314209"></a><a name="zh-cn_topic_0108272787_zh-cn_topic_0108275319_parmname106751314209"></a>“过滤类型”</span>选择<span class="parmvalue" id="zh-cn_topic_0108272787_zh-cn_topic_0108275319_parmvalue13675131413012"><a name="zh-cn_topic_0108272787_zh-cn_topic_0108275319_parmvalue13675131413012"></a><a name="zh-cn_topic_0108272787_zh-cn_topic_0108275319_parmvalue13675131413012"></a>“时间过滤器”</span>时，可以指定一个时间值，当文件的修改时间小于该时间才会被传输，输入的时间格式需为<span class="parmvalue" id="zh-cn_topic_0108272787_zh-cn_topic_0108275319_parmvalue146759148017"><a name="zh-cn_topic_0108272787_zh-cn_topic_0108275319_parmvalue146759148017"></a><a name="zh-cn_topic_0108272787_zh-cn_topic_0108275319_parmvalue146759148017"></a>“yyyy-MM-dd HH:mm:ss”</span>。</p>
    <p id="zh-cn_topic_0108272787_p13254806156"><a name="zh-cn_topic_0108272787_p13254806156"></a><a name="zh-cn_topic_0108272787_p13254806156"></a>该参数支持配置为时间宏变量，例如<strong id="zh-cn_topic_0108272787_zh-cn_topic_0108275319_b1521616538112"><a name="zh-cn_topic_0108272787_zh-cn_topic_0108275319_b1521616538112"></a><a name="zh-cn_topic_0108272787_zh-cn_topic_0108275319_b1521616538112"></a>${timestamp(dateformat(yyyy-MM-dd HH:mm:ss))}</strong>表示：只迁移修改时间为当前时间以前的文件。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272787_row88218247315"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272787_p48211124739"><a name="zh-cn_topic_0108272787_p48211124739"></a><a name="zh-cn_topic_0108272787_p48211124739"></a>fromJobConfig.createSnapshot</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.96800319968003%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272787_p158211124537"><a name="zh-cn_topic_0108272787_p158211124537"></a><a name="zh-cn_topic_0108272787_p158211124537"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272787_p1982182415320"><a name="zh-cn_topic_0108272787_p1982182415320"></a><a name="zh-cn_topic_0108272787_p1982182415320"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.135986401359865%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272787_p17617269485"><a name="zh-cn_topic_0108272787_p17617269485"></a><a name="zh-cn_topic_0108272787_p17617269485"></a>如果配置为<span class="parmvalue" id="zh-cn_topic_0108272787_parmvalue4617176154813"><a name="zh-cn_topic_0108272787_parmvalue4617176154813"></a><a name="zh-cn_topic_0108272787_parmvalue4617176154813"></a>“true”</span>，CDM读取HDFS系统上的文件时，会先对待迁移的源目录创建快照（不允许对单个文件创建快照），然后CDM迁移快照中的数据。</p>
    <p id="zh-cn_topic_0108272787_p20194131216207"><a name="zh-cn_topic_0108272787_p20194131216207"></a><a name="zh-cn_topic_0108272787_p20194131216207"></a>需要HDFS系统的管理员权限才可以创建快照，CDM作业完成后，快照会被删除。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272787_row64475722155949"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272787_p32328561155955"><a name="zh-cn_topic_0108272787_p32328561155955"></a><a name="zh-cn_topic_0108272787_p32328561155955"></a>fromJobConfig.formats</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.96800319968003%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272787_p1367823155955"><a name="zh-cn_topic_0108272787_p1367823155955"></a><a name="zh-cn_topic_0108272787_p1367823155955"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272787_p43684849155955"><a name="zh-cn_topic_0108272787_p43684849155955"></a><a name="zh-cn_topic_0108272787_p43684849155955"></a>数据结构</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.135986401359865%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272787_p48811904155955"><a name="zh-cn_topic_0108272787_p48811904155955"></a><a name="zh-cn_topic_0108272787_p48811904155955"></a>时间格式，当<span class="parmname" id="zh-cn_topic_0108272787_parmname2109606695218"><a name="zh-cn_topic_0108272787_parmname2109606695218"></a><a name="zh-cn_topic_0108272787_parmname2109606695218"></a>“fromJobConfig.inputFormat”</span>（文件格式）为<span class="parmvalue" id="zh-cn_topic_0108272787_parmvalue2230480195223"><a name="zh-cn_topic_0108272787_parmvalue2230480195223"></a><a name="zh-cn_topic_0108272787_parmvalue2230480195223"></a>“CSV_FILE”</span>（CSV格式），并且文件中有时间类型字段时，才需要输入，具体说明请参见<a href="#zh-cn_topic_0108272787_li8656627114417">fromJobConfig.formats参数说明</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272787_row168341736112920"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272787_p5622115931110"><a name="zh-cn_topic_0108272787_p5622115931110"></a><a name="zh-cn_topic_0108272787_p5622115931110"></a>fromJobConfig.decryption</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.96800319968003%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272787_p10622125919118"><a name="zh-cn_topic_0108272787_p10622125919118"></a><a name="zh-cn_topic_0108272787_p10622125919118"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272787_p1762214595111"><a name="zh-cn_topic_0108272787_p1762214595111"></a><a name="zh-cn_topic_0108272787_p1762214595111"></a>枚举</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.135986401359865%" headers="mcps1.1.5.1.4 "><div class="p" id="zh-cn_topic_0108272787_p268631112373"><a name="zh-cn_topic_0108272787_p268631112373"></a><a name="zh-cn_topic_0108272787_p268631112373"></a><span class="parmname" id="zh-cn_topic_0108272787_parmname1050910131064"><a name="zh-cn_topic_0108272787_parmname1050910131064"></a><a name="zh-cn_topic_0108272787_parmname1050910131064"></a>“fromJobConfig.inputFormat”</span>（文件格式）选择为<span class="parmvalue" id="zh-cn_topic_0108272787_parmvalue15321226162614"><a name="zh-cn_topic_0108272787_parmvalue15321226162614"></a><a name="zh-cn_topic_0108272787_parmvalue15321226162614"></a>“BINARY_FILE”</span>（二进制格式）时才有该参数，选择是否对已加密的文件解密后再导出，以及解密方式：<a name="zh-cn_topic_0108272787_ul193603764111"></a><a name="zh-cn_topic_0108272787_ul193603764111"></a><ul id="zh-cn_topic_0108272787_ul193603764111"><li>NONE：不解密，直接导出文件。</li><li>AES-256-GCM：使用AES-256-GCM（NoPadding）算法解密后再导出文件。</li></ul>
    </div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272787_row14459123772917"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272787_p167122217132"><a name="zh-cn_topic_0108272787_p167122217132"></a><a name="zh-cn_topic_0108272787_p167122217132"></a>fromJobConfig.dek</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.96800319968003%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272787_p74741127142115"><a name="zh-cn_topic_0108272787_p74741127142115"></a><a name="zh-cn_topic_0108272787_p74741127142115"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272787_p2474627102111"><a name="zh-cn_topic_0108272787_p2474627102111"></a><a name="zh-cn_topic_0108272787_p2474627102111"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.135986401359865%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272787_p23281415172211"><a name="zh-cn_topic_0108272787_p23281415172211"></a><a name="zh-cn_topic_0108272787_p23281415172211"></a>数据解密密钥，密钥由长度64的十六进制数组成，且必须与加密时配置的<span class="parmname" id="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmname1660363014167"><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmname1660363014167"></a><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmname1660363014167"></a>“toJobConfig.dek”</span>（导入时配置的数据加密密钥）一致。如果不一致系统不会报异常，只是解密出来的数据会错误。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272787_row249323862914"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272787_p26851918151311"><a name="zh-cn_topic_0108272787_p26851918151311"></a><a name="zh-cn_topic_0108272787_p26851918151311"></a>fromJobConfig.iv</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.96800319968003%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272787_p1114152632113"><a name="zh-cn_topic_0108272787_p1114152632113"></a><a name="zh-cn_topic_0108272787_p1114152632113"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.23827617238276%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272787_p1414162617212"><a name="zh-cn_topic_0108272787_p1414162617212"></a><a name="zh-cn_topic_0108272787_p1414162617212"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.135986401359865%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272787_p24771354512"><a name="zh-cn_topic_0108272787_p24771354512"></a><a name="zh-cn_topic_0108272787_p24771354512"></a>解密需要的初始化向量，初始化向量由长度32的十六进制数组成，且必须与加密时配置的<span class="parmname" id="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmname1257711377164"><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmname1257711377164"></a><a name="zh-cn_topic_0108272787_zh-cn_topic_0108272831_parmname1257711377164"></a>“toJobConfig.iv”</span>（导入时配置的初始化向量）一致。如果不一致系统不会报异常，只是解密出来的数据会错误。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   <a name="zh-cn_topic_0108272787_li8656627114417"></a>fromJobConfig.formats参数说明

    <a name="zh-cn_topic_0108272787_table1965782716445"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0108272787_row165802724414"><th class="cellrowborder" valign="top" width="20.987901209879013%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272787_p13658527194415"><a name="zh-cn_topic_0108272787_p13658527194415"></a><a name="zh-cn_topic_0108272787_p13658527194415"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.567843215678433%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272787_p186581627174419"><a name="zh-cn_topic_0108272787_p186581627174419"></a><a name="zh-cn_topic_0108272787_p186581627174419"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.25827417258274%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272787_p12658527144418"><a name="zh-cn_topic_0108272787_p12658527144418"></a><a name="zh-cn_topic_0108272787_p12658527144418"></a>类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="40.18598140185981%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272787_p19659127104411"><a name="zh-cn_topic_0108272787_p19659127104411"></a><a name="zh-cn_topic_0108272787_p19659127104411"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0108272787_row266082784414"><td class="cellrowborder" valign="top" width="20.987901209879013%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272787_p96601227124420"><a name="zh-cn_topic_0108272787_p96601227124420"></a><a name="zh-cn_topic_0108272787_p96601227124420"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.567843215678433%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272787_p466072714441"><a name="zh-cn_topic_0108272787_p466072714441"></a><a name="zh-cn_topic_0108272787_p466072714441"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.25827417258274%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272787_p1166042714416"><a name="zh-cn_topic_0108272787_p1166042714416"></a><a name="zh-cn_topic_0108272787_p1166042714416"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.18598140185981%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272787_p1661327174410"><a name="zh-cn_topic_0108272787_p1661327174410"></a><a name="zh-cn_topic_0108272787_p1661327174410"></a>列号，例如：<span class="parmvalue" id="zh-cn_topic_0108272787_parmvalue66611727104415"><a name="zh-cn_topic_0108272787_parmvalue66611727104415"></a><a name="zh-cn_topic_0108272787_parmvalue66611727104415"></a>“1”</span>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272787_row6661132734417"><td class="cellrowborder" valign="top" width="20.987901209879013%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272787_p866122712443"><a name="zh-cn_topic_0108272787_p866122712443"></a><a name="zh-cn_topic_0108272787_p866122712443"></a>value</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.567843215678433%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272787_p266292713448"><a name="zh-cn_topic_0108272787_p266292713448"></a><a name="zh-cn_topic_0108272787_p266292713448"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.25827417258274%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272787_p4662132734420"><a name="zh-cn_topic_0108272787_p4662132734420"></a><a name="zh-cn_topic_0108272787_p4662132734420"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.18598140185981%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272787_p11662182744412"><a name="zh-cn_topic_0108272787_p11662182744412"></a><a name="zh-cn_topic_0108272787_p11662182744412"></a>时间格式，例如：<span class="parmvalue" id="zh-cn_topic_0108272787_parmvalue12662182724413"><a name="zh-cn_topic_0108272787_parmvalue12662182724413"></a><a name="zh-cn_topic_0108272787_parmvalue12662182724413"></a>“yyyy-MM-dd”</span>。</p>
    </td>
    </tr>
    </tbody>
    </table>


