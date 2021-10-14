# 安装DIS Flume Plugin前准备<a name="dgc_01_0228"></a>

## 检查依赖<a name="zh-cn_topic_0120206067_section10672620173559"></a>

1.  确认Flume已经安装并能正常运行。
2.  确认Flume版本为1.4.0及以上版本。进入Flume安装目录，执行如下命令查看Flume版本。

    ```
    $ bin/flume-ng version | grep Flume
    ```

3.  确认使用的Java版本为1.8.0及以上版本。执行如下命令查看java版本。

    ```
    java -version
    ```


## 检查DIS通道<a name="zh-cn_topic_0120206067_section45060126173622"></a>

确认有通道用于数据上传且通道状态为“运行中”。

## 检查认证信息<a name="zh-cn_topic_0120206067_section65401174173650"></a>

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


## 获取DIS Flume Plugin包<a name="zh-cn_topic_0120206067_section12435635173724"></a>

在[https://dis-publish.obs-website.cn-north-1.myhuaweicloud.com/](https://dis-publish.obs-website.cn-north-1.myhuaweicloud.com/)中下载“dis-flume-Plugin-_X.X.X_.zip”压缩包。

