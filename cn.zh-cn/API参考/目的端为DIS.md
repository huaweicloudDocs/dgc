# 目的端为DIS<a name="dgc_02_0306"></a>

## JSON样例<a name="zh-cn_topic_0129101185_section33401108172339"></a>

```
"to-config-values": {
        "configs": [
          {
            "inputs": [
              {
                "name": "toJobConfig.streamName",
                "value": "cdm"
              },
              {
                "name": "toJobConfig.separator",
                "value": ","
              },
              {
                "name": "toJobConfig.identifierEnclose",
                "value": "'"
              }
            ],
            "name": "toJobConfig"
          }
        ]
      }
```

## 参数说明<a name="zh-cn_topic_0129101185_section28186120174818"></a>

<a name="zh-cn_topic_0129101185_table13922888141527"></a>
<table><thead align="left"><tr id="zh-cn_topic_0129101185_row229143141527"><th class="cellrowborder" valign="top" width="22.66%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0129101185_p66756185141527"><a name="zh-cn_topic_0129101185_p66756185141527"></a><a name="zh-cn_topic_0129101185_p66756185141527"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="19.78%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0129101185_p38541938141527"><a name="zh-cn_topic_0129101185_p38541938141527"></a><a name="zh-cn_topic_0129101185_p38541938141527"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.05%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0129101185_p34889279141527"><a name="zh-cn_topic_0129101185_p34889279141527"></a><a name="zh-cn_topic_0129101185_p34889279141527"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="40.510000000000005%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0129101185_p7459369141527"><a name="zh-cn_topic_0129101185_p7459369141527"></a><a name="zh-cn_topic_0129101185_p7459369141527"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0129101185_row62628929141527"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0129101185_p18560626141527"><a name="zh-cn_topic_0129101185_p18560626141527"></a><a name="zh-cn_topic_0129101185_p18560626141527"></a>toJobConfig.streamName</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0129101185_p27015713141527"><a name="zh-cn_topic_0129101185_p27015713141527"></a><a name="zh-cn_topic_0129101185_p27015713141527"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0129101185_p50167516142856"><a name="zh-cn_topic_0129101185_p50167516142856"></a><a name="zh-cn_topic_0129101185_p50167516142856"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0129101185_p32605071143018"><a name="zh-cn_topic_0129101185_p32605071143018"></a><a name="zh-cn_topic_0129101185_p32605071143018"></a>DIS的通道名。</p>
</td>
</tr>
<tr id="zh-cn_topic_0129101185_row4268185173352"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0129101185_p177595045715"><a name="zh-cn_topic_0129101185_p177595045715"></a><a name="zh-cn_topic_0129101185_p177595045715"></a>toJobConfig.separator</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0129101185_p19169610173352"><a name="zh-cn_topic_0129101185_p19169610173352"></a><a name="zh-cn_topic_0129101185_p19169610173352"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0129101185_p9234573173352"><a name="zh-cn_topic_0129101185_p9234573173352"></a><a name="zh-cn_topic_0129101185_p9234573173352"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0129101185_p9802957173352"><a name="zh-cn_topic_0129101185_p9802957173352"></a><a name="zh-cn_topic_0129101185_p9802957173352"></a>字段分隔符，默认为空格。</p>
</td>
</tr>
<tr id="zh-cn_topic_0129101185_row8201182620484"><td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0129101185_p2020117268481"><a name="zh-cn_topic_0129101185_p2020117268481"></a><a name="zh-cn_topic_0129101185_p2020117268481"></a>toJobConfig.identifierEnclose</p>
</td>
<td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0129101185_p13201126194815"><a name="zh-cn_topic_0129101185_p13201126194815"></a><a name="zh-cn_topic_0129101185_p13201126194815"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.05%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0129101185_p1420162613485"><a name="zh-cn_topic_0129101185_p1420162613485"></a><a name="zh-cn_topic_0129101185_p1420162613485"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.510000000000005%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0129101185_p32011926114812"><a name="zh-cn_topic_0129101185_p32011926114812"></a><a name="zh-cn_topic_0129101185_p32011926114812"></a>连接引用表名或列名时的分隔符号，默认为空。</p>
</td>
</tr>
</tbody>
</table>

