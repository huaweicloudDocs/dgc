# 源端为HBase/CloudTable<a name="dgc_02_0286"></a>

## JSON样例<a name="zh-cn_topic_0108272812_section33401108172339"></a>

```
"from-config-values": {
        "configs": [
          {
            "inputs": [
              {
                "name": "fromJobConfig.table",
                "value": "rf_from"
              },
              {
                "name": "fromJobConfig.columnFamily",
                "value": "rowkey&f"
              },
              {
                "name": "fromJobConfig.columns",
                "value": "rowkey:rowkey&f:_small"
              },
              {
                "name": "fromJobConfig.formats",
                "value": {
                  "f:_date": "yyyy-MM-dd",
                  "f:_timestamp": "yyyy-MM-dd HH:mm:ss"
                }
              }
            ],
            "name": "fromJobConfig"
          }
        ]
      }
```

## 参数说明<a name="zh-cn_topic_0108272812_section25503323174151"></a>

-   HBase/CloudTable作业参数说明

    <a name="zh-cn_topic_0108272812_table31064216174444"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0108272812_row24452861174444"><th class="cellrowborder" valign="top" width="19.650000000000002%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272812_p34524738174444"><a name="zh-cn_topic_0108272812_p34524738174444"></a><a name="zh-cn_topic_0108272812_p34524738174444"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.59%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272812_p45040379174444"><a name="zh-cn_topic_0108272812_p45040379174444"></a><a name="zh-cn_topic_0108272812_p45040379174444"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="16.11%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272812_p24392081174444"><a name="zh-cn_topic_0108272812_p24392081174444"></a><a name="zh-cn_topic_0108272812_p24392081174444"></a>类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="44.65%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272812_p29601515174444"><a name="zh-cn_topic_0108272812_p29601515174444"></a><a name="zh-cn_topic_0108272812_p29601515174444"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0108272812_row48912497174444"><td class="cellrowborder" valign="top" width="19.650000000000002%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272812_p2489357174444"><a name="zh-cn_topic_0108272812_p2489357174444"></a><a name="zh-cn_topic_0108272812_p2489357174444"></a>fromJobConfig.table</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.59%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272812_p311332174444"><a name="zh-cn_topic_0108272812_p311332174444"></a><a name="zh-cn_topic_0108272812_p311332174444"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.11%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272812_p25217952174444"><a name="zh-cn_topic_0108272812_p25217952174444"></a><a name="zh-cn_topic_0108272812_p25217952174444"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.65%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272812_p29388265174444"><a name="zh-cn_topic_0108272812_p29388265174444"></a><a name="zh-cn_topic_0108272812_p29388265174444"></a>需要抽取数据的表名，例如<span class="parmvalue" id="zh-cn_topic_0108272812_parmvalue63167798174444"><a name="zh-cn_topic_0108272812_parmvalue63167798174444"></a><a name="zh-cn_topic_0108272812_parmvalue63167798174444"></a>“cdm”</span>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272812_row7956167153414"><td class="cellrowborder" valign="top" width="19.650000000000002%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272812_p1386111216271"><a name="zh-cn_topic_0108272812_p1386111216271"></a><a name="zh-cn_topic_0108272812_p1386111216271"></a>fromJobConfig.columnFamilies</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.59%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272812_p2750481264"><a name="zh-cn_topic_0108272812_p2750481264"></a><a name="zh-cn_topic_0108272812_p2750481264"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.11%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272812_p7643141317276"><a name="zh-cn_topic_0108272812_p7643141317276"></a><a name="zh-cn_topic_0108272812_p7643141317276"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.65%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272812_p187501987269"><a name="zh-cn_topic_0108272812_p187501987269"></a><a name="zh-cn_topic_0108272812_p187501987269"></a>抽取数据所属的列族。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272812_row31639270174444"><td class="cellrowborder" valign="top" width="19.650000000000002%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272812_p12644096174444"><a name="zh-cn_topic_0108272812_p12644096174444"></a><a name="zh-cn_topic_0108272812_p12644096174444"></a>fromJobConfig.columns</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.59%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272812_p17538846174444"><a name="zh-cn_topic_0108272812_p17538846174444"></a><a name="zh-cn_topic_0108272812_p17538846174444"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.11%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272812_p11360425174444"><a name="zh-cn_topic_0108272812_p11360425174444"></a><a name="zh-cn_topic_0108272812_p11360425174444"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.65%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272812_p47779208174444"><a name="zh-cn_topic_0108272812_p47779208174444"></a><a name="zh-cn_topic_0108272812_p47779208174444"></a>需要抽取的列，列号之间使用<span class="parmvalue" id="zh-cn_topic_0108272812_parmvalue27359691174444"><a name="zh-cn_topic_0108272812_parmvalue27359691174444"></a><a name="zh-cn_topic_0108272812_parmvalue27359691174444"></a>“&amp;”</span>分割，列族与列之间用<span class="parmvalue" id="zh-cn_topic_0108272812_parmvalue44910628174444"><a name="zh-cn_topic_0108272812_parmvalue44910628174444"></a><a name="zh-cn_topic_0108272812_parmvalue44910628174444"></a>“:”</span>分隔，例如：<span class="parmvalue" id="zh-cn_topic_0108272812_parmvalue1542468174444"><a name="zh-cn_topic_0108272812_parmvalue1542468174444"></a><a name="zh-cn_topic_0108272812_parmvalue1542468174444"></a>“cf1:c1&amp;cf2:c2”</span>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272812_row4793145333813"><td class="cellrowborder" valign="top" width="19.650000000000002%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272812_p1879355313811"><a name="zh-cn_topic_0108272812_p1879355313811"></a><a name="zh-cn_topic_0108272812_p1879355313811"></a>fromJobConfig.isSplit</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.59%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272812_p1793175333815"><a name="zh-cn_topic_0108272812_p1793175333815"></a><a name="zh-cn_topic_0108272812_p1793175333815"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.11%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272812_p679319530388"><a name="zh-cn_topic_0108272812_p679319530388"></a><a name="zh-cn_topic_0108272812_p679319530388"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.65%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272812_p1079315533383"><a name="zh-cn_topic_0108272812_p1079315533383"></a><a name="zh-cn_topic_0108272812_p1079315533383"></a>选择是否拆分Rowkey，例如<span class="parmvalue" id="zh-cn_topic_0108272812_parmvalue7663131084214"><a name="zh-cn_topic_0108272812_parmvalue7663131084214"></a><a name="zh-cn_topic_0108272812_parmvalue7663131084214"></a>“true”</span>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272812_row8754755153813"><td class="cellrowborder" valign="top" width="19.650000000000002%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272812_p77541255143819"><a name="zh-cn_topic_0108272812_p77541255143819"></a><a name="zh-cn_topic_0108272812_p77541255143819"></a>fromJobConfig.delimiter</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.59%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272812_p47541455153817"><a name="zh-cn_topic_0108272812_p47541455153817"></a><a name="zh-cn_topic_0108272812_p47541455153817"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.11%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272812_p075425573816"><a name="zh-cn_topic_0108272812_p075425573816"></a><a name="zh-cn_topic_0108272812_p075425573816"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.65%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272812_p27548554387"><a name="zh-cn_topic_0108272812_p27548554387"></a><a name="zh-cn_topic_0108272812_p27548554387"></a>用于切分Rowkey的分隔符，若不设置则不切分，例如<span class="parmvalue" id="zh-cn_topic_0108272812_parmvalue3496185420425"><a name="zh-cn_topic_0108272812_parmvalue3496185420425"></a><a name="zh-cn_topic_0108272812_parmvalue3496185420425"></a>“|”</span>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272812_row1942619268358"><td class="cellrowborder" valign="top" width="19.650000000000002%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272812_p134261268354"><a name="zh-cn_topic_0108272812_p134261268354"></a><a name="zh-cn_topic_0108272812_p134261268354"></a>fromJobConfig.startTime</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.59%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272812_p1217094913387"><a name="zh-cn_topic_0108272812_p1217094913387"></a><a name="zh-cn_topic_0108272812_p1217094913387"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.11%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272812_p1917064953811"><a name="zh-cn_topic_0108272812_p1917064953811"></a><a name="zh-cn_topic_0108272812_p1917064953811"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.65%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272812_p091005834018"><a name="zh-cn_topic_0108272812_p091005834018"></a><a name="zh-cn_topic_0108272812_p091005834018"></a>时间区间左边界（包含该值），格式为<span class="uicontrol" id="zh-cn_topic_0108272812_uicontrol1791019582400"><a name="zh-cn_topic_0108272812_uicontrol1791019582400"></a><a name="zh-cn_topic_0108272812_uicontrol1791019582400"></a>“yyyy-MM-dd hh:mm:ss”</span>。</p>
    <p id="zh-cn_topic_0108272812_p367020385522"><a name="zh-cn_topic_0108272812_p367020385522"></a><a name="zh-cn_topic_0108272812_p367020385522"></a>表示只抽取该时间及以后的数据。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272812_row15145143083511"><td class="cellrowborder" valign="top" width="19.650000000000002%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272812_p201451830173516"><a name="zh-cn_topic_0108272812_p201451830173516"></a><a name="zh-cn_topic_0108272812_p201451830173516"></a>fromJobConfig.endTime</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.59%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272812_p14170125153817"><a name="zh-cn_topic_0108272812_p14170125153817"></a><a name="zh-cn_topic_0108272812_p14170125153817"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.11%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272812_p11170175113383"><a name="zh-cn_topic_0108272812_p11170175113383"></a><a name="zh-cn_topic_0108272812_p11170175113383"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.65%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272812_p2700041145210"><a name="zh-cn_topic_0108272812_p2700041145210"></a><a name="zh-cn_topic_0108272812_p2700041145210"></a>时间区间右边界（不包含该值），格式为<span class="uicontrol" id="zh-cn_topic_0108272812_uicontrol922161113549"><a name="zh-cn_topic_0108272812_uicontrol922161113549"></a><a name="zh-cn_topic_0108272812_uicontrol922161113549"></a>“yyyy-MM-dd hh:mm:ss”</span>。</p>
    <p id="zh-cn_topic_0108272812_p377123219419"><a name="zh-cn_topic_0108272812_p377123219419"></a><a name="zh-cn_topic_0108272812_p377123219419"></a>表示只抽取该时间以前的数据。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272812_row6411101514504"><td class="cellrowborder" valign="top" width="19.650000000000002%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272812_p32277056174737"><a name="zh-cn_topic_0108272812_p32277056174737"></a><a name="zh-cn_topic_0108272812_p32277056174737"></a>fromJobConfig.formats</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.59%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272812_p64304758174737"><a name="zh-cn_topic_0108272812_p64304758174737"></a><a name="zh-cn_topic_0108272812_p64304758174737"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.11%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272812_p41302916174737"><a name="zh-cn_topic_0108272812_p41302916174737"></a><a name="zh-cn_topic_0108272812_p41302916174737"></a>数据结构</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.65%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272812_p57201939174737"><a name="zh-cn_topic_0108272812_p57201939174737"></a><a name="zh-cn_topic_0108272812_p57201939174737"></a>时间格式，请参见<a href="#zh-cn_topic_0108272812_li45055411174737">fromJobConfig.formats参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="zh-cn_topic_0108272812_li45055411174737"></a>fromJobConfig.formats参数说明

    <a name="zh-cn_topic_0108272812_table37875375203058"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0108272812_row57939309203058"><th class="cellrowborder" valign="top" width="20.987901209879013%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272812_p62572456203058"><a name="zh-cn_topic_0108272812_p62572456203058"></a><a name="zh-cn_topic_0108272812_p62572456203058"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.567843215678433%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272812_p35204151203058"><a name="zh-cn_topic_0108272812_p35204151203058"></a><a name="zh-cn_topic_0108272812_p35204151203058"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.25827417258274%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272812_p32963971203058"><a name="zh-cn_topic_0108272812_p32963971203058"></a><a name="zh-cn_topic_0108272812_p32963971203058"></a>类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="40.18598140185981%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272812_p52835955203058"><a name="zh-cn_topic_0108272812_p52835955203058"></a><a name="zh-cn_topic_0108272812_p52835955203058"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0108272812_row51853935203058"><td class="cellrowborder" valign="top" width="20.987901209879013%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272812_p39419232203058"><a name="zh-cn_topic_0108272812_p39419232203058"></a><a name="zh-cn_topic_0108272812_p39419232203058"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.567843215678433%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272812_p38841262203058"><a name="zh-cn_topic_0108272812_p38841262203058"></a><a name="zh-cn_topic_0108272812_p38841262203058"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.25827417258274%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272812_p59134528203058"><a name="zh-cn_topic_0108272812_p59134528203058"></a><a name="zh-cn_topic_0108272812_p59134528203058"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.18598140185981%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272812_p25167487203058"><a name="zh-cn_topic_0108272812_p25167487203058"></a><a name="zh-cn_topic_0108272812_p25167487203058"></a>列号，例如：<span class="parmvalue" id="zh-cn_topic_0108272812_parmvalue25180794203058"><a name="zh-cn_topic_0108272812_parmvalue25180794203058"></a><a name="zh-cn_topic_0108272812_parmvalue25180794203058"></a>“1”</span>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272812_row25300562203058"><td class="cellrowborder" valign="top" width="20.987901209879013%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272812_p36079650203058"><a name="zh-cn_topic_0108272812_p36079650203058"></a><a name="zh-cn_topic_0108272812_p36079650203058"></a>value</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.567843215678433%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272812_p36770518203058"><a name="zh-cn_topic_0108272812_p36770518203058"></a><a name="zh-cn_topic_0108272812_p36770518203058"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.25827417258274%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272812_p25621975203058"><a name="zh-cn_topic_0108272812_p25621975203058"></a><a name="zh-cn_topic_0108272812_p25621975203058"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.18598140185981%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272812_p62114060203058"><a name="zh-cn_topic_0108272812_p62114060203058"></a><a name="zh-cn_topic_0108272812_p62114060203058"></a>时间格式，例如：<span class="parmvalue" id="zh-cn_topic_0108272812_parmvalue22155629203058"><a name="zh-cn_topic_0108272812_parmvalue22155629203058"></a><a name="zh-cn_topic_0108272812_parmvalue22155629203058"></a>“yyyy-MM-dd”</span>。</p>
    </td>
    </tr>
    </tbody>
    </table>


