# 安装DIS Logstash Plugin前准备<a name="dayu_01_0235"></a>

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

1.  登录[DIS控制台](https://auth.huaweicloud.com/authui/login?service=https%3A%2F%2Fconsole.huaweicloud.com%2Fdis%2F%3Fcloud_route_state%3D%2Fmanage%2FoverView#/login)。
2.  单击管理控制台左上角的![](figures/wwx437827-中软基础平台部-DataSight-image-bbfbe22f-2a2d-4e1b-8f10-a7782fd1d3ed.png)，选择区域和项目。
3.  在左侧列表栏中选择“通道管理”。
4.  确认有通道用于数据上传且通道状态为“运行中”。

## 检查认证信息<a name="zh-cn_topic_0194140704_section358154133815"></a>

-   检查AK/SK

    AK/SK \(Access Key ID/Secret Access Key\)是用户调用接口的访问密钥。由用户在Iam中创建，可在“我的凭证 \> 管理访问密钥“页面下载生成。

-   检查项目ID

    ProjectID表示租户的资源，每个Region都有一个唯一的项目ID。可在页面查看不同Region对应的项目ID值。


## 获取DIS Logstash Plugin包<a name="zh-cn_topic_0194140704_section19855119123911"></a>

在[https://dis-publish.obs-website.cn-north-1.myhwclouds.com/](https://dis-publish.obs-website.cn-north-1.myhwclouds.com/)获取“dis-logstash-Plugin-_X.X.X_.zip”压缩包。


