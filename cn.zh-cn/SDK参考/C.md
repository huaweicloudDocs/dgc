# C\#<a name="dayu_06_1007"></a>

## 操作场景<a name="zh-cn_topic_0184564487_section18586174761315"></a>

使用C\#语言调用APP认证的API时，您需要先获取SDK，然后打开SDK包中的工程文件，最后参考API调用示例调用API。

## 准备环境<a name="zh-cn_topic_0184564487_section1495121117502"></a>

-   已获取API的域名、请求url、请求方法、AppKey和AppSecret等信息，具体参见[认证前准备](认证前准备.md#dayu_06_1003)。
-   获取并安装Visual Studio，如果未安装，请至[Visual Studio官方网站](https://www.visualstudio.com/zh-hans/downloads/)下载。

## 获取SDK<a name="zh-cn_topic_0184564487_section17783814506"></a>

请访问https://apig.$\{OBS服务的域名\}/apig-sdk/ApiGateway-csharp-sdk.zip下载SDK。

其中，$\{OBS服务的域名\}需要根据实际情况进行替换，请向管理员获取OBS服务的域名。

[下载SDK](https://obs.cn-north-1.myhuaweicloud.com/apig-sdk/ApiGateway-csharp-sdk.zip)，获取“ApiGateway-csharp-sdk.zip”压缩包，解压后目录结构如下：

<a name="zh-cn_topic_0184564487_table98162204301"></a>
<table><thead align="left"><tr id="zh-cn_topic_0184564487_row38171220113013"><th class="cellrowborder" valign="top" width="35%" id="mcps1.1.3.1.1"><p id="zh-cn_topic_0184564487_p08202020163012"><a name="zh-cn_topic_0184564487_p08202020163012"></a><a name="zh-cn_topic_0184564487_p08202020163012"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="65%" id="mcps1.1.3.1.2"><p id="zh-cn_topic_0184564487_p18211420183016"><a name="zh-cn_topic_0184564487_p18211420183016"></a><a name="zh-cn_topic_0184564487_p18211420183016"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0184564487_row178221920163017"><td class="cellrowborder" valign="top" width="35%" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0184564487_p26441155133210"><a name="zh-cn_topic_0184564487_p26441155133210"></a><a name="zh-cn_topic_0184564487_p26441155133210"></a>apigateway-signature\Signer.cs</p>
</td>
<td class="cellrowborder" rowspan="2" valign="top" width="65%" headers="mcps1.1.3.1.2 "><p id="zh-cn_topic_0184564487_p128221420133013"><a name="zh-cn_topic_0184564487_p128221420133013"></a><a name="zh-cn_topic_0184564487_p128221420133013"></a>SDK代码</p>
<p id="zh-cn_topic_0184564487_p17823720183010"><a name="zh-cn_topic_0184564487_p17823720183010"></a><a name="zh-cn_topic_0184564487_p17823720183010"></a></p>
</td>
</tr>
<tr id="zh-cn_topic_0184564487_row3826132015303"><td class="cellrowborder" valign="top" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0184564487_p75519415335"><a name="zh-cn_topic_0184564487_p75519415335"></a><a name="zh-cn_topic_0184564487_p75519415335"></a>apigateway-signature\HttpEncoder.cs</p>
</td>
</tr>
<tr id="zh-cn_topic_0184564487_row1773122811302"><td class="cellrowborder" valign="top" width="35%" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0184564487_p839551218334"><a name="zh-cn_topic_0184564487_p839551218334"></a><a name="zh-cn_topic_0184564487_p839551218334"></a>sdk-request\Program.cs</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.1.3.1.2 "><p id="zh-cn_topic_0184564487_p19774132816301"><a name="zh-cn_topic_0184564487_p19774132816301"></a><a name="zh-cn_topic_0184564487_p19774132816301"></a>签名请求示例代码</p>
</td>
</tr>
<tr id="zh-cn_topic_0184564487_row530810155322"><td class="cellrowborder" valign="top" width="35%" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0184564487_p627914101352"><a name="zh-cn_topic_0184564487_p627914101352"></a><a name="zh-cn_topic_0184564487_p627914101352"></a>backend-signature\</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.1.3.1.2 "><p id="zh-cn_topic_0184564487_p033203133214"><a name="zh-cn_topic_0184564487_p033203133214"></a><a name="zh-cn_topic_0184564487_p033203133214"></a>后端签名示例工程</p>
</td>
</tr>
<tr id="zh-cn_topic_0184564487_row192061142132"><td class="cellrowborder" valign="top" width="35%" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0184564487_p73082015153214"><a name="zh-cn_topic_0184564487_p73082015153214"></a><a name="zh-cn_topic_0184564487_p73082015153214"></a>csharp.sln</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.1.3.1.2 "><p id="zh-cn_topic_0184564487_p132061442933"><a name="zh-cn_topic_0184564487_p132061442933"></a><a name="zh-cn_topic_0184564487_p132061442933"></a>工程文件</p>
</td>
</tr>
<tr id="zh-cn_topic_0184564487_row692919447393"><td class="cellrowborder" valign="top" width="35%" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0184564487_p12721814113211"><a name="zh-cn_topic_0184564487_p12721814113211"></a><a name="zh-cn_topic_0184564487_p12721814113211"></a>licenses\license-referencesource</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.1.3.1.2 "><p id="zh-cn_topic_0184564487_p0358153317314"><a name="zh-cn_topic_0184564487_p0358153317314"></a><a name="zh-cn_topic_0184564487_p0358153317314"></a>第三方库license文件</p>
</td>
</tr>
</tbody>
</table>

## 打开工程<a name="zh-cn_topic_0184564487_section1350838105019"></a>

双击SDK包中的“csharp.sln”文件，打开工程。工程中包含如下3个项目：

-   apigateway-signature：实现签名算法的共享库，可用于.Net Framework与.Net Core项目。
-   backend-signature：后端服务签名示例。
-   sdk-request：签名算法的调用示例，请根据实际情况修改参数后使用。具体代码说明请参考[调用API示例](#zh-cn_topic_0184564487_section14815524162316)。

## 调用API示例<a name="zh-cn_topic_0184564487_section14815524162316"></a>

1.  在工程中引入sdk。

    ```
    using APIGATEWAY_SDK;
    ```

2.  生成一个新的Signer， 填入AppKey和AppSecret。

    ```
    Signer signer = new Signer();
    signer.Key = "4f5f626b-073f-402f-a1e0-e52171c6100c";
    signer.Secret = "******";
    ```

3.  生成一个HttpRequest对象，指定域方法名、请求url和body。

    ```
    HttpRequest r = new HttpRequest("POST",    
                        new Uri("https://c967a237-cd6c-470e-906f-a8655461897e.apigw.cn-north-1.huaweicloud.comserviceEndpoint/app1?query=value"));
    r.body = "{\"a\":1}";
    ```

4.  给请求添加header头，内容为具体参数数据。如有需要，添加需要签名的其他头域。其中所访问API的ID为必填项，需要填入具体的ID信息，示例代码如“x-api-id”作为样例。

    ```
    r.headers.Add("x-stage", "RELEASE");
    r.headers.Add("x-api-id","*******");
    ```

5.  进行签名，执行此函数会生成一个新的HttpWebRequest，并在请求参数中添加用于签名的X-Sdk-Date头和Authorization头。然后为请求添加x-Authorization头，值与Authorization头相同。

    ```
    HttpWebRequest req = signer.Sign(r);
    req.Headers.Add("x-Authorization", req.Headers.GetValues("authorization")[0]);
    ```

6.  访问API，查看访问结果。

    ```
    var writer = new StreamWriter(req.GetRequestStream());
    writer.Write(r.body);
    writer.Flush();
    HttpWebResponse resp = (HttpWebResponse)req.GetResponse();
    var reader = newStreamReader(resp.GetResponseStream());
    Console.WriteLine(reader.ReadToEnd());
    ```


