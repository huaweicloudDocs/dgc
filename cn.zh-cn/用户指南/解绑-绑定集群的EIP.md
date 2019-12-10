# 解绑/绑定集群的EIP<a name="dayu_01_0020"></a>

## 操作场景<a name="zh-cn_topic_0108275471_section6082040915224"></a>

在CDM集群已经创建完成后，支持解绑或绑定EIP。弹性公网IP，由虚拟私有云（Virtual Private Cloud）负责其计费。

-   如果CDM需要访问本地数据源、Internet的数据源，或者跨VPC的云服务，则必须要为CDM集群绑定一个弹性IP，或者使用NAT网关让CDM集群与其他弹性云服务器共享弹性IP访问Internet，具体操作请见[添加SNAT规则](https://support.huaweicloud.com/cdm_faq/cdm_01_0102.html)。
-   EIP的异常通知，需要先在[IAM控制台](https://console.huaweicloud.com/iam/?locale=zh-cn#/iam/agencies)创建对应Region的VPC策略委托才能生效。也可以在CDM集群管理界面单击“弹性IP检测授权  \>  创建委托“来创建。

>![](public_sys-resources/icon-note.gif) **说明：**   
>如果用户对本地数据源的访问通道做了SSL加密，则CDM无法通过弹性IP连接数据源。  

## 前提条件<a name="zh-cn_topic_0108275471_section5781841515252"></a>

-   已创建CDM集群。
-   如果是绑定EIP，需要拥有EIP配额。

## 操作步骤<a name="zh-cn_topic_0108275471_section1674818115330"></a>

1.  [登录DAYU控制台](https://console.huaweicloud.com/dayu/)，找到所需要的DAYU实例，单击实例卡片上的“进入控制台”，进入概览页面。

    选择“空间管理”页签，完成工作空间的创建。

    在工作空间列表中，找到所需要的工作空间。



1.  单击相应工作空间的“数据集成“。

    系统跳转至数据集成页面。


1.  选择批量数据迁移集群管理，进入集群管理界面。
    1.  绑定EIP：单击集群操作列中的“绑定弹性IP“，进入EIP选择界面。

        **图 1**  绑定EIP<a name="zh-cn_topic_0108275471_fig4803125133011"></a>  
        ![](figures/绑定EIP.png "绑定EIP")

    2.  解绑EIP：单击“更多  \>  解绑弹性IP“。
    3.  解绑并释放EIP：单击“更多  \>  解绑并释放弹性IP“。

2.  单击“确定“绑定或解绑EIP。

