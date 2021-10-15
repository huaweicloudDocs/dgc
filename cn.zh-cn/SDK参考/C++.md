# C++<a name="dgc_06_1010"></a>

## 操作场景<a name="zh-cn_topic_0184564527_section18586174761315"></a>

使用C++语言调用APP认证的API时，您需要先获取SDK，参考API调用示例调用API。

## 准备环境<a name="zh-cn_topic_0184564527_section1495121117502"></a>

1.  已获取API的域名、请求url、请求方法、AppKey和AppSecret等信息，具体参见[认证前准备](认证前准备.md)。
2.  安装openssl库。

    ```
    apt-get install libssl-dev
    ```

3.  安装curl库。

    ```
    apt-get install libcurl4-openssl-dev
    ```


## 获取SDK<a name="zh-cn_topic_0184564527_section17783814506"></a>

1.  登录DGC控制台。
2.  单击“数据服务”模块。
3.  单击左侧菜单“共享版\> SDK”或“专享版 \> SDK”。
4.  单击SDK使用引导区域里对应语言的SDK进行下载。

获取“ApiGateway-cpp-sdk.zip”压缩包，解压后目录结构如下：

<a name="zh-cn_topic_0184564527_table98162204301"></a>
<table><thead align="left"><tr id="zh-cn_topic_0184564527_row38171220113013"><th class="cellrowborder" valign="top" width="35%" id="mcps1.1.3.1.1"><p id="zh-cn_topic_0184564527_p08202020163012"><a name="zh-cn_topic_0184564527_p08202020163012"></a><a name="zh-cn_topic_0184564527_p08202020163012"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="65%" id="mcps1.1.3.1.2"><p id="zh-cn_topic_0184564527_p18211420183016"><a name="zh-cn_topic_0184564527_p18211420183016"></a><a name="zh-cn_topic_0184564527_p18211420183016"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0184564527_row13962924163615"><td class="cellrowborder" valign="top" width="35%" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0184564527_p13602163519383"><a name="zh-cn_topic_0184564527_p13602163519383"></a><a name="zh-cn_topic_0184564527_p13602163519383"></a>hasher.cpp</p>
</td>
<td class="cellrowborder" rowspan="7" valign="top" width="65%" headers="mcps1.1.3.1.2 "><p id="zh-cn_topic_0184564527_p1962424183613"><a name="zh-cn_topic_0184564527_p1962424183613"></a><a name="zh-cn_topic_0184564527_p1962424183613"></a>SDK代码</p>
<p id="zh-cn_topic_0184564527_p115322053203812"><a name="zh-cn_topic_0184564527_p115322053203812"></a><a name="zh-cn_topic_0184564527_p115322053203812"></a></p>
<p id="zh-cn_topic_0184564527_p139425783817"><a name="zh-cn_topic_0184564527_p139425783817"></a><a name="zh-cn_topic_0184564527_p139425783817"></a></p>
<p id="zh-cn_topic_0184564527_p17193155503815"><a name="zh-cn_topic_0184564527_p17193155503815"></a><a name="zh-cn_topic_0184564527_p17193155503815"></a></p>
<p id="zh-cn_topic_0184564527_p61725273813"><a name="zh-cn_topic_0184564527_p61725273813"></a><a name="zh-cn_topic_0184564527_p61725273813"></a></p>
<p id="zh-cn_topic_0184564527_p5453154911381"><a name="zh-cn_topic_0184564527_p5453154911381"></a><a name="zh-cn_topic_0184564527_p5453154911381"></a></p>
<p id="zh-cn_topic_0184564527_p15734756123917"><a name="zh-cn_topic_0184564527_p15734756123917"></a><a name="zh-cn_topic_0184564527_p15734756123917"></a></p>
</td>
</tr>
<tr id="zh-cn_topic_0184564527_row8532153153816"><td class="cellrowborder" valign="top" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0184564527_p11532553173817"><a name="zh-cn_topic_0184564527_p11532553173817"></a><a name="zh-cn_topic_0184564527_p11532553173817"></a>hasher.h</p>
</td>
</tr>
<tr id="zh-cn_topic_0184564527_row29416571380"><td class="cellrowborder" valign="top" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0184564527_p19941157143817"><a name="zh-cn_topic_0184564527_p19941157143817"></a><a name="zh-cn_topic_0184564527_p19941157143817"></a>header.h</p>
</td>
</tr>
<tr id="zh-cn_topic_0184564527_row11193255143813"><td class="cellrowborder" valign="top" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0184564527_p17193195510386"><a name="zh-cn_topic_0184564527_p17193195510386"></a><a name="zh-cn_topic_0184564527_p17193195510386"></a>RequestParams.cpp</p>
</td>
</tr>
<tr id="zh-cn_topic_0184564527_row617155218383"><td class="cellrowborder" valign="top" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0184564527_p4176528389"><a name="zh-cn_topic_0184564527_p4176528389"></a><a name="zh-cn_topic_0184564527_p4176528389"></a>RequestParams.h</p>
</td>
</tr>
<tr id="zh-cn_topic_0184564527_row114531449183817"><td class="cellrowborder" valign="top" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0184564527_p2045304983811"><a name="zh-cn_topic_0184564527_p2045304983811"></a><a name="zh-cn_topic_0184564527_p2045304983811"></a>signer.cpp</p>
</td>
</tr>
<tr id="zh-cn_topic_0184564527_row12734175643917"><td class="cellrowborder" valign="top" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0184564527_p17734105653911"><a name="zh-cn_topic_0184564527_p17734105653911"></a><a name="zh-cn_topic_0184564527_p17734105653911"></a>signer.h</p>
</td>
</tr>
<tr id="zh-cn_topic_0184564527_row15305124673814"><td class="cellrowborder" valign="top" width="35%" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0184564527_p130624633817"><a name="zh-cn_topic_0184564527_p130624633817"></a><a name="zh-cn_topic_0184564527_p130624633817"></a>Makefile</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.1.3.1.2 "><p id="zh-cn_topic_0184564527_p12306946183810"><a name="zh-cn_topic_0184564527_p12306946183810"></a><a name="zh-cn_topic_0184564527_p12306946183810"></a>Makefile文件</p>
</td>
</tr>
<tr id="zh-cn_topic_0184564527_row756816379373"><td class="cellrowborder" valign="top" width="35%" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0184564527_p1956823703720"><a name="zh-cn_topic_0184564527_p1956823703720"></a><a name="zh-cn_topic_0184564527_p1956823703720"></a>main.cpp</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.1.3.1.2 "><p id="zh-cn_topic_0184564527_p55681737183719"><a name="zh-cn_topic_0184564527_p55681737183719"></a><a name="zh-cn_topic_0184564527_p55681737183719"></a>示例代码</p>
</td>
</tr>
</tbody>
</table>

