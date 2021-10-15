# curl<a name="dgc_06_1013"></a>

## 操作场景<a name="zh-cn_topic_0184564544_section18586174761315"></a>

使用curl命令调用APP认证的API时，您需要先下载JavaScript SDK生成curl命令，然后将curl命令复制到命令行调用API。

## 前提条件<a name="zh-cn_topic_0184564544_section9546443152513"></a>

已获取API的域名、请求url、请求方法、AppKey和AppSecret等信息，具体参见[认证前准备](认证前准备.md)。

## 调用API示例<a name="zh-cn_topic_0184564544_section18450652112514"></a>

1.  使用JavaScript SDK生成curl命令。

    [下载SDK](https://obs.cn-north-1.myhuaweicloud.com/apig-sdk/ApiGateway-javascript-sdk.zip)，并解压。在浏览器中打开demo.html，页面如下图所示。

    ![](figures/zh-cn_image_0000001148888625.png)

2.  填入Key、Secret、方法名、请求协议、域名和url。例如：

    ```
    Key=4f5f626b-073f-402f-a1e0-e52171c6100c
    Secret=******
    Method=POST
    Url=https://{apig-endpoint}serviceEndpoint
    ```

3.  填入json格式的Query和Headers，填入Body。其中所访问API的ID为必填项，需要填入具体的ID信息，以参数"x-api-id"填入Headers中。
4.  单击“Send request”，生成curl命令。

    ```
    $ curl -X POST "https://{apig-endpoint}serviceEndpoint/" -H "X-Sdk-Date: 20180530T115847Z" -H "Authorization: SDK-HMAC-SHA256 Access=071fe245-9cf6-4d75-822d-c29945a1e06a, SignedHeaders=host;x-sdk-date, Signature=9e5314bd156d517******dd3e5765fdde4" -d ""
    ```

5.  为命令添加x-Authorization头，值与Authorization头相同。将curl命令复制到命令行，访问API。

    ```
    $ curl -X POST "https://{apig-endpoint}serviceEndpoint/" -H "X-Sdk-Date: 20180530T115847Z" -H "Authorization: SDK-HMAC-SHA256 Access=071fe245-9cf6-4d75-822d-c29945a1e06a, SignedHeaders=host;x-sdk-date, Signature=9e5314bd156d517******dd3e5765fdde4" -H "X-Authorization: SDK-HMAC-SHA256 Access=071fe245-9cf6-4d75-822d-c29945a1e06a, SignedHeaders=host;x-sdk-date, Signature=9e5314bd156d517******dd3e5765fdde4" -d ""
    Congratulations, sdk demo is running
    ```


