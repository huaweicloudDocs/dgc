# 批量数据迁移API错误码<a name="dgc_02_0311"></a>

调用API出错后，将不会返回结果数据。调用方可根据每个API对应的错误码来定位错误原因。当调用出错时，HTTP请求返回一个4xx或5xx的HTTP状态码。返回的消息体中是具体的错误代码及错误信息。在调用方找不到错误原因时，可以联系客服，并提供错误码，以便尽快帮您解决问题。

-   异常响应样例

    ```
    {
      "errCode": "Cdm.0100",
      "externalMessage": "Job[jdbc2hive] doesn't exist."
    }
    ```

-   参数说明

    <a name="zh-cn_topic_0108272830_table20859163144534"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0108272830_row14559227144534"><th class="cellrowborder" valign="top" width="25.979999999999997%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0108272830_p42006478144534"><a name="zh-cn_topic_0108272830_p42006478144534"></a><a name="zh-cn_topic_0108272830_p42006478144534"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="24.63%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0108272830_p47081585144534"><a name="zh-cn_topic_0108272830_p47081585144534"></a><a name="zh-cn_topic_0108272830_p47081585144534"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.21%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0108272830_p55512020144534"><a name="zh-cn_topic_0108272830_p55512020144534"></a><a name="zh-cn_topic_0108272830_p55512020144534"></a>类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="27.18%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0108272830_p179743144534"><a name="zh-cn_topic_0108272830_p179743144534"></a><a name="zh-cn_topic_0108272830_p179743144534"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0108272830_row58467510144534"><td class="cellrowborder" valign="top" width="25.979999999999997%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272830_p38446735144534"><a name="zh-cn_topic_0108272830_p38446735144534"></a><a name="zh-cn_topic_0108272830_p38446735144534"></a>errCode</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.63%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272830_p27177860144534"><a name="zh-cn_topic_0108272830_p27177860144534"></a><a name="zh-cn_topic_0108272830_p27177860144534"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.21%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272830_p53923074144534"><a name="zh-cn_topic_0108272830_p53923074144534"></a><a name="zh-cn_topic_0108272830_p53923074144534"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.18%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272830_p5692848144534"><a name="zh-cn_topic_0108272830_p5692848144534"></a><a name="zh-cn_topic_0108272830_p5692848144534"></a>错误码。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row62810842144534"><td class="cellrowborder" valign="top" width="25.979999999999997%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0108272830_p38247869144534"><a name="zh-cn_topic_0108272830_p38247869144534"></a><a name="zh-cn_topic_0108272830_p38247869144534"></a>externalMessage</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.63%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0108272830_p32518227144534"><a name="zh-cn_topic_0108272830_p32518227144534"></a><a name="zh-cn_topic_0108272830_p32518227144534"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.21%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0108272830_p16358629144534"><a name="zh-cn_topic_0108272830_p16358629144534"></a><a name="zh-cn_topic_0108272830_p16358629144534"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.18%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0108272830_p47171694144534"><a name="zh-cn_topic_0108272830_p47171694144534"></a><a name="zh-cn_topic_0108272830_p47171694144534"></a>错误消息。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   错误码说明

    以下错误信息中的_%s_为变量，实际返回信息时会替换为具体的参数名、表名、作业名、连接名等。

    当您调用API时，如果遇到“APIGW”开头的错误码，请参见[API网关错误码](https://support.huaweicloud.com/devg-apisign/api-sign-errorcode.html)进行处理。

    <a name="zh-cn_topic_0108272830_table2697114214287"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0108272830_row202561544172811"><th class="cellrowborder" valign="top" width="15.96159615961596%" id="mcps1.1.6.1.1"><p id="zh-cn_topic_0108272830_p17256344132818"><a name="zh-cn_topic_0108272830_p17256344132818"></a><a name="zh-cn_topic_0108272830_p17256344132818"></a>错误码</p>
    </th>
    <th class="cellrowborder" valign="top" width="9.8009800980098%" id="mcps1.1.6.1.2"><p id="zh-cn_topic_0108272830_p16256114432811"><a name="zh-cn_topic_0108272830_p16256114432811"></a><a name="zh-cn_topic_0108272830_p16256114432811"></a>状态码</p>
    </th>
    <th class="cellrowborder" valign="top" width="20.72207220722072%" id="mcps1.1.6.1.3"><p id="zh-cn_topic_0108272830_p18256134452815"><a name="zh-cn_topic_0108272830_p18256134452815"></a><a name="zh-cn_topic_0108272830_p18256134452815"></a>错误信息</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.962596259625965%" id="mcps1.1.6.1.4"><p id="zh-cn_topic_0108272830_p425634422812"><a name="zh-cn_topic_0108272830_p425634422812"></a><a name="zh-cn_topic_0108272830_p425634422812"></a>描述</p>
    </th>
    <th class="cellrowborder" valign="top" width="27.552755275527556%" id="mcps1.1.6.1.5"><p id="zh-cn_topic_0108272830_p1825674412283"><a name="zh-cn_topic_0108272830_p1825674412283"></a><a name="zh-cn_topic_0108272830_p1825674412283"></a>处理措施</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0108272830_row3256544202816"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p14256184422812"><a name="zh-cn_topic_0108272830_p14256184422812"></a><a name="zh-cn_topic_0108272830_p14256184422812"></a>Cdm.0000</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p16256124410284"><a name="zh-cn_topic_0108272830_p16256124410284"></a><a name="zh-cn_topic_0108272830_p16256124410284"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p102569440282"><a name="zh-cn_topic_0108272830_p102569440282"></a><a name="zh-cn_topic_0108272830_p102569440282"></a>系统错误。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p8256104419287"><a name="zh-cn_topic_0108272830_p8256104419287"></a><a name="zh-cn_topic_0108272830_p8256104419287"></a>系统错误。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p8256164422812"><a name="zh-cn_topic_0108272830_p8256164422812"></a><a name="zh-cn_topic_0108272830_p8256164422812"></a>请联系<span id="zh-cn_topic_0108272830_text12963171833813"><a name="zh-cn_topic_0108272830_text12963171833813"></a><a name="zh-cn_topic_0108272830_text12963171833813"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row136471049204910"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p164713498496"><a name="zh-cn_topic_0108272830_p164713498496"></a><a name="zh-cn_topic_0108272830_p164713498496"></a>Cdm.0001</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p156477492497"><a name="zh-cn_topic_0108272830_p156477492497"></a><a name="zh-cn_topic_0108272830_p156477492497"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p16476491499"><a name="zh-cn_topic_0108272830_p16476491499"></a><a name="zh-cn_topic_0108272830_p16476491499"></a>资源不存在或不合法。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p1664713495493"><a name="zh-cn_topic_0108272830_p1664713495493"></a><a name="zh-cn_topic_0108272830_p1664713495493"></a>请求的资源不存在或无访问权限。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p11648154924918"><a name="zh-cn_topic_0108272830_p11648154924918"></a><a name="zh-cn_topic_0108272830_p11648154924918"></a>请联系<span id="zh-cn_topic_0108272830_text127551597379"><a name="zh-cn_topic_0108272830_text127551597379"></a><a name="zh-cn_topic_0108272830_text127551597379"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row5256544102814"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p17256144432819"><a name="zh-cn_topic_0108272830_p17256144432819"></a><a name="zh-cn_topic_0108272830_p17256144432819"></a>Cdm.0009</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p12565442283"><a name="zh-cn_topic_0108272830_p12565442283"></a><a name="zh-cn_topic_0108272830_p12565442283"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p16256124412283"><a name="zh-cn_topic_0108272830_p16256124412283"></a><a name="zh-cn_topic_0108272830_p16256124412283"></a><em id="zh-cn_topic_0108272830_i625644442814"><a name="zh-cn_topic_0108272830_i625644442814"></a><a name="zh-cn_topic_0108272830_i625644442814"></a>%s</em>不是整型数字或超出整型数的取值范围[0～2147483647]。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p112567443280"><a name="zh-cn_topic_0108272830_p112567443280"></a><a name="zh-cn_topic_0108272830_p112567443280"></a>输入参数不是整型数字或超出整型数的取值范围。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p72566442282"><a name="zh-cn_topic_0108272830_p72566442282"></a><a name="zh-cn_topic_0108272830_p72566442282"></a>请根据错误提示将参数修改正确后请重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row2256244132812"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p42561344152815"><a name="zh-cn_topic_0108272830_p42561344152815"></a><a name="zh-cn_topic_0108272830_p42561344152815"></a>Cdm.0010</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p625711445289"><a name="zh-cn_topic_0108272830_p625711445289"></a><a name="zh-cn_topic_0108272830_p625711445289"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p82577446280"><a name="zh-cn_topic_0108272830_p82577446280"></a><a name="zh-cn_topic_0108272830_p82577446280"></a>整数必须在区间[<em id="zh-cn_topic_0108272830_i5257344102814"><a name="zh-cn_topic_0108272830_i5257344102814"></a><a name="zh-cn_topic_0108272830_i5257344102814"></a>%s</em>]。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p6257174420286"><a name="zh-cn_topic_0108272830_p6257174420286"></a><a name="zh-cn_topic_0108272830_p6257174420286"></a>校验程序的参数缺失或长度为0。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p9257134413282"><a name="zh-cn_topic_0108272830_p9257134413282"></a><a name="zh-cn_topic_0108272830_p9257134413282"></a>请根据错误提示将参数修改正确后请重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row925718442284"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p13257114413280"><a name="zh-cn_topic_0108272830_p13257114413280"></a><a name="zh-cn_topic_0108272830_p13257114413280"></a>Cdm.0011</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p17257444172816"><a name="zh-cn_topic_0108272830_p17257444172816"></a><a name="zh-cn_topic_0108272830_p17257444172816"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p225712440287"><a name="zh-cn_topic_0108272830_p225712440287"></a><a name="zh-cn_topic_0108272830_p225712440287"></a>输入超过取值范围。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p102571244182817"><a name="zh-cn_topic_0108272830_p102571244182817"></a><a name="zh-cn_topic_0108272830_p102571244182817"></a>参数格式不正确或超过取值范围，无法解析。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p8257114419288"><a name="zh-cn_topic_0108272830_p8257114419288"></a><a name="zh-cn_topic_0108272830_p8257114419288"></a>请根据返回的详细错误信息，确认参数值是否合法，修改正确后请重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row10257194462815"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p172571544172818"><a name="zh-cn_topic_0108272830_p172571544172818"></a><a name="zh-cn_topic_0108272830_p172571544172818"></a>Cdm.0012</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p172571644142815"><a name="zh-cn_topic_0108272830_p172571644142815"></a><a name="zh-cn_topic_0108272830_p172571644142815"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p3257644142816"><a name="zh-cn_topic_0108272830_p3257644142816"></a><a name="zh-cn_topic_0108272830_p3257644142816"></a>没有匹配的数据库JDBC驱动。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p225710449289"><a name="zh-cn_topic_0108272830_p225710449289"></a><a name="zh-cn_topic_0108272830_p225710449289"></a>没有匹配的数据库JDBC驱动。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p142572441283"><a name="zh-cn_topic_0108272830_p142572441283"></a><a name="zh-cn_topic_0108272830_p142572441283"></a>请联系<span id="zh-cn_topic_0108272830_text1256950143810"><a name="zh-cn_topic_0108272830_text1256950143810"></a><a name="zh-cn_topic_0108272830_text1256950143810"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row152571144202818"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p16257744132810"><a name="zh-cn_topic_0108272830_p16257744132810"></a><a name="zh-cn_topic_0108272830_p16257744132810"></a>Cdm.0013</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p20257944112810"><a name="zh-cn_topic_0108272830_p20257944112810"></a><a name="zh-cn_topic_0108272830_p20257944112810"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p12257154432810"><a name="zh-cn_topic_0108272830_p12257154432810"></a><a name="zh-cn_topic_0108272830_p12257154432810"></a>Agent连接失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p42577447289"><a name="zh-cn_topic_0108272830_p42577447289"></a><a name="zh-cn_topic_0108272830_p42577447289"></a>Agent连接失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p52579444282"><a name="zh-cn_topic_0108272830_p52579444282"></a><a name="zh-cn_topic_0108272830_p52579444282"></a>可能是由于网络不通、安全组或防火墙规则未放行等原因。若排除上述原因后仍无法解决，请联系技术支持人员协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row15257144422815"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p9257144482818"><a name="zh-cn_topic_0108272830_p9257144482818"></a><a name="zh-cn_topic_0108272830_p9257144482818"></a>Cdm.0014</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p15257174419284"><a name="zh-cn_topic_0108272830_p15257174419284"></a><a name="zh-cn_topic_0108272830_p15257174419284"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p14257104442811"><a name="zh-cn_topic_0108272830_p14257104442811"></a><a name="zh-cn_topic_0108272830_p14257104442811"></a>非法参数。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p925794414282"><a name="zh-cn_topic_0108272830_p925794414282"></a><a name="zh-cn_topic_0108272830_p925794414282"></a>参数不合法。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p19257124418284"><a name="zh-cn_topic_0108272830_p19257124418284"></a><a name="zh-cn_topic_0108272830_p19257124418284"></a>请确认参数值是否合法，修改正确后请重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row112581244102814"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p9258114419281"><a name="zh-cn_topic_0108272830_p9258114419281"></a><a name="zh-cn_topic_0108272830_p9258114419281"></a>Cdm.0015</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p1625817447281"><a name="zh-cn_topic_0108272830_p1625817447281"></a><a name="zh-cn_topic_0108272830_p1625817447281"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p4258544152818"><a name="zh-cn_topic_0108272830_p4258544152818"></a><a name="zh-cn_topic_0108272830_p4258544152818"></a>解析文件内容出错。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p132581244192811"><a name="zh-cn_topic_0108272830_p132581244192811"></a><a name="zh-cn_topic_0108272830_p132581244192811"></a>解析文件内容失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p1625874432811"><a name="zh-cn_topic_0108272830_p1625874432811"></a><a name="zh-cn_topic_0108272830_p1625874432811"></a>请确认上传的文件内容或格式是否正确，修改正确后请重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row525813441289"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p72589446283"><a name="zh-cn_topic_0108272830_p72589446283"></a><a name="zh-cn_topic_0108272830_p72589446283"></a>Cdm.0016</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p525814412812"><a name="zh-cn_topic_0108272830_p525814412812"></a><a name="zh-cn_topic_0108272830_p525814412812"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p4258194410284"><a name="zh-cn_topic_0108272830_p4258194410284"></a><a name="zh-cn_topic_0108272830_p4258194410284"></a>上传文件不能为空。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p32581344162819"><a name="zh-cn_topic_0108272830_p32581344162819"></a><a name="zh-cn_topic_0108272830_p32581344162819"></a>上传的文件为空。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p1258134462818"><a name="zh-cn_topic_0108272830_p1258134462818"></a><a name="zh-cn_topic_0108272830_p1258134462818"></a>请确认上传的文件是否为空，修改正确后请重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row18258174411283"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p1625824419282"><a name="zh-cn_topic_0108272830_p1625824419282"></a><a name="zh-cn_topic_0108272830_p1625824419282"></a>Cdm.0017</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p42580442281"><a name="zh-cn_topic_0108272830_p42580442281"></a><a name="zh-cn_topic_0108272830_p42580442281"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p725854412815"><a name="zh-cn_topic_0108272830_p725854412815"></a><a name="zh-cn_topic_0108272830_p725854412815"></a>无法将输入值保存到存储库</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p10258144192817"><a name="zh-cn_topic_0108272830_p10258144192817"></a><a name="zh-cn_topic_0108272830_p10258144192817"></a>无法将输入值保存到存储库。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p7258184422815"><a name="zh-cn_topic_0108272830_p7258184422815"></a><a name="zh-cn_topic_0108272830_p7258184422815"></a>请联系<span id="zh-cn_topic_0108272830_text078915015385"><a name="zh-cn_topic_0108272830_text078915015385"></a><a name="zh-cn_topic_0108272830_text078915015385"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row82581744142820"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p125814452817"><a name="zh-cn_topic_0108272830_p125814452817"></a><a name="zh-cn_topic_0108272830_p125814452817"></a>Cdm.0018</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p1425884420286"><a name="zh-cn_topic_0108272830_p1425884420286"></a><a name="zh-cn_topic_0108272830_p1425884420286"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p12258144182820"><a name="zh-cn_topic_0108272830_p12258144182820"></a><a name="zh-cn_topic_0108272830_p12258144182820"></a>作业和连接内容不合法。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p13258164416288"><a name="zh-cn_topic_0108272830_p13258164416288"></a><a name="zh-cn_topic_0108272830_p13258164416288"></a>作业和连接内容非法。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p1259184410281"><a name="zh-cn_topic_0108272830_p1259184410281"></a><a name="zh-cn_topic_0108272830_p1259184410281"></a>请联系<span id="zh-cn_topic_0108272830_text196119384"><a name="zh-cn_topic_0108272830_text196119384"></a><a name="zh-cn_topic_0108272830_text196119384"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row925954492818"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p92591144152820"><a name="zh-cn_topic_0108272830_p92591144152820"></a><a name="zh-cn_topic_0108272830_p92591144152820"></a>Cdm.0019</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p13259644142813"><a name="zh-cn_topic_0108272830_p13259644142813"></a><a name="zh-cn_topic_0108272830_p13259644142813"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p92591444122812"><a name="zh-cn_topic_0108272830_p92591444122812"></a><a name="zh-cn_topic_0108272830_p92591444122812"></a>无法删除存储库中的链接</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p122595443287"><a name="zh-cn_topic_0108272830_p122595443287"></a><a name="zh-cn_topic_0108272830_p122595443287"></a>删除存储库中的链接失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p425964482815"><a name="zh-cn_topic_0108272830_p425964482815"></a><a name="zh-cn_topic_0108272830_p425964482815"></a>请稍后重试，或联系或<span id="zh-cn_topic_0108272830_text182394113386"><a name="zh-cn_topic_0108272830_text182394113386"></a><a name="zh-cn_topic_0108272830_text182394113386"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row9259114462814"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p8259164462812"><a name="zh-cn_topic_0108272830_p8259164462812"></a><a name="zh-cn_topic_0108272830_p8259164462812"></a>Cdm.0020</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p11259204411284"><a name="zh-cn_topic_0108272830_p11259204411284"></a><a name="zh-cn_topic_0108272830_p11259204411284"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p925994410288"><a name="zh-cn_topic_0108272830_p925994410288"></a><a name="zh-cn_topic_0108272830_p925994410288"></a>必须包含子字符串：<em id="zh-cn_topic_0108272830_i1825974452811"><a name="zh-cn_topic_0108272830_i1825974452811"></a><a name="zh-cn_topic_0108272830_i1825974452811"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p13259144102810"><a name="zh-cn_topic_0108272830_p13259144102810"></a><a name="zh-cn_topic_0108272830_p13259144102810"></a>被校验参数为空或不包含指定子字符串。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p1625994418285"><a name="zh-cn_topic_0108272830_p1625994418285"></a><a name="zh-cn_topic_0108272830_p1625994418285"></a>请根据错误提示将参数修改正确后，再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row12594440284"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p162594444285"><a name="zh-cn_topic_0108272830_p162594444285"></a><a name="zh-cn_topic_0108272830_p162594444285"></a>Cdm.0021</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p42590442289"><a name="zh-cn_topic_0108272830_p42590442289"></a><a name="zh-cn_topic_0108272830_p42590442289"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p22591344112817"><a name="zh-cn_topic_0108272830_p22591344112817"></a><a name="zh-cn_topic_0108272830_p22591344112817"></a>不能连接服务器：<em id="zh-cn_topic_0108272830_i14259184432816"><a name="zh-cn_topic_0108272830_i14259184432816"></a><a name="zh-cn_topic_0108272830_i14259184432816"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p825984442813"><a name="zh-cn_topic_0108272830_p825984442813"></a><a name="zh-cn_topic_0108272830_p825984442813"></a>连接服务器失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p192591644102818"><a name="zh-cn_topic_0108272830_p192591644102818"></a><a name="zh-cn_topic_0108272830_p192591644102818"></a>请联系<span id="zh-cn_topic_0108272830_text645712133811"><a name="zh-cn_topic_0108272830_text645712133811"></a><a name="zh-cn_topic_0108272830_text645712133811"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row0259444182810"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p132592044112818"><a name="zh-cn_topic_0108272830_p132592044112818"></a><a name="zh-cn_topic_0108272830_p132592044112818"></a>Cdm.0024</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p5259344132819"><a name="zh-cn_topic_0108272830_p5259344132819"></a><a name="zh-cn_topic_0108272830_p5259344132819"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p125984462812"><a name="zh-cn_topic_0108272830_p125984462812"></a><a name="zh-cn_topic_0108272830_p125984462812"></a>[<em id="zh-cn_topic_0108272830_i125911444287"><a name="zh-cn_topic_0108272830_i125911444287"></a><a name="zh-cn_topic_0108272830_i125911444287"></a>%s</em>]必须在区间[<em id="zh-cn_topic_0108272830_i825910442289"><a name="zh-cn_topic_0108272830_i825910442289"></a><a name="zh-cn_topic_0108272830_i825910442289"></a>%s</em>]。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p15259164417283"><a name="zh-cn_topic_0108272830_p15259164417283"></a><a name="zh-cn_topic_0108272830_p15259164417283"></a>被校验参数不在指定区间范围内。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p125910449284"><a name="zh-cn_topic_0108272830_p125910449284"></a><a name="zh-cn_topic_0108272830_p125910449284"></a>请根据错误提示将参数修改正确后，再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row122592448282"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p32591344112818"><a name="zh-cn_topic_0108272830_p32591344112818"></a><a name="zh-cn_topic_0108272830_p32591344112818"></a>Cdm.0037</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p9259144417281"><a name="zh-cn_topic_0108272830_p9259144417281"></a><a name="zh-cn_topic_0108272830_p9259144417281"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p926094417284"><a name="zh-cn_topic_0108272830_p926094417284"></a><a name="zh-cn_topic_0108272830_p926094417284"></a>无法提交作业。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p0260244192812"><a name="zh-cn_topic_0108272830_p0260244192812"></a><a name="zh-cn_topic_0108272830_p0260244192812"></a>无法提交作业。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p126044411287"><a name="zh-cn_topic_0108272830_p126044411287"></a><a name="zh-cn_topic_0108272830_p126044411287"></a>请联系<span id="zh-cn_topic_0108272830_text1967114113382"><a name="zh-cn_topic_0108272830_text1967114113382"></a><a name="zh-cn_topic_0108272830_text1967114113382"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row14260184419284"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p9260124412815"><a name="zh-cn_topic_0108272830_p9260124412815"></a><a name="zh-cn_topic_0108272830_p9260124412815"></a>Cdm.0051</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p926014412810"><a name="zh-cn_topic_0108272830_p926014412810"></a><a name="zh-cn_topic_0108272830_p926014412810"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p126014449288"><a name="zh-cn_topic_0108272830_p126014449288"></a><a name="zh-cn_topic_0108272830_p126014449288"></a>无效的提交引擎：<em id="zh-cn_topic_0108272830_i226044452815"><a name="zh-cn_topic_0108272830_i226044452815"></a><a name="zh-cn_topic_0108272830_i226044452815"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p7260114418285"><a name="zh-cn_topic_0108272830_p7260114418285"></a><a name="zh-cn_topic_0108272830_p7260114418285"></a>作业引擎名称非法。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p13260344142811"><a name="zh-cn_topic_0108272830_p13260344142811"></a><a name="zh-cn_topic_0108272830_p13260344142811"></a>请指定正确的作业引擎后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row0260944162814"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p52607448288"><a name="zh-cn_topic_0108272830_p52607448288"></a><a name="zh-cn_topic_0108272830_p52607448288"></a>Cdm.0052</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p5260144152810"><a name="zh-cn_topic_0108272830_p5260144152810"></a><a name="zh-cn_topic_0108272830_p5260144152810"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p6260244132810"><a name="zh-cn_topic_0108272830_p6260244132810"></a><a name="zh-cn_topic_0108272830_p6260244132810"></a>作业<em id="zh-cn_topic_0108272830_i17260174411284"><a name="zh-cn_topic_0108272830_i17260174411284"></a><a name="zh-cn_topic_0108272830_i17260174411284"></a>%s</em>正在运行。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p4260544122813"><a name="zh-cn_topic_0108272830_p4260544122813"></a><a name="zh-cn_topic_0108272830_p4260544122813"></a>作业正在运行。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p182601044132817"><a name="zh-cn_topic_0108272830_p182601044132817"></a><a name="zh-cn_topic_0108272830_p182601044132817"></a>作业正在运行，无法执行当前操作，请等待作业运行结束后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row1226034412286"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p112603443288"><a name="zh-cn_topic_0108272830_p112603443288"></a><a name="zh-cn_topic_0108272830_p112603443288"></a>Cdm.0053</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p1326094416288"><a name="zh-cn_topic_0108272830_p1326094416288"></a><a name="zh-cn_topic_0108272830_p1326094416288"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p82607445283"><a name="zh-cn_topic_0108272830_p82607445283"></a><a name="zh-cn_topic_0108272830_p82607445283"></a>作业<em id="zh-cn_topic_0108272830_i2260134417288"><a name="zh-cn_topic_0108272830_i2260134417288"></a><a name="zh-cn_topic_0108272830_i2260134417288"></a>%s</em>未运行。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p18260184472811"><a name="zh-cn_topic_0108272830_p18260184472811"></a><a name="zh-cn_topic_0108272830_p18260184472811"></a>作业未运行。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p626014412814"><a name="zh-cn_topic_0108272830_p626014412814"></a><a name="zh-cn_topic_0108272830_p626014412814"></a>请运行作业后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row17260944112818"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p226044415285"><a name="zh-cn_topic_0108272830_p226044415285"></a><a name="zh-cn_topic_0108272830_p226044415285"></a>Cdm.0054</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p17260544112814"><a name="zh-cn_topic_0108272830_p17260544112814"></a><a name="zh-cn_topic_0108272830_p17260544112814"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p19260194418287"><a name="zh-cn_topic_0108272830_p19260194418287"></a><a name="zh-cn_topic_0108272830_p19260194418287"></a>作业<em id="zh-cn_topic_0108272830_i12260194402814"><a name="zh-cn_topic_0108272830_i12260194402814"></a><a name="zh-cn_topic_0108272830_i12260194402814"></a>%s</em>不存在。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p13260134414283"><a name="zh-cn_topic_0108272830_p13260134414283"></a><a name="zh-cn_topic_0108272830_p13260134414283"></a>作业不存在。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p122601844112818"><a name="zh-cn_topic_0108272830_p122601844112818"></a><a name="zh-cn_topic_0108272830_p122601844112818"></a>请确认作业是否存在。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row10260184402812"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p1260194452810"><a name="zh-cn_topic_0108272830_p1260194452810"></a><a name="zh-cn_topic_0108272830_p1260194452810"></a>Cdm.0056</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p1626054422814"><a name="zh-cn_topic_0108272830_p1626054422814"></a><a name="zh-cn_topic_0108272830_p1626054422814"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p1260104416285"><a name="zh-cn_topic_0108272830_p1260104416285"></a><a name="zh-cn_topic_0108272830_p1260104416285"></a>不能提交作业。原因：<em id="zh-cn_topic_0108272830_i16261144412818"><a name="zh-cn_topic_0108272830_i16261144412818"></a><a name="zh-cn_topic_0108272830_i16261144412818"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p1326134412813"><a name="zh-cn_topic_0108272830_p1326134412813"></a><a name="zh-cn_topic_0108272830_p1326134412813"></a>作业提交失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p11261184452816"><a name="zh-cn_topic_0108272830_p11261184452816"></a><a name="zh-cn_topic_0108272830_p11261184452816"></a>请根据返回的详细错误信息，定位原因，修改正确后请重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row11261124413280"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p1426111441287"><a name="zh-cn_topic_0108272830_p1426111441287"></a><a name="zh-cn_topic_0108272830_p1426111441287"></a>Cdm.0057</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p122611244122810"><a name="zh-cn_topic_0108272830_p122611244122810"></a><a name="zh-cn_topic_0108272830_p122611244122810"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p15261844142815"><a name="zh-cn_topic_0108272830_p15261844142815"></a><a name="zh-cn_topic_0108272830_p15261844142815"></a>无效的作业执行引擎：<em id="zh-cn_topic_0108272830_i20261154417286"><a name="zh-cn_topic_0108272830_i20261154417286"></a><a name="zh-cn_topic_0108272830_i20261154417286"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p1326154482811"><a name="zh-cn_topic_0108272830_p1326154482811"></a><a name="zh-cn_topic_0108272830_p1326154482811"></a>作业引擎无效。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p02611344102820"><a name="zh-cn_topic_0108272830_p02611344102820"></a><a name="zh-cn_topic_0108272830_p02611344102820"></a>请指定正确的作业引擎后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row42611344162810"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p1261194415284"><a name="zh-cn_topic_0108272830_p1261194415284"></a><a name="zh-cn_topic_0108272830_p1261194415284"></a>Cdm.0058</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p132611944142814"><a name="zh-cn_topic_0108272830_p132611944142814"></a><a name="zh-cn_topic_0108272830_p132611944142814"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p22611344122817"><a name="zh-cn_topic_0108272830_p22611344122817"></a><a name="zh-cn_topic_0108272830_p22611344122817"></a>提交和执行引擎组合不合法。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p9261184420285"><a name="zh-cn_topic_0108272830_p9261184420285"></a><a name="zh-cn_topic_0108272830_p9261184420285"></a>提交和执行引擎组合不合法。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p1026174415282"><a name="zh-cn_topic_0108272830_p1026174415282"></a><a name="zh-cn_topic_0108272830_p1026174415282"></a>请指定正确的作业引擎后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row626144413283"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p826104432816"><a name="zh-cn_topic_0108272830_p826104432816"></a><a name="zh-cn_topic_0108272830_p826104432816"></a>Cdm.0059</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p1326116445288"><a name="zh-cn_topic_0108272830_p1326116445288"></a><a name="zh-cn_topic_0108272830_p1326116445288"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p226104472813"><a name="zh-cn_topic_0108272830_p226104472813"></a><a name="zh-cn_topic_0108272830_p226104472813"></a>作业<em id="zh-cn_topic_0108272830_i026119441283"><a name="zh-cn_topic_0108272830_i026119441283"></a><a name="zh-cn_topic_0108272830_i026119441283"></a>%s</em>已被禁用。不能提交作业。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p1726154416286"><a name="zh-cn_topic_0108272830_p1726154416286"></a><a name="zh-cn_topic_0108272830_p1726154416286"></a>作业已被禁用，无法提交。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p1526134418286"><a name="zh-cn_topic_0108272830_p1526134418286"></a><a name="zh-cn_topic_0108272830_p1526134418286"></a>当前作业无法提交，建议重新创建一个作业后再重试。或者，请联系<span id="zh-cn_topic_0108272830_text288311115380"><a name="zh-cn_topic_0108272830_text288311115380"></a><a name="zh-cn_topic_0108272830_text288311115380"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row1026154419285"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p18261144112818"><a name="zh-cn_topic_0108272830_p18261144112818"></a><a name="zh-cn_topic_0108272830_p18261144112818"></a>Cdm.0060</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p0261124419284"><a name="zh-cn_topic_0108272830_p0261124419284"></a><a name="zh-cn_topic_0108272830_p0261124419284"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p10262144462819"><a name="zh-cn_topic_0108272830_p10262144462819"></a><a name="zh-cn_topic_0108272830_p10262144462819"></a>作业使用的连接<em id="zh-cn_topic_0108272830_i626214442284"><a name="zh-cn_topic_0108272830_i626214442284"></a><a name="zh-cn_topic_0108272830_i626214442284"></a>%s</em>已被禁用。不能提交作业。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p226219448289"><a name="zh-cn_topic_0108272830_p226219448289"></a><a name="zh-cn_topic_0108272830_p226219448289"></a>作业使用的连接已被禁用。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p32626449287"><a name="zh-cn_topic_0108272830_p32626449287"></a><a name="zh-cn_topic_0108272830_p32626449287"></a>请改为其他连接后，再重新提交作业。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row926212449288"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p126254482813"><a name="zh-cn_topic_0108272830_p126254482813"></a><a name="zh-cn_topic_0108272830_p126254482813"></a>Cdm.0061</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p152621144122813"><a name="zh-cn_topic_0108272830_p152621144122813"></a><a name="zh-cn_topic_0108272830_p152621144122813"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p14262344132812"><a name="zh-cn_topic_0108272830_p14262344132812"></a><a name="zh-cn_topic_0108272830_p14262344132812"></a>连接器<em id="zh-cn_topic_0108272830_i10262174492810"><a name="zh-cn_topic_0108272830_i10262174492810"></a><a name="zh-cn_topic_0108272830_i10262174492810"></a>%s</em>不支持此方向。不能提交作业。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p22628441288"><a name="zh-cn_topic_0108272830_p22628441288"></a><a name="zh-cn_topic_0108272830_p22628441288"></a>该连接器不能作为作业的源端或目的端。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p92621944152813"><a name="zh-cn_topic_0108272830_p92621944152813"></a><a name="zh-cn_topic_0108272830_p92621944152813"></a>该连接器不能作为作业的源端或目的端，请改为其他连接后，再重新提交作业。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row172621144162815"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p102623443287"><a name="zh-cn_topic_0108272830_p102623443287"></a><a name="zh-cn_topic_0108272830_p102623443287"></a>Cdm.0062</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p926244432815"><a name="zh-cn_topic_0108272830_p926244432815"></a><a name="zh-cn_topic_0108272830_p926244432815"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p10262844102813"><a name="zh-cn_topic_0108272830_p10262844102813"></a><a name="zh-cn_topic_0108272830_p10262844102813"></a>二进制文件仅适合SFTP/FTP/HDFS/OBS连接器。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p82624448280"><a name="zh-cn_topic_0108272830_p82624448280"></a><a name="zh-cn_topic_0108272830_p82624448280"></a>连接器不在指定的范围内。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p6262104432818"><a name="zh-cn_topic_0108272830_p6262104432818"></a><a name="zh-cn_topic_0108272830_p6262104432818"></a>请指定正确的连接器后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row0262944142818"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p8262174452812"><a name="zh-cn_topic_0108272830_p8262174452812"></a><a name="zh-cn_topic_0108272830_p8262174452812"></a>Cdm.0063</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p7262174422819"><a name="zh-cn_topic_0108272830_p7262174422819"></a><a name="zh-cn_topic_0108272830_p7262174422819"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p12621443285"><a name="zh-cn_topic_0108272830_p12621443285"></a><a name="zh-cn_topic_0108272830_p12621443285"></a>创建表格错误。原因：<em id="zh-cn_topic_0108272830_i172622044202812"><a name="zh-cn_topic_0108272830_i172622044202812"></a><a name="zh-cn_topic_0108272830_i172622044202812"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p7262184410281"><a name="zh-cn_topic_0108272830_p7262184410281"></a><a name="zh-cn_topic_0108272830_p7262184410281"></a>创建表格失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p9262154432820"><a name="zh-cn_topic_0108272830_p9262154432820"></a><a name="zh-cn_topic_0108272830_p9262154432820"></a>请根据返回的详细错误信息定位原因，修改正确后请重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row326219442286"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p1726219448282"><a name="zh-cn_topic_0108272830_p1726219448282"></a><a name="zh-cn_topic_0108272830_p1726219448282"></a>Cdm.0064</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p22621844102816"><a name="zh-cn_topic_0108272830_p22621844102816"></a><a name="zh-cn_topic_0108272830_p22621844102816"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p172621744182810"><a name="zh-cn_topic_0108272830_p172621744182810"></a><a name="zh-cn_topic_0108272830_p172621744182810"></a>数据格式不匹配。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p12262644112811"><a name="zh-cn_topic_0108272830_p12262644112811"></a><a name="zh-cn_topic_0108272830_p12262644112811"></a>数据格式不匹配。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p72622445287"><a name="zh-cn_topic_0108272830_p72622445287"></a><a name="zh-cn_topic_0108272830_p72622445287"></a>请根据返回的详细错误信息，确认数据格式是否正确，修改正确后请重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row1326217447289"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p12626444284"><a name="zh-cn_topic_0108272830_p12626444284"></a><a name="zh-cn_topic_0108272830_p12626444284"></a>Cdm.0065</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p326264420282"><a name="zh-cn_topic_0108272830_p326264420282"></a><a name="zh-cn_topic_0108272830_p326264420282"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p10262154414289"><a name="zh-cn_topic_0108272830_p10262154414289"></a><a name="zh-cn_topic_0108272830_p10262154414289"></a>定时器启动失败，原因<em id="zh-cn_topic_0108272830_i1626217449283"><a name="zh-cn_topic_0108272830_i1626217449283"></a><a name="zh-cn_topic_0108272830_i1626217449283"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p1826214442815"><a name="zh-cn_topic_0108272830_p1826214442815"></a><a name="zh-cn_topic_0108272830_p1826214442815"></a>定时器启动失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p14263174413282"><a name="zh-cn_topic_0108272830_p14263174413282"></a><a name="zh-cn_topic_0108272830_p14263174413282"></a>请联系<span id="zh-cn_topic_0108272830_text210622133811"><a name="zh-cn_topic_0108272830_text210622133811"></a><a name="zh-cn_topic_0108272830_text210622133811"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row10263944192813"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p926314492812"><a name="zh-cn_topic_0108272830_p926314492812"></a><a name="zh-cn_topic_0108272830_p926314492812"></a>Cdm.0066</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p5263344112813"><a name="zh-cn_topic_0108272830_p5263344112813"></a><a name="zh-cn_topic_0108272830_p5263344112813"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p10263944122816"><a name="zh-cn_topic_0108272830_p10263944122816"></a><a name="zh-cn_topic_0108272830_p10263944122816"></a>获取样值失败，原因：<em id="zh-cn_topic_0108272830_i122631844142818"><a name="zh-cn_topic_0108272830_i122631844142818"></a><a name="zh-cn_topic_0108272830_i122631844142818"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p152631744152814"><a name="zh-cn_topic_0108272830_p152631744152814"></a><a name="zh-cn_topic_0108272830_p152631744152814"></a>获取样值失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p14263174410282"><a name="zh-cn_topic_0108272830_p14263174410282"></a><a name="zh-cn_topic_0108272830_p14263174410282"></a>请联系<span id="zh-cn_topic_0108272830_text203091724381"><a name="zh-cn_topic_0108272830_text203091724381"></a><a name="zh-cn_topic_0108272830_text203091724381"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row92631244142816"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p12263444132810"><a name="zh-cn_topic_0108272830_p12263444132810"></a><a name="zh-cn_topic_0108272830_p12263444132810"></a>Cdm.0067</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p2026334420287"><a name="zh-cn_topic_0108272830_p2026334420287"></a><a name="zh-cn_topic_0108272830_p2026334420287"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p18263154492818"><a name="zh-cn_topic_0108272830_p18263154492818"></a><a name="zh-cn_topic_0108272830_p18263154492818"></a>获取Schema失败，原因：<em id="zh-cn_topic_0108272830_i15263174418286"><a name="zh-cn_topic_0108272830_i15263174418286"></a><a name="zh-cn_topic_0108272830_i15263174418286"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p1263644192819"><a name="zh-cn_topic_0108272830_p1263644192819"></a><a name="zh-cn_topic_0108272830_p1263644192819"></a>获取Schema失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p626320448284"><a name="zh-cn_topic_0108272830_p626320448284"></a><a name="zh-cn_topic_0108272830_p626320448284"></a>请联系<span id="zh-cn_topic_0108272830_text75237216383"><a name="zh-cn_topic_0108272830_text75237216383"></a><a name="zh-cn_topic_0108272830_text75237216383"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row1426311449283"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p13263154452818"><a name="zh-cn_topic_0108272830_p13263154452818"></a><a name="zh-cn_topic_0108272830_p13263154452818"></a>Cdm.0085</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p1726319446281"><a name="zh-cn_topic_0108272830_p1726319446281"></a><a name="zh-cn_topic_0108272830_p1726319446281"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p1526344492814"><a name="zh-cn_topic_0108272830_p1526344492814"></a><a name="zh-cn_topic_0108272830_p1526344492814"></a>%s 超过最大值 %s。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p22631044172818"><a name="zh-cn_topic_0108272830_p22631044172818"></a><a name="zh-cn_topic_0108272830_p22631044172818"></a>参数超过最大值。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p1826324418287"><a name="zh-cn_topic_0108272830_p1826324418287"></a><a name="zh-cn_topic_0108272830_p1826324418287"></a>请根据错误提示进行定位，若无法解决，请联系<span id="zh-cn_topic_0108272830_text19753172203813"><a name="zh-cn_topic_0108272830_text19753172203813"></a><a name="zh-cn_topic_0108272830_text19753172203813"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row2263124410286"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p1526304415289"><a name="zh-cn_topic_0108272830_p1526304415289"></a><a name="zh-cn_topic_0108272830_p1526304415289"></a>Cdm.0089</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p19263124432814"><a name="zh-cn_topic_0108272830_p19263124432814"></a><a name="zh-cn_topic_0108272830_p19263124432814"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p132634444289"><a name="zh-cn_topic_0108272830_p132634444289"></a><a name="zh-cn_topic_0108272830_p132634444289"></a>配置项 [%s] 不存在。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p326314445283"><a name="zh-cn_topic_0108272830_p326314445283"></a><a name="zh-cn_topic_0108272830_p326314445283"></a>配置项不存在。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p726316446282"><a name="zh-cn_topic_0108272830_p726316446282"></a><a name="zh-cn_topic_0108272830_p726316446282"></a>请根据错误提示进行定位，若无法解决，请联系<span id="zh-cn_topic_0108272830_text097510263810"><a name="zh-cn_topic_0108272830_text097510263810"></a><a name="zh-cn_topic_0108272830_text097510263810"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row2263144162819"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p15263174492811"><a name="zh-cn_topic_0108272830_p15263174492811"></a><a name="zh-cn_topic_0108272830_p15263174492811"></a>Cdm.0100</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p17263164410283"><a name="zh-cn_topic_0108272830_p17263164410283"></a><a name="zh-cn_topic_0108272830_p17263164410283"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p726334482813"><a name="zh-cn_topic_0108272830_p726334482813"></a><a name="zh-cn_topic_0108272830_p726334482813"></a>作业[<em id="zh-cn_topic_0108272830_i9263104410283"><a name="zh-cn_topic_0108272830_i9263104410283"></a><a name="zh-cn_topic_0108272830_i9263104410283"></a>%s</em>]不存在。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p6263144482819"><a name="zh-cn_topic_0108272830_p6263144482819"></a><a name="zh-cn_topic_0108272830_p6263144482819"></a>作业不存在。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p6263194411287"><a name="zh-cn_topic_0108272830_p6263194411287"></a><a name="zh-cn_topic_0108272830_p6263194411287"></a>请指定正确的作业后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row02632447289"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p15263444132819"><a name="zh-cn_topic_0108272830_p15263444132819"></a><a name="zh-cn_topic_0108272830_p15263444132819"></a>Cdm.0101</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p42641444122820"><a name="zh-cn_topic_0108272830_p42641444122820"></a><a name="zh-cn_topic_0108272830_p42641444122820"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p13264044202811"><a name="zh-cn_topic_0108272830_p13264044202811"></a><a name="zh-cn_topic_0108272830_p13264044202811"></a>连接[<em id="zh-cn_topic_0108272830_i62641844112810"><a name="zh-cn_topic_0108272830_i62641844112810"></a><a name="zh-cn_topic_0108272830_i62641844112810"></a>%s</em>]不存在。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p9264164432812"><a name="zh-cn_topic_0108272830_p9264164432812"></a><a name="zh-cn_topic_0108272830_p9264164432812"></a>连接不存在。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p42645449284"><a name="zh-cn_topic_0108272830_p42645449284"></a><a name="zh-cn_topic_0108272830_p42645449284"></a>请指定正确的连接后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row1926416446281"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p152641344192813"><a name="zh-cn_topic_0108272830_p152641344192813"></a><a name="zh-cn_topic_0108272830_p152641344192813"></a>Cdm.0102</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p122641544202816"><a name="zh-cn_topic_0108272830_p122641544202816"></a><a name="zh-cn_topic_0108272830_p122641544202816"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p13264124492814"><a name="zh-cn_topic_0108272830_p13264124492814"></a><a name="zh-cn_topic_0108272830_p13264124492814"></a>连接器[<em id="zh-cn_topic_0108272830_i4264944122816"><a name="zh-cn_topic_0108272830_i4264944122816"></a><a name="zh-cn_topic_0108272830_i4264944122816"></a>%s</em>]不存在。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p1126484413281"><a name="zh-cn_topic_0108272830_p1126484413281"></a><a name="zh-cn_topic_0108272830_p1126484413281"></a>连接器不存在。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p026416448282"><a name="zh-cn_topic_0108272830_p026416448282"></a><a name="zh-cn_topic_0108272830_p026416448282"></a>请指定正确的连接器后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row1426474482820"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p1826494419284"><a name="zh-cn_topic_0108272830_p1826494419284"></a><a name="zh-cn_topic_0108272830_p1826494419284"></a>Cdm.0104</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p52641447286"><a name="zh-cn_topic_0108272830_p52641447286"></a><a name="zh-cn_topic_0108272830_p52641447286"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p1726464416285"><a name="zh-cn_topic_0108272830_p1726464416285"></a><a name="zh-cn_topic_0108272830_p1726464416285"></a>作业名已存在。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p1264134462810"><a name="zh-cn_topic_0108272830_p1264134462810"></a><a name="zh-cn_topic_0108272830_p1264134462810"></a>作业名已存在。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p2026484492819"><a name="zh-cn_topic_0108272830_p2026484492819"></a><a name="zh-cn_topic_0108272830_p2026484492819"></a>作业名已存在，请重新命名后，再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row18264154417282"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p92641544172820"><a name="zh-cn_topic_0108272830_p92641544172820"></a><a name="zh-cn_topic_0108272830_p92641544172820"></a>Cdm.0201</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p226464412283"><a name="zh-cn_topic_0108272830_p226464412283"></a><a name="zh-cn_topic_0108272830_p226464412283"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p02646444280"><a name="zh-cn_topic_0108272830_p02646444280"></a><a name="zh-cn_topic_0108272830_p02646444280"></a>获取实例失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p1826419446282"><a name="zh-cn_topic_0108272830_p1826419446282"></a><a name="zh-cn_topic_0108272830_p1826419446282"></a>获取实例失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p62641844162820"><a name="zh-cn_topic_0108272830_p62641844162820"></a><a name="zh-cn_topic_0108272830_p62641844162820"></a>请联系<span id="zh-cn_topic_0108272830_text71815319386"><a name="zh-cn_topic_0108272830_text71815319386"></a><a name="zh-cn_topic_0108272830_text71815319386"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row82642443281"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p1526474411289"><a name="zh-cn_topic_0108272830_p1526474411289"></a><a name="zh-cn_topic_0108272830_p1526474411289"></a>Cdm.0202</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p62651044142814"><a name="zh-cn_topic_0108272830_p62651044142814"></a><a name="zh-cn_topic_0108272830_p62651044142814"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p72651144102816"><a name="zh-cn_topic_0108272830_p72651144102816"></a><a name="zh-cn_topic_0108272830_p72651144102816"></a>作业状态未知。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p626524402816"><a name="zh-cn_topic_0108272830_p626524402816"></a><a name="zh-cn_topic_0108272830_p626524402816"></a>作业状态未知。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p6265154413286"><a name="zh-cn_topic_0108272830_p6265154413286"></a><a name="zh-cn_topic_0108272830_p6265154413286"></a>请稍后重试，或请联系<span id="zh-cn_topic_0108272830_text1412432380"><a name="zh-cn_topic_0108272830_text1412432380"></a><a name="zh-cn_topic_0108272830_text1412432380"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row18265544152814"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p92651144192812"><a name="zh-cn_topic_0108272830_p92651144192812"></a><a name="zh-cn_topic_0108272830_p92651144192812"></a>Cdm.0204</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p152651244112811"><a name="zh-cn_topic_0108272830_p152651244112811"></a><a name="zh-cn_topic_0108272830_p152651244112811"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p12265164412281"><a name="zh-cn_topic_0108272830_p12265164412281"></a><a name="zh-cn_topic_0108272830_p12265164412281"></a>没有已创建的MRS连接。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p192657441283"><a name="zh-cn_topic_0108272830_p192657441283"></a><a name="zh-cn_topic_0108272830_p192657441283"></a>没有已创建的MRS连接。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p15265104412811"><a name="zh-cn_topic_0108272830_p15265104412811"></a><a name="zh-cn_topic_0108272830_p15265104412811"></a>当前没有MRS连接，您需要先前往集群的“连接管理”页面创建一个MRS连接，然后再重新执行当前的操作。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row4265124419286"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p11265174422813"><a name="zh-cn_topic_0108272830_p11265174422813"></a><a name="zh-cn_topic_0108272830_p11265174422813"></a>Cdm.0230</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p526524415286"><a name="zh-cn_topic_0108272830_p526524415286"></a><a name="zh-cn_topic_0108272830_p526524415286"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p72656448284"><a name="zh-cn_topic_0108272830_p72656448284"></a><a name="zh-cn_topic_0108272830_p72656448284"></a>不能加载该类：<em id="zh-cn_topic_0108272830_i4265144412286"><a name="zh-cn_topic_0108272830_i4265144412286"></a><a name="zh-cn_topic_0108272830_i4265144412286"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p12265114412816"><a name="zh-cn_topic_0108272830_p12265114412816"></a><a name="zh-cn_topic_0108272830_p12265114412816"></a>类加载失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p182651144142811"><a name="zh-cn_topic_0108272830_p182651144142811"></a><a name="zh-cn_topic_0108272830_p182651144142811"></a>请联系<span id="zh-cn_topic_0108272830_text14592103173816"><a name="zh-cn_topic_0108272830_text14592103173816"></a><a name="zh-cn_topic_0108272830_text14592103173816"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row1326511446281"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p17265144202817"><a name="zh-cn_topic_0108272830_p17265144202817"></a><a name="zh-cn_topic_0108272830_p17265144202817"></a>Cdm.0231</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p16265184417280"><a name="zh-cn_topic_0108272830_p16265184417280"></a><a name="zh-cn_topic_0108272830_p16265184417280"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p5265204442816"><a name="zh-cn_topic_0108272830_p5265204442816"></a><a name="zh-cn_topic_0108272830_p5265204442816"></a>不能初始化该类：<em id="zh-cn_topic_0108272830_i12265124413282"><a name="zh-cn_topic_0108272830_i12265124413282"></a><a name="zh-cn_topic_0108272830_i12265124413282"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p1326518442285"><a name="zh-cn_topic_0108272830_p1326518442285"></a><a name="zh-cn_topic_0108272830_p1326518442285"></a>类初始化失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p4265104412817"><a name="zh-cn_topic_0108272830_p4265104412817"></a><a name="zh-cn_topic_0108272830_p4265104412817"></a>请联系<span id="zh-cn_topic_0108272830_text1480114319384"><a name="zh-cn_topic_0108272830_text1480114319384"></a><a name="zh-cn_topic_0108272830_text1480114319384"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row42655446280"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p226512445283"><a name="zh-cn_topic_0108272830_p226512445283"></a><a name="zh-cn_topic_0108272830_p226512445283"></a>Cdm.0232</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p026584412287"><a name="zh-cn_topic_0108272830_p026584412287"></a><a name="zh-cn_topic_0108272830_p026584412287"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p726514422818"><a name="zh-cn_topic_0108272830_p726514422818"></a><a name="zh-cn_topic_0108272830_p726514422818"></a>数据写入失败。原因：<em id="zh-cn_topic_0108272830_i16265644132815"><a name="zh-cn_topic_0108272830_i16265644132815"></a><a name="zh-cn_topic_0108272830_i16265644132815"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p6265114432815"><a name="zh-cn_topic_0108272830_p6265114432815"></a><a name="zh-cn_topic_0108272830_p6265114432815"></a>数据写入失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p126512446286"><a name="zh-cn_topic_0108272830_p126512446286"></a><a name="zh-cn_topic_0108272830_p126512446286"></a>请联系<span id="zh-cn_topic_0108272830_text1131443816"><a name="zh-cn_topic_0108272830_text1131443816"></a><a name="zh-cn_topic_0108272830_text1131443816"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row326574417289"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p226512446284"><a name="zh-cn_topic_0108272830_p226512446284"></a><a name="zh-cn_topic_0108272830_p226512446284"></a>Cdm.0233</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p172651444162815"><a name="zh-cn_topic_0108272830_p172651444162815"></a><a name="zh-cn_topic_0108272830_p172651444162815"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p13265144492815"><a name="zh-cn_topic_0108272830_p13265144492815"></a><a name="zh-cn_topic_0108272830_p13265144492815"></a>提取数据过程异常。原因：<em id="zh-cn_topic_0108272830_i17265164452811"><a name="zh-cn_topic_0108272830_i17265164452811"></a><a name="zh-cn_topic_0108272830_i17265164452811"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p1326514440280"><a name="zh-cn_topic_0108272830_p1326514440280"></a><a name="zh-cn_topic_0108272830_p1326514440280"></a>提取数据过程异常。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p926618449285"><a name="zh-cn_topic_0108272830_p926618449285"></a><a name="zh-cn_topic_0108272830_p926618449285"></a>请联系<span id="zh-cn_topic_0108272830_text162391540387"><a name="zh-cn_topic_0108272830_text162391540387"></a><a name="zh-cn_topic_0108272830_text162391540387"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row2266244182810"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p626604422816"><a name="zh-cn_topic_0108272830_p626604422816"></a><a name="zh-cn_topic_0108272830_p626604422816"></a>Cdm.0234</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p1126664412286"><a name="zh-cn_topic_0108272830_p1126664412286"></a><a name="zh-cn_topic_0108272830_p1126664412286"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p202661744142812"><a name="zh-cn_topic_0108272830_p202661744142812"></a><a name="zh-cn_topic_0108272830_p202661744142812"></a>载入数据过程异常。原因：<em id="zh-cn_topic_0108272830_i2266844122817"><a name="zh-cn_topic_0108272830_i2266844122817"></a><a name="zh-cn_topic_0108272830_i2266844122817"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p12661944152814"><a name="zh-cn_topic_0108272830_p12661944152814"></a><a name="zh-cn_topic_0108272830_p12661944152814"></a>载入数据过程异常。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p626634432820"><a name="zh-cn_topic_0108272830_p626634432820"></a><a name="zh-cn_topic_0108272830_p626634432820"></a>请联系<span id="zh-cn_topic_0108272830_text243613473819"><a name="zh-cn_topic_0108272830_text243613473819"></a><a name="zh-cn_topic_0108272830_text243613473819"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row826611445286"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p17266744122812"><a name="zh-cn_topic_0108272830_p17266744122812"></a><a name="zh-cn_topic_0108272830_p17266744122812"></a>Cdm.0235</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p192661344162818"><a name="zh-cn_topic_0108272830_p192661344162818"></a><a name="zh-cn_topic_0108272830_p192661344162818"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p1326619441280"><a name="zh-cn_topic_0108272830_p1326619441280"></a><a name="zh-cn_topic_0108272830_p1326619441280"></a>数据已全部消费完毕。原因：<em id="zh-cn_topic_0108272830_i9266144182813"><a name="zh-cn_topic_0108272830_i9266144182813"></a><a name="zh-cn_topic_0108272830_i9266144182813"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p17266144415286"><a name="zh-cn_topic_0108272830_p17266144415286"></a><a name="zh-cn_topic_0108272830_p17266144415286"></a>数据已全部消费完毕。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p32661944162811"><a name="zh-cn_topic_0108272830_p32661944162811"></a><a name="zh-cn_topic_0108272830_p32661944162811"></a>请根据错误提示进行定位，若无法解决，请联系<span id="zh-cn_topic_0108272830_text665110483812"><a name="zh-cn_topic_0108272830_text665110483812"></a><a name="zh-cn_topic_0108272830_text665110483812"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row426613441286"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p126618449283"><a name="zh-cn_topic_0108272830_p126618449283"></a><a name="zh-cn_topic_0108272830_p126618449283"></a>Cdm.0236</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p326616445284"><a name="zh-cn_topic_0108272830_p326616445284"></a><a name="zh-cn_topic_0108272830_p326616445284"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p19266044142814"><a name="zh-cn_topic_0108272830_p19266044142814"></a><a name="zh-cn_topic_0108272830_p19266044142814"></a>从分区程序中检索到无效分区数。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p82665445286"><a name="zh-cn_topic_0108272830_p82665445286"></a><a name="zh-cn_topic_0108272830_p82665445286"></a>从分区程序中检索到无效分区数。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p92668443286"><a name="zh-cn_topic_0108272830_p92668443286"></a><a name="zh-cn_topic_0108272830_p92668443286"></a>请根据错误提示进行定位，若无法解决，请联系<span id="zh-cn_topic_0108272830_text108751473817"><a name="zh-cn_topic_0108272830_text108751473817"></a><a name="zh-cn_topic_0108272830_text108751473817"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row5266114418280"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p19266134452815"><a name="zh-cn_topic_0108272830_p19266134452815"></a><a name="zh-cn_topic_0108272830_p19266134452815"></a>Cdm.0238</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p126616448287"><a name="zh-cn_topic_0108272830_p126616448287"></a><a name="zh-cn_topic_0108272830_p126616448287"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p926684419288"><a name="zh-cn_topic_0108272830_p926684419288"></a><a name="zh-cn_topic_0108272830_p926684419288"></a><em id="zh-cn_topic_0108272830_i826644417284"><a name="zh-cn_topic_0108272830_i826644417284"></a><a name="zh-cn_topic_0108272830_i826644417284"></a>%s</em>不能为空。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p7266544102819"><a name="zh-cn_topic_0108272830_p7266544102819"></a><a name="zh-cn_topic_0108272830_p7266544102819"></a>参数不合法。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p2266144202819"><a name="zh-cn_topic_0108272830_p2266144202819"></a><a name="zh-cn_topic_0108272830_p2266144202819"></a>请根据错误提示将参数修改正确后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row1626694410289"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p20266844162811"><a name="zh-cn_topic_0108272830_p20266844162811"></a><a name="zh-cn_topic_0108272830_p20266844162811"></a>Cdm.0240</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p6266544112816"><a name="zh-cn_topic_0108272830_p6266544112816"></a><a name="zh-cn_topic_0108272830_p6266544112816"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p19266114452810"><a name="zh-cn_topic_0108272830_p19266114452810"></a><a name="zh-cn_topic_0108272830_p19266114452810"></a>获取文件<em id="zh-cn_topic_0108272830_i3266104411288"><a name="zh-cn_topic_0108272830_i3266104411288"></a><a name="zh-cn_topic_0108272830_i3266104411288"></a>%s</em>状态失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p1226619447281"><a name="zh-cn_topic_0108272830_p1226619447281"></a><a name="zh-cn_topic_0108272830_p1226619447281"></a>获取文件状态失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p1026620447282"><a name="zh-cn_topic_0108272830_p1026620447282"></a><a name="zh-cn_topic_0108272830_p1026620447282"></a>请联系<span id="zh-cn_topic_0108272830_text11939520381"><a name="zh-cn_topic_0108272830_text11939520381"></a><a name="zh-cn_topic_0108272830_text11939520381"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row5266114492817"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p19267044112811"><a name="zh-cn_topic_0108272830_p19267044112811"></a><a name="zh-cn_topic_0108272830_p19267044112811"></a>Cdm.0241</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p2026724420281"><a name="zh-cn_topic_0108272830_p2026724420281"></a><a name="zh-cn_topic_0108272830_p2026724420281"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p1267944132814"><a name="zh-cn_topic_0108272830_p1267944132814"></a><a name="zh-cn_topic_0108272830_p1267944132814"></a>获取文件<em id="zh-cn_topic_0108272830_i1326714419281"><a name="zh-cn_topic_0108272830_i1326714419281"></a><a name="zh-cn_topic_0108272830_i1326714419281"></a>%s</em>类型失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p62671444192816"><a name="zh-cn_topic_0108272830_p62671444192816"></a><a name="zh-cn_topic_0108272830_p62671444192816"></a>获取文件类型失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p82671444182819"><a name="zh-cn_topic_0108272830_p82671444182819"></a><a name="zh-cn_topic_0108272830_p82671444182819"></a>请联系<span id="zh-cn_topic_0108272830_text13299185203814"><a name="zh-cn_topic_0108272830_text13299185203814"></a><a name="zh-cn_topic_0108272830_text13299185203814"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row32675446286"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p32678447289"><a name="zh-cn_topic_0108272830_p32678447289"></a><a name="zh-cn_topic_0108272830_p32678447289"></a>Cdm.0242</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p14267114411288"><a name="zh-cn_topic_0108272830_p14267114411288"></a><a name="zh-cn_topic_0108272830_p14267114411288"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p92671044202817"><a name="zh-cn_topic_0108272830_p92671044202817"></a><a name="zh-cn_topic_0108272830_p92671044202817"></a>文件检查异常：<em id="zh-cn_topic_0108272830_i42671544192811"><a name="zh-cn_topic_0108272830_i42671544192811"></a><a name="zh-cn_topic_0108272830_i42671544192811"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p8267184420287"><a name="zh-cn_topic_0108272830_p8267184420287"></a><a name="zh-cn_topic_0108272830_p8267184420287"></a>文件检查异常。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p14267444122811"><a name="zh-cn_topic_0108272830_p14267444122811"></a><a name="zh-cn_topic_0108272830_p14267444122811"></a>请联系<span id="zh-cn_topic_0108272830_text1252535113820"><a name="zh-cn_topic_0108272830_text1252535113820"></a><a name="zh-cn_topic_0108272830_text1252535113820"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row226734432812"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p172672044162811"><a name="zh-cn_topic_0108272830_p172672044162811"></a><a name="zh-cn_topic_0108272830_p172672044162811"></a>Cdm.0243</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p11267154412810"><a name="zh-cn_topic_0108272830_p11267154412810"></a><a name="zh-cn_topic_0108272830_p11267154412810"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p226794411283"><a name="zh-cn_topic_0108272830_p226794411283"></a><a name="zh-cn_topic_0108272830_p226794411283"></a>重命名<em id="zh-cn_topic_0108272830_i32672441283"><a name="zh-cn_topic_0108272830_i32672441283"></a><a name="zh-cn_topic_0108272830_i32672441283"></a>%s</em>为<em id="zh-cn_topic_0108272830_i1626744413281"><a name="zh-cn_topic_0108272830_i1626744413281"></a><a name="zh-cn_topic_0108272830_i1626744413281"></a>%s</em>失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p8267184442815"><a name="zh-cn_topic_0108272830_p8267184442815"></a><a name="zh-cn_topic_0108272830_p8267184442815"></a>重命名失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p3267124492812"><a name="zh-cn_topic_0108272830_p3267124492812"></a><a name="zh-cn_topic_0108272830_p3267124492812"></a>可能是名称已存在，请重新命名后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row19267124432817"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p17267744182818"><a name="zh-cn_topic_0108272830_p17267744182818"></a><a name="zh-cn_topic_0108272830_p17267744182818"></a>Cdm.0244</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p2268104432820"><a name="zh-cn_topic_0108272830_p2268104432820"></a><a name="zh-cn_topic_0108272830_p2268104432820"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p18268544132818"><a name="zh-cn_topic_0108272830_p18268544132818"></a><a name="zh-cn_topic_0108272830_p18268544132818"></a>创建文件<em id="zh-cn_topic_0108272830_i52681144112819"><a name="zh-cn_topic_0108272830_i52681144112819"></a><a name="zh-cn_topic_0108272830_i52681144112819"></a>%s</em>失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p14268154412818"><a name="zh-cn_topic_0108272830_p14268154412818"></a><a name="zh-cn_topic_0108272830_p14268154412818"></a>创建文件失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p112681644152812"><a name="zh-cn_topic_0108272830_p112681644152812"></a><a name="zh-cn_topic_0108272830_p112681644152812"></a>请确认是否具有创建权限，或稍后重试。若无法解决，请联系<span id="zh-cn_topic_0108272830_text973110512387"><a name="zh-cn_topic_0108272830_text973110512387"></a><a name="zh-cn_topic_0108272830_text973110512387"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row6268104442818"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p626874452811"><a name="zh-cn_topic_0108272830_p626874452811"></a><a name="zh-cn_topic_0108272830_p626874452811"></a>Cdm.0245</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p152689440282"><a name="zh-cn_topic_0108272830_p152689440282"></a><a name="zh-cn_topic_0108272830_p152689440282"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p1726834413286"><a name="zh-cn_topic_0108272830_p1726834413286"></a><a name="zh-cn_topic_0108272830_p1726834413286"></a>删除文件<em id="zh-cn_topic_0108272830_i12268104472815"><a name="zh-cn_topic_0108272830_i12268104472815"></a><a name="zh-cn_topic_0108272830_i12268104472815"></a>%s</em>失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p1326815447284"><a name="zh-cn_topic_0108272830_p1326815447284"></a><a name="zh-cn_topic_0108272830_p1326815447284"></a>删除文件失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p13268544192812"><a name="zh-cn_topic_0108272830_p13268544192812"></a><a name="zh-cn_topic_0108272830_p13268544192812"></a>请确认是否具有删除权限，或稍后重试。若无法解决，请联系<span id="zh-cn_topic_0108272830_text159431511385"><a name="zh-cn_topic_0108272830_text159431511385"></a><a name="zh-cn_topic_0108272830_text159431511385"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row1426854410282"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p182681044122811"><a name="zh-cn_topic_0108272830_p182681044122811"></a><a name="zh-cn_topic_0108272830_p182681044122811"></a>Cdm.0246</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p5268104419281"><a name="zh-cn_topic_0108272830_p5268104419281"></a><a name="zh-cn_topic_0108272830_p5268104419281"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p20268344192810"><a name="zh-cn_topic_0108272830_p20268344192810"></a><a name="zh-cn_topic_0108272830_p20268344192810"></a>创建目录<em id="zh-cn_topic_0108272830_i13268124462817"><a name="zh-cn_topic_0108272830_i13268124462817"></a><a name="zh-cn_topic_0108272830_i13268124462817"></a>%s</em>失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p192688443288"><a name="zh-cn_topic_0108272830_p192688443288"></a><a name="zh-cn_topic_0108272830_p192688443288"></a>创建目录失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p726824416285"><a name="zh-cn_topic_0108272830_p726824416285"></a><a name="zh-cn_topic_0108272830_p726824416285"></a>请确认是否具有创建权限，或稍后重试。若无法解决，请联系<span id="zh-cn_topic_0108272830_text1018117613388"><a name="zh-cn_topic_0108272830_text1018117613388"></a><a name="zh-cn_topic_0108272830_text1018117613388"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row8268154415288"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p132681644162810"><a name="zh-cn_topic_0108272830_p132681644162810"></a><a name="zh-cn_topic_0108272830_p132681644162810"></a>Cdm.0247</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p1326810448284"><a name="zh-cn_topic_0108272830_p1326810448284"></a><a name="zh-cn_topic_0108272830_p1326810448284"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p626810446281"><a name="zh-cn_topic_0108272830_p626810446281"></a><a name="zh-cn_topic_0108272830_p626810446281"></a>操作HBase失败。原因：<em id="zh-cn_topic_0108272830_i1826854472820"><a name="zh-cn_topic_0108272830_i1826854472820"></a><a name="zh-cn_topic_0108272830_i1826854472820"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p14269644152815"><a name="zh-cn_topic_0108272830_p14269644152815"></a><a name="zh-cn_topic_0108272830_p14269644152815"></a>操作HBase失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p626934482815"><a name="zh-cn_topic_0108272830_p626934482815"></a><a name="zh-cn_topic_0108272830_p626934482815"></a>请根据错误提示进行定位，若无法解决，请联系<span id="zh-cn_topic_0108272830_text12395163383"><a name="zh-cn_topic_0108272830_text12395163383"></a><a name="zh-cn_topic_0108272830_text12395163383"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row1726944417284"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p1269344182820"><a name="zh-cn_topic_0108272830_p1269344182820"></a><a name="zh-cn_topic_0108272830_p1269344182820"></a>Cdm.0248</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p52694446283"><a name="zh-cn_topic_0108272830_p52694446283"></a><a name="zh-cn_topic_0108272830_p52694446283"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p026904472810"><a name="zh-cn_topic_0108272830_p026904472810"></a><a name="zh-cn_topic_0108272830_p026904472810"></a>清空<em id="zh-cn_topic_0108272830_i226974411280"><a name="zh-cn_topic_0108272830_i226974411280"></a><a name="zh-cn_topic_0108272830_i226974411280"></a>%s</em>数据失败。原因：<em id="zh-cn_topic_0108272830_i5269044192819"><a name="zh-cn_topic_0108272830_i5269044192819"></a><a name="zh-cn_topic_0108272830_i5269044192819"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p20269194414281"><a name="zh-cn_topic_0108272830_p20269194414281"></a><a name="zh-cn_topic_0108272830_p20269194414281"></a>清空数据失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p182691344162817"><a name="zh-cn_topic_0108272830_p182691344162817"></a><a name="zh-cn_topic_0108272830_p182691344162817"></a>请根据错误提示进行定位，若无法解决，请联系<span id="zh-cn_topic_0108272830_text1762376103810"><a name="zh-cn_topic_0108272830_text1762376103810"></a><a name="zh-cn_topic_0108272830_text1762376103810"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row2026904482810"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p1126974482817"><a name="zh-cn_topic_0108272830_p1126974482817"></a><a name="zh-cn_topic_0108272830_p1126974482817"></a>Cdm.0249</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p1726917442286"><a name="zh-cn_topic_0108272830_p1726917442286"></a><a name="zh-cn_topic_0108272830_p1726917442286"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p426914472819"><a name="zh-cn_topic_0108272830_p426914472819"></a><a name="zh-cn_topic_0108272830_p426914472819"></a>文件名<em id="zh-cn_topic_0108272830_i3269344152819"><a name="zh-cn_topic_0108272830_i3269344152819"></a><a name="zh-cn_topic_0108272830_i3269344152819"></a>%s</em>无效。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p11269194414285"><a name="zh-cn_topic_0108272830_p11269194414285"></a><a name="zh-cn_topic_0108272830_p11269194414285"></a>文件名无效。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p1326954416288"><a name="zh-cn_topic_0108272830_p1326954416288"></a><a name="zh-cn_topic_0108272830_p1326954416288"></a>请将文件名修改正确后，再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row12269174413288"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p526944412288"><a name="zh-cn_topic_0108272830_p526944412288"></a><a name="zh-cn_topic_0108272830_p526944412288"></a>Cdm.0250</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p426944419285"><a name="zh-cn_topic_0108272830_p426944419285"></a><a name="zh-cn_topic_0108272830_p426944419285"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p126914415282"><a name="zh-cn_topic_0108272830_p126914415282"></a><a name="zh-cn_topic_0108272830_p126914415282"></a>不能操作该路径：<em id="zh-cn_topic_0108272830_i9269144414289"><a name="zh-cn_topic_0108272830_i9269144414289"></a><a name="zh-cn_topic_0108272830_i9269144414289"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p226994462810"><a name="zh-cn_topic_0108272830_p226994462810"></a><a name="zh-cn_topic_0108272830_p226994462810"></a>不能操作该路径。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p19269344192820"><a name="zh-cn_topic_0108272830_p19269344192820"></a><a name="zh-cn_topic_0108272830_p19269344192820"></a>请确认是否具有该路径的操作权限，或稍后重试。若无法解决，请联系<span id="zh-cn_topic_0108272830_text1841365381"><a name="zh-cn_topic_0108272830_text1841365381"></a><a name="zh-cn_topic_0108272830_text1841365381"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row1326984414282"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p162697449285"><a name="zh-cn_topic_0108272830_p162697449285"></a><a name="zh-cn_topic_0108272830_p162697449285"></a>Cdm.0251</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p8269144102817"><a name="zh-cn_topic_0108272830_p8269144102817"></a><a name="zh-cn_topic_0108272830_p8269144102817"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p1126924414282"><a name="zh-cn_topic_0108272830_p1126924414282"></a><a name="zh-cn_topic_0108272830_p1126924414282"></a>向HBase加载数据失败。原因：<em id="zh-cn_topic_0108272830_i17269134413283"><a name="zh-cn_topic_0108272830_i17269134413283"></a><a name="zh-cn_topic_0108272830_i17269134413283"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p11269164412284"><a name="zh-cn_topic_0108272830_p11269164412284"></a><a name="zh-cn_topic_0108272830_p11269164412284"></a>向HBase加载数据失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p1726974492811"><a name="zh-cn_topic_0108272830_p1726974492811"></a><a name="zh-cn_topic_0108272830_p1726974492811"></a>请根据错误提示进行定位，若无法解决，请联系<span id="zh-cn_topic_0108272830_text106797163814"><a name="zh-cn_topic_0108272830_text106797163814"></a><a name="zh-cn_topic_0108272830_text106797163814"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row16269144122818"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p226994482814"><a name="zh-cn_topic_0108272830_p226994482814"></a><a name="zh-cn_topic_0108272830_p226994482814"></a>Cdm.0307</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p15269184472818"><a name="zh-cn_topic_0108272830_p15269184472818"></a><a name="zh-cn_topic_0108272830_p15269184472818"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p13269154416284"><a name="zh-cn_topic_0108272830_p13269154416284"></a><a name="zh-cn_topic_0108272830_p13269154416284"></a>无法获得请求事务的链接租约，原因：<em id="zh-cn_topic_0108272830_i426974472816"><a name="zh-cn_topic_0108272830_i426974472816"></a><a name="zh-cn_topic_0108272830_i426974472816"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p8269174416281"><a name="zh-cn_topic_0108272830_p8269174416281"></a><a name="zh-cn_topic_0108272830_p8269174416281"></a>无法获得请求事务的链接租约。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p12270444172812"><a name="zh-cn_topic_0108272830_p12270444172812"></a><a name="zh-cn_topic_0108272830_p12270444172812"></a>请根据错误提示进行定位，若无法解决，请联系<span id="zh-cn_topic_0108272830_text1929710733814"><a name="zh-cn_topic_0108272830_text1929710733814"></a><a name="zh-cn_topic_0108272830_text1929710733814"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row162701444112813"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p13270144416289"><a name="zh-cn_topic_0108272830_p13270144416289"></a><a name="zh-cn_topic_0108272830_p13270144416289"></a>Cdm.0315</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p32704447284"><a name="zh-cn_topic_0108272830_p32704447284"></a><a name="zh-cn_topic_0108272830_p32704447284"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p10270184492813"><a name="zh-cn_topic_0108272830_p10270184492813"></a><a name="zh-cn_topic_0108272830_p10270184492813"></a>连接名<em id="zh-cn_topic_0108272830_i112701944192811"><a name="zh-cn_topic_0108272830_i112701944192811"></a><a name="zh-cn_topic_0108272830_i112701944192811"></a>%s</em>已存在。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p4270164422819"><a name="zh-cn_topic_0108272830_p4270164422819"></a><a name="zh-cn_topic_0108272830_p4270164422819"></a>该连接已存在。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p162709444287"><a name="zh-cn_topic_0108272830_p162709444287"></a><a name="zh-cn_topic_0108272830_p162709444287"></a>请指定其他连接名后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row102701344162812"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p8270134414281"><a name="zh-cn_topic_0108272830_p8270134414281"></a><a name="zh-cn_topic_0108272830_p8270134414281"></a>Cdm.0316</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p13270104416281"><a name="zh-cn_topic_0108272830_p13270104416281"></a><a name="zh-cn_topic_0108272830_p13270104416281"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p1327094452813"><a name="zh-cn_topic_0108272830_p1327094452813"></a><a name="zh-cn_topic_0108272830_p1327094452813"></a>无法更新不存在的连接。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p4270844152814"><a name="zh-cn_topic_0108272830_p4270844152814"></a><a name="zh-cn_topic_0108272830_p4270844152814"></a>无法更新不存在的连接。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p17270114412285"><a name="zh-cn_topic_0108272830_p17270114412285"></a><a name="zh-cn_topic_0108272830_p17270114412285"></a>请指定正确的连接后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row1270164412287"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p3270144142816"><a name="zh-cn_topic_0108272830_p3270144142816"></a><a name="zh-cn_topic_0108272830_p3270144142816"></a>Cdm.0317</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p132701444112813"><a name="zh-cn_topic_0108272830_p132701444112813"></a><a name="zh-cn_topic_0108272830_p132701444112813"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p162705445285"><a name="zh-cn_topic_0108272830_p162705445285"></a><a name="zh-cn_topic_0108272830_p162705445285"></a>连接<em id="zh-cn_topic_0108272830_i127014417281"><a name="zh-cn_topic_0108272830_i127014417281"></a><a name="zh-cn_topic_0108272830_i127014417281"></a>%s</em>无效。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p11270194415282"><a name="zh-cn_topic_0108272830_p11270194415282"></a><a name="zh-cn_topic_0108272830_p11270194415282"></a>连接无效。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p1827013442289"><a name="zh-cn_topic_0108272830_p1827013442289"></a><a name="zh-cn_topic_0108272830_p1827013442289"></a>请指定正确的连接后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row72701244112810"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p52708443281"><a name="zh-cn_topic_0108272830_p52708443281"></a><a name="zh-cn_topic_0108272830_p52708443281"></a>Cdm.0318</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p172701944122811"><a name="zh-cn_topic_0108272830_p172701944122811"></a><a name="zh-cn_topic_0108272830_p172701944122811"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p227016445286"><a name="zh-cn_topic_0108272830_p227016445286"></a><a name="zh-cn_topic_0108272830_p227016445286"></a>作业已存在，无法重复创建。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p32701044152810"><a name="zh-cn_topic_0108272830_p32701044152810"></a><a name="zh-cn_topic_0108272830_p32701044152810"></a>作业已存在。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p227084442819"><a name="zh-cn_topic_0108272830_p227084442819"></a><a name="zh-cn_topic_0108272830_p227084442819"></a>请指定其他作业名再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row1327064432818"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p192701744102817"><a name="zh-cn_topic_0108272830_p192701744102817"></a><a name="zh-cn_topic_0108272830_p192701744102817"></a>Cdm.0319</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p52701844112816"><a name="zh-cn_topic_0108272830_p52701844112816"></a><a name="zh-cn_topic_0108272830_p52701844112816"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p9270174432814"><a name="zh-cn_topic_0108272830_p9270174432814"></a><a name="zh-cn_topic_0108272830_p9270174432814"></a>无法更新不存在的作业。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p172701844132814"><a name="zh-cn_topic_0108272830_p172701844132814"></a><a name="zh-cn_topic_0108272830_p172701844132814"></a>无法更新不存在的作业。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p22701544182820"><a name="zh-cn_topic_0108272830_p22701544182820"></a><a name="zh-cn_topic_0108272830_p22701544182820"></a>请确认待更新的作业是否存在，作业名修改正确后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row19270244172812"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p8270144412285"><a name="zh-cn_topic_0108272830_p8270144412285"></a><a name="zh-cn_topic_0108272830_p8270144412285"></a>Cdm.0320</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p1827144412814"><a name="zh-cn_topic_0108272830_p1827144412814"></a><a name="zh-cn_topic_0108272830_p1827144412814"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p15271444112813"><a name="zh-cn_topic_0108272830_p15271444112813"></a><a name="zh-cn_topic_0108272830_p15271444112813"></a>作业<em id="zh-cn_topic_0108272830_i1127116440287"><a name="zh-cn_topic_0108272830_i1127116440287"></a><a name="zh-cn_topic_0108272830_i1127116440287"></a>%s</em>无效。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p627113444283"><a name="zh-cn_topic_0108272830_p627113444283"></a><a name="zh-cn_topic_0108272830_p627113444283"></a>作业无效。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p8271114412811"><a name="zh-cn_topic_0108272830_p8271114412811"></a><a name="zh-cn_topic_0108272830_p8271114412811"></a>请联系<span id="zh-cn_topic_0108272830_text105156713810"><a name="zh-cn_topic_0108272830_text105156713810"></a><a name="zh-cn_topic_0108272830_text105156713810"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row5271194411284"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p72711443281"><a name="zh-cn_topic_0108272830_p72711443281"></a><a name="zh-cn_topic_0108272830_p72711443281"></a>Cdm.0321</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p627124412288"><a name="zh-cn_topic_0108272830_p627124412288"></a><a name="zh-cn_topic_0108272830_p627124412288"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p6271744132817"><a name="zh-cn_topic_0108272830_p6271744132817"></a><a name="zh-cn_topic_0108272830_p6271744132817"></a>连接<em id="zh-cn_topic_0108272830_i14271174413283"><a name="zh-cn_topic_0108272830_i14271174413283"></a><a name="zh-cn_topic_0108272830_i14271174413283"></a>%s</em>已被使用。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p17271194410284"><a name="zh-cn_topic_0108272830_p17271194410284"></a><a name="zh-cn_topic_0108272830_p17271194410284"></a>连接已被使用。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p6271154419288"><a name="zh-cn_topic_0108272830_p6271154419288"></a><a name="zh-cn_topic_0108272830_p6271154419288"></a>连接已被使用，无法执行当前的操作，请将连接释放后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row112711844162812"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p9271204452816"><a name="zh-cn_topic_0108272830_p9271204452816"></a><a name="zh-cn_topic_0108272830_p9271204452816"></a>Cdm.0322</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p13271164412285"><a name="zh-cn_topic_0108272830_p13271164412285"></a><a name="zh-cn_topic_0108272830_p13271164412285"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p14271344102817"><a name="zh-cn_topic_0108272830_p14271344102817"></a><a name="zh-cn_topic_0108272830_p14271344102817"></a>作业<em id="zh-cn_topic_0108272830_i1271194418281"><a name="zh-cn_topic_0108272830_i1271194418281"></a><a name="zh-cn_topic_0108272830_i1271194418281"></a>%s</em>已被使用。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p5271174412813"><a name="zh-cn_topic_0108272830_p5271174412813"></a><a name="zh-cn_topic_0108272830_p5271174412813"></a>作业已被使用。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p202711644132815"><a name="zh-cn_topic_0108272830_p202711644132815"></a><a name="zh-cn_topic_0108272830_p202711644132815"></a>请联系<span id="zh-cn_topic_0108272830_text67251472382"><a name="zh-cn_topic_0108272830_text67251472382"></a><a name="zh-cn_topic_0108272830_text67251472382"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row327117447284"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p92711144122811"><a name="zh-cn_topic_0108272830_p92711144122811"></a><a name="zh-cn_topic_0108272830_p92711144122811"></a>Cdm.0323</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p52713449281"><a name="zh-cn_topic_0108272830_p52713449281"></a><a name="zh-cn_topic_0108272830_p52713449281"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p1127144415283"><a name="zh-cn_topic_0108272830_p1127144415283"></a><a name="zh-cn_topic_0108272830_p1127144415283"></a>该提交已存在，无法重复创建。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p1827116445281"><a name="zh-cn_topic_0108272830_p1827116445281"></a><a name="zh-cn_topic_0108272830_p1827116445281"></a>该提交已存在。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p12271104452811"><a name="zh-cn_topic_0108272830_p12271104452811"></a><a name="zh-cn_topic_0108272830_p12271104452811"></a>您已提交过相同操作的请求，请稍后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row4271444142818"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p172711344172814"><a name="zh-cn_topic_0108272830_p172711344172814"></a><a name="zh-cn_topic_0108272830_p172711344172814"></a>Cdm.0327</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p192711844102818"><a name="zh-cn_topic_0108272830_p192711844102818"></a><a name="zh-cn_topic_0108272830_p192711844102818"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p1827114419287"><a name="zh-cn_topic_0108272830_p1827114419287"></a><a name="zh-cn_topic_0108272830_p1827114419287"></a>无效的连接或作业：<em id="zh-cn_topic_0108272830_i3271134410283"><a name="zh-cn_topic_0108272830_i3271134410283"></a><a name="zh-cn_topic_0108272830_i3271134410283"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p1227114412817"><a name="zh-cn_topic_0108272830_p1227114412817"></a><a name="zh-cn_topic_0108272830_p1227114412817"></a>无效的连接或作业。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p1327114414282"><a name="zh-cn_topic_0108272830_p1327114414282"></a><a name="zh-cn_topic_0108272830_p1327114414282"></a>请指定正确的连接或作业再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row102711844112810"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p13271134416289"><a name="zh-cn_topic_0108272830_p13271134416289"></a><a name="zh-cn_topic_0108272830_p13271134416289"></a>Cdm.0411</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p127144452819"><a name="zh-cn_topic_0108272830_p127144452819"></a><a name="zh-cn_topic_0108272830_p127144452819"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p8271154412283"><a name="zh-cn_topic_0108272830_p8271154412283"></a><a name="zh-cn_topic_0108272830_p8271154412283"></a>连接到文件服务器时出错。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p62711544172817"><a name="zh-cn_topic_0108272830_p62711544172817"></a><a name="zh-cn_topic_0108272830_p62711544172817"></a>连接到文件服务器时出错。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p1227184432813"><a name="zh-cn_topic_0108272830_p1227184432813"></a><a name="zh-cn_topic_0108272830_p1227184432813"></a>请联系<span id="zh-cn_topic_0108272830_text1794937153811"><a name="zh-cn_topic_0108272830_text1794937153811"></a><a name="zh-cn_topic_0108272830_text1794937153811"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row1927164418288"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p7271144418282"><a name="zh-cn_topic_0108272830_p7271144418282"></a><a name="zh-cn_topic_0108272830_p7271144418282"></a>Cdm.0413</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p1227114482812"><a name="zh-cn_topic_0108272830_p1227114482812"></a><a name="zh-cn_topic_0108272830_p1227114482812"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p12272164492816"><a name="zh-cn_topic_0108272830_p12272164492816"></a><a name="zh-cn_topic_0108272830_p12272164492816"></a>向文件服务器传输数据时出错。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p14272104462820"><a name="zh-cn_topic_0108272830_p14272104462820"></a><a name="zh-cn_topic_0108272830_p14272104462820"></a>向文件服务器传输数据时出错。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p15272844202810"><a name="zh-cn_topic_0108272830_p15272844202810"></a><a name="zh-cn_topic_0108272830_p15272844202810"></a>请联系<span id="zh-cn_topic_0108272830_text518710815389"><a name="zh-cn_topic_0108272830_text518710815389"></a><a name="zh-cn_topic_0108272830_text518710815389"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row1627274419283"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p32721144192816"><a name="zh-cn_topic_0108272830_p32721144192816"></a><a name="zh-cn_topic_0108272830_p32721144192816"></a>Cdm.0415</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p1272134472815"><a name="zh-cn_topic_0108272830_p1272134472815"></a><a name="zh-cn_topic_0108272830_p1272134472815"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p7272644142814"><a name="zh-cn_topic_0108272830_p7272644142814"></a><a name="zh-cn_topic_0108272830_p7272644142814"></a>从文件服务器下载文件出错。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p8272134422818"><a name="zh-cn_topic_0108272830_p8272134422818"></a><a name="zh-cn_topic_0108272830_p8272134422818"></a>从文件服务器下载文件出错。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p32729441286"><a name="zh-cn_topic_0108272830_p32729441286"></a><a name="zh-cn_topic_0108272830_p32729441286"></a>请联系<span id="zh-cn_topic_0108272830_text1407880387"><a name="zh-cn_topic_0108272830_text1407880387"></a><a name="zh-cn_topic_0108272830_text1407880387"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row1327217442283"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p14272344102814"><a name="zh-cn_topic_0108272830_p14272344102814"></a><a name="zh-cn_topic_0108272830_p14272344102814"></a>Cdm.0416</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p8272644152817"><a name="zh-cn_topic_0108272830_p8272644152817"></a><a name="zh-cn_topic_0108272830_p8272644152817"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p82721844122812"><a name="zh-cn_topic_0108272830_p82721844122812"></a><a name="zh-cn_topic_0108272830_p82721844122812"></a>抽取数据时出错。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p027264462816"><a name="zh-cn_topic_0108272830_p027264462816"></a><a name="zh-cn_topic_0108272830_p027264462816"></a>抽取数据时出错。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p1827284462813"><a name="zh-cn_topic_0108272830_p1827284462813"></a><a name="zh-cn_topic_0108272830_p1827284462813"></a>请联系<span id="zh-cn_topic_0108272830_text1664514811380"><a name="zh-cn_topic_0108272830_text1664514811380"></a><a name="zh-cn_topic_0108272830_text1664514811380"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row1627234416286"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p227204472816"><a name="zh-cn_topic_0108272830_p227204472816"></a><a name="zh-cn_topic_0108272830_p227204472816"></a>Cdm.0420</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p16272344182819"><a name="zh-cn_topic_0108272830_p16272344182819"></a><a name="zh-cn_topic_0108272830_p16272344182819"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p9272544192817"><a name="zh-cn_topic_0108272830_p9272544192817"></a><a name="zh-cn_topic_0108272830_p9272544192817"></a>源文件或源目录不存在。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p1927244418283"><a name="zh-cn_topic_0108272830_p1927244418283"></a><a name="zh-cn_topic_0108272830_p1927244418283"></a>源文件或源目录不存在。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p18272844122812"><a name="zh-cn_topic_0108272830_p18272844122812"></a><a name="zh-cn_topic_0108272830_p18272844122812"></a>请确认源文件或源目录是否存在，修改正确后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row1727294418281"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p727264432814"><a name="zh-cn_topic_0108272830_p727264432814"></a><a name="zh-cn_topic_0108272830_p727264432814"></a>Cdm.0423</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p182721244162819"><a name="zh-cn_topic_0108272830_p182721244162819"></a><a name="zh-cn_topic_0108272830_p182721244162819"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p1227294482818"><a name="zh-cn_topic_0108272830_p1227294482818"></a><a name="zh-cn_topic_0108272830_p1227294482818"></a>目的路径存在重复文件。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p12272644122811"><a name="zh-cn_topic_0108272830_p12272644122811"></a><a name="zh-cn_topic_0108272830_p12272644122811"></a>目的路径存在重复文件。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p32721044202818"><a name="zh-cn_topic_0108272830_p32721044202818"></a><a name="zh-cn_topic_0108272830_p32721044202818"></a>请在目的路径中删除重复文件后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row3272154414284"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p62721644132814"><a name="zh-cn_topic_0108272830_p62721644132814"></a><a name="zh-cn_topic_0108272830_p62721644132814"></a>Cdm.0501</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p827254472820"><a name="zh-cn_topic_0108272830_p827254472820"></a><a name="zh-cn_topic_0108272830_p827254472820"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p62721844102816"><a name="zh-cn_topic_0108272830_p62721844102816"></a><a name="zh-cn_topic_0108272830_p62721844102816"></a>无效的URI[<em id="zh-cn_topic_0108272830_i127264414282"><a name="zh-cn_topic_0108272830_i127264414282"></a><a name="zh-cn_topic_0108272830_i127264414282"></a>%s</em>]。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p9272104492813"><a name="zh-cn_topic_0108272830_p9272104492813"></a><a name="zh-cn_topic_0108272830_p9272104492813"></a>无效的URI。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p32721944132813"><a name="zh-cn_topic_0108272830_p32721944132813"></a><a name="zh-cn_topic_0108272830_p32721944132813"></a>请指定正确的URI后，再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row1027294422816"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p027264411282"><a name="zh-cn_topic_0108272830_p027264411282"></a><a name="zh-cn_topic_0108272830_p027264411282"></a>Cdm.0518</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p0272644162811"><a name="zh-cn_topic_0108272830_p0272644162811"></a><a name="zh-cn_topic_0108272830_p0272644162811"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p12272244172810"><a name="zh-cn_topic_0108272830_p12272244172810"></a><a name="zh-cn_topic_0108272830_p12272244172810"></a>连接HDFS失败。原因：<em id="zh-cn_topic_0108272830_i42721744172819"><a name="zh-cn_topic_0108272830_i42721744172819"></a><a name="zh-cn_topic_0108272830_i42721744172819"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p1727374422819"><a name="zh-cn_topic_0108272830_p1727374422819"></a><a name="zh-cn_topic_0108272830_p1727374422819"></a>连接HDFS失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p227313445287"><a name="zh-cn_topic_0108272830_p227313445287"></a><a name="zh-cn_topic_0108272830_p227313445287"></a>请根据错误提示进行定位，若无法解决，请联系<span id="zh-cn_topic_0108272830_text386519811386"><a name="zh-cn_topic_0108272830_text386519811386"></a><a name="zh-cn_topic_0108272830_text386519811386"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row192731244102813"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p1727317448286"><a name="zh-cn_topic_0108272830_p1727317448286"></a><a name="zh-cn_topic_0108272830_p1727317448286"></a>Cdm.0600</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p8273164414283"><a name="zh-cn_topic_0108272830_p8273164414283"></a><a name="zh-cn_topic_0108272830_p8273164414283"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p9273114415286"><a name="zh-cn_topic_0108272830_p9273114415286"></a><a name="zh-cn_topic_0108272830_p9273114415286"></a>无法连接FTP服务器。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p92731944152815"><a name="zh-cn_topic_0108272830_p92731944152815"></a><a name="zh-cn_topic_0108272830_p92731944152815"></a>无法连接FTP服务器。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p227384416286"><a name="zh-cn_topic_0108272830_p227384416286"></a><a name="zh-cn_topic_0108272830_p227384416286"></a>可能是由于网络不通、安全组或防火墙规则未放行、FTP主机名无法解析、FTP用户名密码错误等原因。若排除上述原因后仍无法解决，请联系<span id="zh-cn_topic_0108272830_text128729173810"><a name="zh-cn_topic_0108272830_text128729173810"></a><a name="zh-cn_topic_0108272830_text128729173810"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row122731044112815"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p22731944112811"><a name="zh-cn_topic_0108272830_p22731944112811"></a><a name="zh-cn_topic_0108272830_p22731944112811"></a>Cdm.0700</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p9273184416286"><a name="zh-cn_topic_0108272830_p9273184416286"></a><a name="zh-cn_topic_0108272830_p9273184416286"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p102730448286"><a name="zh-cn_topic_0108272830_p102730448286"></a><a name="zh-cn_topic_0108272830_p102730448286"></a>无法连接SFTP服务器。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p162733448284"><a name="zh-cn_topic_0108272830_p162733448284"></a><a name="zh-cn_topic_0108272830_p162733448284"></a>无法连接SFTP服务器。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p162731844162810"><a name="zh-cn_topic_0108272830_p162731844162810"></a><a name="zh-cn_topic_0108272830_p162731844162810"></a>可能是由于网络不通、安全组或防火墙规则未放行、SFTP主机名无法解析、SFTP用户名密码错误等原因。若排除上述原因后仍无法解决，请联系<span id="zh-cn_topic_0108272830_text10327693388"><a name="zh-cn_topic_0108272830_text10327693388"></a><a name="zh-cn_topic_0108272830_text10327693388"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row22731244102812"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p1527315442281"><a name="zh-cn_topic_0108272830_p1527315442281"></a><a name="zh-cn_topic_0108272830_p1527315442281"></a>Cdm.0800</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p102731344132811"><a name="zh-cn_topic_0108272830_p102731344132811"></a><a name="zh-cn_topic_0108272830_p102731344132811"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p827334418285"><a name="zh-cn_topic_0108272830_p827334418285"></a><a name="zh-cn_topic_0108272830_p827334418285"></a>无法连接OBS服务器。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p8273104462817"><a name="zh-cn_topic_0108272830_p8273104462817"></a><a name="zh-cn_topic_0108272830_p8273104462817"></a>无法连接OBS服务器。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p14273114416282"><a name="zh-cn_topic_0108272830_p14273114416282"></a><a name="zh-cn_topic_0108272830_p14273114416282"></a>可能是由于OBS终端节点与当前区域不一致、AK/SK错误、AK/SK不是当前用户的AK/SK、安全组或防火墙规则未放行等原因。若排除上述原因后仍无法解决，请联系<span id="zh-cn_topic_0108272830_text654920953818"><a name="zh-cn_topic_0108272830_text654920953818"></a><a name="zh-cn_topic_0108272830_text654920953818"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row9273164472819"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p202734444286"><a name="zh-cn_topic_0108272830_p202734444286"></a><a name="zh-cn_topic_0108272830_p202734444286"></a>Cdm.0801</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p162735445285"><a name="zh-cn_topic_0108272830_p162735445285"></a><a name="zh-cn_topic_0108272830_p162735445285"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p3273104482818"><a name="zh-cn_topic_0108272830_p3273104482818"></a><a name="zh-cn_topic_0108272830_p3273104482818"></a>OBS桶[<em id="zh-cn_topic_0108272830_i1327304412289"><a name="zh-cn_topic_0108272830_i1327304412289"></a><a name="zh-cn_topic_0108272830_i1327304412289"></a>%s</em>]不存在。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p1273134420286"><a name="zh-cn_topic_0108272830_p1273134420286"></a><a name="zh-cn_topic_0108272830_p1273134420286"></a>OBS桶不存在。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p13273244132816"><a name="zh-cn_topic_0108272830_p13273244132816"></a><a name="zh-cn_topic_0108272830_p13273244132816"></a>指定的OBS桶可能不存在或不在当前区域，请指定正确的OBS桶后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row16273114442815"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p32731744182810"><a name="zh-cn_topic_0108272830_p32731744182810"></a><a name="zh-cn_topic_0108272830_p32731744182810"></a>Cdm.0831</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p927315448284"><a name="zh-cn_topic_0108272830_p927315448284"></a><a name="zh-cn_topic_0108272830_p927315448284"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p13273194422813"><a name="zh-cn_topic_0108272830_p13273194422813"></a><a name="zh-cn_topic_0108272830_p13273194422813"></a>无法连接到KODO服务器。原因：<em id="zh-cn_topic_0108272830_i3273124416285"><a name="zh-cn_topic_0108272830_i3273124416285"></a><a name="zh-cn_topic_0108272830_i3273124416285"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p1273044202818"><a name="zh-cn_topic_0108272830_p1273044202818"></a><a name="zh-cn_topic_0108272830_p1273044202818"></a>无法连接到KODO服务器。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p82731244132816"><a name="zh-cn_topic_0108272830_p82731244132816"></a><a name="zh-cn_topic_0108272830_p82731244132816"></a>请联系<span id="zh-cn_topic_0108272830_text137818915386"><a name="zh-cn_topic_0108272830_text137818915386"></a><a name="zh-cn_topic_0108272830_text137818915386"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row6273154416282"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p7273114419286"><a name="zh-cn_topic_0108272830_p7273114419286"></a><a name="zh-cn_topic_0108272830_p7273114419286"></a>Cdm.0900</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p16273114422817"><a name="zh-cn_topic_0108272830_p16273114422817"></a><a name="zh-cn_topic_0108272830_p16273114422817"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p132732044102813"><a name="zh-cn_topic_0108272830_p132732044102813"></a><a name="zh-cn_topic_0108272830_p132732044102813"></a>表[<em id="zh-cn_topic_0108272830_i22736445288"><a name="zh-cn_topic_0108272830_i22736445288"></a><a name="zh-cn_topic_0108272830_i22736445288"></a>%s</em>]不存在。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p1027424452819"><a name="zh-cn_topic_0108272830_p1027424452819"></a><a name="zh-cn_topic_0108272830_p1027424452819"></a>表不存在。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p1127417448285"><a name="zh-cn_topic_0108272830_p1127417448285"></a><a name="zh-cn_topic_0108272830_p1127417448285"></a>请指定正确的表名后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row1127454411286"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p6274244102819"><a name="zh-cn_topic_0108272830_p6274244102819"></a><a name="zh-cn_topic_0108272830_p6274244102819"></a>Cdm.0901</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p5274174482819"><a name="zh-cn_topic_0108272830_p5274174482819"></a><a name="zh-cn_topic_0108272830_p5274174482819"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p11274544142813"><a name="zh-cn_topic_0108272830_p11274544142813"></a><a name="zh-cn_topic_0108272830_p11274544142813"></a>无法连接数据库服务器。原因：<em id="zh-cn_topic_0108272830_i9274944102816"><a name="zh-cn_topic_0108272830_i9274944102816"></a><a name="zh-cn_topic_0108272830_i9274944102816"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p427424414287"><a name="zh-cn_topic_0108272830_p427424414287"></a><a name="zh-cn_topic_0108272830_p427424414287"></a>无法连接数据库服务器。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p1527454415283"><a name="zh-cn_topic_0108272830_p1527454415283"></a><a name="zh-cn_topic_0108272830_p1527454415283"></a>请联系<span id="zh-cn_topic_0108272830_text1413910153813"><a name="zh-cn_topic_0108272830_text1413910153813"></a><a name="zh-cn_topic_0108272830_text1413910153813"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row1274204415285"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p927414449288"><a name="zh-cn_topic_0108272830_p927414449288"></a><a name="zh-cn_topic_0108272830_p927414449288"></a>Cdm.0902</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p1274194452814"><a name="zh-cn_topic_0108272830_p1274194452814"></a><a name="zh-cn_topic_0108272830_p1274194452814"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p1427404418289"><a name="zh-cn_topic_0108272830_p1427404418289"></a><a name="zh-cn_topic_0108272830_p1427404418289"></a>SQL语句无法执行。原因<em id="zh-cn_topic_0108272830_i1627417443283"><a name="zh-cn_topic_0108272830_i1627417443283"></a><a name="zh-cn_topic_0108272830_i1627417443283"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p72742447287"><a name="zh-cn_topic_0108272830_p72742447287"></a><a name="zh-cn_topic_0108272830_p72742447287"></a>SQL语句无法执行。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p1527417446289"><a name="zh-cn_topic_0108272830_p1527417446289"></a><a name="zh-cn_topic_0108272830_p1527417446289"></a>请根据错误提示进行定位，若无法解决，请联系<span id="zh-cn_topic_0108272830_text825951073811"><a name="zh-cn_topic_0108272830_text825951073811"></a><a name="zh-cn_topic_0108272830_text825951073811"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row10274194414285"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p7274044132814"><a name="zh-cn_topic_0108272830_p7274044132814"></a><a name="zh-cn_topic_0108272830_p7274044132814"></a>Cdm.0903</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p122740445287"><a name="zh-cn_topic_0108272830_p122740445287"></a><a name="zh-cn_topic_0108272830_p122740445287"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p1274154414288"><a name="zh-cn_topic_0108272830_p1274154414288"></a><a name="zh-cn_topic_0108272830_p1274154414288"></a>元数据获取失败。原因：<em id="zh-cn_topic_0108272830_i12274154411286"><a name="zh-cn_topic_0108272830_i12274154411286"></a><a name="zh-cn_topic_0108272830_i12274154411286"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p0274844132813"><a name="zh-cn_topic_0108272830_p0274844132813"></a><a name="zh-cn_topic_0108272830_p0274844132813"></a>元数据获取失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p122741444182811"><a name="zh-cn_topic_0108272830_p122741444182811"></a><a name="zh-cn_topic_0108272830_p122741444182811"></a>请确认在集群的“连接管理”页面创建连接时引用符号是否正确或查看数据库表是否存在。若仍无法解决，请联系<span id="zh-cn_topic_0108272830_text13503101023812"><a name="zh-cn_topic_0108272830_text13503101023812"></a><a name="zh-cn_topic_0108272830_text13503101023812"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row17274344112810"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p142741644142813"><a name="zh-cn_topic_0108272830_p142741644142813"></a><a name="zh-cn_topic_0108272830_p142741644142813"></a>Cdm.0904</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p9274944122812"><a name="zh-cn_topic_0108272830_p9274944122812"></a><a name="zh-cn_topic_0108272830_p9274944122812"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p122741544132816"><a name="zh-cn_topic_0108272830_p122741544132816"></a><a name="zh-cn_topic_0108272830_p122741544132816"></a>从结果中检索数据时发生错误。原因：<em id="zh-cn_topic_0108272830_i1827494412284"><a name="zh-cn_topic_0108272830_i1827494412284"></a><a name="zh-cn_topic_0108272830_i1827494412284"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p527419449285"><a name="zh-cn_topic_0108272830_p527419449285"></a><a name="zh-cn_topic_0108272830_p527419449285"></a>从结果中检索数据时发生错误。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p6274194402818"><a name="zh-cn_topic_0108272830_p6274194402818"></a><a name="zh-cn_topic_0108272830_p6274194402818"></a>请根据错误提示进行定位，若无法解决，请联系<span id="zh-cn_topic_0108272830_text3734810163814"><a name="zh-cn_topic_0108272830_text3734810163814"></a><a name="zh-cn_topic_0108272830_text3734810163814"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row32746444285"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p527417445287"><a name="zh-cn_topic_0108272830_p527417445287"></a><a name="zh-cn_topic_0108272830_p527417445287"></a>Cdm.0913</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p927414419281"><a name="zh-cn_topic_0108272830_p927414419281"></a><a name="zh-cn_topic_0108272830_p927414419281"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p1274194462819"><a name="zh-cn_topic_0108272830_p1274194462819"></a><a name="zh-cn_topic_0108272830_p1274194462819"></a>Schema和SQL不可以同时为空。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p0274194411282"><a name="zh-cn_topic_0108272830_p0274194411282"></a><a name="zh-cn_topic_0108272830_p0274194411282"></a>Schema和SQL需指定其中一项。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p2027515442280"><a name="zh-cn_topic_0108272830_p2027515442280"></a><a name="zh-cn_topic_0108272830_p2027515442280"></a>请确认Schema和SQL是否同时为空，请指定其中一项后，再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row162751544122812"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p82751844132812"><a name="zh-cn_topic_0108272830_p82751844132812"></a><a name="zh-cn_topic_0108272830_p82751844132812"></a>Cdm.0916</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p13275744162810"><a name="zh-cn_topic_0108272830_p13275744162810"></a><a name="zh-cn_topic_0108272830_p13275744162810"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p18275344132815"><a name="zh-cn_topic_0108272830_p18275344132815"></a><a name="zh-cn_topic_0108272830_p18275344132815"></a>增量读取情况下必须指定上次的值。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p32751442287"><a name="zh-cn_topic_0108272830_p32751442287"></a><a name="zh-cn_topic_0108272830_p32751442287"></a>增量读取时未指定上次的值。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p327534452812"><a name="zh-cn_topic_0108272830_p327534452812"></a><a name="zh-cn_topic_0108272830_p327534452812"></a>请指定上次的值后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row22751544122813"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p6275154417282"><a name="zh-cn_topic_0108272830_p6275154417282"></a><a name="zh-cn_topic_0108272830_p6275154417282"></a>Cdm.0917</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p1275184412811"><a name="zh-cn_topic_0108272830_p1275184412811"></a><a name="zh-cn_topic_0108272830_p1275184412811"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p3275844172814"><a name="zh-cn_topic_0108272830_p3275844172814"></a><a name="zh-cn_topic_0108272830_p3275844172814"></a>缺少字段检查将无法获得上次的值。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p92751044102811"><a name="zh-cn_topic_0108272830_p92751044102811"></a><a name="zh-cn_topic_0108272830_p92751044102811"></a>缺少字段。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p527517441284"><a name="zh-cn_topic_0108272830_p527517441284"></a><a name="zh-cn_topic_0108272830_p527517441284"></a>请联系<span id="zh-cn_topic_0108272830_text1743381123816"><a name="zh-cn_topic_0108272830_text1743381123816"></a><a name="zh-cn_topic_0108272830_text1743381123816"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row427513447288"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p327524452815"><a name="zh-cn_topic_0108272830_p327524452815"></a><a name="zh-cn_topic_0108272830_p327524452815"></a>Cdm.0921</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p18275164402820"><a name="zh-cn_topic_0108272830_p18275164402820"></a><a name="zh-cn_topic_0108272830_p18275164402820"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p72751944142817"><a name="zh-cn_topic_0108272830_p72751944142817"></a><a name="zh-cn_topic_0108272830_p72751944142817"></a>不支持类型<em id="zh-cn_topic_0108272830_i12275104422815"><a name="zh-cn_topic_0108272830_i12275104422815"></a><a name="zh-cn_topic_0108272830_i12275104422815"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p527564417285"><a name="zh-cn_topic_0108272830_p527564417285"></a><a name="zh-cn_topic_0108272830_p527564417285"></a>类型不合法。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p2275164419288"><a name="zh-cn_topic_0108272830_p2275164419288"></a><a name="zh-cn_topic_0108272830_p2275164419288"></a>请指定正确的类型后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row52751244132811"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p13275194472810"><a name="zh-cn_topic_0108272830_p13275194472810"></a><a name="zh-cn_topic_0108272830_p13275194472810"></a>Cdm.0925</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p122754445284"><a name="zh-cn_topic_0108272830_p122754445284"></a><a name="zh-cn_topic_0108272830_p122754445284"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p5275344162812"><a name="zh-cn_topic_0108272830_p5275344162812"></a><a name="zh-cn_topic_0108272830_p5275344162812"></a>分区字段含有不支持的值。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p927510444282"><a name="zh-cn_topic_0108272830_p927510444282"></a><a name="zh-cn_topic_0108272830_p927510444282"></a>分区字段含有不支持的值。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p72752441285"><a name="zh-cn_topic_0108272830_p72752441285"></a><a name="zh-cn_topic_0108272830_p72752441285"></a>请确认分区字段是否含有不支持的值，修改正确后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row527584413283"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p13275164411282"><a name="zh-cn_topic_0108272830_p13275164411282"></a><a name="zh-cn_topic_0108272830_p13275164411282"></a>Cdm.0926</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p127518444280"><a name="zh-cn_topic_0108272830_p127518444280"></a><a name="zh-cn_topic_0108272830_p127518444280"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p1827614412819"><a name="zh-cn_topic_0108272830_p1827614412819"></a><a name="zh-cn_topic_0108272830_p1827614412819"></a>取不到Schema。原因：<em id="zh-cn_topic_0108272830_i192761544152811"><a name="zh-cn_topic_0108272830_i192761544152811"></a><a name="zh-cn_topic_0108272830_i192761544152811"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p1027664442816"><a name="zh-cn_topic_0108272830_p1027664442816"></a><a name="zh-cn_topic_0108272830_p1027664442816"></a>获取Schema失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p8276134419288"><a name="zh-cn_topic_0108272830_p8276134419288"></a><a name="zh-cn_topic_0108272830_p8276134419288"></a>请根据错误提示进行定位，若无法解决，请联系<span id="zh-cn_topic_0108272830_text176598112385"><a name="zh-cn_topic_0108272830_text176598112385"></a><a name="zh-cn_topic_0108272830_text176598112385"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row8276944122818"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p7276344202812"><a name="zh-cn_topic_0108272830_p7276344202812"></a><a name="zh-cn_topic_0108272830_p7276344202812"></a>Cdm.0927</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p2276174462819"><a name="zh-cn_topic_0108272830_p2276174462819"></a><a name="zh-cn_topic_0108272830_p2276174462819"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p027654413281"><a name="zh-cn_topic_0108272830_p027654413281"></a><a name="zh-cn_topic_0108272830_p027654413281"></a>中转表不为空。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p14276144422813"><a name="zh-cn_topic_0108272830_p14276144422813"></a><a name="zh-cn_topic_0108272830_p14276144422813"></a>中转表不为空。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p13276154420283"><a name="zh-cn_topic_0108272830_p13276154420283"></a><a name="zh-cn_topic_0108272830_p13276154420283"></a>请指定一个空的中转表后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row1627684411285"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p427620442282"><a name="zh-cn_topic_0108272830_p427620442282"></a><a name="zh-cn_topic_0108272830_p427620442282"></a>Cdm.0928</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p1727624415284"><a name="zh-cn_topic_0108272830_p1727624415284"></a><a name="zh-cn_topic_0108272830_p1727624415284"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p5276124492818"><a name="zh-cn_topic_0108272830_p5276124492818"></a><a name="zh-cn_topic_0108272830_p5276124492818"></a>中转表到目的表进行数据迁移时发生错误。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p3276444132814"><a name="zh-cn_topic_0108272830_p3276444132814"></a><a name="zh-cn_topic_0108272830_p3276444132814"></a>中转表到目的表进行数据迁移时发生错误。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p1927617448288"><a name="zh-cn_topic_0108272830_p1927617448288"></a><a name="zh-cn_topic_0108272830_p1927617448288"></a>请联系<span id="zh-cn_topic_0108272830_text990931115385"><a name="zh-cn_topic_0108272830_text990931115385"></a><a name="zh-cn_topic_0108272830_text990931115385"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row12276134413289"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p6276844102815"><a name="zh-cn_topic_0108272830_p6276844102815"></a><a name="zh-cn_topic_0108272830_p6276844102815"></a>Cdm.0931</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p19276164452813"><a name="zh-cn_topic_0108272830_p19276164452813"></a><a name="zh-cn_topic_0108272830_p19276164452813"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p627604414286"><a name="zh-cn_topic_0108272830_p627604414286"></a><a name="zh-cn_topic_0108272830_p627604414286"></a>Schema字段大小[<em id="zh-cn_topic_0108272830_i027615448285"><a name="zh-cn_topic_0108272830_i027615448285"></a><a name="zh-cn_topic_0108272830_i027615448285"></a>%s</em>]与结果集的字段大小[<em id="zh-cn_topic_0108272830_i2276154452816"><a name="zh-cn_topic_0108272830_i2276154452816"></a><a name="zh-cn_topic_0108272830_i2276154452816"></a>%s</em>]不匹配。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p1127611442280"><a name="zh-cn_topic_0108272830_p1127611442280"></a><a name="zh-cn_topic_0108272830_p1127611442280"></a>Schema字段大小与结果集的字段大小不匹配。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p327624412283"><a name="zh-cn_topic_0108272830_p327624412283"></a><a name="zh-cn_topic_0108272830_p327624412283"></a>请将Schema字段大小和结果集中的字段大小改为一致后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row20276114462811"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p10276104422818"><a name="zh-cn_topic_0108272830_p10276104422818"></a><a name="zh-cn_topic_0108272830_p10276104422818"></a>Cdm.0932</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p927664414282"><a name="zh-cn_topic_0108272830_p927664414282"></a><a name="zh-cn_topic_0108272830_p927664414282"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p727614410289"><a name="zh-cn_topic_0108272830_p727614410289"></a><a name="zh-cn_topic_0108272830_p727614410289"></a>找不到字段最大值。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p14276154422820"><a name="zh-cn_topic_0108272830_p14276154422820"></a><a name="zh-cn_topic_0108272830_p14276154422820"></a>找不到字段最大值。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p122771144172818"><a name="zh-cn_topic_0108272830_p122771144172818"></a><a name="zh-cn_topic_0108272830_p122771144172818"></a>请联系<span id="zh-cn_topic_0108272830_text114951218389"><a name="zh-cn_topic_0108272830_text114951218389"></a><a name="zh-cn_topic_0108272830_text114951218389"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row1727714472815"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p527710443287"><a name="zh-cn_topic_0108272830_p527710443287"></a><a name="zh-cn_topic_0108272830_p527710443287"></a>Cdm.0934</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p13277124418289"><a name="zh-cn_topic_0108272830_p13277124418289"></a><a name="zh-cn_topic_0108272830_p13277124418289"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p827764415287"><a name="zh-cn_topic_0108272830_p827764415287"></a><a name="zh-cn_topic_0108272830_p827764415287"></a>不同Schema/Catalog下有重名表。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p9277044122814"><a name="zh-cn_topic_0108272830_p9277044122814"></a><a name="zh-cn_topic_0108272830_p9277044122814"></a>不同Schema/Catalog下有重名表。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p1327714414286"><a name="zh-cn_topic_0108272830_p1327714414286"></a><a name="zh-cn_topic_0108272830_p1327714414286"></a>请联系<span id="zh-cn_topic_0108272830_text153778129386"><a name="zh-cn_topic_0108272830_text153778129386"></a><a name="zh-cn_topic_0108272830_text153778129386"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row1127713443284"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p13277184417282"><a name="zh-cn_topic_0108272830_p13277184417282"></a><a name="zh-cn_topic_0108272830_p13277184417282"></a>Cdm.0936</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p027716446282"><a name="zh-cn_topic_0108272830_p027716446282"></a><a name="zh-cn_topic_0108272830_p027716446282"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p1527744416285"><a name="zh-cn_topic_0108272830_p1527744416285"></a><a name="zh-cn_topic_0108272830_p1527744416285"></a>错误脏数据条数达到上限。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p1027764418286"><a name="zh-cn_topic_0108272830_p1027764418286"></a><a name="zh-cn_topic_0108272830_p1027764418286"></a>错误脏数据条数达到上限。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p72775447283"><a name="zh-cn_topic_0108272830_p72775447283"></a><a name="zh-cn_topic_0108272830_p72775447283"></a>您可以编辑作业，在作业的任务配置中将错误脏数据条数增大。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row142770449288"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p427720448282"><a name="zh-cn_topic_0108272830_p427720448282"></a><a name="zh-cn_topic_0108272830_p427720448282"></a>Cdm.0940</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p02772447284"><a name="zh-cn_topic_0108272830_p02772447284"></a><a name="zh-cn_topic_0108272830_p02772447284"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p5277164418285"><a name="zh-cn_topic_0108272830_p5277164418285"></a><a name="zh-cn_topic_0108272830_p5277164418285"></a>表名准确匹配失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p162771344172816"><a name="zh-cn_topic_0108272830_p162771344172816"></a><a name="zh-cn_topic_0108272830_p162771344172816"></a>表名准确匹配失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p132772044142819"><a name="zh-cn_topic_0108272830_p132772044142819"></a><a name="zh-cn_topic_0108272830_p132772044142819"></a>匹配不到表名，请指定正确的表名后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row12277144132811"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p32772445287"><a name="zh-cn_topic_0108272830_p32772445287"></a><a name="zh-cn_topic_0108272830_p32772445287"></a>Cdm.0941</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p10277164422811"><a name="zh-cn_topic_0108272830_p10277164422811"></a><a name="zh-cn_topic_0108272830_p10277164422811"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p2027734432816"><a name="zh-cn_topic_0108272830_p2027734432816"></a><a name="zh-cn_topic_0108272830_p2027734432816"></a>无法连接服务器。原因：[<em id="zh-cn_topic_0108272830_i82771444192816"><a name="zh-cn_topic_0108272830_i82771444192816"></a><a name="zh-cn_topic_0108272830_i82771444192816"></a>%s</em>]</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p3277744182815"><a name="zh-cn_topic_0108272830_p3277744182815"></a><a name="zh-cn_topic_0108272830_p3277744182815"></a>无法连接服务器。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p5277184417285"><a name="zh-cn_topic_0108272830_p5277184417285"></a><a name="zh-cn_topic_0108272830_p5277184417285"></a>请检查IP、主机名、端口填写是否正确，检查网络安全组和防火墙配置是否正确，参考数据库返回消息进行定位。若仍无法解决，请联系<span id="zh-cn_topic_0108272830_text161351210383"><a name="zh-cn_topic_0108272830_text161351210383"></a><a name="zh-cn_topic_0108272830_text161351210383"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row527734410285"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p162771844162816"><a name="zh-cn_topic_0108272830_p162771844162816"></a><a name="zh-cn_topic_0108272830_p162771844162816"></a>Cdm.0950</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p6277144472819"><a name="zh-cn_topic_0108272830_p6277144472819"></a><a name="zh-cn_topic_0108272830_p6277144472819"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p92771444202820"><a name="zh-cn_topic_0108272830_p92771444202820"></a><a name="zh-cn_topic_0108272830_p92771444202820"></a>当前认证信息无法连接到数据库。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p10277114412810"><a name="zh-cn_topic_0108272830_p10277114412810"></a><a name="zh-cn_topic_0108272830_p10277114412810"></a>当前认证信息无法连接到数据库。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p1627715449283"><a name="zh-cn_topic_0108272830_p1627715449283"></a><a name="zh-cn_topic_0108272830_p1627715449283"></a>认证信息错误，请修改正确后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row182771144152819"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p427754413285"><a name="zh-cn_topic_0108272830_p427754413285"></a><a name="zh-cn_topic_0108272830_p427754413285"></a>Cdm.0962</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p1278194411287"><a name="zh-cn_topic_0108272830_p1278194411287"></a><a name="zh-cn_topic_0108272830_p1278194411287"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p5278164419281"><a name="zh-cn_topic_0108272830_p5278164419281"></a><a name="zh-cn_topic_0108272830_p5278164419281"></a>必须指定主机IP。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p627804472811"><a name="zh-cn_topic_0108272830_p627804472811"></a><a name="zh-cn_topic_0108272830_p627804472811"></a>未指定主机IP。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p202783447280"><a name="zh-cn_topic_0108272830_p202783447280"></a><a name="zh-cn_topic_0108272830_p202783447280"></a>未指定主机IP，请指定主机IP后，再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row5278744142820"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p427864482815"><a name="zh-cn_topic_0108272830_p427864482815"></a><a name="zh-cn_topic_0108272830_p427864482815"></a>Cdm.0963</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p11278144202813"><a name="zh-cn_topic_0108272830_p11278144202813"></a><a name="zh-cn_topic_0108272830_p11278144202813"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p42786447285"><a name="zh-cn_topic_0108272830_p42786447285"></a><a name="zh-cn_topic_0108272830_p42786447285"></a>必须指定主机端口。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p8278154482816"><a name="zh-cn_topic_0108272830_p8278154482816"></a><a name="zh-cn_topic_0108272830_p8278154482816"></a>未指定主机端口。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p13278184492815"><a name="zh-cn_topic_0108272830_p13278184492815"></a><a name="zh-cn_topic_0108272830_p13278184492815"></a>未指定主机端口，请指定主机端口后，再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row122781644192815"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p7278104462820"><a name="zh-cn_topic_0108272830_p7278104462820"></a><a name="zh-cn_topic_0108272830_p7278104462820"></a>Cdm.0964</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p927812445284"><a name="zh-cn_topic_0108272830_p927812445284"></a><a name="zh-cn_topic_0108272830_p927812445284"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p1127811446287"><a name="zh-cn_topic_0108272830_p1127811446287"></a><a name="zh-cn_topic_0108272830_p1127811446287"></a>必须指定数据库。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p102781844142815"><a name="zh-cn_topic_0108272830_p102781844142815"></a><a name="zh-cn_topic_0108272830_p102781844142815"></a>未指定数据库。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p727894422812"><a name="zh-cn_topic_0108272830_p727894422812"></a><a name="zh-cn_topic_0108272830_p727894422812"></a>未指定数据库，请指定数据库后，再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row22781244202811"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p127844415285"><a name="zh-cn_topic_0108272830_p127844415285"></a><a name="zh-cn_topic_0108272830_p127844415285"></a>Cdm.1000</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p3278154411284"><a name="zh-cn_topic_0108272830_p3278154411284"></a><a name="zh-cn_topic_0108272830_p3278154411284"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p1127874442817"><a name="zh-cn_topic_0108272830_p1127874442817"></a><a name="zh-cn_topic_0108272830_p1127874442817"></a>Hive表[<em id="zh-cn_topic_0108272830_i11278184418282"><a name="zh-cn_topic_0108272830_i11278184418282"></a><a name="zh-cn_topic_0108272830_i11278184418282"></a>%s</em>]不存在。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p227874462814"><a name="zh-cn_topic_0108272830_p227874462814"></a><a name="zh-cn_topic_0108272830_p227874462814"></a>Hive表不存在。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p152781844202810"><a name="zh-cn_topic_0108272830_p152781844202810"></a><a name="zh-cn_topic_0108272830_p152781844202810"></a>请输入正确的Hive表名后，再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row10278844142819"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p15278164413281"><a name="zh-cn_topic_0108272830_p15278164413281"></a><a name="zh-cn_topic_0108272830_p15278164413281"></a>Cdm.1010</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p12780446287"><a name="zh-cn_topic_0108272830_p12780446287"></a><a name="zh-cn_topic_0108272830_p12780446287"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p1827824432814"><a name="zh-cn_topic_0108272830_p1827824432814"></a><a name="zh-cn_topic_0108272830_p1827824432814"></a>无效的URI <em id="zh-cn_topic_0108272830_i227811448286"><a name="zh-cn_topic_0108272830_i227811448286"></a><a name="zh-cn_topic_0108272830_i227811448286"></a>%s</em>。URI必须为null或有效的URI。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p172781044132818"><a name="zh-cn_topic_0108272830_p172781044132818"></a><a name="zh-cn_topic_0108272830_p172781044132818"></a>无效的URI。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p1627817446280"><a name="zh-cn_topic_0108272830_p1627817446280"></a><a name="zh-cn_topic_0108272830_p1627817446280"></a>请输入正确的URI后，再重试。下面是一些URI示例：</p>
    <a name="zh-cn_topic_0108272830_ul6278134482811"></a><a name="zh-cn_topic_0108272830_ul6278134482811"></a><ul id="zh-cn_topic_0108272830_ul6278134482811"><li>hdfs://example.com:8020/</li><li>hdfs://example.com/</li><li>file:///</li><li>file:///tmp</li><li>file://localhost/tmp</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row1927874442811"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p15278844132813"><a name="zh-cn_topic_0108272830_p15278844132813"></a><a name="zh-cn_topic_0108272830_p15278844132813"></a>Cdm.1011</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p132781644132813"><a name="zh-cn_topic_0108272830_p132781644132813"></a><a name="zh-cn_topic_0108272830_p132781644132813"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p1527864422810"><a name="zh-cn_topic_0108272830_p1527864422810"></a><a name="zh-cn_topic_0108272830_p1527864422810"></a>连接Hive失败，原因：<em id="zh-cn_topic_0108272830_i14279944142819"><a name="zh-cn_topic_0108272830_i14279944142819"></a><a name="zh-cn_topic_0108272830_i14279944142819"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p2279644132814"><a name="zh-cn_topic_0108272830_p2279644132814"></a><a name="zh-cn_topic_0108272830_p2279644132814"></a>连接Hive失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p2279154482818"><a name="zh-cn_topic_0108272830_p2279154482818"></a><a name="zh-cn_topic_0108272830_p2279154482818"></a>请根据错误提示进行定位，若无法解决，请联系<span id="zh-cn_topic_0108272830_text38411212103814"><a name="zh-cn_topic_0108272830_text38411212103814"></a><a name="zh-cn_topic_0108272830_text38411212103814"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row1427954462810"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p16279944152814"><a name="zh-cn_topic_0108272830_p16279944152814"></a><a name="zh-cn_topic_0108272830_p16279944152814"></a>Cdm.1100</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p1527916447282"><a name="zh-cn_topic_0108272830_p1527916447282"></a><a name="zh-cn_topic_0108272830_p1527916447282"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p1127914447287"><a name="zh-cn_topic_0108272830_p1127914447287"></a><a name="zh-cn_topic_0108272830_p1127914447287"></a>表[<em id="zh-cn_topic_0108272830_i6279744102819"><a name="zh-cn_topic_0108272830_i6279744102819"></a><a name="zh-cn_topic_0108272830_i6279744102819"></a>%s</em>]不存在。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p427914472814"><a name="zh-cn_topic_0108272830_p427914472814"></a><a name="zh-cn_topic_0108272830_p427914472814"></a>表不存在。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p13279844132820"><a name="zh-cn_topic_0108272830_p13279844132820"></a><a name="zh-cn_topic_0108272830_p13279844132820"></a>请确认表是否存在，输入正确的表名后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row132791744192817"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p2279154482811"><a name="zh-cn_topic_0108272830_p2279154482811"></a><a name="zh-cn_topic_0108272830_p2279154482811"></a>Cdm.1101</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p162791344112811"><a name="zh-cn_topic_0108272830_p162791344112811"></a><a name="zh-cn_topic_0108272830_p162791344112811"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p12279144122814"><a name="zh-cn_topic_0108272830_p12279144122814"></a><a name="zh-cn_topic_0108272830_p12279144122814"></a>获取连接失败，原因：<em id="zh-cn_topic_0108272830_i14279154418282"><a name="zh-cn_topic_0108272830_i14279154418282"></a><a name="zh-cn_topic_0108272830_i14279154418282"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p132799444286"><a name="zh-cn_topic_0108272830_p132799444286"></a><a name="zh-cn_topic_0108272830_p132799444286"></a>获取连接失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p18279544132818"><a name="zh-cn_topic_0108272830_p18279544132818"></a><a name="zh-cn_topic_0108272830_p18279544132818"></a>请根据错误提示进行定位，若无法解决，请联系<span id="zh-cn_topic_0108272830_text88021313817"><a name="zh-cn_topic_0108272830_text88021313817"></a><a name="zh-cn_topic_0108272830_text88021313817"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row19279104492811"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p527924416286"><a name="zh-cn_topic_0108272830_p527924416286"></a><a name="zh-cn_topic_0108272830_p527924416286"></a>Cdm.1102</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p5279844182817"><a name="zh-cn_topic_0108272830_p5279844182817"></a><a name="zh-cn_topic_0108272830_p5279844182817"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p727954452813"><a name="zh-cn_topic_0108272830_p727954452813"></a><a name="zh-cn_topic_0108272830_p727954452813"></a>创表失败，原因：<em id="zh-cn_topic_0108272830_i72797440285"><a name="zh-cn_topic_0108272830_i72797440285"></a><a name="zh-cn_topic_0108272830_i72797440285"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p17279344102811"><a name="zh-cn_topic_0108272830_p17279344102811"></a><a name="zh-cn_topic_0108272830_p17279344102811"></a>创建表失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p1279154442819"><a name="zh-cn_topic_0108272830_p1279154442819"></a><a name="zh-cn_topic_0108272830_p1279154442819"></a>请根据错误提示进行定位，若无法解决，请联系<span id="zh-cn_topic_0108272830_text633121318388"><a name="zh-cn_topic_0108272830_text633121318388"></a><a name="zh-cn_topic_0108272830_text633121318388"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row927934413283"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p7279544142819"><a name="zh-cn_topic_0108272830_p7279544142819"></a><a name="zh-cn_topic_0108272830_p7279544142819"></a>Cdm.1103</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p027994411287"><a name="zh-cn_topic_0108272830_p027994411287"></a><a name="zh-cn_topic_0108272830_p027994411287"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p1279104482820"><a name="zh-cn_topic_0108272830_p1279104482820"></a><a name="zh-cn_topic_0108272830_p1279104482820"></a>未设置Rowkey。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p132791344162810"><a name="zh-cn_topic_0108272830_p132791344162810"></a><a name="zh-cn_topic_0108272830_p132791344162810"></a>未设置Rowkey。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p16279114452818"><a name="zh-cn_topic_0108272830_p16279114452818"></a><a name="zh-cn_topic_0108272830_p16279114452818"></a>请设置Rowkey后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row427920441281"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p327934414284"><a name="zh-cn_topic_0108272830_p327934414284"></a><a name="zh-cn_topic_0108272830_p327934414284"></a>Cdm.1104</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p12791344102812"><a name="zh-cn_topic_0108272830_p12791344102812"></a><a name="zh-cn_topic_0108272830_p12791344102812"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p82791544142816"><a name="zh-cn_topic_0108272830_p82791544142816"></a><a name="zh-cn_topic_0108272830_p82791544142816"></a>打开表格失败。原因：<em id="zh-cn_topic_0108272830_i02791844112810"><a name="zh-cn_topic_0108272830_i02791844112810"></a><a name="zh-cn_topic_0108272830_i02791844112810"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p1327974414282"><a name="zh-cn_topic_0108272830_p1327974414282"></a><a name="zh-cn_topic_0108272830_p1327974414282"></a>打开表格失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p7279744202819"><a name="zh-cn_topic_0108272830_p7279744202819"></a><a name="zh-cn_topic_0108272830_p7279744202819"></a>请根据错误提示进行定位，若无法解决，请联系<span id="zh-cn_topic_0108272830_text45654134385"><a name="zh-cn_topic_0108272830_text45654134385"></a><a name="zh-cn_topic_0108272830_text45654134385"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row427944462817"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p13279944132814"><a name="zh-cn_topic_0108272830_p13279944132814"></a><a name="zh-cn_topic_0108272830_p13279944132814"></a>Cdm.1105</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p1027917446289"><a name="zh-cn_topic_0108272830_p1027917446289"></a><a name="zh-cn_topic_0108272830_p1027917446289"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p18279134452817"><a name="zh-cn_topic_0108272830_p18279134452817"></a><a name="zh-cn_topic_0108272830_p18279134452817"></a>作业初始化失败。原因<em id="zh-cn_topic_0108272830_i17279124413286"><a name="zh-cn_topic_0108272830_i17279124413286"></a><a name="zh-cn_topic_0108272830_i17279124413286"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p2280344162819"><a name="zh-cn_topic_0108272830_p2280344162819"></a><a name="zh-cn_topic_0108272830_p2280344162819"></a>作业初始化失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p102801544182820"><a name="zh-cn_topic_0108272830_p102801544182820"></a><a name="zh-cn_topic_0108272830_p102801544182820"></a>请根据错误提示进行定位，若无法解决，请联系<span id="zh-cn_topic_0108272830_text5815313123816"><a name="zh-cn_topic_0108272830_text5815313123816"></a><a name="zh-cn_topic_0108272830_text5815313123816"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row22808443280"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p1280134402814"><a name="zh-cn_topic_0108272830_p1280134402814"></a><a name="zh-cn_topic_0108272830_p1280134402814"></a>Cdm.1111</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p1028020446286"><a name="zh-cn_topic_0108272830_p1028020446286"></a><a name="zh-cn_topic_0108272830_p1028020446286"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p15280204412812"><a name="zh-cn_topic_0108272830_p15280204412812"></a><a name="zh-cn_topic_0108272830_p15280204412812"></a>表名不能为空。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p628014442285"><a name="zh-cn_topic_0108272830_p628014442285"></a><a name="zh-cn_topic_0108272830_p628014442285"></a>表名为空。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p828254413288"><a name="zh-cn_topic_0108272830_p828254413288"></a><a name="zh-cn_topic_0108272830_p828254413288"></a>请输入正确的表名后，再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row1928294412811"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p102829443280"><a name="zh-cn_topic_0108272830_p102829443280"></a><a name="zh-cn_topic_0108272830_p102829443280"></a>Cdm.1114</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p19282124452812"><a name="zh-cn_topic_0108272830_p19282124452812"></a><a name="zh-cn_topic_0108272830_p19282124452812"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p1628214432818"><a name="zh-cn_topic_0108272830_p1628214432818"></a><a name="zh-cn_topic_0108272830_p1628214432818"></a>Rowkey为空，请在字段映射步骤重新设置。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p5282134411286"><a name="zh-cn_topic_0108272830_p5282134411286"></a><a name="zh-cn_topic_0108272830_p5282134411286"></a>Rowkey为空。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p112821144122817"><a name="zh-cn_topic_0108272830_p112821144122817"></a><a name="zh-cn_topic_0108272830_p112821144122817"></a>请按照错误提示进行处理。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row828214482810"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p8282104482811"><a name="zh-cn_topic_0108272830_p8282104482811"></a><a name="zh-cn_topic_0108272830_p8282104482811"></a>Cdm.1115</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p52821744112811"><a name="zh-cn_topic_0108272830_p52821744112811"></a><a name="zh-cn_topic_0108272830_p52821744112811"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p102821344192815"><a name="zh-cn_topic_0108272830_p102821344192815"></a><a name="zh-cn_topic_0108272830_p102821344192815"></a>Columns为空，请在字段映射步骤重新设置。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p828216446286"><a name="zh-cn_topic_0108272830_p828216446286"></a><a name="zh-cn_topic_0108272830_p828216446286"></a>Columns为空。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p428264416282"><a name="zh-cn_topic_0108272830_p428264416282"></a><a name="zh-cn_topic_0108272830_p428264416282"></a>请按照错误提示进行处理。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row528211448285"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p162821544132814"><a name="zh-cn_topic_0108272830_p162821544132814"></a><a name="zh-cn_topic_0108272830_p162821544132814"></a>Cdm.1116</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p122820446289"><a name="zh-cn_topic_0108272830_p122820446289"></a><a name="zh-cn_topic_0108272830_p122820446289"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p82821244132811"><a name="zh-cn_topic_0108272830_p82821244132811"></a><a name="zh-cn_topic_0108272830_p82821244132811"></a>列名重复，请在字段映射步骤重新设置。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p19282174442810"><a name="zh-cn_topic_0108272830_p19282174442810"></a><a name="zh-cn_topic_0108272830_p19282174442810"></a>列名重复。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p128218449281"><a name="zh-cn_topic_0108272830_p128218449281"></a><a name="zh-cn_topic_0108272830_p128218449281"></a>请按照错误提示进行处理。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row7282124414283"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p1528274402812"><a name="zh-cn_topic_0108272830_p1528274402812"></a><a name="zh-cn_topic_0108272830_p1528274402812"></a>Cdm.1117</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p20282104422817"><a name="zh-cn_topic_0108272830_p20282104422817"></a><a name="zh-cn_topic_0108272830_p20282104422817"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p192826445285"><a name="zh-cn_topic_0108272830_p192826445285"></a><a name="zh-cn_topic_0108272830_p192826445285"></a>判断表格是否存在失败，原因：<em id="zh-cn_topic_0108272830_i42821744172811"><a name="zh-cn_topic_0108272830_i42821744172811"></a><a name="zh-cn_topic_0108272830_i42821744172811"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p11283164422815"><a name="zh-cn_topic_0108272830_p11283164422815"></a><a name="zh-cn_topic_0108272830_p11283164422815"></a>判断表格是否存在失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p328344410285"><a name="zh-cn_topic_0108272830_p328344410285"></a><a name="zh-cn_topic_0108272830_p328344410285"></a>请根据错误提示进行定位，若无法解决，请联系<span id="zh-cn_topic_0108272830_text641114203817"><a name="zh-cn_topic_0108272830_text641114203817"></a><a name="zh-cn_topic_0108272830_text641114203817"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row6283184492816"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p1128317449285"><a name="zh-cn_topic_0108272830_p1128317449285"></a><a name="zh-cn_topic_0108272830_p1128317449285"></a>Cdm.1118</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p1128364417282"><a name="zh-cn_topic_0108272830_p1128364417282"></a><a name="zh-cn_topic_0108272830_p1128364417282"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p18283544172816"><a name="zh-cn_topic_0108272830_p18283544172816"></a><a name="zh-cn_topic_0108272830_p18283544172816"></a>表<em id="zh-cn_topic_0108272830_i528364442810"><a name="zh-cn_topic_0108272830_i528364442810"></a><a name="zh-cn_topic_0108272830_i528364442810"></a>%s</em>不包含列族<em id="zh-cn_topic_0108272830_i1728344462811"><a name="zh-cn_topic_0108272830_i1728344462811"></a><a name="zh-cn_topic_0108272830_i1728344462811"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p4283444112812"><a name="zh-cn_topic_0108272830_p4283444112812"></a><a name="zh-cn_topic_0108272830_p4283444112812"></a>表中不包含列族。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p7283144442820"><a name="zh-cn_topic_0108272830_p7283144442820"></a><a name="zh-cn_topic_0108272830_p7283144442820"></a>请指定列族后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row32830445286"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p1028394492812"><a name="zh-cn_topic_0108272830_p1028394492812"></a><a name="zh-cn_topic_0108272830_p1028394492812"></a>Cdm.1120</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p182831447283"><a name="zh-cn_topic_0108272830_p182831447283"></a><a name="zh-cn_topic_0108272830_p182831447283"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p32831444152811"><a name="zh-cn_topic_0108272830_p32831444152811"></a><a name="zh-cn_topic_0108272830_p32831444152811"></a>表中有数据，请清空表数据或重新设置导入前是否清空表数据配置项。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p172831844112812"><a name="zh-cn_topic_0108272830_p172831844112812"></a><a name="zh-cn_topic_0108272830_p172831844112812"></a>表中有数据，请清空表数据或重新设置导入前是否清空表数据配置项。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p1428415449288"><a name="zh-cn_topic_0108272830_p1428415449288"></a><a name="zh-cn_topic_0108272830_p1428415449288"></a>请按照错误提示进行处理。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row17284144402810"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p42848440287"><a name="zh-cn_topic_0108272830_p42848440287"></a><a name="zh-cn_topic_0108272830_p42848440287"></a>Cdm.1121</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p32841844142817"><a name="zh-cn_topic_0108272830_p32841844142817"></a><a name="zh-cn_topic_0108272830_p32841844142817"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p82841644192820"><a name="zh-cn_topic_0108272830_p82841644192820"></a><a name="zh-cn_topic_0108272830_p82841644192820"></a>关闭连接已失败。原因：<em id="zh-cn_topic_0108272830_i428474419282"><a name="zh-cn_topic_0108272830_i428474419282"></a><a name="zh-cn_topic_0108272830_i428474419282"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p2028410447280"><a name="zh-cn_topic_0108272830_p2028410447280"></a><a name="zh-cn_topic_0108272830_p2028410447280"></a>关闭连接失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p112846441287"><a name="zh-cn_topic_0108272830_p112846441287"></a><a name="zh-cn_topic_0108272830_p112846441287"></a>请根据错误提示进行定位，若无法解决，请联系<span id="zh-cn_topic_0108272830_text1730911142389"><a name="zh-cn_topic_0108272830_text1730911142389"></a><a name="zh-cn_topic_0108272830_text1730911142389"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row7284174462816"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p228464492815"><a name="zh-cn_topic_0108272830_p228464492815"></a><a name="zh-cn_topic_0108272830_p228464492815"></a>Cdm.1201</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p72847447281"><a name="zh-cn_topic_0108272830_p72847447281"></a><a name="zh-cn_topic_0108272830_p72847447281"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p16284144172813"><a name="zh-cn_topic_0108272830_p16284144172813"></a><a name="zh-cn_topic_0108272830_p16284144172813"></a>不能连接到Redis服务器，原因：<em id="zh-cn_topic_0108272830_i228464482819"><a name="zh-cn_topic_0108272830_i228464482819"></a><a name="zh-cn_topic_0108272830_i228464482819"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p5284184422812"><a name="zh-cn_topic_0108272830_p5284184422812"></a><a name="zh-cn_topic_0108272830_p5284184422812"></a>无法连接到Redis服务器。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p228414452810"><a name="zh-cn_topic_0108272830_p228414452810"></a><a name="zh-cn_topic_0108272830_p228414452810"></a>请根据错误提示进行定位，若无法解决，请联系<span id="zh-cn_topic_0108272830_text16515514123812"><a name="zh-cn_topic_0108272830_text16515514123812"></a><a name="zh-cn_topic_0108272830_text16515514123812"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row1128474415289"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p2284194412815"><a name="zh-cn_topic_0108272830_p2284194412815"></a><a name="zh-cn_topic_0108272830_p2284194412815"></a>Cdm.1203</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p4284044152819"><a name="zh-cn_topic_0108272830_p4284044152819"></a><a name="zh-cn_topic_0108272830_p4284044152819"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p528454492814"><a name="zh-cn_topic_0108272830_p528454492814"></a><a name="zh-cn_topic_0108272830_p528454492814"></a>从Redis服务器抽取数据失败，原因：<em id="zh-cn_topic_0108272830_i628474417282"><a name="zh-cn_topic_0108272830_i628474417282"></a><a name="zh-cn_topic_0108272830_i628474417282"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p1528444416288"><a name="zh-cn_topic_0108272830_p1528444416288"></a><a name="zh-cn_topic_0108272830_p1528444416288"></a>从Redis服务器获取数据失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p62841844102815"><a name="zh-cn_topic_0108272830_p62841844102815"></a><a name="zh-cn_topic_0108272830_p62841844102815"></a>请根据错误提示进行定位，若无法解决，请联系<span id="zh-cn_topic_0108272830_text157516148388"><a name="zh-cn_topic_0108272830_text157516148388"></a><a name="zh-cn_topic_0108272830_text157516148388"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row228414416289"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p2028434415281"><a name="zh-cn_topic_0108272830_p2028434415281"></a><a name="zh-cn_topic_0108272830_p2028434415281"></a>Cdm.1205</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p7284194492815"><a name="zh-cn_topic_0108272830_p7284194492815"></a><a name="zh-cn_topic_0108272830_p7284194492815"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p1528464414281"><a name="zh-cn_topic_0108272830_p1528464414281"></a><a name="zh-cn_topic_0108272830_p1528464414281"></a>Redis值前缀不能为空白符。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p228494432816"><a name="zh-cn_topic_0108272830_p228494432816"></a><a name="zh-cn_topic_0108272830_p228494432816"></a>Redis值前缀不能为空白符。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p228474411282"><a name="zh-cn_topic_0108272830_p228474411282"></a><a name="zh-cn_topic_0108272830_p228474411282"></a>请去除Redis前缀前的空白符，然后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row728444402816"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p2028564414284"><a name="zh-cn_topic_0108272830_p2028564414284"></a><a name="zh-cn_topic_0108272830_p2028564414284"></a>Cdm.1206</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p10285124420288"><a name="zh-cn_topic_0108272830_p10285124420288"></a><a name="zh-cn_topic_0108272830_p10285124420288"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p4285244202817"><a name="zh-cn_topic_0108272830_p4285244202817"></a><a name="zh-cn_topic_0108272830_p4285244202817"></a>Redis值存储类型必须指定为“string”或“hash”。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p1328511444282"><a name="zh-cn_topic_0108272830_p1328511444282"></a><a name="zh-cn_topic_0108272830_p1328511444282"></a>Redis值存储类型必须指定为“string”或“hash”。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p1928574418285"><a name="zh-cn_topic_0108272830_p1928574418285"></a><a name="zh-cn_topic_0108272830_p1928574418285"></a>请按照错误提示进行处理。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row17285544192815"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p2285114482817"><a name="zh-cn_topic_0108272830_p2285114482817"></a><a name="zh-cn_topic_0108272830_p2285114482817"></a>Cdm.1207</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p7285544132812"><a name="zh-cn_topic_0108272830_p7285544132812"></a><a name="zh-cn_topic_0108272830_p7285544132812"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p7285194442812"><a name="zh-cn_topic_0108272830_p7285194442812"></a><a name="zh-cn_topic_0108272830_p7285194442812"></a>当值存储类型为“string”时，必须指定值分隔符。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p1128510449284"><a name="zh-cn_topic_0108272830_p1128510449284"></a><a name="zh-cn_topic_0108272830_p1128510449284"></a>值存储类型为“string”，未指定值分隔符。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p16285044152819"><a name="zh-cn_topic_0108272830_p16285044152819"></a><a name="zh-cn_topic_0108272830_p16285044152819"></a>请指定分隔符后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row5285204417288"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p5285114452819"><a name="zh-cn_topic_0108272830_p5285114452819"></a><a name="zh-cn_topic_0108272830_p5285114452819"></a>Cdm.1208</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p32859446284"><a name="zh-cn_topic_0108272830_p32859446284"></a><a name="zh-cn_topic_0108272830_p32859446284"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p42851144132817"><a name="zh-cn_topic_0108272830_p42851144132817"></a><a name="zh-cn_topic_0108272830_p42851144132817"></a>Redis存储字段列表必须指定。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p202857447287"><a name="zh-cn_topic_0108272830_p202857447287"></a><a name="zh-cn_topic_0108272830_p202857447287"></a>Redis存储字段列表未指定。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p2285124413289"><a name="zh-cn_topic_0108272830_p2285124413289"></a><a name="zh-cn_topic_0108272830_p2285124413289"></a>请指定Redis存储字段列表后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row12850449286"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p14285144182816"><a name="zh-cn_topic_0108272830_p14285144182816"></a><a name="zh-cn_topic_0108272830_p14285144182816"></a>Cdm.1209</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p328564492816"><a name="zh-cn_topic_0108272830_p328564492816"></a><a name="zh-cn_topic_0108272830_p328564492816"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p3291204410284"><a name="zh-cn_topic_0108272830_p3291204410284"></a><a name="zh-cn_topic_0108272830_p3291204410284"></a>Redis键分隔符不能为空白符。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p13291124417284"><a name="zh-cn_topic_0108272830_p13291124417284"></a><a name="zh-cn_topic_0108272830_p13291124417284"></a>Redis键分隔符不能为空白符。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p129110448289"><a name="zh-cn_topic_0108272830_p129110448289"></a><a name="zh-cn_topic_0108272830_p129110448289"></a>请输入正确的分隔符后，再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row4291194419286"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p132911444202817"><a name="zh-cn_topic_0108272830_p132911444202817"></a><a name="zh-cn_topic_0108272830_p132911444202817"></a>Cdm.1210</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p14291144432811"><a name="zh-cn_topic_0108272830_p14291144432811"></a><a name="zh-cn_topic_0108272830_p14291144432811"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p1329184416289"><a name="zh-cn_topic_0108272830_p1329184416289"></a><a name="zh-cn_topic_0108272830_p1329184416289"></a>必须指定Redis主键字段列表。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p2291144102815"><a name="zh-cn_topic_0108272830_p2291144102815"></a><a name="zh-cn_topic_0108272830_p2291144102815"></a>Redis主键字段列表未指定。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p929215444289"><a name="zh-cn_topic_0108272830_p929215444289"></a><a name="zh-cn_topic_0108272830_p929215444289"></a>请指定Redis主键字段列表后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row3292844152812"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p1929274402817"><a name="zh-cn_topic_0108272830_p1929274402817"></a><a name="zh-cn_topic_0108272830_p1929274402817"></a>Cdm.1211</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p92928443289"><a name="zh-cn_topic_0108272830_p92928443289"></a><a name="zh-cn_topic_0108272830_p92928443289"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p4292644102812"><a name="zh-cn_topic_0108272830_p4292644102812"></a><a name="zh-cn_topic_0108272830_p4292644102812"></a>Redis主键字段列表必须在字段列表中存在。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p11292164422816"><a name="zh-cn_topic_0108272830_p11292164422816"></a><a name="zh-cn_topic_0108272830_p11292164422816"></a>Redis主键字段列表不在字段列表中。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p2292184416281"><a name="zh-cn_topic_0108272830_p2292184416281"></a><a name="zh-cn_topic_0108272830_p2292184416281"></a>请指定Redis主键字段列表后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row13292644132817"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p32928447281"><a name="zh-cn_topic_0108272830_p32928447281"></a><a name="zh-cn_topic_0108272830_p32928447281"></a>Cdm.1213</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p1029204416284"><a name="zh-cn_topic_0108272830_p1029204416284"></a><a name="zh-cn_topic_0108272830_p1029204416284"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p9292644132817"><a name="zh-cn_topic_0108272830_p9292644132817"></a><a name="zh-cn_topic_0108272830_p9292644132817"></a>必须指定Redis服务器列表。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p14292194432810"><a name="zh-cn_topic_0108272830_p14292194432810"></a><a name="zh-cn_topic_0108272830_p14292194432810"></a>未指定Redis服务器列表。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p529224418284"><a name="zh-cn_topic_0108272830_p529224418284"></a><a name="zh-cn_topic_0108272830_p529224418284"></a>请指定Redis服务器列表后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row5292244132812"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p5292344122812"><a name="zh-cn_topic_0108272830_p5292344122812"></a><a name="zh-cn_topic_0108272830_p5292344122812"></a>Cdm.1301</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p729214412285"><a name="zh-cn_topic_0108272830_p729214412285"></a><a name="zh-cn_topic_0108272830_p729214412285"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p1229294411286"><a name="zh-cn_topic_0108272830_p1229294411286"></a><a name="zh-cn_topic_0108272830_p1229294411286"></a>不能连接到MongoDB服务器，原因：<em id="zh-cn_topic_0108272830_i1729212443287"><a name="zh-cn_topic_0108272830_i1729212443287"></a><a name="zh-cn_topic_0108272830_i1729212443287"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p11292204420283"><a name="zh-cn_topic_0108272830_p11292204420283"></a><a name="zh-cn_topic_0108272830_p11292204420283"></a>连接到MongoDB服务器失败</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p5292104462816"><a name="zh-cn_topic_0108272830_p5292104462816"></a><a name="zh-cn_topic_0108272830_p5292104462816"></a>请根据错误提示进行定位，若无法解决，请联系<span id="zh-cn_topic_0108272830_text119679144389"><a name="zh-cn_topic_0108272830_text119679144389"></a><a name="zh-cn_topic_0108272830_text119679144389"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row6292164417285"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p529244422816"><a name="zh-cn_topic_0108272830_p529244422816"></a><a name="zh-cn_topic_0108272830_p529244422816"></a>Cdm.1302</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p329294418285"><a name="zh-cn_topic_0108272830_p329294418285"></a><a name="zh-cn_topic_0108272830_p329294418285"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p14292114414284"><a name="zh-cn_topic_0108272830_p14292114414284"></a><a name="zh-cn_topic_0108272830_p14292114414284"></a>从MongoDB服务器抽取数据失败，原因：<em id="zh-cn_topic_0108272830_i429234419289"><a name="zh-cn_topic_0108272830_i429234419289"></a><a name="zh-cn_topic_0108272830_i429234419289"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p1629284412281"><a name="zh-cn_topic_0108272830_p1629284412281"></a><a name="zh-cn_topic_0108272830_p1629284412281"></a>从MongoDB服务器抽取数据失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p52921544102813"><a name="zh-cn_topic_0108272830_p52921544102813"></a><a name="zh-cn_topic_0108272830_p52921544102813"></a>请根据错误提示进行定位，若无法解决，请联系<span id="zh-cn_topic_0108272830_text4221415203812"><a name="zh-cn_topic_0108272830_text4221415203812"></a><a name="zh-cn_topic_0108272830_text4221415203812"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row529254482820"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p1829224472810"><a name="zh-cn_topic_0108272830_p1829224472810"></a><a name="zh-cn_topic_0108272830_p1829224472810"></a>Cdm.1304</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p11292144416285"><a name="zh-cn_topic_0108272830_p11292144416285"></a><a name="zh-cn_topic_0108272830_p11292144416285"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p42931244122812"><a name="zh-cn_topic_0108272830_p42931244122812"></a><a name="zh-cn_topic_0108272830_p42931244122812"></a>必须指定MongoDB服务器的集合。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p11293644132810"><a name="zh-cn_topic_0108272830_p11293644132810"></a><a name="zh-cn_topic_0108272830_p11293644132810"></a>未指定MongoDB服务器的集合。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p15293124412282"><a name="zh-cn_topic_0108272830_p15293124412282"></a><a name="zh-cn_topic_0108272830_p15293124412282"></a>未指定MongoDB服务器的集合，请指定后，再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row19293244192819"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p629320442287"><a name="zh-cn_topic_0108272830_p629320442287"></a><a name="zh-cn_topic_0108272830_p629320442287"></a>Cdm.1305</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p17293184415283"><a name="zh-cn_topic_0108272830_p17293184415283"></a><a name="zh-cn_topic_0108272830_p17293184415283"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p6293194432819"><a name="zh-cn_topic_0108272830_p6293194432819"></a><a name="zh-cn_topic_0108272830_p6293194432819"></a>必须指定MongoDB服务列表。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p02931944202818"><a name="zh-cn_topic_0108272830_p02931944202818"></a><a name="zh-cn_topic_0108272830_p02931944202818"></a>未指定MongoDB服务列表。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p1929311441285"><a name="zh-cn_topic_0108272830_p1929311441285"></a><a name="zh-cn_topic_0108272830_p1929311441285"></a>未指定MongoDB服务列表，请指定后，再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row22931144112814"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p429317445282"><a name="zh-cn_topic_0108272830_p429317445282"></a><a name="zh-cn_topic_0108272830_p429317445282"></a>Cdm.1306</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p529304420287"><a name="zh-cn_topic_0108272830_p529304420287"></a><a name="zh-cn_topic_0108272830_p529304420287"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p1829314462812"><a name="zh-cn_topic_0108272830_p1829314462812"></a><a name="zh-cn_topic_0108272830_p1829314462812"></a>必须指定MongoDB服务的数据库名称。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p1629320447289"><a name="zh-cn_topic_0108272830_p1629320447289"></a><a name="zh-cn_topic_0108272830_p1629320447289"></a>未指定MongoDB服务的数据库名称。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p1429312440285"><a name="zh-cn_topic_0108272830_p1429312440285"></a><a name="zh-cn_topic_0108272830_p1429312440285"></a>未指定MongoDB服务的数据库名称，请指定数据库后，再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row729324413286"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p329314412816"><a name="zh-cn_topic_0108272830_p329314412816"></a><a name="zh-cn_topic_0108272830_p329314412816"></a>Cdm.1307</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p6293344152817"><a name="zh-cn_topic_0108272830_p6293344152817"></a><a name="zh-cn_topic_0108272830_p6293344152817"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p16293344202811"><a name="zh-cn_topic_0108272830_p16293344202811"></a><a name="zh-cn_topic_0108272830_p16293344202811"></a>必须指定MongoDB服务的字段列表。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p15293124452818"><a name="zh-cn_topic_0108272830_p15293124452818"></a><a name="zh-cn_topic_0108272830_p15293124452818"></a>未指定MongoDB服务的字段列表。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p182933445284"><a name="zh-cn_topic_0108272830_p182933445284"></a><a name="zh-cn_topic_0108272830_p182933445284"></a>未指定MongoDB服务的字段列表，请指定字段列表后，再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row729304422813"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p329334414281"><a name="zh-cn_topic_0108272830_p329334414281"></a><a name="zh-cn_topic_0108272830_p329334414281"></a>Cdm.1501</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p329316445287"><a name="zh-cn_topic_0108272830_p329316445287"></a><a name="zh-cn_topic_0108272830_p329316445287"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p5293204472817"><a name="zh-cn_topic_0108272830_p5293204472817"></a><a name="zh-cn_topic_0108272830_p5293204472817"></a>不能连接到Elasticsearch服务器，原因：<em id="zh-cn_topic_0108272830_i16293194472815"><a name="zh-cn_topic_0108272830_i16293194472815"></a><a name="zh-cn_topic_0108272830_i16293194472815"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p16293134482813"><a name="zh-cn_topic_0108272830_p16293134482813"></a><a name="zh-cn_topic_0108272830_p16293134482813"></a>无法连接到Elasticsearch服务器</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p15293124452810"><a name="zh-cn_topic_0108272830_p15293124452810"></a><a name="zh-cn_topic_0108272830_p15293124452810"></a>请根据错误提示进行定位，若无法解决，请联系<span id="zh-cn_topic_0108272830_text1470701511389"><a name="zh-cn_topic_0108272830_text1470701511389"></a><a name="zh-cn_topic_0108272830_text1470701511389"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row92931244162815"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p1293124482820"><a name="zh-cn_topic_0108272830_p1293124482820"></a><a name="zh-cn_topic_0108272830_p1293124482820"></a>Cdm.1502</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p629310441281"><a name="zh-cn_topic_0108272830_p629310441281"></a><a name="zh-cn_topic_0108272830_p629310441281"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p1829414411289"><a name="zh-cn_topic_0108272830_p1829414411289"></a><a name="zh-cn_topic_0108272830_p1829414411289"></a>向Elasticsearch服务器写入数据失败，原因：<em id="zh-cn_topic_0108272830_i15294134419287"><a name="zh-cn_topic_0108272830_i15294134419287"></a><a name="zh-cn_topic_0108272830_i15294134419287"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p12294154472818"><a name="zh-cn_topic_0108272830_p12294154472818"></a><a name="zh-cn_topic_0108272830_p12294154472818"></a>向Elasticsearch服务器写入数据失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p19294154402811"><a name="zh-cn_topic_0108272830_p19294154402811"></a><a name="zh-cn_topic_0108272830_p19294154402811"></a>请根据错误提示进行定位，若无法解决，请联系<span id="zh-cn_topic_0108272830_text15945815133817"><a name="zh-cn_topic_0108272830_text15945815133817"></a><a name="zh-cn_topic_0108272830_text15945815133817"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row3294144422816"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p1929414414288"><a name="zh-cn_topic_0108272830_p1929414414288"></a><a name="zh-cn_topic_0108272830_p1929414414288"></a>Cdm.1503</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p162943449286"><a name="zh-cn_topic_0108272830_p162943449286"></a><a name="zh-cn_topic_0108272830_p162943449286"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p11294134442815"><a name="zh-cn_topic_0108272830_p11294134442815"></a><a name="zh-cn_topic_0108272830_p11294134442815"></a>关闭Elasticsearch连接失败，原因：<em id="zh-cn_topic_0108272830_i10294444102820"><a name="zh-cn_topic_0108272830_i10294444102820"></a><a name="zh-cn_topic_0108272830_i10294444102820"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p3294204422810"><a name="zh-cn_topic_0108272830_p3294204422810"></a><a name="zh-cn_topic_0108272830_p3294204422810"></a>关闭Elasticsearch连接失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p92944444286"><a name="zh-cn_topic_0108272830_p92944444286"></a><a name="zh-cn_topic_0108272830_p92944444286"></a>请根据错误提示进行定位，若无法解决，请联系<span id="zh-cn_topic_0108272830_text11201151612383"><a name="zh-cn_topic_0108272830_text11201151612383"></a><a name="zh-cn_topic_0108272830_text11201151612383"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row9294144112818"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p11294184413288"><a name="zh-cn_topic_0108272830_p11294184413288"></a><a name="zh-cn_topic_0108272830_p11294184413288"></a>Cdm.1504</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p112942044122815"><a name="zh-cn_topic_0108272830_p112942044122815"></a><a name="zh-cn_topic_0108272830_p112942044122815"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p1329444418289"><a name="zh-cn_topic_0108272830_p1329444418289"></a><a name="zh-cn_topic_0108272830_p1329444418289"></a>获取Elasticsearch索引错误，原因：<em id="zh-cn_topic_0108272830_i929444482810"><a name="zh-cn_topic_0108272830_i929444482810"></a><a name="zh-cn_topic_0108272830_i929444482810"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p15294944152812"><a name="zh-cn_topic_0108272830_p15294944152812"></a><a name="zh-cn_topic_0108272830_p15294944152812"></a>获取Elasticsearch索引错误</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p152942044172816"><a name="zh-cn_topic_0108272830_p152942044172816"></a><a name="zh-cn_topic_0108272830_p152942044172816"></a>请根据错误提示进行定位，若无法解决，请联系<span id="zh-cn_topic_0108272830_text164091816123810"><a name="zh-cn_topic_0108272830_text164091816123810"></a><a name="zh-cn_topic_0108272830_text164091816123810"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row12941644102818"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p5294344142820"><a name="zh-cn_topic_0108272830_p5294344142820"></a><a name="zh-cn_topic_0108272830_p5294344142820"></a>Cdm.1505</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p13294204482813"><a name="zh-cn_topic_0108272830_p13294204482813"></a><a name="zh-cn_topic_0108272830_p13294204482813"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p62941744202814"><a name="zh-cn_topic_0108272830_p62941744202814"></a><a name="zh-cn_topic_0108272830_p62941744202814"></a>获取Elasticsearch类型错误，原因：<em id="zh-cn_topic_0108272830_i82944449285"><a name="zh-cn_topic_0108272830_i82944449285"></a><a name="zh-cn_topic_0108272830_i82944449285"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p6294154413287"><a name="zh-cn_topic_0108272830_p6294154413287"></a><a name="zh-cn_topic_0108272830_p6294154413287"></a>获取Elasticsearch类型错误。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p172941344192817"><a name="zh-cn_topic_0108272830_p172941344192817"></a><a name="zh-cn_topic_0108272830_p172941344192817"></a>请根据错误提示进行定位，若无法解决，请联系<span id="zh-cn_topic_0108272830_text4657816193811"><a name="zh-cn_topic_0108272830_text4657816193811"></a><a name="zh-cn_topic_0108272830_text4657816193811"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row7294154442819"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p15294244132812"><a name="zh-cn_topic_0108272830_p15294244132812"></a><a name="zh-cn_topic_0108272830_p15294244132812"></a>Cdm.1506</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p11294104410283"><a name="zh-cn_topic_0108272830_p11294104410283"></a><a name="zh-cn_topic_0108272830_p11294104410283"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p1294134472810"><a name="zh-cn_topic_0108272830_p1294134472810"></a><a name="zh-cn_topic_0108272830_p1294134472810"></a>获取Elasticsearch文档字段错误，原因：<em id="zh-cn_topic_0108272830_i32941144142811"><a name="zh-cn_topic_0108272830_i32941144142811"></a><a name="zh-cn_topic_0108272830_i32941144142811"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p15294744122819"><a name="zh-cn_topic_0108272830_p15294744122819"></a><a name="zh-cn_topic_0108272830_p15294744122819"></a>获取Elasticsearch文档字段错误。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p18294444152816"><a name="zh-cn_topic_0108272830_p18294444152816"></a><a name="zh-cn_topic_0108272830_p18294444152816"></a>请根据错误提示进行定位，若无法解决，请联系<span id="zh-cn_topic_0108272830_text288561663815"><a name="zh-cn_topic_0108272830_text288561663815"></a><a name="zh-cn_topic_0108272830_text288561663815"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row1294244182817"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p1429417443289"><a name="zh-cn_topic_0108272830_p1429417443289"></a><a name="zh-cn_topic_0108272830_p1429417443289"></a>Cdm.1508</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p4294644202811"><a name="zh-cn_topic_0108272830_p4294644202811"></a><a name="zh-cn_topic_0108272830_p4294644202811"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p16294104415287"><a name="zh-cn_topic_0108272830_p16294104415287"></a><a name="zh-cn_topic_0108272830_p16294104415287"></a>必须指定Elasticsearch服务器主机名或IP地址。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p152951144182817"><a name="zh-cn_topic_0108272830_p152951144182817"></a><a name="zh-cn_topic_0108272830_p152951144182817"></a>未指定Elasticsearch服务器主机名或IP地址。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p132951444152815"><a name="zh-cn_topic_0108272830_p132951444152815"></a><a name="zh-cn_topic_0108272830_p132951444152815"></a>未指定Elasticsearch服务器主机名或IP地址，请指定后，再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row729534492820"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p1329564415289"><a name="zh-cn_topic_0108272830_p1329564415289"></a><a name="zh-cn_topic_0108272830_p1329564415289"></a>Cdm.1510</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p1729519443281"><a name="zh-cn_topic_0108272830_p1729519443281"></a><a name="zh-cn_topic_0108272830_p1729519443281"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p14295154462818"><a name="zh-cn_topic_0108272830_p14295154462818"></a><a name="zh-cn_topic_0108272830_p14295154462818"></a>必须指定Elasticsearch索引。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p1029564432813"><a name="zh-cn_topic_0108272830_p1029564432813"></a><a name="zh-cn_topic_0108272830_p1029564432813"></a>未指定Elasticsearch索引。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p6295154402818"><a name="zh-cn_topic_0108272830_p6295154402818"></a><a name="zh-cn_topic_0108272830_p6295154402818"></a>当前未指定Elasticsearch索引，请指定后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row202951544102810"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p9295204492811"><a name="zh-cn_topic_0108272830_p9295204492811"></a><a name="zh-cn_topic_0108272830_p9295204492811"></a>Cdm.1511</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p429544462815"><a name="zh-cn_topic_0108272830_p429544462815"></a><a name="zh-cn_topic_0108272830_p429544462815"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p9295744172818"><a name="zh-cn_topic_0108272830_p9295744172818"></a><a name="zh-cn_topic_0108272830_p9295744172818"></a>必须指定Elasticsearch类型。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p429564413288"><a name="zh-cn_topic_0108272830_p429564413288"></a><a name="zh-cn_topic_0108272830_p429564413288"></a>未指定Elasticsearch类型。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p829518442280"><a name="zh-cn_topic_0108272830_p829518442280"></a><a name="zh-cn_topic_0108272830_p829518442280"></a>当前未指定Elasticsearch类型，请指定后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row2295154415288"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p16295174492815"><a name="zh-cn_topic_0108272830_p16295174492815"></a><a name="zh-cn_topic_0108272830_p16295174492815"></a>Cdm.1513</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p102951344192818"><a name="zh-cn_topic_0108272830_p102951344192818"></a><a name="zh-cn_topic_0108272830_p102951344192818"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p10295204416289"><a name="zh-cn_topic_0108272830_p10295204416289"></a><a name="zh-cn_topic_0108272830_p10295204416289"></a>字段列表中必须包含字段类型定义。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p132951944162812"><a name="zh-cn_topic_0108272830_p132951944162812"></a><a name="zh-cn_topic_0108272830_p132951944162812"></a>字段列表中未包含字段类型定义。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p1129574414289"><a name="zh-cn_topic_0108272830_p1129574414289"></a><a name="zh-cn_topic_0108272830_p1129574414289"></a>请确认字段列表中是否包含字段类型定义，修改正确后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row13295194402816"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p2029517443289"><a name="zh-cn_topic_0108272830_p2029517443289"></a><a name="zh-cn_topic_0108272830_p2029517443289"></a>Cdm.1514</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p172954441281"><a name="zh-cn_topic_0108272830_p172954441281"></a><a name="zh-cn_topic_0108272830_p172954441281"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p1829534432812"><a name="zh-cn_topic_0108272830_p1829534432812"></a><a name="zh-cn_topic_0108272830_p1829534432812"></a>字段列表中必须包含主键字段。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p4295184419286"><a name="zh-cn_topic_0108272830_p4295184419286"></a><a name="zh-cn_topic_0108272830_p4295184419286"></a>未设置主键字段。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p14295844102817"><a name="zh-cn_topic_0108272830_p14295844102817"></a><a name="zh-cn_topic_0108272830_p14295844102817"></a>当前未设置主键字段，请设置主键字段后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row122956440287"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p18295194413288"><a name="zh-cn_topic_0108272830_p18295194413288"></a><a name="zh-cn_topic_0108272830_p18295194413288"></a>Cdm.1516</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p7295164411287"><a name="zh-cn_topic_0108272830_p7295164411287"></a><a name="zh-cn_topic_0108272830_p7295164411287"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p102961344132814"><a name="zh-cn_topic_0108272830_p102961344132814"></a><a name="zh-cn_topic_0108272830_p102961344132814"></a>非法列名<em id="zh-cn_topic_0108272830_i1329674417281"><a name="zh-cn_topic_0108272830_i1329674417281"></a><a name="zh-cn_topic_0108272830_i1329674417281"></a>%s</em>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p22960449285"><a name="zh-cn_topic_0108272830_p22960449285"></a><a name="zh-cn_topic_0108272830_p22960449285"></a>列名不合法。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p029610447284"><a name="zh-cn_topic_0108272830_p029610447284"></a><a name="zh-cn_topic_0108272830_p029610447284"></a>请确认列名是否合法，输入正确的列名后再重试。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row7296204413285"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p1529604432815"><a name="zh-cn_topic_0108272830_p1529604432815"></a><a name="zh-cn_topic_0108272830_p1529604432815"></a>Cdm.1517</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p162961644152819"><a name="zh-cn_topic_0108272830_p162961644152819"></a><a name="zh-cn_topic_0108272830_p162961644152819"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p52967444289"><a name="zh-cn_topic_0108272830_p52967444289"></a><a name="zh-cn_topic_0108272830_p52967444289"></a>获取文档数量产生错误。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p17296104492818"><a name="zh-cn_topic_0108272830_p17296104492818"></a><a name="zh-cn_topic_0108272830_p17296104492818"></a>获取文档数量产生错误。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p10296164412817"><a name="zh-cn_topic_0108272830_p10296164412817"></a><a name="zh-cn_topic_0108272830_p10296164412817"></a>请联系<span id="zh-cn_topic_0108272830_text4131111714381"><a name="zh-cn_topic_0108272830_text4131111714381"></a><a name="zh-cn_topic_0108272830_text4131111714381"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row129644420285"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p1929618447288"><a name="zh-cn_topic_0108272830_p1929618447288"></a><a name="zh-cn_topic_0108272830_p1929618447288"></a>Cdm.1519</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p32961449288"><a name="zh-cn_topic_0108272830_p32961449288"></a><a name="zh-cn_topic_0108272830_p32961449288"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p13296194452815"><a name="zh-cn_topic_0108272830_p13296194452815"></a><a name="zh-cn_topic_0108272830_p13296194452815"></a>抽取数据错误。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p12961544162812"><a name="zh-cn_topic_0108272830_p12961544162812"></a><a name="zh-cn_topic_0108272830_p12961544162812"></a>抽取数据错误。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p12296184452814"><a name="zh-cn_topic_0108272830_p12296184452814"></a><a name="zh-cn_topic_0108272830_p12296184452814"></a>请联系<span id="zh-cn_topic_0108272830_text153723171387"><a name="zh-cn_topic_0108272830_text153723171387"></a><a name="zh-cn_topic_0108272830_text153723171387"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row10296194414283"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p9296544162815"><a name="zh-cn_topic_0108272830_p9296544162815"></a><a name="zh-cn_topic_0108272830_p9296544162815"></a>Cdm.1601</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p729617443284"><a name="zh-cn_topic_0108272830_p729617443284"></a><a name="zh-cn_topic_0108272830_p729617443284"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p32961144102817"><a name="zh-cn_topic_0108272830_p32961144102817"></a><a name="zh-cn_topic_0108272830_p32961144102817"></a>连接服务器失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p02961644142812"><a name="zh-cn_topic_0108272830_p02961644142812"></a><a name="zh-cn_topic_0108272830_p02961644142812"></a>连接服务器失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p82961344182811"><a name="zh-cn_topic_0108272830_p82961344182811"></a><a name="zh-cn_topic_0108272830_p82961344182811"></a>请联系<span id="zh-cn_topic_0108272830_text56321517143816"><a name="zh-cn_topic_0108272830_text56321517143816"></a><a name="zh-cn_topic_0108272830_text56321517143816"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row02961544172818"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p14296134492818"><a name="zh-cn_topic_0108272830_p14296134492818"></a><a name="zh-cn_topic_0108272830_p14296134492818"></a>Cdm.1603</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p829684419281"><a name="zh-cn_topic_0108272830_p829684419281"></a><a name="zh-cn_topic_0108272830_p829684419281"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p1329664419280"><a name="zh-cn_topic_0108272830_p1329664419280"></a><a name="zh-cn_topic_0108272830_p1329664419280"></a>获取topic <em id="zh-cn_topic_0108272830_i142962044182816"><a name="zh-cn_topic_0108272830_i142962044182816"></a><a name="zh-cn_topic_0108272830_i142962044182816"></a>%s</em>的样值失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p16296344172817"><a name="zh-cn_topic_0108272830_p16296344172817"></a><a name="zh-cn_topic_0108272830_p16296344172817"></a>获取topic样值失败。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p4296744142817"><a name="zh-cn_topic_0108272830_p4296744142817"></a><a name="zh-cn_topic_0108272830_p4296744142817"></a>请联系<span id="zh-cn_topic_0108272830_text1190521793812"><a name="zh-cn_topic_0108272830_text1190521793812"></a><a name="zh-cn_topic_0108272830_text1190521793812"></a>客服或技术支持人员</span>协助解决。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0108272830_row182962443280"><td class="cellrowborder" valign="top" width="15.96159615961596%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0108272830_p15296124416283"><a name="zh-cn_topic_0108272830_p15296124416283"></a><a name="zh-cn_topic_0108272830_p15296124416283"></a>Cdm.1604</p>
    </td>
    <td class="cellrowborder" valign="top" width="9.8009800980098%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0108272830_p12296344122818"><a name="zh-cn_topic_0108272830_p12296344122818"></a><a name="zh-cn_topic_0108272830_p12296344122818"></a>400</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.72207220722072%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0108272830_p3296164419282"><a name="zh-cn_topic_0108272830_p3296164419282"></a><a name="zh-cn_topic_0108272830_p3296164419282"></a>topic <em id="zh-cn_topic_0108272830_i142961644172819"><a name="zh-cn_topic_0108272830_i142961644172819"></a><a name="zh-cn_topic_0108272830_i142961644172819"></a>%s</em>没有数据。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.962596259625965%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0108272830_p122973445284"><a name="zh-cn_topic_0108272830_p122973445284"></a><a name="zh-cn_topic_0108272830_p122973445284"></a>该topic中无数据。</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.552755275527556%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0108272830_p20297174410283"><a name="zh-cn_topic_0108272830_p20297174410283"></a><a name="zh-cn_topic_0108272830_p20297174410283"></a>该topic中无数据，请排查无数据的原因。或者，请改为其他topic后再重试。</p>
    </td>
    </tr>
    </tbody>
    </table>


