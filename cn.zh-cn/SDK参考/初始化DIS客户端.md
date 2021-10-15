# 初始化DIS客户端<a name="dgc_06_0050"></a>

您可以使用以下两种方法初始化DIS SDK客户端实例，优先选择使用代码进行初始化。其中，“endpoint“，“ak“，“sk“，“region“，“projectId“信息请参看[获取认证信息](获取认证信息.md#dgc_06_0005)。

-   使用代码初始化DIS SDK客户端实例。

    ```
    // 创建DIS客户端实例
    DIS dic = DISClientBuilder.standard()
        .withEndpoint("YOUR_ENDPOINT")
        .withAk("YOUR_AK")
        .withSk("YOUR_SK")
        .withProjectId("YOUR_PROJECT_ID")
        .withRegion("YOUR_REGION")
        // 以下配置失败时的重试次数
        .withProperty(DISConfig.PROPERTY_PRODUCER_RECORDS_RETRIES, "-1")
        .withProperty(DISConfig.PROPERTY_PRODUCER_EXCEPTION_RETRIES, "-1")
        .build();
    ```

-   若需要使用代理，请使用如下方法初始化DIS客户端：

    ```
    // 创建DIS客户端实例 
    DIS dic = DISClientBuilder.standard() 
        .withEndpoint("YOUR_ENDPOINT") 
        .withAk("YOUR_AK") 
        .withSk("YOUR_SK") 
        .withProjectId("YOUR_PROJECT_ID") 
        .withRegion("YOUR_REGION") 
        .withProxyHost("YOUR_PROXY_HOST") // 代理IP
        .withProxyPort("YOUR_PROXY_PORT") // 代理端口
        .withProxyProtocol(Protocol.HTTP) // 代理协议，默认为HTTP
        .withProxyUsername("YOUR_PROXY_USER_NAME") // 代理用户名（可选）
        .withProxyPassword("YOUR_PROXY_PASSWORD") // 代理密码（可选）    
        // 以下配置失败时的重试次数
        .withProperty(DISConfig.PROPERTY_PRODUCER_RECORDS_RETRIES, "-1")
        .withProperty(DISConfig.PROPERTY_PRODUCER_EXCEPTION_RETRIES, "-1")
        .build();
    ```

-   若需要开启传输压缩，请使用如下方法初始化DIS客户端：

    ```
    // 创建DIS客户端实例
    DIS dic = DISClientBuilder.standard()
        .withEndpoint("YOUR_ENDPOINT")
        .withAk("YOUR_AK")
        .withSk("YOUR_SK")
        .withProjectId("YOUR_PROJECT_ID")
        .withRegion("YOUR_REGION")
        .withBodyCompressEnabled(true)
        .withBodyCompressType(CompressionType.ZSTD) // 配置压缩算法，当前支持lz4和zstd，默认值为lz4
        // 以下配置失败时的重试次数
        .withProperty(DISConfig.PROPERTY_PRODUCER_RECORDS_RETRIES, "-1")
        .withProperty(DISConfig.PROPERTY_PRODUCER_EXCEPTION_RETRIES, "-1")
        .build();
    ```

-   若需在客户端将数据加密后再上传到DIS，DIS SDK提供了加密方法。即在构建disclient时增加参数DataEncryptEnabled和data.password。

    ```
    // 创建DIS客户端实例
    DIS dic = DISClientBuilder.standard()
        .withEndpoint("YOUR_ENDPOINT")
        .withAk("YOUR_AK")
        .withSk("YOUR_SK")
        .withProjectId("YOUR_PROJECT_ID")
        .withRegion("YOUR_REGION")
        .withDataEncryptEnabled(true)
        .withProperty("data.password", "xxx") //xxx替换为用户配置的数据加密秘钥
        // 以下配置失败时的重试次数
        .withProperty(DISConfig.PROPERTY_PRODUCER_RECORDS_RETRIES, "-1")
        .withProperty(DISConfig.PROPERTY_PRODUCER_EXCEPTION_RETRIES, "-1")
        .build();
    ```

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >若使用JAVA SDK加密上传数据，读取数据也需要使用JAVA SDK配置相同的秘钥。

-   使用配置文件初始化DIS SDK客户端实例。

    在“dis-sdk-demo\\src\\main\\resources“目录下的“dis.properties“文件中添加如下配置项。

    -   ak/sk：用户在IAM中创建的AK/SK。
    -   region：用户使用通道所在的区域。
    -   endpoint：DIS的访问地址。
    -   projectId：通道所在的资源ID。

    ```
    // 创建DIS客户端实例
                DIS dic = DISClientBuilder.standard().build();
    ```


