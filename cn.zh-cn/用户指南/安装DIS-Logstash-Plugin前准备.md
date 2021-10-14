# 安装DIS Logstash Plugin前准备<a name="dgc_01_0235"></a>

## 检查依赖<a name="zh-cn_topic_0194140704_section19941830172917"></a>

1.  确认Logstash已安装并能正常运行。
2.  确认Logstash版本为6.0.0\~6.1.0版本。进入Logstash安装目录，执行如下命令查看Logstash版本。

    ```
    $ bin/logstash --version
    ```

3.  确认使用的Java版本为1.8.0及以上版本。执行如下命令查看Java版本。

    ```
    java -version
    ```

4.  确认使用的JRuby版本为9.0.0.0及以上版本。执行如下命令查看JRuby版本。

    ```
    $ bin/jruby -v
    ```


## 检查DIS通道<a name="zh-cn_topic_0194140704_section1937061743818"></a>

1.  [登录DGC控制台](https://console.huaweicloud.com/dgc/)，找到所需要的DGC实例，单击实例卡片上的“进入控制台”，进入概览页面。

    选择“空间管理”页签，完成工作空间的创建。

    在工作空间列表中，找到所需要的工作空间。

2.  单击相应工作空间的“数据集成“。

    系统跳转至数据集成页面。

3.  在左侧列表栏中选择“实时数据接入通道管理 \> 通道管理”。
4.  确认有通道用于数据上传且通道状态为“运行中”。

## 检查认证信息<a name="zh-cn_topic_0194140704_section358154133815"></a>

-   检查AK/SK

    AK/SK \(Access Key ID/Secret Access Key\)是用户调用接口的访问密钥。

    您可以通过如下方式获取访问密钥。

    1.  登录控制台，在用户名额下拉列表中选择“我的凭证”。
    2.  进入“我的凭证“页面，选择“访问密钥 \> 新增访问密钥“，如[图1](#dgc_01_0220_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_fig1552229194615)所示。

        **图 1**  单击新增访问密钥<a name="dgc_01_0220_zh-cn_topic_0000001129241845_zh-cn_topic_0183643042_fig1552229194615"></a>  
        ![](figures/单击新增访问密钥.png "单击新增访问密钥")

    3.  单击“确定”，根据浏览器提示，保存密钥文件。密钥文件会直接保存到浏览器默认的下载文件夹中。打开名称为“credentials.csv”的文件，即可查看访问密钥（Access Key Id和Secret Access Key）。

-   检查项目ID

    ProjectID表示租户的资源，每个Region都有一个唯一的项目ID。

    项目ID表示租户的资源，帐号ID对应当前帐号。用户可在对应页面下查看不同Region对应的项目ID和帐号ID。

    1.  注册并登录管理控制台。
    2.  在用户名的下拉列表中单击“我的凭证“。
    3.  在“我的凭证“页面，查看帐号名和帐号ID，在项目列表中查看项目ID。


## 获取DIS Logstash Plugin包<a name="zh-cn_topic_0194140704_section19855119123911"></a>

若已单独安装Logstash，请通过“dis-logstash-Plugin-_X.X.X_.zip”安装DIS插件。若不单独安装Logstash，请选择“logstash-_X.X.X_-with-dis-_X.X.X_.tar.gz”，此安装包为已安装好DIS插件的Logstash包。在[https://dis-publish.obs-website.cn-north-1.myhuaweicloud.com/](https://dis-publish.obs-website.cn-north-1.myhuaweicloud.com/)中下载对应压缩包。

