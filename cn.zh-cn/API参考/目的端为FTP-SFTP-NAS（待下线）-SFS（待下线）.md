# 目的端为FTP/SFTP/NAS（待下线）/SFS（待下线）<a name="dgc_02_0301"></a>

## JSON样例<a name="zh-cn_topic_0108272836_section33401108172339"></a>

```
"to-config-values": {
                "configs": [
                    {
                        "inputs": [
                          {
                           "name": "toJobConfig.outputDirectory",
                           "value": "/opt/data"
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
                           "name": "toJobConfig.duplicateFileOpType",
                           "value": "REPLACE"
                            }
                        ],
                        "name": "toJobConfig"
                    }
                ]
            }
```

## 参数说明<a name="zh-cn_topic_0108272836_section51591486111841"></a>

<a name="zh-cn_topic_0108272836_table25798531111924"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108272836_row40288864111924"><th class="cellrowborder" valign="top" width="22.66%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272836_p42172552111924"><a name="zh-cn_topic_0108272836_p42172552111924"></a><a name="zh-cn_topic_0108272836_p42172552111924"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="19.78%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272836_p60533565111924"><a name="zh-cn_topic_0108272836_p60533565111924"></a><a name="zh-cn_topic_0108272836_p60533565111924"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.419999999999998%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272836_p4271718111924"><a name="zh-cn_topic_0108272836_p4271718111924"></a><a name="zh-cn_topic_0108272836_p4271718111924"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="40.14%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272836_p10464876111924"><a name="zh-cn_topic_0108272836_p10464876111924"></a><a name="zh-cn_topic_0108272836_p10464876111924"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108272836_row42348598111924"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272836_p7684396111924"><a name="zh-cn_topic_0108272836_p7684396111924"></a><a name="zh-cn_topic_0108272836_p7684396111924"></a>toJobConfig.outputDirectory</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272836_p18456376111924"><a name="zh-cn_topic_0108272836_p18456376111924"></a><a name="zh-cn_topic_0108272836_p18456376111924"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272836_p18571455111924"><a name="zh-cn_topic_0108272836_p18571455111924"></a><a name="zh-cn_topic_0108272836_p18571455111924"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272836_p27892907111924"><a name="zh-cn_topic_0108272836_p27892907111924"></a><a name="zh-cn_topic_0108272836_p27892907111924"></a>数据写入的路径，例如：<span class="parmvalue" id="zh-cn_topic_0108272836_parmvalue49709579111924"><a name="zh-cn_topic_0108272836_parmvalue49709579111924"></a><a name="zh-cn_topic_0108272836_parmvalue49709579111924"></a>“/data_dir”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272836_row44733028111924"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272836_p66605521111924"><a name="zh-cn_topic_0108272836_p66605521111924"></a><a name="zh-cn_topic_0108272836_p66605521111924"></a>toJobConfig.outputFormat</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272836_p26338139111924"><a name="zh-cn_topic_0108272836_p26338139111924"></a><a name="zh-cn_topic_0108272836_p26338139111924"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272836_p53014505111924"><a name="zh-cn_topic_0108272836_p53014505111924"></a><a name="zh-cn_topic_0108272836_p53014505111924"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.1.5.1.4 "><div class="p" id="zh-cn_topic_0108272836_p66316516111924"><a name="zh-cn_topic_0108272836_p66316516111924"></a><a name="zh-cn_topic_0108272836_p66316516111924"></a>写入数据时所用的文件格式（二进制除外），支持以下文件格式：<a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_ul6294852210148"></a><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_ul6294852210148"></a><ul id="zh-cn_topic_0108272836_zh-cn_topic_0108272820_ul6294852210148"><li>CSV_FILE：按照CSV格式写入数据。</li><li>BINARY_FILE：二进制格式，不解析文件内容直接传输，CDM会原样写入文件，不改变原始文件格式。</li></ul>
</div>
<p id="zh-cn_topic_0108272836_p35897407111924"><a name="zh-cn_topic_0108272836_p35897407111924"></a><a name="zh-cn_topic_0108272836_p35897407111924"></a>当选择<span class="parmvalue" id="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmvalue24403448101417"><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmvalue24403448101417"></a><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmvalue24403448101417"></a>“BINARY_FILE”</span>时，源端也必须为文件系统。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272836_row22008815111924"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272836_p37883563111924"><a name="zh-cn_topic_0108272836_p37883563111924"></a><a name="zh-cn_topic_0108272836_p37883563111924"></a>toJobConfig.duplicateFileOpType</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272836_p48669788111924"><a name="zh-cn_topic_0108272836_p48669788111924"></a><a name="zh-cn_topic_0108272836_p48669788111924"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272836_p49938794111924"><a name="zh-cn_topic_0108272836_p49938794111924"></a><a name="zh-cn_topic_0108272836_p49938794111924"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.1.5.1.4 "><div class="p" id="zh-cn_topic_0108272836_p18510524111924"><a name="zh-cn_topic_0108272836_p18510524111924"></a><a name="zh-cn_topic_0108272836_p18510524111924"></a>重复文件处理方式，只有文件名和文件大小都相同才会判定为重复文件。重复文件支持以下处理方式：<a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_ul33108444155527"></a><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_ul33108444155527"></a><ul id="zh-cn_topic_0108272836_zh-cn_topic_0108272820_ul33108444155527"><li>REPLACE：替换重复文件。</li><li>SKIP：跳过重复文件。</li><li>ABANDON：发现重复文件停止任务。</li></ul>
</div>
</td>
</tr>
<tr id="zh-cn_topic_0108272836_row25909955111924"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272836_p18331600111924"><a name="zh-cn_topic_0108272836_p18331600111924"></a><a name="zh-cn_topic_0108272836_p18331600111924"></a>toJobConfig.lineSeparator</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272836_p8464613111924"><a name="zh-cn_topic_0108272836_p8464613111924"></a><a name="zh-cn_topic_0108272836_p8464613111924"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272836_p14545067111924"><a name="zh-cn_topic_0108272836_p14545067111924"></a><a name="zh-cn_topic_0108272836_p14545067111924"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272836_p37299785111924"><a name="zh-cn_topic_0108272836_p37299785111924"></a><a name="zh-cn_topic_0108272836_p37299785111924"></a>行分割符号，当<span class="parmname" id="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmname16832101781710"><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmname16832101781710"></a><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmname16832101781710"></a>“toJobConfig.outputFormat”</span>（文件格式）为<span class="parmvalue" id="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmvalue32760165111255"><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmvalue32760165111255"></a><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmvalue32760165111255"></a>“CSV_FILE”</span>时此参数有效，默认值为：<span class="parmvalue" id="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmvalue26406035111255"><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmvalue26406035111255"></a><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmvalue26406035111255"></a>“\<span id="zh-cn_topic_0108272836_zh-cn_topic_0108272820_text36327723111255"><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_text36327723111255"></a><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_text36327723111255"></a>r</span>\<span id="zh-cn_topic_0108272836_zh-cn_topic_0108272820_text58514056111255"><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_text58514056111255"></a><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_text58514056111255"></a>n</span>”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272836_row19316040111924"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272836_p21095384111924"><a name="zh-cn_topic_0108272836_p21095384111924"></a><a name="zh-cn_topic_0108272836_p21095384111924"></a>toJobConfig.fieldSeparator</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272836_p31004553111924"><a name="zh-cn_topic_0108272836_p31004553111924"></a><a name="zh-cn_topic_0108272836_p31004553111924"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272836_p28340866111924"><a name="zh-cn_topic_0108272836_p28340866111924"></a><a name="zh-cn_topic_0108272836_p28340866111924"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272836_p13908844111924"><a name="zh-cn_topic_0108272836_p13908844111924"></a><a name="zh-cn_topic_0108272836_p13908844111924"></a>列分割符号，当<span class="parmname" id="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmname11724115615167"><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmname11724115615167"></a><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmname11724115615167"></a>“toJobConfig.outputFormat”</span>（文件格式）为<span class="parmvalue" id="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmvalue5911601102324"><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmvalue5911601102324"></a><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmvalue5911601102324"></a>“CSV_FILE”</span>时此参数有效，默认值为：<span class="parmvalue" id="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmvalue53204411102324"><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmvalue53204411102324"></a><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmvalue53204411102324"></a>“,”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272836_row54984754111924"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272836_p24580061111924"><a name="zh-cn_topic_0108272836_p24580061111924"></a><a name="zh-cn_topic_0108272836_p24580061111924"></a>toJobConfig.encodeType</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272836_p44827929111924"><a name="zh-cn_topic_0108272836_p44827929111924"></a><a name="zh-cn_topic_0108272836_p44827929111924"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272836_p7183629111924"><a name="zh-cn_topic_0108272836_p7183629111924"></a><a name="zh-cn_topic_0108272836_p7183629111924"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272836_p45003106111924"><a name="zh-cn_topic_0108272836_p45003106111924"></a><a name="zh-cn_topic_0108272836_p45003106111924"></a>编码类型，例如：<span class="parmvalue" id="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmvalue2525514110158"><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmvalue2525514110158"></a><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmvalue2525514110158"></a>“UTF_8”</span>或<span class="parmvalue" id="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmvalue33413473101512"><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmvalue33413473101512"></a><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmvalue33413473101512"></a>“GBK”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272836_row156471313152119"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272836_p19647151314211"><a name="zh-cn_topic_0108272836_p19647151314211"></a><a name="zh-cn_topic_0108272836_p19647151314211"></a>toJobConfig.writeToTempFile</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272836_p14647413162114"><a name="zh-cn_topic_0108272836_p14647413162114"></a><a name="zh-cn_topic_0108272836_p14647413162114"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272836_p156471313122110"><a name="zh-cn_topic_0108272836_p156471313122110"></a><a name="zh-cn_topic_0108272836_p156471313122110"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272836_p16461527104615"><a name="zh-cn_topic_0108272836_p16461527104615"></a><a name="zh-cn_topic_0108272836_p16461527104615"></a>将二进制文件先写入到临时文件（临时文件以<span class="uicontrol" id="zh-cn_topic_0108272836_uicontrol1814221324816"><a name="zh-cn_topic_0108272836_uicontrol1814221324816"></a><a name="zh-cn_topic_0108272836_uicontrol1814221324816"></a>“.tmp”</span>作为后缀），迁移成功后，再进行rename或move操作，在目的端恢复文件。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272836_row2036621617215"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272836_p136620169214"><a name="zh-cn_topic_0108272836_p136620169214"></a><a name="zh-cn_topic_0108272836_p136620169214"></a>toJobConfig.recordMD5Result</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272836_p23661816172111"><a name="zh-cn_topic_0108272836_p23661816172111"></a><a name="zh-cn_topic_0108272836_p23661816172111"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272836_p1636615164218"><a name="zh-cn_topic_0108272836_p1636615164218"></a><a name="zh-cn_topic_0108272836_p1636615164218"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272836_p53601941494"><a name="zh-cn_topic_0108272836_p53601941494"></a><a name="zh-cn_topic_0108272836_p53601941494"></a>文件格式为<span class="parmvalue" id="zh-cn_topic_0108272836_parmvalue03601240499"><a name="zh-cn_topic_0108272836_parmvalue03601240499"></a><a name="zh-cn_topic_0108272836_parmvalue03601240499"></a>“二进制”</span>时，该参数有效。对每个传输的文件都生成一个MD5值，并将该值记录在一个新文件中（新文件以<span class="uicontrol" id="zh-cn_topic_0108272836_uicontrol78827455013"><a name="zh-cn_topic_0108272836_uicontrol78827455013"></a><a name="zh-cn_topic_0108272836_uicontrol78827455013"></a>“.md5”</span>作为后缀），且可以指定MD5值生成的目录。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272836_row511631082111"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272836_p0116910102113"><a name="zh-cn_topic_0108272836_p0116910102113"></a><a name="zh-cn_topic_0108272836_p0116910102113"></a>toJobConfig.recordMD5Directory</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272836_p15116101011212"><a name="zh-cn_topic_0108272836_p15116101011212"></a><a name="zh-cn_topic_0108272836_p15116101011212"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272836_p1746115328229"><a name="zh-cn_topic_0108272836_p1746115328229"></a><a name="zh-cn_topic_0108272836_p1746115328229"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272836_p17116131062118"><a name="zh-cn_topic_0108272836_p17116131062118"></a><a name="zh-cn_topic_0108272836_p17116131062118"></a>自定义MD5值写入的目录。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272836_row898654814178"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272836_p18508310443"><a name="zh-cn_topic_0108272836_p18508310443"></a><a name="zh-cn_topic_0108272836_p18508310443"></a>toJobConfig.markerFile</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272836_p85012364412"><a name="zh-cn_topic_0108272836_p85012364412"></a><a name="zh-cn_topic_0108272836_p85012364412"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272836_p1750103124416"><a name="zh-cn_topic_0108272836_p1750103124416"></a><a name="zh-cn_topic_0108272836_p1750103124416"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272836_p195014313441"><a name="zh-cn_topic_0108272836_p195014313441"></a><a name="zh-cn_topic_0108272836_p195014313441"></a>当作业执行成功时，会在写入目录下生成一个标识文件，文件名由用户指定，不指定时默认关闭该功能。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272836_row198531046012"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272836_p344406195416"><a name="zh-cn_topic_0108272836_p344406195416"></a><a name="zh-cn_topic_0108272836_p344406195416"></a>toJobConfig.firstRowAsHeader</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272836_p1244417635410"><a name="zh-cn_topic_0108272836_p1244417635410"></a><a name="zh-cn_topic_0108272836_p1244417635410"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272836_p124445615545"><a name="zh-cn_topic_0108272836_p124445615545"></a><a name="zh-cn_topic_0108272836_p124445615545"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272836_p54449616542"><a name="zh-cn_topic_0108272836_p54449616542"></a><a name="zh-cn_topic_0108272836_p54449616542"></a><span class="parmname" id="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmname1742242213195"><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmname1742242213195"></a><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmname1742242213195"></a>“toJobConfig.outputFormat”</span>（文件格式）为<span class="parmvalue" id="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmvalue739785211338"><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmvalue739785211338"></a><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmvalue739785211338"></a>“CSV_FILE”</span>时才有该参数。在迁移表到CSV文件时，CDM默认是不迁移表的标题行，如果该参数选择<span class="parmvalue" id="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmvalue11024151389"><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmvalue11024151389"></a><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmvalue11024151389"></a>“是”</span>，CDM在才会将表的标题行数据写入文件。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272836_row109575229288"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272836_p5622115931110"><a name="zh-cn_topic_0108272836_p5622115931110"></a><a name="zh-cn_topic_0108272836_p5622115931110"></a>toJobConfig.encryption</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272836_p10622125919118"><a name="zh-cn_topic_0108272836_p10622125919118"></a><a name="zh-cn_topic_0108272836_p10622125919118"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272836_p1762214595111"><a name="zh-cn_topic_0108272836_p1762214595111"></a><a name="zh-cn_topic_0108272836_p1762214595111"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.1.5.1.4 "><div class="p" id="zh-cn_topic_0108272836_p268631112373"><a name="zh-cn_topic_0108272836_p268631112373"></a><a name="zh-cn_topic_0108272836_p268631112373"></a>选择是否对上传的数据进行加密，以及加密方式：<a name="zh-cn_topic_0108272836_ul193603764111"></a><a name="zh-cn_topic_0108272836_ul193603764111"></a><ul id="zh-cn_topic_0108272836_ul193603764111"><li>NONE：不加密，直接写入数据。</li><li>AES-256-GCM：使用长度为256byte的AES对称加密算法，目前加密算法只支持AES-256-GCM（NoPadding）。</li></ul>
</div>
</td>
</tr>
<tr id="zh-cn_topic_0108272836_row1744292382815"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272836_p167122217132"><a name="zh-cn_topic_0108272836_p167122217132"></a><a name="zh-cn_topic_0108272836_p167122217132"></a>toJobConfig.dek</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272836_p74741127142115"><a name="zh-cn_topic_0108272836_p74741127142115"></a><a name="zh-cn_topic_0108272836_p74741127142115"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272836_p2474627102111"><a name="zh-cn_topic_0108272836_p2474627102111"></a><a name="zh-cn_topic_0108272836_p2474627102111"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272836_p23281415172211"><a name="zh-cn_topic_0108272836_p23281415172211"></a><a name="zh-cn_topic_0108272836_p23281415172211"></a>数据加密密钥，<span class="parmname" id="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmname697410131151"><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmname697410131151"></a><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmname697410131151"></a>“toJobConfig.encryption”</span>（加密方式）选择<span class="parmvalue" id="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmvalue838117223225"><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmvalue838117223225"></a><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmvalue838117223225"></a>“AES-256-GCM”</span>时有该参数，密钥由长度64的十六进制数组成。</p>
<p id="zh-cn_topic_0108272836_p18430442724"><a name="zh-cn_topic_0108272836_p18430442724"></a><a name="zh-cn_topic_0108272836_p18430442724"></a>请您牢记这里配置的密钥，解密时的密钥与这里配置的必须一致。如果不一致系统不会报异常，只是解密出来的数据会错误。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272836_row12331624112815"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272836_p26851918151311"><a name="zh-cn_topic_0108272836_p26851918151311"></a><a name="zh-cn_topic_0108272836_p26851918151311"></a>toJobConfig.iv</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272836_p1114152632113"><a name="zh-cn_topic_0108272836_p1114152632113"></a><a name="zh-cn_topic_0108272836_p1114152632113"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272836_p1414162617212"><a name="zh-cn_topic_0108272836_p1414162617212"></a><a name="zh-cn_topic_0108272836_p1414162617212"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272836_p24771354512"><a name="zh-cn_topic_0108272836_p24771354512"></a><a name="zh-cn_topic_0108272836_p24771354512"></a>初始化向量，<span class="parmname" id="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmname953919017169"><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmname953919017169"></a><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmname953919017169"></a>“toJobConfig.encryption”</span>（加密方式）选择<span class="parmvalue" id="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmvalue125661973247"><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmvalue125661973247"></a><a name="zh-cn_topic_0108272836_zh-cn_topic_0108272820_parmvalue125661973247"></a>“AES-256-GCM”</span>时有该参数，初始化向量由长度32的十六进制数组成。</p>
<p id="zh-cn_topic_0108272836_p51641322122914"><a name="zh-cn_topic_0108272836_p51641322122914"></a><a name="zh-cn_topic_0108272836_p51641322122914"></a>请您牢记这里配置的初始化向量，解密时的初始化向量与这里配置的必须一致。如果不一致系统不会报异常，只是解密出来的数据会错误。</p>
</td>
</tr>
</tbody>
</table>

