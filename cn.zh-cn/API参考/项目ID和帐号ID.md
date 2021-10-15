# 项目ID和帐号ID<a name="dgc_02_0314"></a>

## 获取项目ID和帐号ID<a name="zh-cn_topic_0000001129537317_zh-cn_topic_0183643042_section41152976192830"></a>

项目ID表示租户的资源，帐号ID对应当前帐号。用户可在对应页面下查看不同Region对应的项目ID和帐号ID。

1.  注册并登录管理控制台。
2.  在用户名的下拉列表中单击“我的凭证“。
3.  在“我的凭证“页面，查看帐号名和帐号ID，在项目列表中查看项目ID。

## 调用API获取项目ID<a name="zh-cn_topic_0000001129537317_zh-cn_topic_0191815273_section1691341861315"></a>

项目ID可以通过调用[查询指定条件下的项目信息](https://support.huaweicloud.com/api-iam/iam_06_0001.html)API获取。

获取项目ID的接口为“GET https://\{Endpoint\}/v3/projects”，其中\{Endpoint\}为IAM的终端节点。

终端节点（Endpoint）即调用API的**请求地址**，不同服务不同区域的终端节点不同。Endpoint您可以从[终端节点及区域说明](https://developer.huaweicloud.com/endpoint)获取。

接口的认证鉴权请参见[认证鉴权](认证鉴权.md)。

响应示例如下，其中projects下的“id”即为项目ID。当返回多个id，请依据实际的区域（name）获取。

```
{
    "projects": [
        {
            "domain_id": "65382450e8f64ac0870cd180d14e684b",
            "is_domain": false,
            "parent_id": "65382450e8f64ac0870cd180d14e684b",
            "name": "region-name",
            "description": "",
            "links": {
                "next": null,
                "previous": null,
                "self": "https://www.example.com/v3/projects/a4a5d4098fb4474fa22cd05f897d6b99"
            },
            "id": "a4a5d4098fb4474fa22cd05f897d6b99",
            "enabled": true
        }
    ],
    "links": {
        "next": null,
        "previous": null,
        "self": "https://www.example.com/v3/projects"
    }
}
```

