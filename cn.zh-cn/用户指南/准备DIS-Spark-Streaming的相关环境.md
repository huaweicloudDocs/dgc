# 准备DIS Spark Streaming的相关环境<a name="dgc_01_0252"></a>

## 准备DIS应用开发环境<a name="zh-cn_topic_0120206049_section4878917318230"></a>

1.  参考[按需计费方式购买实时数据接入通道](实时数据接入快速入门.md#section12577139103116)准备相应DIS环境。
2.  安装Maven并配置本地仓库地址。
3.  安装scala-sdk。

## 配置DIS Spark Streaming依赖<a name="zh-cn_topic_0120206049_section088795613245"></a>

项目中可通过以下配置引入DIS Spark Streaming依赖：

```
<dependency>
    <groupId>com.huaweicloud.dis</groupId>
    <artifactId>huaweicloud-dis-spark-streaming_2.11</artifactId>
    <version>1.2.1</version>
    <scope>compile</scope>
</dependency>
```

## 检查认证信息<a name="zh-cn_topic_0120206049_section509986971841"></a>

-   检查AK/SK

    AK/SK \(Access Key ID/Secret Access Key\)是用户调用接口的访问密钥。

-   检查项目ID

    ProjectID表示租户的资源，每个Region都有一个唯一的项目ID。可在页面查看不同Region对应的项目ID值。


