# 源端为FTP/SFTP/NAS（待下线）/SFS（待下线）<a name="dgc_02_0287"></a>

## JSON样例<a name="zh-cn_topic_0108272814_section33401108172339"></a>

```
"from-config-values": {
        "configs": [
          {
            "inputs": [
              {
                "name": "fromJobConfig.inputDirectory",
                "value": "/sftpfrom/from_sftp.csv"
              },
              {
                "name": "fromJobConfig.inputFormat",
                "value": "CSV_FILE"
              },
              {
                "name": "fromJobConfig.columnList",
                "value": "1&2&3&4&5&6&7&8&9&10&11&12"
              },
              {
                "name": "fromJobConfig.fieldSeparator",
                "value": ","
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
                "name": "fromJobConfig.splitType",
                "value": "FILE"
              }
            ],
            "name": "fromJobConfig"
          }
        ]
      }
```

## 参数说明<a name="zh-cn_topic_0108272814_section46589520174555"></a>

FTP、SFTP的源端作业参数相同，如[表1](#zh-cn_topic_0108272814_table13922888141527)所示。

**表 1**  文件类源端作业参数

<a name="zh-cn_topic_0108272814_table13922888141527"></a>
<table><thead align="left"><tr id="zh-cn_topic_0108272814_row229143141527"><th class="cellrowborder" valign="top" width="22.66%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0108272814_p66756185141527"><a name="zh-cn_topic_0108272814_p66756185141527"></a><a name="zh-cn_topic_0108272814_p66756185141527"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="19.78%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0108272814_p38541938141527"><a name="zh-cn_topic_0108272814_p38541938141527"></a><a name="zh-cn_topic_0108272814_p38541938141527"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.419999999999998%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0108272814_p34889279141527"><a name="zh-cn_topic_0108272814_p34889279141527"></a><a name="zh-cn_topic_0108272814_p34889279141527"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="40.14%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0108272814_p7459369141527"><a name="zh-cn_topic_0108272814_p7459369141527"></a><a name="zh-cn_topic_0108272814_p7459369141527"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0108272814_row62628929141527"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272814_p18560626141527"><a name="zh-cn_topic_0108272814_p18560626141527"></a><a name="zh-cn_topic_0108272814_p18560626141527"></a>fromJobConfig.inputDirectory</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272814_p27015713141527"><a name="zh-cn_topic_0108272814_p27015713141527"></a><a name="zh-cn_topic_0108272814_p27015713141527"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272814_p50167516142856"><a name="zh-cn_topic_0108272814_p50167516142856"></a><a name="zh-cn_topic_0108272814_p50167516142856"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108272814_p2430205141527"><a name="zh-cn_topic_0108272814_p2430205141527"></a><a name="zh-cn_topic_0108272814_p2430205141527"></a>抽取文件的路径。支持输入多个文件路径（最多50个），默认以<span class="parmvalue" id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue164501515620"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue164501515620"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue164501515620"></a>“|”</span>分隔，也可以自定义文件分隔符，例如：<span class="parmvalue" id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue1586848295718"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue1586848295718"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue1586848295718"></a>“FROM/example.csv|FROM/b.txt”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272814_row42094113141527"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272814_p26789449141527"><a name="zh-cn_topic_0108272814_p26789449141527"></a><a name="zh-cn_topic_0108272814_p26789449141527"></a>fromJobConfig.inputFormat</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272814_p22461756141527"><a name="zh-cn_topic_0108272814_p22461756141527"></a><a name="zh-cn_topic_0108272814_p22461756141527"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272814_p7462956141527"><a name="zh-cn_topic_0108272814_p7462956141527"></a><a name="zh-cn_topic_0108272814_p7462956141527"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.2.5.1.4 "><div class="p" id="zh-cn_topic_0108272814_p519680141527"><a name="zh-cn_topic_0108272814_p519680141527"></a><a name="zh-cn_topic_0108272814_p519680141527"></a>传输数据时所用的文件格式，目前支持以下文件格式：<a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_ul6517190495730"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_ul6517190495730"></a><ul id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_ul6517190495730"><li>CSV_FILE：CSV格式，用于迁移文件到数据表的场景。</li><li>JSON_FILE：JSON格式，一般都是用于迁移文件到数据表的场景。</li><li>BINARY_FILE：二进制格式，不解析文件内容直接传输，不要求文件格式必须为二进制。适用于文件到文件的原样复制。</li></ul>
</div>
<p id="zh-cn_topic_0108272814_p3415682014487"><a name="zh-cn_topic_0108272814_p3415682014487"></a><a name="zh-cn_topic_0108272814_p3415682014487"></a>当选择<span class="parmvalue" id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue4805818695742"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue4805818695742"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue4805818695742"></a>“BINARY_FILE”</span>时，目的端也必须为文件系统。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272814_row8336449141527"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272814_p48880710193940"><a name="zh-cn_topic_0108272814_p48880710193940"></a><a name="zh-cn_topic_0108272814_p48880710193940"></a>fromJobConfig.lineSeparator</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272814_p67023407193940"><a name="zh-cn_topic_0108272814_p67023407193940"></a><a name="zh-cn_topic_0108272814_p67023407193940"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272814_p60186848193940"><a name="zh-cn_topic_0108272814_p60186848193940"></a><a name="zh-cn_topic_0108272814_p60186848193940"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108272814_p43296514193940"><a name="zh-cn_topic_0108272814_p43296514193940"></a><a name="zh-cn_topic_0108272814_p43296514193940"></a>文件中的换行符，默认自动识别<span class="parmvalue" id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue33347698191227"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue33347698191227"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue33347698191227"></a>“\n”</span>、<span class="parmvalue" id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue3294893191243"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue3294893191243"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue3294893191243"></a>“\r”</span>或<span class="parmvalue" id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue61235067191258"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue61235067191258"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue61235067191258"></a>“\r\n”</span>，例如：<span class="parmvalue" id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue4747194191314"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue4747194191314"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue4747194191314"></a>“\n”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272814_row2070931215120"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272814_p59153600193940"><a name="zh-cn_topic_0108272814_p59153600193940"></a><a name="zh-cn_topic_0108272814_p59153600193940"></a>fromJobConfig.columnList</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272814_p26712273193940"><a name="zh-cn_topic_0108272814_p26712273193940"></a><a name="zh-cn_topic_0108272814_p26712273193940"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272814_p16210536193940"><a name="zh-cn_topic_0108272814_p16210536193940"></a><a name="zh-cn_topic_0108272814_p16210536193940"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108272814_p37985002193940"><a name="zh-cn_topic_0108272814_p37985002193940"></a><a name="zh-cn_topic_0108272814_p37985002193940"></a>需要抽取的列号，列号之间使用<span class="parmvalue" id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue36226019586"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue36226019586"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue36226019586"></a>“&amp;”</span>分割，并由小到大排序，例如：<span class="parmvalue" id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue6416671195818"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue6416671195818"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue6416671195818"></a>“1&amp;3&amp;5”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272814_row12312261165154"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272814_p63971201193940"><a name="zh-cn_topic_0108272814_p63971201193940"></a><a name="zh-cn_topic_0108272814_p63971201193940"></a>fromJobConfig.lineSeparator</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272814_p14284794193940"><a name="zh-cn_topic_0108272814_p14284794193940"></a><a name="zh-cn_topic_0108272814_p14284794193940"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272814_p16217700193940"><a name="zh-cn_topic_0108272814_p16217700193940"></a><a name="zh-cn_topic_0108272814_p16217700193940"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108272814_p38565351193940"><a name="zh-cn_topic_0108272814_p38565351193940"></a><a name="zh-cn_topic_0108272814_p38565351193940"></a>换行符，当文件格式为<span class="parmvalue" id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue5573206395833"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue5573206395833"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue5573206395833"></a>“CSV_FILE”</span>时此参数有效，默认值为：<span class="parmvalue" id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue1131293795837"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue1131293795837"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue1131293795837"></a>“\r\n”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272814_row20086039165159"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272814_p40343041193940"><a name="zh-cn_topic_0108272814_p40343041193940"></a><a name="zh-cn_topic_0108272814_p40343041193940"></a>fromJobConfig.fieldSeparator</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272814_p46560925193940"><a name="zh-cn_topic_0108272814_p46560925193940"></a><a name="zh-cn_topic_0108272814_p46560925193940"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272814_p13338548193940"><a name="zh-cn_topic_0108272814_p13338548193940"></a><a name="zh-cn_topic_0108272814_p13338548193940"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108272814_p6680624193940"><a name="zh-cn_topic_0108272814_p6680624193940"></a><a name="zh-cn_topic_0108272814_p6680624193940"></a>字段分隔符，当文件格式为<span class="parmvalue" id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue3066733595853"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue3066733595853"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue3066733595853"></a>“CSV_FILE”</span>时此参数有效，默认值为：<span class="parmvalue" id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue1399095795859"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue1399095795859"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue1399095795859"></a>“,”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272814_row201058415316"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272814_p179629179572"><a name="zh-cn_topic_0108272814_p179629179572"></a><a name="zh-cn_topic_0108272814_p179629179572"></a>fromJobConfig.quoteChar</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272814_p1896201711572"><a name="zh-cn_topic_0108272814_p1896201711572"></a><a name="zh-cn_topic_0108272814_p1896201711572"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272814_p9962817165718"><a name="zh-cn_topic_0108272814_p9962817165718"></a><a name="zh-cn_topic_0108272814_p9962817165718"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108272814_p113238488438"><a name="zh-cn_topic_0108272814_p113238488438"></a><a name="zh-cn_topic_0108272814_p113238488438"></a>是否使用包围符，选择<span class="parmvalue" id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue1512517923819"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue1512517923819"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue1512517923819"></a>“true”</span>时，包围符内的字段分隔符会被视为字符串值的一部分，目前CDM默认的包围符为："。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272814_row610901871125"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272814_p326661711235"><a name="zh-cn_topic_0108272814_p326661711235"></a><a name="zh-cn_topic_0108272814_p326661711235"></a>fromJobConfig.regexSeparator</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272814_p6326942511235"><a name="zh-cn_topic_0108272814_p6326942511235"></a><a name="zh-cn_topic_0108272814_p6326942511235"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272814_p2454981411235"><a name="zh-cn_topic_0108272814_p2454981411235"></a><a name="zh-cn_topic_0108272814_p2454981411235"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108272814_p4237790311235"><a name="zh-cn_topic_0108272814_p4237790311235"></a><a name="zh-cn_topic_0108272814_p4237790311235"></a>是否使用正则表达式分割字段，当文件格式为<span class="parmvalue" id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue1431442714113"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue1431442714113"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue1431442714113"></a>“CSV_FILE”</span>时此参数有效。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272814_row1740365611231"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272814_p2341419011235"><a name="zh-cn_topic_0108272814_p2341419011235"></a><a name="zh-cn_topic_0108272814_p2341419011235"></a>fromJobConfig.regex</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272814_p1750120911235"><a name="zh-cn_topic_0108272814_p1750120911235"></a><a name="zh-cn_topic_0108272814_p1750120911235"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272814_p831182911235"><a name="zh-cn_topic_0108272814_p831182911235"></a><a name="zh-cn_topic_0108272814_p831182911235"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108272814_p216954511235"><a name="zh-cn_topic_0108272814_p216954511235"></a><a name="zh-cn_topic_0108272814_p216954511235"></a>正则表达式，当选择使用正则表达式分割字段时，此参数有效。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272814_row1868417394538"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272814_p7684103915314"><a name="zh-cn_topic_0108272814_p7684103915314"></a><a name="zh-cn_topic_0108272814_p7684103915314"></a>fromJobConfig.firstRowAsHeader</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272814_p1968433985310"><a name="zh-cn_topic_0108272814_p1968433985310"></a><a name="zh-cn_topic_0108272814_p1968433985310"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272814_p1868483985320"><a name="zh-cn_topic_0108272814_p1868483985320"></a><a name="zh-cn_topic_0108272814_p1868483985320"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108272814_p18684539155318"><a name="zh-cn_topic_0108272814_p18684539155318"></a><a name="zh-cn_topic_0108272814_p18684539155318"></a>是否默认首行为标题行，当文件格式为<span class="parmvalue" id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue1467312083111"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue1467312083111"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue1467312083111"></a>“CSV_FILE”</span>时此参数有效。在迁移CSV文件到表时，CDM默认是全部写入，当该参数选择<span class="parmvalue" id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue11024151389"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue11024151389"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue11024151389"></a>“true”</span>时，CDM会将CSV文件的第一行数据作为标题行，不写入目的端的表。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272814_row4606474911518"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272814_p4025721311518"><a name="zh-cn_topic_0108272814_p4025721311518"></a><a name="zh-cn_topic_0108272814_p4025721311518"></a>fromJobConfig.fromCompression</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272814_p3960883811518"><a name="zh-cn_topic_0108272814_p3960883811518"></a><a name="zh-cn_topic_0108272814_p3960883811518"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272814_p5419927911518"><a name="zh-cn_topic_0108272814_p5419927911518"></a><a name="zh-cn_topic_0108272814_p5419927911518"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.2.5.1.4 "><div class="p" id="zh-cn_topic_0108272814_p2806544011518"><a name="zh-cn_topic_0108272814_p2806544011518"></a><a name="zh-cn_topic_0108272814_p2806544011518"></a>压缩格式，当文件格式为<span class="parmvalue" id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue119890444132"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue119890444132"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue119890444132"></a>“CSV_FILE”</span>或<span class="parmvalue" id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue66712132148"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue66712132148"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue66712132148"></a>“JSON”</span>时此参数有效。选择对应压缩格式的源文件：<a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_ul64234801103023"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_ul64234801103023"></a><ul id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_ul64234801103023"><li>NONE：表示传输所有格式的文件。</li><li>GZIP：表示只传输GZIP格式的文件。</li><li>ZIP：表示只传输ZIP格式的文件。</li></ul>
</div>
</td>
</tr>
<tr id="zh-cn_topic_0108272814_row28370483155251"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272814_p18317612193940"><a name="zh-cn_topic_0108272814_p18317612193940"></a><a name="zh-cn_topic_0108272814_p18317612193940"></a>fromJobConfig.jsonReferenceNode</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272814_p7331603193940"><a name="zh-cn_topic_0108272814_p7331603193940"></a><a name="zh-cn_topic_0108272814_p7331603193940"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272814_p56988962193940"><a name="zh-cn_topic_0108272814_p56988962193940"></a><a name="zh-cn_topic_0108272814_p56988962193940"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108272814_p52703234193940"><a name="zh-cn_topic_0108272814_p52703234193940"></a><a name="zh-cn_topic_0108272814_p52703234193940"></a>记录节点，当文件格式为<span class="parmvalue" id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue57862435184727"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue57862435184727"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue57862435184727"></a>“JSON_FILE”</span>时此参数有效。对该JSON节点下的数据进行解析，如果该节点对应的数据为JSON数组，那么系统会以同一模式从该数组中提取数据。多层嵌套的JSON节点以字符<span class="parmvalue" id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue22292394184637"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue22292394184637"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue22292394184637"></a>“.”</span>分割，例如：<span class="parmvalue" id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue28343361184643"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue28343361184643"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue28343361184643"></a>“data.list”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272814_row62580131193857"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272814_p66009299193940"><a name="zh-cn_topic_0108272814_p66009299193940"></a><a name="zh-cn_topic_0108272814_p66009299193940"></a>fromJobConfig.encodeType</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272814_p45152983193940"><a name="zh-cn_topic_0108272814_p45152983193940"></a><a name="zh-cn_topic_0108272814_p45152983193940"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272814_p33513000193940"><a name="zh-cn_topic_0108272814_p33513000193940"></a><a name="zh-cn_topic_0108272814_p33513000193940"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108272814_p30198445193940"><a name="zh-cn_topic_0108272814_p30198445193940"></a><a name="zh-cn_topic_0108272814_p30198445193940"></a>编码类型，例如：<span class="parmvalue" id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue4489407595918"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue4489407595918"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue4489407595918"></a>“UTF_8”</span>或<span class="parmvalue" id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue3309953795922"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue3309953795922"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue3309953795922"></a>“GBK”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272814_row226444193923"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272814_p10703804193940"><a name="zh-cn_topic_0108272814_p10703804193940"></a><a name="zh-cn_topic_0108272814_p10703804193940"></a>fromJobConfig.fromFileOpType</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272814_p61701775193940"><a name="zh-cn_topic_0108272814_p61701775193940"></a><a name="zh-cn_topic_0108272814_p61701775193940"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272814_p31787850193940"><a name="zh-cn_topic_0108272814_p31787850193940"></a><a name="zh-cn_topic_0108272814_p31787850193940"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108272814_p24679062193940"><a name="zh-cn_topic_0108272814_p24679062193940"></a><a name="zh-cn_topic_0108272814_p24679062193940"></a>源文件处理方式，作业完成后对源端文件的操作，支持重命名或删除源端文件。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272814_row17380182010103"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272814_p108051742228"><a name="zh-cn_topic_0108272814_p108051742228"></a><a name="zh-cn_topic_0108272814_p108051742228"></a>fromJobConfig.useMarkerFile</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272814_p1238010205108"><a name="zh-cn_topic_0108272814_p1238010205108"></a><a name="zh-cn_topic_0108272814_p1238010205108"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272814_p16380520181011"><a name="zh-cn_topic_0108272814_p16380520181011"></a><a name="zh-cn_topic_0108272814_p16380520181011"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108272814_p538062091010"><a name="zh-cn_topic_0108272814_p538062091010"></a><a name="zh-cn_topic_0108272814_p538062091010"></a>选择是否开启作业标识文件的功能。当源端路径下存在启动作业的标识文件时才启动作业，否则会挂起等待一段时间，等待时长在下方“fromJobConfig.waitTime”（等待时间）参数中配置。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272814_row40508618193924"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272814_p21496433171234"><a name="zh-cn_topic_0108272814_p21496433171234"></a><a name="zh-cn_topic_0108272814_p21496433171234"></a>fromJobConfig.markerFile</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272814_p4977149193940"><a name="zh-cn_topic_0108272814_p4977149193940"></a><a name="zh-cn_topic_0108272814_p4977149193940"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272814_p495958193940"><a name="zh-cn_topic_0108272814_p495958193940"></a><a name="zh-cn_topic_0108272814_p495958193940"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108272814_p40172643193940"><a name="zh-cn_topic_0108272814_p40172643193940"></a><a name="zh-cn_topic_0108272814_p40172643193940"></a>启动作业的标识文件名。指定文件后，只有在源端路径下存在该文件的情况下才会运行任务，不指定时默认不启用该功能，例如：<span class="filepath" id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_filepath47013227185444"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_filepath47013227185444"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_filepath47013227185444"></a>“ok.txt”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272814_row111592441016"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272814_p1784925765913"><a name="zh-cn_topic_0108272814_p1784925765913"></a><a name="zh-cn_topic_0108272814_p1784925765913"></a>fromJobConfig.waitTime</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272814_p111542431016"><a name="zh-cn_topic_0108272814_p111542431016"></a><a name="zh-cn_topic_0108272814_p111542431016"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272814_p811512418103"><a name="zh-cn_topic_0108272814_p811512418103"></a><a name="zh-cn_topic_0108272814_p811512418103"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108272814_p15247819764"><a name="zh-cn_topic_0108272814_p15247819764"></a><a name="zh-cn_topic_0108272814_p15247819764"></a>选择开启作业标识文件的功能时，如果源路径下不存在启动作业的标识文件，作业挂机等待的时长，当超时后任务会失败。</p>
<p id="zh-cn_topic_0108272814_p149111137114"><a name="zh-cn_topic_0108272814_p149111137114"></a><a name="zh-cn_topic_0108272814_p149111137114"></a>等待时间设置为0时，当源端路径下不存在标识文件，任务会立即失败。</p>
<p id="zh-cn_topic_0108272814_p104529915719"><a name="zh-cn_topic_0108272814_p104529915719"></a><a name="zh-cn_topic_0108272814_p104529915719"></a>单位：秒。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272814_row28947646193924"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272814_p36206523193940"><a name="zh-cn_topic_0108272814_p36206523193940"></a><a name="zh-cn_topic_0108272814_p36206523193940"></a>fromJobConfig.filterType</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272814_p47047254193940"><a name="zh-cn_topic_0108272814_p47047254193940"></a><a name="zh-cn_topic_0108272814_p47047254193940"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272814_p52731205193940"><a name="zh-cn_topic_0108272814_p52731205193940"></a><a name="zh-cn_topic_0108272814_p52731205193940"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.2.5.1.4 "><div class="p" id="zh-cn_topic_0108272814_p43369201193940"><a name="zh-cn_topic_0108272814_p43369201193940"></a><a name="zh-cn_topic_0108272814_p43369201193940"></a>选择过滤器类型：<a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_ul32827929185645"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_ul32827929185645"></a><ul id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_ul32827929185645"><li>WILDCARD：输入通配符作为过滤文件，满足过滤条件的路径或文件会被传输。</li><li>TIME：时间过滤器，当文件的修改时间晚于输入的时间时，该文件才会被传输。</li></ul>
</div>
</td>
</tr>
<tr id="zh-cn_topic_0108272814_row45121003193925"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272814_p34862062193940"><a name="zh-cn_topic_0108272814_p34862062193940"></a><a name="zh-cn_topic_0108272814_p34862062193940"></a>fromJobConfig.pathFilter</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272814_p5254812193940"><a name="zh-cn_topic_0108272814_p5254812193940"></a><a name="zh-cn_topic_0108272814_p5254812193940"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272814_p22986638193940"><a name="zh-cn_topic_0108272814_p22986638193940"></a><a name="zh-cn_topic_0108272814_p22986638193940"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108272814_p49978413193940"><a name="zh-cn_topic_0108272814_p49978413193940"></a><a name="zh-cn_topic_0108272814_p49978413193940"></a>路径过滤器，过滤类型为通配符时配置，用于过滤文件目录，例如：<span class="uicontrol" id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_uicontrol66669561185917"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_uicontrol66669561185917"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_uicontrol66669561185917"></a>“*input”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272814_row44400770193926"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272814_p14461072193940"><a name="zh-cn_topic_0108272814_p14461072193940"></a><a name="zh-cn_topic_0108272814_p14461072193940"></a>fromJobConfig.fileFilter</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272814_p30496164193940"><a name="zh-cn_topic_0108272814_p30496164193940"></a><a name="zh-cn_topic_0108272814_p30496164193940"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272814_p54270213193940"><a name="zh-cn_topic_0108272814_p54270213193940"></a><a name="zh-cn_topic_0108272814_p54270213193940"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108272814_p33811098193940"><a name="zh-cn_topic_0108272814_p33811098193940"></a><a name="zh-cn_topic_0108272814_p33811098193940"></a>文件过滤器，过滤类型为通配符时配置，用于过滤目录下的文件，支持配置多个文件，中间使用<span class="parmvalue" id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue125501853131710"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue125501853131710"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue125501853131710"></a>“,”</span>分隔，例如：<span class="uicontrol" id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_uicontrol4491163718912"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_uicontrol4491163718912"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_uicontrol4491163718912"></a>“*.csv,*.txt”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272814_row69481138151612"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272814_p101771547152117"><a name="zh-cn_topic_0108272814_p101771547152117"></a><a name="zh-cn_topic_0108272814_p101771547152117"></a>fromJobConfig.startTime</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272814_p574033312314"><a name="zh-cn_topic_0108272814_p574033312314"></a><a name="zh-cn_topic_0108272814_p574033312314"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272814_p1085074720811"><a name="zh-cn_topic_0108272814_p1085074720811"></a><a name="zh-cn_topic_0108272814_p1085074720811"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108272814_p18311447203911"><a name="zh-cn_topic_0108272814_p18311447203911"></a><a name="zh-cn_topic_0108272814_p18311447203911"></a><span class="parmname" id="zh-cn_topic_0108272814_zh-cn_topic_0108275319_parmname4237191913013"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108275319_parmname4237191913013"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108275319_parmname4237191913013"></a>“过滤类型”</span>选择<span class="parmvalue" id="zh-cn_topic_0108272814_zh-cn_topic_0108275319_parmvalue933016296308"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108275319_parmvalue933016296308"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108275319_parmvalue933016296308"></a>“时间过滤器”</span>时，可以指定一个时间值，当文件的修改时间大于该时间才会被传输，输入的时间格式需为<span class="parmvalue" id="zh-cn_topic_0108272814_zh-cn_topic_0108275319_parmvalue9313481341"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108275319_parmvalue9313481341"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108275319_parmvalue9313481341"></a>“yyyy-MM-dd HH:mm:ss”</span>。</p>
<p id="zh-cn_topic_0108272814_p12144111817144"><a name="zh-cn_topic_0108272814_p12144111817144"></a><a name="zh-cn_topic_0108272814_p12144111817144"></a>该参数支持配置为时间宏变量，例如<strong id="zh-cn_topic_0108272814_zh-cn_topic_0108275319_b97861314103"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108275319_b97861314103"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108275319_b97861314103"></a>${timestamp(dateformat(yyyy-MM-dd HH:mm:ss,-90,DAY))}</strong>表示：只迁移最近90天内的文件。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272814_row135271461251"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272814_p2076744121718"><a name="zh-cn_topic_0108272814_p2076744121718"></a><a name="zh-cn_topic_0108272814_p2076744121718"></a>fromJobConfig.endTime</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272814_p176712419173"><a name="zh-cn_topic_0108272814_p176712419173"></a><a name="zh-cn_topic_0108272814_p176712419173"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272814_p155977520229"><a name="zh-cn_topic_0108272814_p155977520229"></a><a name="zh-cn_topic_0108272814_p155977520229"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108272814_p34921611171416"><a name="zh-cn_topic_0108272814_p34921611171416"></a><a name="zh-cn_topic_0108272814_p34921611171416"></a><span class="parmname" id="zh-cn_topic_0108272814_zh-cn_topic_0108275319_parmname106751314209"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108275319_parmname106751314209"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108275319_parmname106751314209"></a>“过滤类型”</span>选择<span class="parmvalue" id="zh-cn_topic_0108272814_zh-cn_topic_0108275319_parmvalue13675131413012"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108275319_parmvalue13675131413012"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108275319_parmvalue13675131413012"></a>“时间过滤器”</span>时，可以指定一个时间值，当文件的修改时间小于该时间才会被传输，输入的时间格式需为<span class="parmvalue" id="zh-cn_topic_0108272814_zh-cn_topic_0108275319_parmvalue146759148017"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108275319_parmvalue146759148017"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108275319_parmvalue146759148017"></a>“yyyy-MM-dd HH:mm:ss”</span>。</p>
<p id="zh-cn_topic_0108272814_p13254806156"><a name="zh-cn_topic_0108272814_p13254806156"></a><a name="zh-cn_topic_0108272814_p13254806156"></a>该参数支持配置为时间宏变量，例如<strong id="zh-cn_topic_0108272814_zh-cn_topic_0108275319_b1521616538112"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108275319_b1521616538112"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108275319_b1521616538112"></a>${timestamp(dateformat(yyyy-MM-dd HH:mm:ss))}</strong>表示：只迁移修改时间为当前时间以前的文件。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272814_row20340693193926"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272814_p52262369164538"><a name="zh-cn_topic_0108272814_p52262369164538"></a><a name="zh-cn_topic_0108272814_p52262369164538"></a>fromJobConfig.fileSeparator</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272814_p5393490164538"><a name="zh-cn_topic_0108272814_p5393490164538"></a><a name="zh-cn_topic_0108272814_p5393490164538"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272814_p34219511164538"><a name="zh-cn_topic_0108272814_p34219511164538"></a><a name="zh-cn_topic_0108272814_p34219511164538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108272814_p8813175612198"><a name="zh-cn_topic_0108272814_p8813175612198"></a><a name="zh-cn_topic_0108272814_p8813175612198"></a>“fromJobConfig.inputDirectory”（抽取文件的路径）参数中如果输入的是多个文件路径，CDM使用这里配置的文件分隔符来区分各个文件，默认为<span class="parmvalue" id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue1360984183310"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue1360984183310"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmvalue1360984183310"></a>“|”</span>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272814_row114090221369"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272814_p5622115931110"><a name="zh-cn_topic_0108272814_p5622115931110"></a><a name="zh-cn_topic_0108272814_p5622115931110"></a>fromJobConfig.decryption</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272814_p10622125919118"><a name="zh-cn_topic_0108272814_p10622125919118"></a><a name="zh-cn_topic_0108272814_p10622125919118"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272814_p1762214595111"><a name="zh-cn_topic_0108272814_p1762214595111"></a><a name="zh-cn_topic_0108272814_p1762214595111"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.2.5.1.4 "><div class="p" id="zh-cn_topic_0108272814_p268631112373"><a name="zh-cn_topic_0108272814_p268631112373"></a><a name="zh-cn_topic_0108272814_p268631112373"></a>导出文件时，选择是否对已加密的文件解密后再导出，以及解密方式：<a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_ul193603764111"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_ul193603764111"></a><ul id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_ul193603764111"><li>NONE：不解密，直接导出文件。</li><li>AES-256-GCM：使用AES-256-GCM（NoPadding）算法解密后再导出文件。</li></ul>
</div>
</td>
</tr>
<tr id="zh-cn_topic_0108272814_row169591722153612"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272814_p167122217132"><a name="zh-cn_topic_0108272814_p167122217132"></a><a name="zh-cn_topic_0108272814_p167122217132"></a>fromJobConfig.dek</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272814_p74741127142115"><a name="zh-cn_topic_0108272814_p74741127142115"></a><a name="zh-cn_topic_0108272814_p74741127142115"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272814_p2474627102111"><a name="zh-cn_topic_0108272814_p2474627102111"></a><a name="zh-cn_topic_0108272814_p2474627102111"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108272814_p23281415172211"><a name="zh-cn_topic_0108272814_p23281415172211"></a><a name="zh-cn_topic_0108272814_p23281415172211"></a>数据解密密钥，密钥由长度64的十六进制数组成，且必须与加密时配置的<span class="parmname" id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmname1660363014167"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmname1660363014167"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmname1660363014167"></a>“toJobConfig.dek”</span>（导入时配置的数据加密密钥）一致。如果不一致系统不会报异常，只是解密出来的数据会错误。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272814_row14818523163614"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272814_p26851918151311"><a name="zh-cn_topic_0108272814_p26851918151311"></a><a name="zh-cn_topic_0108272814_p26851918151311"></a>fromJobConfig.iv</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272814_p1114152632113"><a name="zh-cn_topic_0108272814_p1114152632113"></a><a name="zh-cn_topic_0108272814_p1114152632113"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272814_p1414162617212"><a name="zh-cn_topic_0108272814_p1414162617212"></a><a name="zh-cn_topic_0108272814_p1414162617212"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108272814_p24771354512"><a name="zh-cn_topic_0108272814_p24771354512"></a><a name="zh-cn_topic_0108272814_p24771354512"></a>解密需要的初始化向量，初始化向量由长度32的十六进制数组成，且必须与加密时配置的<span class="parmname" id="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmname1257711377164"><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmname1257711377164"></a><a name="zh-cn_topic_0108272814_zh-cn_topic_0108272831_parmname1257711377164"></a>“toJobConfig.iv”</span>（导入时配置的初始化向量）一致。如果不一致系统不会报异常，只是解密出来的数据会错误。</p>
</td>
</tr>
<tr id="zh-cn_topic_0108272814_row191971036141119"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0108272814_p1724715172115"><a name="zh-cn_topic_0108272814_p1724715172115"></a><a name="zh-cn_topic_0108272814_p1724715172115"></a>fromJobConfig.md5FileSuffix</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0108272814_p32471517121116"><a name="zh-cn_topic_0108272814_p32471517121116"></a><a name="zh-cn_topic_0108272814_p32471517121116"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0108272814_p1424720170114"><a name="zh-cn_topic_0108272814_p1424720170114"></a><a name="zh-cn_topic_0108272814_p1424720170114"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0108272814_p72470172110"><a name="zh-cn_topic_0108272814_p72470172110"></a><a name="zh-cn_topic_0108272814_p72470172110"></a>校验CDM抽取的文件，是否与源文件一致。</p>
</td>
</tr>
</tbody>
</table>

