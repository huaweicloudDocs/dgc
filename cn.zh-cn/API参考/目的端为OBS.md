# 目的端为OBS<a name="dgc_02_0297"></a>

## JSON样例<a name="zh-cn_topic_0108272820_section33401108172339"></a>

```
"to-config-values": {
        "configs": [
          {
            "inputs": [
              {
                "name": "toJobConfig.bucketName",
                "value": "cdm"
              },
              {
                "name": "toJobConfig.outputDirectory",
                "value": "/obsfrom/advance/"
              },
              {
                "name": "toJobConfig.outputFormat",
                "value": "CSV_FILE"
              },
              {
                "name": "toJobConfig.fieldSeparator",
                "value": ","
              },
              {
                "name": "toJobConfig.writeToTempFile",
                "value": "false"
              },
              {
                "name": "toJobConfig.validateMD5",
                "value": "false"
              },
              {
                "name": "toJobConfig.recordMD5Result",
                "value": "false"
              },
              {
                "name": "toJobConfig.encodeType",
                "value": "UTF-8"
              },
              {
                "name": "toJobConfig.markerFile",
                "value": "finish.txt"
              },
              {
                "name": "toJobConfig.duplicateFileOpType",
                "value": "REPLACE"
              },
              {
                "name": "toJobConfig.shouldClearTable",
                "value": "false"
              },
              {
                "name": "toJobConfig.columnList",
                "value": "1&2"
              },
              {
                "name": "toJobConfig.quoteChar",
                "value": "false"
              },
              {
                "name": "toJobConfig.encryption",
                "value": "NONE"
              },
              {
                "name": "toJobConfig.copyContentType",
                "value": "false"
              }
            ],
            "name": "toJobConfig"
          }
        ]
      }
```

## 参数说明<a name="zh-cn_topic_0108272820_section4696198610432"></a>

