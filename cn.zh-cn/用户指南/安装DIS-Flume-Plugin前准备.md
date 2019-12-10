# 安装DIS Flume Plugin前准备<a name="dayu_01_0228"></a>

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

    AK/SK \(Access Key ID/Secret Access Key\)是用户调用接口的访问密钥。由用户在Iam中创建，可在页面下载生成。

-   检查项目ID

    ProjectID表示租户的资源，每个Region都有一个唯一的项目ID。可在“我的凭证 \> 项目列表“页面查看不同Region对应的项目ID值。


## 获取DIS Flume Plugin包<a name="zh-cn_topic_0120206067_section12435635173724"></a>

在[https://dis-publish.obs-website.cn-north-1.myhwclouds.com/](https://dis-publish.obs-website.cn-north-1.myhwclouds.com/)获取“dis-flume-Plugin-_X.X.X_.zip”压缩包。

