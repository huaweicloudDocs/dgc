# 初始化DIS客户端<a name="dayu_06_0026"></a>

您可以使用以下方法初始化DIS SDK客户端实例。其中，“endpoint“，“ak“，“sk“，“region“，“projectId“信息请参看[获取认证信息](获取认证信息.md)。

-   使用代码初始化DIS SDK客户端实例，代码样例可参考“dis\_sdk\_python-X.X\\dis\_sdk\_python\\examples”目录下所有（除\_\_init\_\_.py）文件，配置参数如下：

    ```
    // 创建DIS客户端实例
    projectid =" "                  通道所在的资源ID
    endpoint=" "                    DIS的访问地址
    ak = " "                         用户在IAM中创建的AK
    sk = " "                         用户在IAM中创建的SK
    region = " "                    用户使用通道所在的区域
    ```

-   使用配置文件初始化DIS SDK 客户端实例。

    在“dis\_sdk\_python-X.X\\dis\_sdk\_python\\”目录下的“initialization\_dis\_sdk.py”文件中设置配置文件信息。

    ```
    conf.set('Section1', 'projectid', '** your projectid **')
    conf.set('Section1', 'ak', '*** Provide your Access Key ***')
    conf.set('Section1', 'sk', '*** Provide your Secret Key ***')
    conf.set('Section1', 'region', '** region **')
    conf.set('Section1', 'endpoint', '** {ip}:{port} ***')
    ```

    配置好以上参数，执行initialization\_dis\_sdk.py，生成conf.ini文件，读取dis\_sdk\_python\\conf.ini配置文件信息。


