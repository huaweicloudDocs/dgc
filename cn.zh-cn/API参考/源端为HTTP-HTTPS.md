# 源端为HTTP/HTTPS<a name="dgc_02_0288"></a>

## JSON样例<a name="zh-cn_topic_0115187940_section33401108172339"></a>

```
"from-config-values": {
        "configs": [
          {
            "inputs": [
              {
                "name": "fromJobConfig.inputDirectory",
                "value": "http://10.114.196.186:8080/httpfrom/symbol.txt"
              },
              {
                "name": "fromJobConfig.inputFormat",
                "value": "BINARY_FILE"
              },
              {
                "name": "fromJobConfig.fromCompression",
                "value": "TARGZ"
              },
              {
                "name": "fromJobConfig.compressedFileSuffix",
                "value": "*"
              },
              {
                "name": "fromJobConfig.fileSeparator",
                "value": "|"
              }
            ],
            "name": "fromJobConfig"
          }
        ]
      }
```

## 参数说明<a name="zh-cn_topic_0115187940_section46589520174555"></a>

<a name="zh-cn_topic_0115187940_table13922888141527"></a>
<table><thead align="left"><tr id="zh-cn_topic_0115187940_row229143141527"><th class="cellrowborder" valign="top" width="22.66%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0115187940_p66756185141527"><a name="zh-cn_topic_0115187940_p66756185141527"></a><a name="zh-cn_topic_0115187940_p66756185141527"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="19.78%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0115187940_p38541938141527"><a name="zh-cn_topic_0115187940_p38541938141527"></a><a name="zh-cn_topic_0115187940_p38541938141527"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.419999999999998%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0115187940_p34889279141527"><a name="zh-cn_topic_0115187940_p34889279141527"></a><a name="zh-cn_topic_0115187940_p34889279141527"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="40.14%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0115187940_p7459369141527"><a name="zh-cn_topic_0115187940_p7459369141527"></a><a name="zh-cn_topic_0115187940_p7459369141527"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0115187940_row62628929141527"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0115187940_p18560626141527"><a name="zh-cn_topic_0115187940_p18560626141527"></a><a name="zh-cn_topic_0115187940_p18560626141527"></a>fromJobConfig.inputDirectory</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0115187940_p27015713141527"><a name="zh-cn_topic_0115187940_p27015713141527"></a><a name="zh-cn_topic_0115187940_p27015713141527"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0115187940_p50167516142856"><a name="zh-cn_topic_0115187940_p50167516142856"></a><a name="zh-cn_topic_0115187940_p50167516142856"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0115187940_p15904104063219"><a name="zh-cn_topic_0115187940_p15904104063219"></a><a name="zh-cn_topic_0115187940_p15904104063219"></a>待抽取文件的URL。</p>
<p id="zh-cn_topic_0115187940_p0123115172917"><a name="zh-cn_topic_0115187940_p0123115172917"></a><a name="zh-cn_topic_0115187940_p0123115172917"></a>用于读取一个公网HTTP/HTTPS URL的文件，包括第三方对象存储的公共读取场景和网盘场景。</p>
</td>
</tr>
<tr id="zh-cn_topic_0115187940_row42094113141527"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0115187940_p26789449141527"><a name="zh-cn_topic_0115187940_p26789449141527"></a><a name="zh-cn_topic_0115187940_p26789449141527"></a>fromJobConfig.inputFormat</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0115187940_p22461756141527"><a name="zh-cn_topic_0115187940_p22461756141527"></a><a name="zh-cn_topic_0115187940_p22461756141527"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0115187940_p7462956141527"><a name="zh-cn_topic_0115187940_p7462956141527"></a><a name="zh-cn_topic_0115187940_p7462956141527"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0115187940_p1465533914361"><a name="zh-cn_topic_0115187940_p1465533914361"></a><a name="zh-cn_topic_0115187940_p1465533914361"></a>传输数据时所用的文件格式，目前只支持二进制格式。</p>
</td>
</tr>
<tr id="zh-cn_topic_0115187940_row9447745533"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0115187940_p4025721311518"><a name="zh-cn_topic_0115187940_p4025721311518"></a><a name="zh-cn_topic_0115187940_p4025721311518"></a>fromJobConfig.fromCompression</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0115187940_p3960883811518"><a name="zh-cn_topic_0115187940_p3960883811518"></a><a name="zh-cn_topic_0115187940_p3960883811518"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0115187940_p5419927911518"><a name="zh-cn_topic_0115187940_p5419927911518"></a><a name="zh-cn_topic_0115187940_p5419927911518"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.1.5.1.4 "><div class="p" id="zh-cn_topic_0115187940_p2806544011518"><a name="zh-cn_topic_0115187940_p2806544011518"></a><a name="zh-cn_topic_0115187940_p2806544011518"></a>选择对应压缩格式的源文件进行迁移：<a name="zh-cn_topic_0115187940_zh-cn_topic_0108272831_ul64234801103023"></a><a name="zh-cn_topic_0115187940_zh-cn_topic_0108272831_ul64234801103023"></a><ul id="zh-cn_topic_0115187940_zh-cn_topic_0108272831_ul64234801103023"><li>NONE：表示传输所有格式的文件。</li><li>GZIP：表示只传输GZIP格式的文件。</li><li>ZIP：表示只传输ZIP格式的文件。</li><li>TAR.GZ：表示只传输TAR.GZ格式的文件。</li></ul>
</div>
</td>
</tr>
<tr id="zh-cn_topic_0115187940_row81878171452"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0115187940_p11187517355"><a name="zh-cn_topic_0115187940_p11187517355"></a><a name="zh-cn_topic_0115187940_p11187517355"></a>fromJobConfig.compressedFileSuffix</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0115187940_p101873176517"><a name="zh-cn_topic_0115187940_p101873176517"></a><a name="zh-cn_topic_0115187940_p101873176517"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0115187940_p1418731718517"><a name="zh-cn_topic_0115187940_p1418731718517"></a><a name="zh-cn_topic_0115187940_p1418731718517"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0115187940_p13187191714515"><a name="zh-cn_topic_0115187940_p13187191714515"></a><a name="zh-cn_topic_0115187940_p13187191714515"></a>需要解压缩的文件后缀名。当一批文件中以该值为后缀时，才会执行解压缩操作，否则则保持原样传输。当输入*或为空时，所有文件都会被解压。</p>
</td>
</tr>
<tr id="zh-cn_topic_0115187940_row24617461835"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0115187940_p104644610314"><a name="zh-cn_topic_0115187940_p104644610314"></a><a name="zh-cn_topic_0115187940_p104644610314"></a>fromJobConfig.fileSeparator</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0115187940_p38965081218"><a name="zh-cn_topic_0115187940_p38965081218"></a><a name="zh-cn_topic_0115187940_p38965081218"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0115187940_p589710191214"><a name="zh-cn_topic_0115187940_p589710191214"></a><a name="zh-cn_topic_0115187940_p589710191214"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0115187940_p8813175612198"><a name="zh-cn_topic_0115187940_p8813175612198"></a><a name="zh-cn_topic_0115187940_p8813175612198"></a>传输多个文件时，CDM使用这里配置的文件分隔符来区分各个文件，默认为|。</p>
</td>
</tr>
<tr id="zh-cn_topic_0115187940_row882482611141"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0115187940_p7825026201418"><a name="zh-cn_topic_0115187940_p7825026201418"></a><a name="zh-cn_topic_0115187940_p7825026201418"></a>fromJobConfig.useQuery</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0115187940_p1482611260145"><a name="zh-cn_topic_0115187940_p1482611260145"></a><a name="zh-cn_topic_0115187940_p1482611260145"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0115187940_p382620264145"><a name="zh-cn_topic_0115187940_p382620264145"></a><a name="zh-cn_topic_0115187940_p382620264145"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.1.5.1.4 "><a name="zh-cn_topic_0115187940_ul887516311069"></a><a name="zh-cn_topic_0115187940_ul887516311069"></a><ul id="zh-cn_topic_0115187940_ul887516311069"><li>该参数设置为<span class="parmvalue" id="zh-cn_topic_0115187940_parmvalue8561326597"><a name="zh-cn_topic_0115187940_parmvalue8561326597"></a><a name="zh-cn_topic_0115187940_parmvalue8561326597"></a>“true”</span>时，上传到OBS的对象使用的对象名，为去掉query参数后的字符。</li><li>该参数设置为<span class="parmvalue" id="zh-cn_topic_0115187940_parmvalue598043819711"><a name="zh-cn_topic_0115187940_parmvalue598043819711"></a><a name="zh-cn_topic_0115187940_parmvalue598043819711"></a>“false”</span>时，上传到OBS的对象使用的对象名，包含query参数。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0115187940_row1844163653611"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0115187940_p5622115931110"><a name="zh-cn_topic_0115187940_p5622115931110"></a><a name="zh-cn_topic_0115187940_p5622115931110"></a>fromJobConfig.decryption</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0115187940_p10622125919118"><a name="zh-cn_topic_0115187940_p10622125919118"></a><a name="zh-cn_topic_0115187940_p10622125919118"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0115187940_p1762214595111"><a name="zh-cn_topic_0115187940_p1762214595111"></a><a name="zh-cn_topic_0115187940_p1762214595111"></a>枚举</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.1.5.1.4 "><div class="p" id="zh-cn_topic_0115187940_p268631112373"><a name="zh-cn_topic_0115187940_p268631112373"></a><a name="zh-cn_topic_0115187940_p268631112373"></a>导出文件时，选择是否对已加密的文件解密后再导出，以及解密方式：<a name="zh-cn_topic_0115187940_zh-cn_topic_0108272831_ul193603764111"></a><a name="zh-cn_topic_0115187940_zh-cn_topic_0108272831_ul193603764111"></a><ul id="zh-cn_topic_0115187940_zh-cn_topic_0108272831_ul193603764111"><li>NONE：不解密，直接导出文件。</li><li>AES-256-GCM：使用AES-256-GCM（NoPadding）算法解密后再导出文件。</li></ul>
</div>
</td>
</tr>
<tr id="zh-cn_topic_0115187940_row163413714362"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0115187940_p167122217132"><a name="zh-cn_topic_0115187940_p167122217132"></a><a name="zh-cn_topic_0115187940_p167122217132"></a>fromJobConfig.dek</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0115187940_p74741127142115"><a name="zh-cn_topic_0115187940_p74741127142115"></a><a name="zh-cn_topic_0115187940_p74741127142115"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0115187940_p2474627102111"><a name="zh-cn_topic_0115187940_p2474627102111"></a><a name="zh-cn_topic_0115187940_p2474627102111"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0115187940_p23281415172211"><a name="zh-cn_topic_0115187940_p23281415172211"></a><a name="zh-cn_topic_0115187940_p23281415172211"></a>数据解密密钥，密钥由长度64的十六进制数组成，且必须与加密时配置的<span class="parmname" id="zh-cn_topic_0115187940_zh-cn_topic_0108272831_parmname1660363014167"><a name="zh-cn_topic_0115187940_zh-cn_topic_0108272831_parmname1660363014167"></a><a name="zh-cn_topic_0115187940_zh-cn_topic_0108272831_parmname1660363014167"></a>“toJobConfig.dek”</span>（导入时配置的数据加密密钥）一致。如果不一致系统不会报异常，只是解密出来的数据会错误。</p>
</td>
</tr>
<tr id="zh-cn_topic_0115187940_row259514378360"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0115187940_p26851918151311"><a name="zh-cn_topic_0115187940_p26851918151311"></a><a name="zh-cn_topic_0115187940_p26851918151311"></a>fromJobConfig.iv</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0115187940_p1114152632113"><a name="zh-cn_topic_0115187940_p1114152632113"></a><a name="zh-cn_topic_0115187940_p1114152632113"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0115187940_p1414162617212"><a name="zh-cn_topic_0115187940_p1414162617212"></a><a name="zh-cn_topic_0115187940_p1414162617212"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0115187940_p24771354512"><a name="zh-cn_topic_0115187940_p24771354512"></a><a name="zh-cn_topic_0115187940_p24771354512"></a>解密需要的初始化向量，初始化向量由长度32的十六进制数组成，且必须与加密时配置的<span class="parmname" id="zh-cn_topic_0115187940_zh-cn_topic_0108272831_parmname1257711377164"><a name="zh-cn_topic_0115187940_zh-cn_topic_0108272831_parmname1257711377164"></a><a name="zh-cn_topic_0115187940_zh-cn_topic_0108272831_parmname1257711377164"></a>“toJobConfig.iv”</span>（导入时配置的初始化向量）一致。如果不一致系统不会报异常，只是解密出来的数据会错误。</p>
</td>
</tr>
<tr id="zh-cn_topic_0115187940_row83947524118"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0115187940_p1724715172115"><a name="zh-cn_topic_0115187940_p1724715172115"></a><a name="zh-cn_topic_0115187940_p1724715172115"></a>fromJobConfig.md5FileSuffix</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0115187940_p32471517121116"><a name="zh-cn_topic_0115187940_p32471517121116"></a><a name="zh-cn_topic_0115187940_p32471517121116"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.419999999999998%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0115187940_p1424720170114"><a name="zh-cn_topic_0115187940_p1424720170114"></a><a name="zh-cn_topic_0115187940_p1424720170114"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.14%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0115187940_p72470172110"><a name="zh-cn_topic_0115187940_p72470172110"></a><a name="zh-cn_topic_0115187940_p72470172110"></a>校验CDM抽取的文件，是否与源文件一致。</p>
</td>
</tr>
</tbody>
</table>

