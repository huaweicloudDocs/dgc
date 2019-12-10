# 初始化DIS客户端<a name="dayu_06_0009"></a>

您可以使用以下两种方法初始化DIS SDK客户端实例。其中，“endpoint“，“ak“，“sk“，“region“，“projectId“信息请参看[获取认证信息](获取认证信息.md)。

-   使用代码初始化DIS SDK客户端实例，代码样例如下。

    ```
    // 创建DIS客户端实例
    DISConfig disConfig = new DISConfig();
    disConfig.SetEndpoint("https://ip:port");
    disConfig.SetAK("xxxx");
    disConfig.SetSK("xxxx");
    disConfig.SetProjectId("xxxxxxx");
    disConfig.SetRegion("XXX");
    DISIngestionClient dic = new DISIngestionClient(disConfig);
    ```

-   使用配置文件初始化DIS SDK客户端实例。

    在“【$工程路径】\\bin\\Debug“目录下的“dis.propertites“文件中添加如下配置项。

    -   ak/sk：用户在IAM中创建的AK/SK。
    -   region：用户使用通道所在的区域。
    -   endpoint：DIS的访问地址。
    -   projectId：通道所在的资源ID。

    ```
    // 创建DIS客户端实例
               DISIngestionClient dic = new DISIngestionClient();
    ```


