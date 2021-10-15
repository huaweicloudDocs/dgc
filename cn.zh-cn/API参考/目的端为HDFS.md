# 目的端为HDFS<a name="dgc_02_0298"></a>

## JSON样例<a name="zh-cn_topic_0108272844_section33401108172339"></a>

```
"to-config-values": {
        "configs": [
          {
            "inputs": [
              {
                "name": "toJobConfig.outputDirectory",
                "value": "/hdfsto"
              },
              {
                "name": "toJobConfig.outputFormat",
                "value": "BINARY_FILE"
              },
              {
                "name": "toJobConfig.writeToTempFile",
                "value": "false"
              },
              {
                "name": "toJobConfig.duplicateFileOpType",
                "value": "REPLACE"
              },
              {
                "name": "toJobConfig.compression",
                "value": "NONE"
              },
              {
                "name": "toJobConfig.appendMode",
                "value": "true"
              }
            ],
            "name": "toJobConfig"
          }
        ]
      }
```

## 参数说明<a name="zh-cn_topic_0108272844_section64036202102948"></a>

<a name="zh-cn_topic_0108272844_table56137241103023"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108272844_row52082877103023"><th class="cellrowborder" valign="top" width="22.657734226577343%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272844_p57963538103023"><a name="zh-cn_topic_0108272844_p57963538103023"></a><a name="zh-cn_topic_0108272844_p57963538103023"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="19.408059194080593%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272844_p64535024103023"><a name="zh-cn_topic_0108272844_p64535024103023"></a><a name="zh-cn_topic_0108272844_p64535024103023"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="16.858314168583142%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272844_p59954430103023"><a name="zh-cn_topic_0108272844_p59954430103023"></a><a name="zh-cn_topic_0108272844_p59954430103023"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="41.075892410758925%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272844_p24470628103023"><a name="zh-cn_topic_0108272844_p24470628103023"></a><a name="zh-cn_topic_0108272844_p24470628103023"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108272844_row35963851103023"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272844_p27390810103023"><a name="zh-cn_topic_0108272844_p27390810103023"></a><a name="zh-cn_topic_0108272844_p27390810103023"></a>toJobConfig.outputDirectory</p>
</td>
<td class="cellrowborder" valign="top" width="19.408059194080593%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272844_p4063162103023"><a name="zh-cn_topic_0108272844_p4063162103023"></a><a name="zh-cn_topic_0108272844_p4063162103023"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.858314168583142%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272844_p60680723103023"><a name="zh-cn_topic_0108272844_p60680723103023"></a><a name="zh-cn_topic_0108272844_p60680723103023"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.075892410758925%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272844_p16191500103023"><a name="zh-cn_topic_0108272844_p16191500103023"></a><a name="zh-cn_topic_0108272844_p16191500103023"></a>数据写入的路径，例如<span class="parmvalue" id="zh-cn_topic_0108272844_parmvalue11505772103023"><a name="zh-cn_topic_0108272844_parmvalue11505772103023"></a><a name="zh-cn_topic_0108272844_parmvalue11505772103023"></a>“/data_dir”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272844_row36443085103023"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272844_p66208767103023"><a name="zh-cn_topic_0108272844_p66208767103023"></a><a name="zh-cn_topic_0108272844_p66208767103023"></a>toJobConfig.outputFormat</p>
</td>
<td class="cellrowborder" valign="top" width="19.408059194080593%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272844_p61309897103023"><a name="zh-cn_topic_0108272844_p61309897103023"></a><a name="zh-cn_topic_0108272844_p61309897103023"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.858314168583142%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272844_p45780103023"><a name="zh-cn_topic_0108272844_p45780103023"></a><a name="zh-cn_topic_0108272844_p45780103023"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="41.075892410758925%" headers="mcps1.1.5.1.4 "><div class="p" id="zh-cn_topic_0108272844_p66316516111924"><a name="zh-cn_topic_0108272844_p66316516111924"></a><a name="zh-cn_topic_0108272844_p66316516111924"></a>写入数据时所用的文件格式（二进制除外），支持以下文件格式：<a name="zh-cn_topic_0108272844_zh-cn_topic_0108272820_ul6294852210148"></a><a name="zh-cn_topic_0108272844_zh-cn_topic_0108272820_ul6294852210148"></a><ul id="zh-cn_topic_0108272844_zh-cn_topic_0108272820_ul6294852210148"><li>CSV_FILE：按照CSV格式写入数据。</li><li>BINARY_FILE：二进制格式，不解析文件内容直接传输，CDM会原样写入文件，不改变原始文件格式。</li></ul>
</div>
<p id="zh-cn_topic_0108272844_p35897407111924"><a name="zh-cn_topic_0108272844_p35897407111924"></a><a name="zh-cn_topic_0108272844_p35897407111924"></a>当选择<span class="parmvalue" id="zh-cn_topic_0108272844_zh-cn_topic_0108272820_parmvalue24403448101417"><a name="zh-cn_topic_0108272844_zh-cn_topic_0108272820_parmvalue24403448101417"></a><a name="zh-cn_topic_0108272844_zh-cn_topic_0108272820_parmvalue24403448101417"></a>“BINARY_FILE”</span>时，源端也必须为文件系统。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272844_row14202830103433"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272844_p33526379103458"><a name="zh-cn_topic_0108272844_p33526379103458"></a><a name="zh-cn_topic_0108272844_p33526379103458"></a>toJobConfig.lineSeparator</p>
</td>
<td class="cellrowborder" valign="top" width="19.408059194080593%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272844_p31282148103458"><a name="zh-cn_topic_0108272844_p31282148103458"></a><a name="zh-cn_topic_0108272844_p31282148103458"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.858314168583142%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272844_p50826021103458"><a name="zh-cn_topic_0108272844_p50826021103458"></a><a name="zh-cn_topic_0108272844_p50826021103458"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.075892410758925%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272844_p4596973311298"><a name="zh-cn_topic_0108272844_p4596973311298"></a><a name="zh-cn_topic_0108272844_p4596973311298"></a>行分割符号，当<span class="parmname" id="zh-cn_topic_0108272844_zh-cn_topic_0108272820_parmname16832101781710"><a name="zh-cn_topic_0108272844_zh-cn_topic_0108272820_parmname16832101781710"></a><a name="zh-cn_topic_0108272844_zh-cn_topic_0108272820_parmname16832101781710"></a>“toJobConfig.outputFormat”</span>（文件格式）为<span class="parmvalue" id="zh-cn_topic_0108272844_zh-cn_topic_0108272820_parmvalue32760165111255"><a name="zh-cn_topic_0108272844_zh-cn_topic_0108272820_parmvalue32760165111255"></a><a name="zh-cn_topic_0108272844_zh-cn_topic_0108272820_parmvalue32760165111255"></a>“CSV_FILE”</span>时此参数有效，默认值为：<span class="parmvalue" id="zh-cn_topic_0108272844_zh-cn_topic_0108272820_parmvalue26406035111255"><a name="zh-cn_topic_0108272844_zh-cn_topic_0108272820_parmvalue26406035111255"></a><a name="zh-cn_topic_0108272844_zh-cn_topic_0108272820_parmvalue26406035111255"></a>“\<span id="zh-cn_topic_0108272844_zh-cn_topic_0108272820_text36327723111255"><a name="zh-cn_topic_0108272844_zh-cn_topic_0108272820_text36327723111255"></a><a name="zh-cn_topic_0108272844_zh-cn_topic_0108272820_text36327723111255"></a>r</span>\<span id="zh-cn_topic_0108272844_zh-cn_topic_0108272820_text58514056111255"><a name="zh-cn_topic_0108272844_zh-cn_topic_0108272820_text58514056111255"></a><a name="zh-cn_topic_0108272844_zh-cn_topic_0108272820_text58514056111255"></a>n</span>”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272844_row51268928103438"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272844_p41226208103458"><a name="zh-cn_topic_0108272844_p41226208103458"></a><a name="zh-cn_topic_0108272844_p41226208103458"></a>toJobConfig.fieldSeparator</p>
</td>
<td class="cellrowborder" valign="top" width="19.408059194080593%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272844_p50988541103458"><a name="zh-cn_topic_0108272844_p50988541103458"></a><a name="zh-cn_topic_0108272844_p50988541103458"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.858314168583142%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272844_p36431138103458"><a name="zh-cn_topic_0108272844_p36431138103458"></a><a name="zh-cn_topic_0108272844_p36431138103458"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.075892410758925%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272844_p4984816111298"><a name="zh-cn_topic_0108272844_p4984816111298"></a><a name="zh-cn_topic_0108272844_p4984816111298"></a>列分割符号，当<span class="parmname" id="zh-cn_topic_0108272844_zh-cn_topic_0108272820_parmname11724115615167"><a name="zh-cn_topic_0108272844_zh-cn_topic_0108272820_parmname11724115615167"></a><a name="zh-cn_topic_0108272844_zh-cn_topic_0108272820_parmname11724115615167"></a>“toJobConfig.outputFormat”</span>（文件格式）为<span class="parmvalue" id="zh-cn_topic_0108272844_zh-cn_topic_0108272820_parmvalue5911601102324"><a name="zh-cn_topic_0108272844_zh-cn_topic_0108272820_parmvalue5911601102324"></a><a name="zh-cn_topic_0108272844_zh-cn_topic_0108272820_parmvalue5911601102324"></a>“CSV_FILE”</span>时此参数有效，默认值为：<span class="parmvalue" id="zh-cn_topic_0108272844_zh-cn_topic_0108272820_parmvalue53204411102324"><a name="zh-cn_topic_0108272844_zh-cn_topic_0108272820_parmvalue53204411102324"></a><a name="zh-cn_topic_0108272844_zh-cn_topic_0108272820_parmvalue53204411102324"></a>“,”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272844_row165374963415"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272844_p19531149103416"><a name="zh-cn_topic_0108272844_p19531149103416"></a><a name="zh-cn_topic_0108272844_p19531149103416"></a>toJobConfig.writeToTempFile</p>
</td>
<td class="cellrowborder" valign="top" width="19.408059194080593%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272844_p145319497341"><a name="zh-cn_topic_0108272844_p145319497341"></a><a name="zh-cn_topic_0108272844_p145319497341"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.858314168583142%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272844_p8182172215354"><a name="zh-cn_topic_0108272844_p8182172215354"></a><a name="zh-cn_topic_0108272844_p8182172215354"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="41.075892410758925%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272844_p169603823818"><a name="zh-cn_topic_0108272844_p169603823818"></a><a name="zh-cn_topic_0108272844_p169603823818"></a>将二进制文件先写入到临时文件（临时文件以<span class="uicontrol" id="zh-cn_topic_0108272844_zh-cn_topic_0108272836_uicontrol1814221324816"><a name="zh-cn_topic_0108272844_zh-cn_topic_0108272836_uicontrol1814221324816"></a><a name="zh-cn_topic_0108272844_zh-cn_topic_0108272836_uicontrol1814221324816"></a>“.tmp”</span>作为后缀），迁移成功后，再进行rename或move操作，在目的端恢复文件。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272844_row54756901103023"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272844_p6123978103023"><a name="zh-cn_topic_0108272844_p6123978103023"></a><a name="zh-cn_topic_0108272844_p6123978103023"></a>toJobConfig.duplicateFileOpType</p>
</td>
<td class="cellrowborder" valign="top" width="19.408059194080593%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272844_p26280224103023"><a name="zh-cn_topic_0108272844_p26280224103023"></a><a name="zh-cn_topic_0108272844_p26280224103023"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.858314168583142%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272844_p48323406103023"><a name="zh-cn_topic_0108272844_p48323406103023"></a><a name="zh-cn_topic_0108272844_p48323406103023"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="41.075892410758925%" headers="mcps1.1.5.1.4 "><div class="p" id="zh-cn_topic_0108272844_p21881853103023"><a name="zh-cn_topic_0108272844_p21881853103023"></a><a name="zh-cn_topic_0108272844_p21881853103023"></a>重复文件处理方式，只有文件名和文件大小都相同才会判定为重复文件。重复文件支持以下处理方式：<a name="zh-cn_topic_0108272844_zh-cn_topic_0108272820_ul33108444155527"></a><a name="zh-cn_topic_0108272844_zh-cn_topic_0108272820_ul33108444155527"></a><ul id="zh-cn_topic_0108272844_zh-cn_topic_0108272820_ul33108444155527"><li>REPLACE：替换重复文件。</li><li>SKIP：跳过重复文件。</li><li>ABANDON：发现重复文件停止任务。</li></ul>
</div>
</td>
</tr>
<tr id="zh-cn_topic_0108272844_row60754053103023"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272844_p22131251103023"><a name="zh-cn_topic_0108272844_p22131251103023"></a><a name="zh-cn_topic_0108272844_p22131251103023"></a>toJobConfig.compression</p>
</td>
<td class="cellrowborder" valign="top" width="19.408059194080593%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272844_p47800910103023"><a name="zh-cn_topic_0108272844_p47800910103023"></a><a name="zh-cn_topic_0108272844_p47800910103023"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.858314168583142%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272844_p46668477103023"><a name="zh-cn_topic_0108272844_p46668477103023"></a><a name="zh-cn_topic_0108272844_p46668477103023"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="41.075892410758925%" headers="mcps1.1.5.1.4 "><div class="p" id="zh-cn_topic_0108272844_p22050281103023"><a name="zh-cn_topic_0108272844_p22050281103023"></a><a name="zh-cn_topic_0108272844_p22050281103023"></a>写入文件后，选择对文件的压缩格式。支持以下压缩格式：<a name="zh-cn_topic_0108272844_ul64234801103023"></a><a name="zh-cn_topic_0108272844_ul64234801103023"></a><ul id="zh-cn_topic_0108272844_ul64234801103023"><li>NONE：不压缩。</li><li>DEFLATE：压缩为DEFLATE格式。</li><li>GZIP：压缩为GZIP格式。</li><li>BZIP2：压缩为BZIP2格式。</li><li>LZ4：压缩为LZ4格式。</li><li>SNAPPY：压缩为SNAPPY格式。</li></ul>
</div>
</td>
</tr>
<tr id="zh-cn_topic_0108272844_row25552788103023"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272844_p56509958103023"><a name="zh-cn_topic_0108272844_p56509958103023"></a><a name="zh-cn_topic_0108272844_p56509958103023"></a>toJobConfig.appendMode</p>
</td>
<td class="cellrowborder" valign="top" width="19.408059194080593%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272844_p13903909103023"><a name="zh-cn_topic_0108272844_p13903909103023"></a><a name="zh-cn_topic_0108272844_p13903909103023"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.858314168583142%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272844_p52474840103023"><a name="zh-cn_topic_0108272844_p52474840103023"></a><a name="zh-cn_topic_0108272844_p52474840103023"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="41.075892410758925%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272844_p22603656103023"><a name="zh-cn_topic_0108272844_p22603656103023"></a><a name="zh-cn_topic_0108272844_p22603656103023"></a>当加载路径已经存在文件，是否需要写入，默认值为<span class="parmvalue" id="zh-cn_topic_0108272844_parmvalue2106314103023"><a name="zh-cn_topic_0108272844_parmvalue2106314103023"></a><a name="zh-cn_topic_0108272844_parmvalue2106314103023"></a>“false”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272844_row4274153852517"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272844_p5622115931110"><a name="zh-cn_topic_0108272844_p5622115931110"></a><a name="zh-cn_topic_0108272844_p5622115931110"></a>toJobConfig.encryption</p>
</td>
<td class="cellrowborder" valign="top" width="19.408059194080593%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272844_p10622125919118"><a name="zh-cn_topic_0108272844_p10622125919118"></a><a name="zh-cn_topic_0108272844_p10622125919118"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.858314168583142%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272844_p1762214595111"><a name="zh-cn_topic_0108272844_p1762214595111"></a><a name="zh-cn_topic_0108272844_p1762214595111"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="41.075892410758925%" headers="mcps1.1.5.1.4 "><div class="p" id="zh-cn_topic_0108272844_p268631112373"><a name="zh-cn_topic_0108272844_p268631112373"></a><a name="zh-cn_topic_0108272844_p268631112373"></a>当<span class="parmname" id="zh-cn_topic_0108272844_parmname199870284216"><a name="zh-cn_topic_0108272844_parmname199870284216"></a><a name="zh-cn_topic_0108272844_parmname199870284216"></a>“toJobConfig.outputFormat”</span>（文件格式）为<span class="parmvalue" id="zh-cn_topic_0108272844_parmvalue15321226162614"><a name="zh-cn_topic_0108272844_parmvalue15321226162614"></a><a name="zh-cn_topic_0108272844_parmvalue15321226162614"></a>“BINARY_FILE”</span>（二进制）时才有该参数，选择是否对导入的数据进行加密，以及加密方式：<a name="zh-cn_topic_0108272844_ul193603764111"></a><a name="zh-cn_topic_0108272844_ul193603764111"></a><ul id="zh-cn_topic_0108272844_ul193603764111"><li>NONE：不加密，直接写入数据。</li><li>AES-256-GCM：使用长度为256byte的AES对称加密算法，目前加密算法只支持AES-256-GCM（NoPadding）。</li></ul>
</div>
</td>
</tr>
<tr id="zh-cn_topic_0108272844_row183541438142514"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272844_p167122217132"><a name="zh-cn_topic_0108272844_p167122217132"></a><a name="zh-cn_topic_0108272844_p167122217132"></a>toJobConfig.dek</p>
</td>
<td class="cellrowborder" valign="top" width="19.408059194080593%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272844_p74741127142115"><a name="zh-cn_topic_0108272844_p74741127142115"></a><a name="zh-cn_topic_0108272844_p74741127142115"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.858314168583142%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272844_p2474627102111"><a name="zh-cn_topic_0108272844_p2474627102111"></a><a name="zh-cn_topic_0108272844_p2474627102111"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.075892410758925%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272844_p23281415172211"><a name="zh-cn_topic_0108272844_p23281415172211"></a><a name="zh-cn_topic_0108272844_p23281415172211"></a>数据加密密钥，<span class="parmname" id="zh-cn_topic_0108272844_zh-cn_topic_0108272820_parmname697410131151"><a name="zh-cn_topic_0108272844_zh-cn_topic_0108272820_parmname697410131151"></a><a name="zh-cn_topic_0108272844_zh-cn_topic_0108272820_parmname697410131151"></a>“toJobConfig.encryption”</span>（加密方式）选择<span class="parmvalue" id="zh-cn_topic_0108272844_zh-cn_topic_0108272820_parmvalue838117223225"><a name="zh-cn_topic_0108272844_zh-cn_topic_0108272820_parmvalue838117223225"></a><a name="zh-cn_topic_0108272844_zh-cn_topic_0108272820_parmvalue838117223225"></a>“AES-256-GCM”</span>时有该参数，密钥由长度64的十六进制数组成。</p>
<p id="zh-cn_topic_0108272844_p18430442724"><a name="zh-cn_topic_0108272844_p18430442724"></a><a name="zh-cn_topic_0108272844_p18430442724"></a>请您牢记这里配置的密钥，解密时的密钥与这里配置的必须一致。如果不一致系统不会报异常，只是解密出来的数据会错误。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272844_row150113917255"><td class="cellrowborder" valign="top" width="22.657734226577343%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272844_p26851918151311"><a name="zh-cn_topic_0108272844_p26851918151311"></a><a name="zh-cn_topic_0108272844_p26851918151311"></a>toJobConfig.iv</p>
</td>
<td class="cellrowborder" valign="top" width="19.408059194080593%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272844_p1114152632113"><a name="zh-cn_topic_0108272844_p1114152632113"></a><a name="zh-cn_topic_0108272844_p1114152632113"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.858314168583142%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272844_p1414162617212"><a name="zh-cn_topic_0108272844_p1414162617212"></a><a name="zh-cn_topic_0108272844_p1414162617212"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.075892410758925%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272844_p24771354512"><a name="zh-cn_topic_0108272844_p24771354512"></a><a name="zh-cn_topic_0108272844_p24771354512"></a>初始化向量，<span class="parmname" id="zh-cn_topic_0108272844_zh-cn_topic_0108272820_parmname953919017169"><a name="zh-cn_topic_0108272844_zh-cn_topic_0108272820_parmname953919017169"></a><a name="zh-cn_topic_0108272844_zh-cn_topic_0108272820_parmname953919017169"></a>“toJobConfig.encryption”</span>（加密方式）选择<span class="parmvalue" id="zh-cn_topic_0108272844_zh-cn_topic_0108272820_parmvalue125661973247"><a name="zh-cn_topic_0108272844_zh-cn_topic_0108272820_parmvalue125661973247"></a><a name="zh-cn_topic_0108272844_zh-cn_topic_0108272820_parmvalue125661973247"></a>“AES-256-GCM”</span>时有该参数，初始化向量由长度32的十六进制数组成。</p>
<p id="zh-cn_topic_0108272844_p51641322122914"><a name="zh-cn_topic_0108272844_p51641322122914"></a><a name="zh-cn_topic_0108272844_p51641322122914"></a>请您牢记这里配置的初始化向量，解密时的初始化向量与这里配置的必须一致。如果不一致系统不会报异常，只是解密出来的数据会错误。</p>
</td>
</tr>
</tbody>
</table>