## 调用API示例<a name="zh-cn_topic_0184564527_section122171818267"></a>

1.  在main.cpp中加入以下引用。

    ```
    #include <stdio.h>
    #include <stdlib.h>
    #include <string.h>
    #include <curl/curl.h>
    #include "signer.h"
    ```

2.  生成一个新的Signer， 填入AppKey和AppSecret。

    ```
    Signer signer("4f5f626b-073f-402f-a1e0-e52171c6100c", "******");
    ```

3.  生成一个新的RequestParams，指定方法名、域名、请求uri、查询字符串和body。

    ```
     RequestParams* request = new RequestParams("POST", "c967a237-cd6c-470e-906f-a8655461897e.apigw.cn-north-1.huaweicloud.comserviceEndpoint", "/app1",
            "Action=ListUsers&Version=2010-05-08", "demo");
    ```

4.  给请求添加header头，内容为具体参数数据。如果有需要，添加需要签名的其他头域。其中所访问API的ID为必填项，需要填入具体的ID信息，示例代码如“x-api-id”作为样例。

    ```
    request->addHeader("x-stage", "RELEASE");
    request->addHeader("x-api-id","*******");
    ```

5.  进行签名，执行此函数会将生成的签名头加入request变量中。然后为请求添加x-Authorization头，值与Authorization头相同。

    ```
    signer.createSignature(request);
    for (auto header : *request->getHeaders()) {
        if( strcmp(header.getKey().data(), "Authorization") == 0){
            request->addHeader("x-Authorization", header.getValue());
        }
    }
    ```

6.  使用curl库访问API，查看访问结果。

    ```
    static size_t
    WriteMemoryCallback(void *contents, size_t size, size_t nmemb, void *userp)
    {
        size_t realsize = size * nmemb;
        struct MemoryStruct *mem = (struct MemoryStruct *)userp;
    
        mem->memory = (char*)realloc(mem->memory, mem->size + realsize + 1);
        if (mem->memory == NULL) {
            /* out of memory! */
            printf("not enough memory (realloc returned NULL)\n");
            return 0;
        }
    
        memcpy(&(mem->memory[mem->size]), contents, realsize);
        mem->size += realsize;
        mem->memory[mem->size] = 0;
    
        return realsize;
    }
    
    //send http request using curl library
    int perform_request(RequestParams* request)
    {
        CURL *curl;
        CURLcode res;
        struct MemoryStruct resp_header;
        resp_header.memory = (char*)malloc(1);
        resp_header.size = 0;
        struct MemoryStruct resp_body;
        resp_body.memory = (char*)malloc(1);
        resp_body.size = 0;
    
        curl_global_init(CURL_GLOBAL_ALL);
        curl = curl_easy_init();
    
        curl_easy_setopt(curl, CURLOPT_CUSTOMREQUEST, request->getMethod().c_str());
        std::string url = "http://" + request->getHost() + request->getUri() + "?" + request->getQueryParams();
        curl_easy_setopt(curl, CURLOPT_URL, url.c_str());
        struct curl_slist *chunk = NULL;
        std::set<Header>::iterator it;
        for (auto header : *request->getHeaders()) {
            std::string headerEntry = header.getKey() + ": " + header.getValue();
            printf("%s\n", headerEntry.c_str());
            chunk = curl_slist_append(chunk, headerEntry.c_str());
        }
        printf("-------------\n");
        curl_easy_setopt(curl, CURLOPT_HTTPHEADER, chunk);
        curl_easy_setopt(curl, CURLOPT_COPYPOSTFIELDS, request->getPayload().c_str());
        curl_easy_setopt(curl, CURLOPT_NOBODY, 0L);
        curl_easy_setopt(curl, CURLOPT_WRITEFUNCTION, WriteMemoryCallback);
        curl_easy_setopt(curl, CURLOPT_HEADERDATA, (void *)&resp_header);
        curl_easy_setopt(curl, CURLOPT_WRITEDATA, (void *)&resp_body);
        //curl_easy_setopt(curl, CURLOPT_VERBOSE, 1L);
        res = curl_easy_perform(curl);
        if (res != CURLE_OK) {
            fprintf(stderr, "curl_easy_perform() failed: %s\n", curl_easy_strerror(res));
        }
        else {
            long status;
            curl_easy_getinfo(curl, CURLINFO_HTTP_CODE, &status);
            printf("status %d\n", status);
            printf(resp_header.memory);
            printf(resp_body.memory);
        }
        free(resp_header.memory);
        free(resp_body.memory);
        curl_easy_cleanup(curl);
    
        curl_global_cleanup();
    
        return 0;
    }
    ```

7.  运行make命令编译，得到可执行文件main，执行main文件，查看结果。