<a name="zh-cn_topic_0108272820_table13922888141527"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108272820_row229143141527"><th class="cellrowborder" valign="top" width="22.66%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272820_p66756185141527"><a name="zh-cn_topic_0108272820_p66756185141527"></a><a name="zh-cn_topic_0108272820_p66756185141527"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="19.78%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272820_p38541938141527"><a name="zh-cn_topic_0108272820_p38541938141527"></a><a name="zh-cn_topic_0108272820_p38541938141527"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="19.49%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272820_p34889279141527"><a name="zh-cn_topic_0108272820_p34889279141527"></a><a name="zh-cn_topic_0108272820_p34889279141527"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="38.07%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272820_p7459369141527"><a name="zh-cn_topic_0108272820_p7459369141527"></a><a name="zh-cn_topic_0108272820_p7459369141527"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108272820_row200694164748"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272820_p3511073516484"><a name="zh-cn_topic_0108272820_p3511073516484"></a><a name="zh-cn_topic_0108272820_p3511073516484"></a>toJobConfig.bucketName</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272820_p2539731116484"><a name="zh-cn_topic_0108272820_p2539731116484"></a><a name="zh-cn_topic_0108272820_p2539731116484"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.49%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272820_p4391632816484"><a name="zh-cn_topic_0108272820_p4391632816484"></a><a name="zh-cn_topic_0108272820_p4391632816484"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272820_p45278516484"><a name="zh-cn_topic_0108272820_p45278516484"></a><a name="zh-cn_topic_0108272820_p45278516484"></a>OBS的桶名，例如<span class="parmvalue" id="zh-cn_topic_0108272820_parmvalue20492907101353"><a name="zh-cn_topic_0108272820_parmvalue20492907101353"></a><a name="zh-cn_topic_0108272820_parmvalue20492907101353"></a>“cdm”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272820_row62628929141527"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272820_p18560626141527"><a name="zh-cn_topic_0108272820_p18560626141527"></a><a name="zh-cn_topic_0108272820_p18560626141527"></a>toJobConfig.outputDirectory</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272820_p27015713141527"><a name="zh-cn_topic_0108272820_p27015713141527"></a><a name="zh-cn_topic_0108272820_p27015713141527"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.49%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272820_p50167516142856"><a name="zh-cn_topic_0108272820_p50167516142856"></a><a name="zh-cn_topic_0108272820_p50167516142856"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272820_p2430205141527"><a name="zh-cn_topic_0108272820_p2430205141527"></a><a name="zh-cn_topic_0108272820_p2430205141527"></a>数据写入路径，例如<span class="parmvalue" id="zh-cn_topic_0108272820_parmvalue1907513110141"><a name="zh-cn_topic_0108272820_parmvalue1907513110141"></a><a name="zh-cn_topic_0108272820_parmvalue1907513110141"></a>“data_dir”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272820_row42094113141527"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272820_p26789449141527"><a name="zh-cn_topic_0108272820_p26789449141527"></a><a name="zh-cn_topic_0108272820_p26789449141527"></a>toJobConfig.outputFormat</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272820_p22461756141527"><a name="zh-cn_topic_0108272820_p22461756141527"></a><a name="zh-cn_topic_0108272820_p22461756141527"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.49%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272820_p7462956141527"><a name="zh-cn_topic_0108272820_p7462956141527"></a><a name="zh-cn_topic_0108272820_p7462956141527"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><div class="p" id="zh-cn_topic_0108272820_p519680141527"><a name="zh-cn_topic_0108272820_p519680141527"></a><a name="zh-cn_topic_0108272820_p519680141527"></a>写入数据时所用的文件格式（二进制除外），支持以下文件格式：<a name="zh-cn_topic_0108272820_ul6294852210148"></a><a name="zh-cn_topic_0108272820_ul6294852210148"></a><ul id="zh-cn_topic_0108272820_ul6294852210148"><li>CSV_FILE：按照CSV格式写入数据。</li><li>BINARY_FILE：二进制格式，不解析文件内容直接传输，CDM会原样写入文件，不改变原始文件格式。</li></ul>
</div>
<p id="zh-cn_topic_0108272820_p3415682014487"><a name="zh-cn_topic_0108272820_p3415682014487"></a><a name="zh-cn_topic_0108272820_p3415682014487"></a>当选择<span class="parmvalue" id="zh-cn_topic_0108272820_parmvalue24403448101417"><a name="zh-cn_topic_0108272820_parmvalue24403448101417"></a><a name="zh-cn_topic_0108272820_parmvalue24403448101417"></a>“BINARY_FILE”</span>时，源端也必须为文件系统。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272820_row3307208110232"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272820_p33465993102324"><a name="zh-cn_topic_0108272820_p33465993102324"></a><a name="zh-cn_topic_0108272820_p33465993102324"></a>toJobConfig.fieldSeparator</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272820_p26390928102324"><a name="zh-cn_topic_0108272820_p26390928102324"></a><a name="zh-cn_topic_0108272820_p26390928102324"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.49%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272820_p57290452102324"><a name="zh-cn_topic_0108272820_p57290452102324"></a><a name="zh-cn_topic_0108272820_p57290452102324"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272820_p10015036102324"><a name="zh-cn_topic_0108272820_p10015036102324"></a><a name="zh-cn_topic_0108272820_p10015036102324"></a>列分割符号，当<span class="parmname" id="zh-cn_topic_0108272820_parmname11724115615167"><a name="zh-cn_topic_0108272820_parmname11724115615167"></a><a name="zh-cn_topic_0108272820_parmname11724115615167"></a>“toJobConfig.outputFormat”</span>（文件格式）为<span class="parmvalue" id="zh-cn_topic_0108272820_parmvalue5911601102324"><a name="zh-cn_topic_0108272820_parmvalue5911601102324"></a><a name="zh-cn_topic_0108272820_parmvalue5911601102324"></a>“CSV_FILE”</span>时此参数有效，默认值为：<span class="parmvalue" id="zh-cn_topic_0108272820_parmvalue53204411102324"><a name="zh-cn_topic_0108272820_parmvalue53204411102324"></a><a name="zh-cn_topic_0108272820_parmvalue53204411102324"></a>“,”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272820_row59961698111250"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272820_p25633059111255"><a name="zh-cn_topic_0108272820_p25633059111255"></a><a name="zh-cn_topic_0108272820_p25633059111255"></a>toJobConfig.lineSeparator</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272820_p63011862111255"><a name="zh-cn_topic_0108272820_p63011862111255"></a><a name="zh-cn_topic_0108272820_p63011862111255"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.49%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272820_p3687235111255"><a name="zh-cn_topic_0108272820_p3687235111255"></a><a name="zh-cn_topic_0108272820_p3687235111255"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272820_p30230608111255"><a name="zh-cn_topic_0108272820_p30230608111255"></a><a name="zh-cn_topic_0108272820_p30230608111255"></a>行分割符号，当<span class="parmname" id="zh-cn_topic_0108272820_parmname16832101781710"><a name="zh-cn_topic_0108272820_parmname16832101781710"></a><a name="zh-cn_topic_0108272820_parmname16832101781710"></a>“toJobConfig.outputFormat”</span>（文件格式）为<span class="parmvalue" id="zh-cn_topic_0108272820_parmvalue32760165111255"><a name="zh-cn_topic_0108272820_parmvalue32760165111255"></a><a name="zh-cn_topic_0108272820_parmvalue32760165111255"></a>“CSV_FILE”</span>时此参数有效，默认值为：<span class="parmvalue" id="zh-cn_topic_0108272820_parmvalue26406035111255"><a name="zh-cn_topic_0108272820_parmvalue26406035111255"></a><a name="zh-cn_topic_0108272820_parmvalue26406035111255"></a>“\<span id="zh-cn_topic_0108272820_text36327723111255"><a name="zh-cn_topic_0108272820_text36327723111255"></a><a name="zh-cn_topic_0108272820_text36327723111255"></a>r</span>\<span id="zh-cn_topic_0108272820_text58514056111255"><a name="zh-cn_topic_0108272820_text58514056111255"></a><a name="zh-cn_topic_0108272820_text58514056111255"></a>n</span>”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272820_row45671424144916"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272820_p1856762494910"><a name="zh-cn_topic_0108272820_p1856762494910"></a><a name="zh-cn_topic_0108272820_p1856762494910"></a>toJobConfig.writeFileSize</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272820_p1567122434919"><a name="zh-cn_topic_0108272820_p1567122434919"></a><a name="zh-cn_topic_0108272820_p1567122434919"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.49%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272820_p83091218170"><a name="zh-cn_topic_0108272820_p83091218170"></a><a name="zh-cn_topic_0108272820_p83091218170"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272820_p34895339587"><a name="zh-cn_topic_0108272820_p34895339587"></a><a name="zh-cn_topic_0108272820_p34895339587"></a>源端为数据库时该参数有效，支持按大小分成多个文件存储，避免导出的文件过大，单位为MB。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272820_row14439759155521"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272820_p32407119155527"><a name="zh-cn_topic_0108272820_p32407119155527"></a><a name="zh-cn_topic_0108272820_p32407119155527"></a>toJobConfig.duplicateFileOpType</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272820_p7730996155527"><a name="zh-cn_topic_0108272820_p7730996155527"></a><a name="zh-cn_topic_0108272820_p7730996155527"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.49%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272820_p22230925155527"><a name="zh-cn_topic_0108272820_p22230925155527"></a><a name="zh-cn_topic_0108272820_p22230925155527"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><div class="p" id="zh-cn_topic_0108272820_p55874499155527"><a name="zh-cn_topic_0108272820_p55874499155527"></a><a name="zh-cn_topic_0108272820_p55874499155527"></a>重复文件处理方式，只有文件名和文件大小都相同才会判定为重复文件。重复文件支持以下处理方式：<a name="zh-cn_topic_0108272820_ul33108444155527"></a><a name="zh-cn_topic_0108272820_ul33108444155527"></a><ul id="zh-cn_topic_0108272820_ul33108444155527"><li>REPLACE：替换重复文件。</li><li>SKIP：跳过重复文件。</li><li>ABANDON：发现重复文件停止任务。</li></ul>
</div>
</td>
</tr>
<tr id="zh-cn_topic_0108272820_row1362135920116"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272820_p5622115931110"><a name="zh-cn_topic_0108272820_p5622115931110"></a><a name="zh-cn_topic_0108272820_p5622115931110"></a>toJobConfig.encryption</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272820_p10622125919118"><a name="zh-cn_topic_0108272820_p10622125919118"></a><a name="zh-cn_topic_0108272820_p10622125919118"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.49%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272820_p1762214595111"><a name="zh-cn_topic_0108272820_p1762214595111"></a><a name="zh-cn_topic_0108272820_p1762214595111"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><div class="p" id="zh-cn_topic_0108272820_p268631112373"><a name="zh-cn_topic_0108272820_p268631112373"></a><a name="zh-cn_topic_0108272820_p268631112373"></a>选择是否对上传的数据进行加密，以及加密方式：<a name="zh-cn_topic_0108272820_ul193603764111"></a><a name="zh-cn_topic_0108272820_ul193603764111"></a><ul id="zh-cn_topic_0108272820_ul193603764111"><li>NONE：不加密，直接写入数据。</li><li>KMS：使用数据加密服务中的KMS进行加密。如果启用KMS加密则无法进行数据的MD5校验。</li><li>AES-256-GCM：使用长度为256bit的AES对称加密算法，目前加密算法只支持AES-256-GCM（NoPadding）。</li></ul>
</div>
</td>
</tr>
<tr id="zh-cn_topic_0108272820_row1267112218139"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272820_p167122217132"><a name="zh-cn_topic_0108272820_p167122217132"></a><a name="zh-cn_topic_0108272820_p167122217132"></a>toJobConfig.dek</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272820_p74741127142115"><a name="zh-cn_topic_0108272820_p74741127142115"></a><a name="zh-cn_topic_0108272820_p74741127142115"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.49%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272820_p2474627102111"><a name="zh-cn_topic_0108272820_p2474627102111"></a><a name="zh-cn_topic_0108272820_p2474627102111"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272820_p23281415172211"><a name="zh-cn_topic_0108272820_p23281415172211"></a><a name="zh-cn_topic_0108272820_p23281415172211"></a>数据加密密钥，<span class="parmname" id="zh-cn_topic_0108272820_parmname697410131151"><a name="zh-cn_topic_0108272820_parmname697410131151"></a><a name="zh-cn_topic_0108272820_parmname697410131151"></a>“toJobConfig.encryption”</span>（加密方式）选择<span class="parmvalue" id="zh-cn_topic_0108272820_parmvalue838117223225"><a name="zh-cn_topic_0108272820_parmvalue838117223225"></a><a name="zh-cn_topic_0108272820_parmvalue838117223225"></a>“AES-256-GCM”</span>时有该参数，密钥由长度64的十六进制数组成。</p>
<p id="zh-cn_topic_0108272820_p18430442724"><a name="zh-cn_topic_0108272820_p18430442724"></a><a name="zh-cn_topic_0108272820_p18430442724"></a>请您牢记这里配置的密钥，解密时的密钥与这里配置的必须一致。如果不一致系统不会报异常，只是解密出来的数据会错误。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272820_row14106153252116"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272820_p26851918151311"><a name="zh-cn_topic_0108272820_p26851918151311"></a><a name="zh-cn_topic_0108272820_p26851918151311"></a>toJobConfig.iv</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272820_p1114152632113"><a name="zh-cn_topic_0108272820_p1114152632113"></a><a name="zh-cn_topic_0108272820_p1114152632113"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.49%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272820_p1414162617212"><a name="zh-cn_topic_0108272820_p1414162617212"></a><a name="zh-cn_topic_0108272820_p1414162617212"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272820_p24771354512"><a name="zh-cn_topic_0108272820_p24771354512"></a><a name="zh-cn_topic_0108272820_p24771354512"></a>初始化向量，<span class="parmname" id="zh-cn_topic_0108272820_parmname953919017169"><a name="zh-cn_topic_0108272820_parmname953919017169"></a><a name="zh-cn_topic_0108272820_parmname953919017169"></a>“toJobConfig.encryption”</span>（加密方式）选择<span class="parmvalue" id="zh-cn_topic_0108272820_parmvalue125661973247"><a name="zh-cn_topic_0108272820_parmvalue125661973247"></a><a name="zh-cn_topic_0108272820_parmvalue125661973247"></a>“AES-256-GCM”</span>时有该参数，初始化向量由长度32的十六进制数组成。</p>
<p id="zh-cn_topic_0108272820_p51641322122914"><a name="zh-cn_topic_0108272820_p51641322122914"></a><a name="zh-cn_topic_0108272820_p51641322122914"></a>请您牢记这里配置的初始化向量，解密时的初始化向量与这里配置的必须一致。如果不一致系统不会报异常，只是解密出来的数据会错误。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272820_row121169414496"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272820_p61161042495"><a name="zh-cn_topic_0108272820_p61161042495"></a><a name="zh-cn_topic_0108272820_p61161042495"></a>toJobConfig.kmsID</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272820_p8747283512"><a name="zh-cn_topic_0108272820_p8747283512"></a><a name="zh-cn_topic_0108272820_p8747283512"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.49%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272820_p19495182285110"><a name="zh-cn_topic_0108272820_p19495182285110"></a><a name="zh-cn_topic_0108272820_p19495182285110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272820_p1298713015611"><a name="zh-cn_topic_0108272820_p1298713015611"></a><a name="zh-cn_topic_0108272820_p1298713015611"></a>上传时加密使用的密钥。需先在密钥管理服务中创建密钥。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272820_row18291314135"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272820_p42919318131"><a name="zh-cn_topic_0108272820_p42919318131"></a><a name="zh-cn_topic_0108272820_p42919318131"></a>toJobConfig.projectID</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272820_p92917315133"><a name="zh-cn_topic_0108272820_p92917315133"></a><a name="zh-cn_topic_0108272820_p92917315133"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.49%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272820_p167262385207"><a name="zh-cn_topic_0108272820_p167262385207"></a><a name="zh-cn_topic_0108272820_p167262385207"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272820_p18101134914317"><a name="zh-cn_topic_0108272820_p18101134914317"></a><a name="zh-cn_topic_0108272820_p18101134914317"></a>KMS密钥所属的项目ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272820_row156027298502"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272820_p560222965013"><a name="zh-cn_topic_0108272820_p560222965013"></a><a name="zh-cn_topic_0108272820_p560222965013"></a>toJobConfig.validateMD5</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272820_p148814283513"><a name="zh-cn_topic_0108272820_p148814283513"></a><a name="zh-cn_topic_0108272820_p148814283513"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.49%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272820_p128700182517"><a name="zh-cn_topic_0108272820_p128700182517"></a><a name="zh-cn_topic_0108272820_p128700182517"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272820_p315803203318"><a name="zh-cn_topic_0108272820_p315803203318"></a><a name="zh-cn_topic_0108272820_p315803203318"></a>选择是否校验MD5值，不能与KMS加密同时使用。使用二进制格式传输文件时，才能校验MD5值。</p>
<p id="zh-cn_topic_0108272820_p187921432029"><a name="zh-cn_topic_0108272820_p187921432029"></a><a name="zh-cn_topic_0108272820_p187921432029"></a>计算源文件的MD5值，并与OBS返回的MD5值进行校验。如果源端已经存在MD5文件，则直接读取源端的MD5文件与OBS返回的MD5值进行校验。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272820_row414713389207"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272820_p17147193812200"><a name="zh-cn_topic_0108272820_p17147193812200"></a><a name="zh-cn_topic_0108272820_p17147193812200"></a>toJobConfig.recordMD5Result</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272820_p82561650162012"><a name="zh-cn_topic_0108272820_p82561650162012"></a><a name="zh-cn_topic_0108272820_p82561650162012"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.49%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272820_p152561350172015"><a name="zh-cn_topic_0108272820_p152561350172015"></a><a name="zh-cn_topic_0108272820_p152561350172015"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272820_p1327165017202"><a name="zh-cn_topic_0108272820_p1327165017202"></a><a name="zh-cn_topic_0108272820_p1327165017202"></a>当选择校验MD5值时，这里配置是否记录校验结果。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272820_row14648125612210"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272820_p1664817567212"><a name="zh-cn_topic_0108272820_p1664817567212"></a><a name="zh-cn_topic_0108272820_p1664817567212"></a>toJobConfig.recordMD5Link</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272820_p0648185612114"><a name="zh-cn_topic_0108272820_p0648185612114"></a><a name="zh-cn_topic_0108272820_p0648185612114"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.49%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272820_p106484567219"><a name="zh-cn_topic_0108272820_p106484567219"></a><a name="zh-cn_topic_0108272820_p106484567219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272820_p24225018412"><a name="zh-cn_topic_0108272820_p24225018412"></a><a name="zh-cn_topic_0108272820_p24225018412"></a>可以指定任意一个OBS连接，将MD5校验结果写入该连接的桶。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272820_row192884109279"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272820_p1128813105274"><a name="zh-cn_topic_0108272820_p1128813105274"></a><a name="zh-cn_topic_0108272820_p1128813105274"></a>toJobConfig.recordMD5Bucket</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272820_p17288151072718"><a name="zh-cn_topic_0108272820_p17288151072718"></a><a name="zh-cn_topic_0108272820_p17288151072718"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.49%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272820_p1288010152719"><a name="zh-cn_topic_0108272820_p1288010152719"></a><a name="zh-cn_topic_0108272820_p1288010152719"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272820_p10288910142717"><a name="zh-cn_topic_0108272820_p10288910142717"></a><a name="zh-cn_topic_0108272820_p10288910142717"></a>写入MD5校验结果的OBS桶。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272820_row1246233152812"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272820_p1546218312281"><a name="zh-cn_topic_0108272820_p1546218312281"></a><a name="zh-cn_topic_0108272820_p1546218312281"></a>toJobConfig.recordMD5Directory</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272820_p346214316289"><a name="zh-cn_topic_0108272820_p346214316289"></a><a name="zh-cn_topic_0108272820_p346214316289"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.49%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272820_p0462153111289"><a name="zh-cn_topic_0108272820_p0462153111289"></a><a name="zh-cn_topic_0108272820_p0462153111289"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272820_p1346233192813"><a name="zh-cn_topic_0108272820_p1346233192813"></a><a name="zh-cn_topic_0108272820_p1346233192813"></a>写入MD5校验结果的目录。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272820_row1740959314598"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272820_p54503533164925"><a name="zh-cn_topic_0108272820_p54503533164925"></a><a name="zh-cn_topic_0108272820_p54503533164925"></a>toJobConfig.encodeType</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272820_p52710080164925"><a name="zh-cn_topic_0108272820_p52710080164925"></a><a name="zh-cn_topic_0108272820_p52710080164925"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.49%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272820_p41658067164925"><a name="zh-cn_topic_0108272820_p41658067164925"></a><a name="zh-cn_topic_0108272820_p41658067164925"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272820_p18860238164925"><a name="zh-cn_topic_0108272820_p18860238164925"></a><a name="zh-cn_topic_0108272820_p18860238164925"></a>编码类型，例如：<span class="parmvalue" id="zh-cn_topic_0108272820_parmvalue2525514110158"><a name="zh-cn_topic_0108272820_parmvalue2525514110158"></a><a name="zh-cn_topic_0108272820_parmvalue2525514110158"></a>“UTF_8”</span>或<span class="parmvalue" id="zh-cn_topic_0108272820_parmvalue33413473101512"><a name="zh-cn_topic_0108272820_parmvalue33413473101512"></a><a name="zh-cn_topic_0108272820_parmvalue33413473101512"></a>“GBK”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272820_row7509313442"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272820_p18508310443"><a name="zh-cn_topic_0108272820_p18508310443"></a><a name="zh-cn_topic_0108272820_p18508310443"></a>toJobConfig.markerFile</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272820_p85012364412"><a name="zh-cn_topic_0108272820_p85012364412"></a><a name="zh-cn_topic_0108272820_p85012364412"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.49%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272820_p1750103124416"><a name="zh-cn_topic_0108272820_p1750103124416"></a><a name="zh-cn_topic_0108272820_p1750103124416"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272820_p195014313441"><a name="zh-cn_topic_0108272820_p195014313441"></a><a name="zh-cn_topic_0108272820_p195014313441"></a>当作业执行成功时，会在写入目录下生成一个标识文件，文件名由用户指定，不指定时默认关闭该功能。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272820_row1287913316408"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272820_p9879163174014"><a name="zh-cn_topic_0108272820_p9879163174014"></a><a name="zh-cn_topic_0108272820_p9879163174014"></a>toJobConfig.copyContentType</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272820_p1582111414403"><a name="zh-cn_topic_0108272820_p1582111414403"></a><a name="zh-cn_topic_0108272820_p1582111414403"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.49%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272820_p658281416403"><a name="zh-cn_topic_0108272820_p658281416403"></a><a name="zh-cn_topic_0108272820_p658281416403"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272820_p18177191318566"><a name="zh-cn_topic_0108272820_p18177191318566"></a><a name="zh-cn_topic_0108272820_p18177191318566"></a><span class="parmname" id="zh-cn_topic_0108272820_parmname18613330161819"><a name="zh-cn_topic_0108272820_parmname18613330161819"></a><a name="zh-cn_topic_0108272820_parmname18613330161819"></a>“toJobConfig.outputFormat”</span>（文件格式）为<span class="parmvalue" id="zh-cn_topic_0108272820_parmvalue917751375617"><a name="zh-cn_topic_0108272820_parmvalue917751375617"></a><a name="zh-cn_topic_0108272820_parmvalue917751375617"></a>“BINARY_FILE”</span>，且源端、目的端都为对象存储时，才有该参数。</p>
<p id="zh-cn_topic_0108272820_p014919221606"><a name="zh-cn_topic_0108272820_p014919221606"></a><a name="zh-cn_topic_0108272820_p014919221606"></a>选择<span class="parmvalue" id="zh-cn_topic_0108272820_parmvalue514910221608"><a name="zh-cn_topic_0108272820_parmvalue514910221608"></a><a name="zh-cn_topic_0108272820_parmvalue514910221608"></a>“是”</span>后，迁移对象文件时会复制源文件的Content-Type属性，主要用于静态网站的迁移场景。</p>
<p id="zh-cn_topic_0108272820_p9540193215413"><a name="zh-cn_topic_0108272820_p9540193215413"></a><a name="zh-cn_topic_0108272820_p9540193215413"></a>归档存储的桶不支持设置Content-Type属性，所以如果开启了该参数，目的端选择写入的桶时，必须选择非归档存储的桶。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272820_row1051412310366"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272820_p20514235364"><a name="zh-cn_topic_0108272820_p20514235364"></a><a name="zh-cn_topic_0108272820_p20514235364"></a>toJobConfig.quoteChar</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272820_p751473133620"><a name="zh-cn_topic_0108272820_p751473133620"></a><a name="zh-cn_topic_0108272820_p751473133620"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.49%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272820_p1651463123618"><a name="zh-cn_topic_0108272820_p1651463123618"></a><a name="zh-cn_topic_0108272820_p1651463123618"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272820_p1210241263316"><a name="zh-cn_topic_0108272820_p1210241263316"></a><a name="zh-cn_topic_0108272820_p1210241263316"></a><span class="parmname" id="zh-cn_topic_0108272820_parmname1974874181810"><a name="zh-cn_topic_0108272820_parmname1974874181810"></a><a name="zh-cn_topic_0108272820_parmname1974874181810"></a>“toJobConfig.outputFormat”</span>（文件格式）为<span class="parmvalue" id="zh-cn_topic_0108272820_parmvalue910281223312"><a name="zh-cn_topic_0108272820_parmvalue910281223312"></a><a name="zh-cn_topic_0108272820_parmvalue910281223312"></a>“CSV_FILE”</span>，才有该参数，用于将数据库的表迁移到文件系统的场景。</p>
<p id="zh-cn_topic_0108272820_p19249144319"><a name="zh-cn_topic_0108272820_p19249144319"></a><a name="zh-cn_topic_0108272820_p19249144319"></a>选择<span class="parmvalue" id="zh-cn_topic_0108272820_parmvalue13709134210325"><a name="zh-cn_topic_0108272820_parmvalue13709134210325"></a><a name="zh-cn_topic_0108272820_parmvalue13709134210325"></a>“是”</span>时，如果源端数据表中的某一个字段内容包含字段分隔符或换行符，写入目的端时CDM会使用双引号（"）作为包围符将该字段内容括起来，作为一个整体存储，避免其中的字段分隔符误将一个字段分隔成两个，或者换行符误将字段换行。例如：数据库中某字段为hello,world，使用包围符后，导出到CSV文件的时候数据为"hello,world"。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272820_row1744476115415"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272820_p344406195416"><a name="zh-cn_topic_0108272820_p344406195416"></a><a name="zh-cn_topic_0108272820_p344406195416"></a>toJobConfig.firstRowAsHeader</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272820_p1244417635410"><a name="zh-cn_topic_0108272820_p1244417635410"></a><a name="zh-cn_topic_0108272820_p1244417635410"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.49%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272820_p124445615545"><a name="zh-cn_topic_0108272820_p124445615545"></a><a name="zh-cn_topic_0108272820_p124445615545"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272820_p54449616542"><a name="zh-cn_topic_0108272820_p54449616542"></a><a name="zh-cn_topic_0108272820_p54449616542"></a><span class="parmname" id="zh-cn_topic_0108272820_parmname1742242213195"><a name="zh-cn_topic_0108272820_parmname1742242213195"></a><a name="zh-cn_topic_0108272820_parmname1742242213195"></a>“toJobConfig.outputFormat”</span>（文件格式）为<span class="parmvalue" id="zh-cn_topic_0108272820_parmvalue739785211338"><a name="zh-cn_topic_0108272820_parmvalue739785211338"></a><a name="zh-cn_topic_0108272820_parmvalue739785211338"></a>“CSV_FILE”</span>时才有该参数。在迁移表到CSV文件时，CDM默认是不迁移表的标题行，如果该参数选择<span class="parmvalue" id="zh-cn_topic_0108272820_parmvalue11024151389"><a name="zh-cn_topic_0108272820_parmvalue11024151389"></a><a name="zh-cn_topic_0108272820_parmvalue11024151389"></a>“是”</span>，CDM在才会将表的标题行数据写入文件。</p>
</td>
</tr>
</tbody>
</table>

