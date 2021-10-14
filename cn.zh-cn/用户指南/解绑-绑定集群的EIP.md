# 解绑/绑定集群的EIP<a name="dgc_01_0020"></a>

## 操作场景<a name="zh-cn_topic_0108275471_section6082040915224"></a>

CDM集群创建完成后，支持解绑或绑定EIP。弹性公网IP，由虚拟私有云（Virtual Private Cloud，简称VPC）负责其计费。

-   如果CDM需要访问本地数据源、Internet的数据源，或者跨VPC的云服务，则必须要为CDM集群绑定一个弹性IP，或者使用NAT网关让CDM集群与其他弹性云服务器共享弹性IP访问Internet，具体操作请见[添加SNAT规则](https://support.huaweicloud.com/cdm_faq/cdm_01_0102.html)。
-   EIP的异常通知，需要先在IAM控制台创建对应Region的VPC策略委托才能生效。也可以在CDM集群管理界面选择“弹性IP检测授权  \>  创建委托“来创建。

>![](public_sys-resources/icon-note.gif) **说明：** 
>如果用户对本地数据源的访问通道做了SSL加密，则CDM无法通过弹性IP连接数据源。

## 前提条件<a name="zh-cn_topic_0108275471_section5781841515252"></a>

-   已创建CDM集群。
-   已拥有EIP配额，才能绑定EIP。

## 操作步骤<a name="zh-cn_topic_0108275471_section1674818115330"></a>

1.  进入CDM主界面，单击左侧导航上的“集群管理“，进入集群管理界面。

    **图 1**  集群列表<a name="zh-cn_topic_0108275471_fig4803125133011"></a>  
    ![](figures/集群列表.png "集群列表")

2.  对相应需要操作的集群可以进行绑定EIP或解绑EIP的操作。
    -   绑定EIP：单击集群操作列中的“绑定弹性IP“，进入EIP选择界面。
    -   解绑EIP：选择“更多  \>  解绑弹性IP“。

3.  单击“确定“绑定或解绑EIP。

