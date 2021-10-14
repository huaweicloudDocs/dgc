# 调用API<a name="dgc_01_0309"></a>

## 概述<a name="zh-cn_topic_0179716875_section173921475315"></a>

您作为API调用者，需要实现一个API的调用，那么您需要完成以下工作：

1.  获取API

    从服务目录获取需要调用API。仅在API发布后，才支持被调用。

2.  （可选）创建应用并获取授权

    对于使用APP和IAM认证的API，需要完成[创建应用](调用API.md#zh-cn_topic_0179716875_section266103219405)和[将API授权给应用](调用API.md#zh-cn_topic_0179716875_section173071443114111)。在API调用过程中，使用所创建应用的密钥对（AppKey、AppSecret），数据服务根据密钥对进行身份核对，完成鉴权。关于使用APP认证的方法，具体请参考[数据服务SDK参考](https://support.huaweicloud.com/sdkreference-dgc/dgc_06_1001.html)。

3.  [调用API](调用API.md#zh-cn_topic_0179716875_section13147154512613)

    API调用者完成以上步骤后，可以参考[数据服务SDK参考](https://support.huaweicloud.com/sdkreference-dgc/dgc_06_1001.html)进行API调用。


## 创建应用<a name="zh-cn_topic_0179716875_section266103219405"></a>

1.  在DGC控制台首页，选择对应工作空间的“数据服务“模块，进入数据服务页面。

    **图 1**  选择数据服务<a name="dgc_01_0313_dgc_01_0009_fig1540042925813"></a>  
    ![](figures/选择数据服务.png "选择数据服务")


1.  在左侧导航栏选择服务版本（例如：专享版），进入总览页。
2.  单击“调用API \> 应用管理”，进入到应用管理页面。单击“新建”，弹出“新建应用”对话框。填写如[表1](#zh-cn_topic_0179716875_table195413315428)所示信息。

    **表 1**  应用信息

    <a name="zh-cn_topic_0179716875_table195413315428"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0179716875_row45523384220"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0179716875_p65563314423"><a name="zh-cn_topic_0179716875_p65563314423"></a><a name="zh-cn_topic_0179716875_p65563314423"></a>信息项</p>
    </th>
    <th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0179716875_p356183311427"><a name="zh-cn_topic_0179716875_p356183311427"></a><a name="zh-cn_topic_0179716875_p356183311427"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0179716875_row1156183364219"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0179716875_p105616333427"><a name="zh-cn_topic_0179716875_p105616333427"></a><a name="zh-cn_topic_0179716875_p105616333427"></a>应用名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0179716875_p1656123374219"><a name="zh-cn_topic_0179716875_p1656123374219"></a><a name="zh-cn_topic_0179716875_p1656123374219"></a>应用名称。</p>
    </td>
    </tr>
    <tr id="row1075891833218"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p7761618163215"><a name="p7761618163215"></a><a name="p7761618163215"></a>应用类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p1667035213216"><a name="p1667035213216"></a><a name="p1667035213216"></a>DLM：专享版，不对接网关。</p>
    <p id="p11839185615325"><a name="p11839185615325"></a><a name="p11839185615325"></a>ROMA_APIC：专享版，对接ROMA APIC网关。</p>
    <p id="p43212014337"><a name="p43212014337"></a><a name="p43212014337"></a>APIGW：专享版，对接apigw网关。</p>
    <p id="p14761118173214"><a name="p14761118173214"></a><a name="p14761118173214"></a>IAM：使用iam认证，即token访问。</p>
    <p id="p6227184762917"><a name="p6227184762917"></a><a name="p6227184762917"></a>APP：共享版，对接APP。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0179716875_row14879114316433"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0179716875_p12880154304320"><a name="zh-cn_topic_0179716875_p12880154304320"></a><a name="zh-cn_topic_0179716875_p12880154304320"></a>描述</p>
    </td>
    <td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0179716875_p48801043134312"><a name="zh-cn_topic_0179716875_p48801043134312"></a><a name="zh-cn_topic_0179716875_p48801043134312"></a>对应用的介绍。</p>
    </td>
    </tr>
    </tbody>
    </table>

3.  单击“确定”，创建应用。

    创建应用成功后，在“应用管理”页面的列表中显示新创建的应用和应用ID。

4.  单击“应用名称“，进入应用详情页面，查看AppKey和AppSecret。

    **图 2**  应用详情<a name="zh-cn_topic_0179716875_fig12329145204214"></a>  
    ![](figures/应用详情.png "应用详情")


## 将API授权给应用<a name="zh-cn_topic_0179716875_section173071443114111"></a>

1.  在DGC控制台首页，选择对应工作空间的“数据服务“模块，进入数据服务页面。

    **图 3**  选择数据服务<a name="dgc_01_0313_dgc_01_0009_fig1540042925813_1"></a>  
    ![](figures/选择数据服务.png "选择数据服务")


1.  在左侧导航栏选择服务版本（例如：专享版），进入总览页。
2.  通过以下任意一种方式，将API授权给应用。

    主动授权：

    1.  单击“开发API \> API管理”，进入到API管理页面。
    2.  在待绑定应用的API所在行，单击“查看授权”，进入API完整信息界面。

        在“授权信息“页签中，单击“添加授权“。

    3.  设置授权的截止时间，勾选应用名称，单击“确认授权”，完成API的授权。

    申请授权：

    1.  单击“调用API  \>  服务目录“，进入服务市场主页面。
    2.  单击待绑定应用的API名称，进入API完整信息页面。
    3.  在“调用信息”页面，单击“申请权限“。
    4.  设置使用截止时间并选择应用名称，单击“确认“。
    5.  申请后，需要等待审核中心审核，方可授权成功。

3.  授权成功后，可以在应用管理详情页面查看已绑定的API。

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >-   如果已绑定API列表中包含无需绑定的API，在此API所在行的操作列，单击“解绑”，将无需绑定的API删除。
    >-   如果需要调试已绑定的API，单击“测试”，进入调试页面。
    >-   如果需要对已绑定的API延长授权时间，单击“续约”。


## 调用API<a name="zh-cn_topic_0179716875_section13147154512613"></a>

以下三种认证方式区别仅在于认证的内容不同，调用API的方式是相同的。

-   “IAM认证“：需要借助IAM服务进行安全认证。
-   “无认证“：不需要认证，直接调用API即可。

-   “APP认证方式“：API调用者通过APP认证方式调用API。
    -   使用APP认证时，需要通过SDK访问。
    -   其中SDK访问提供了基于Java、Go、Python、JavaScript、C\#、PHP、C++、C、Android等多种语言的SDK包。
    -   各个语言调用API示例请参考[Java调用API](https://support.huaweicloud.com/sdkreference-dgc/dgc_06_1004.html#section5)、[Go调用API](https://support.huaweicloud.com/sdkreference-dgc/dgc_06_1005.html#section4)、[Python调用API](https://support.huaweicloud.com/sdkreference-dgc/dgc_06_1006.html#section4)、[C\#调用API](https://support.huaweicloud.com/sdkreference-dgc/dgc_06_1007.html#section4)、[JavaScript调用API](https://support.huaweicloud.com/sdkreference-dgc/dgc_06_1008.html#section4)、[PHP调用API](https://support.huaweicloud.com/sdkreference-dgc/dgc_06_1009.html#section4)、[C++调用API](https://support.huaweicloud.com/sdkreference-dgc/dgc_06_1010.html#section3)、[C调用API](https://support.huaweicloud.com/sdkreference-dgc/dgc_06_1011.html#section3)、[Android调用API](https://support.huaweicloud.com/sdkreference-dgc/dgc_06_1012.html#section4)。
    -   各个语言调用API示例请参考Java调用API、Go调用API、Python调用API、C\#调用API、JavaScript调用API、PHP调用API、C++调用API、C调用API、Android调用API。


