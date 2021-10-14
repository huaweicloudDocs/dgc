# 调试API<a name="dgc_01_0316"></a>

## 操作场景<a name="section25971517509"></a>

API创建后需要验证服务是否正常，管理控制台提供调试功能，您可以添加HTTP头部参数与body体参数，调试API接口。

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   后端路径中含有环境变量的API，不支持调试。
>-   API绑定签名密钥时，不支持调试。
>-   如果API已绑定流控策略，在调试API时，流控策略无效。

## 前提条件<a name="section1678010231609"></a>

-   已创建API。
-   已搭建完成后端服务。

## 操作步骤<a name="section1857120015545"></a>

1.  在DGC控制台首页，选择对应工作空间的“数据服务“模块，进入数据服务页面。

    **图 1**  选择数据服务<a name="dgc_01_0313_dgc_01_0009_fig1540042925813"></a>  
    ![](figures/选择数据服务.png "选择数据服务")


1.  在左侧导航栏选择服务版本（例如：专享版），进入总览页。
2.  单击“开发API \> API管理”，进入到API管理信息页面。
3.  通过以下任意一种方法，进入API调试页面。
    -   在待调试的API所在行，单击“更多 \> 调试”。
    -   单击“_API名称_”，进入API详情页面，单击“调试”。

        左侧为API请求参数配置区域，参数说明如[表1](#table91001022122714)所示。右侧为API发送的请求信息和API请求调用后的返回结果回显。

        **表 1**  调试API

        <a name="table91001022122714"></a>
        <table><thead align="left"><tr id="row19100102232710"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p131011322192714"><a name="p131011322192714"></a><a name="p131011322192714"></a>参数名称</p>
        </th>
        <th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p0101122182714"><a name="p0101122182714"></a><a name="p0101122182714"></a>说明</p>
        </th>
        </tr>
        </thead>
        <tbody><tr id="row19101622102712"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p110112226278"><a name="p110112226278"></a><a name="p110112226278"></a>参数配置</p>
        </td>
        <td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p6101182217272"><a name="p6101182217272"></a><a name="p6101182217272"></a>Query的参数与参数值。</p>
        </td>
        </tr>
        <tr id="row1531518593309"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p4315759163010"><a name="p4315759163010"></a><a name="p4315759163010"></a>集群配置</p>
        </td>
        <td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p1931585973010"><a name="p1931585973010"></a><a name="p1931585973010"></a>仅专享版支持，选择调试API所依托的实例。</p>
        </td>
        </tr>
        </tbody>
        </table>

        >![](public_sys-resources/icon-note.gif) **说明：** 
        >不同类型的请求，调试界面展现的信息项有差异。


4.  添加请求参数后，单击“开始测试”。

    右侧返回结果回显区域打印API调用的Response信息。

    -   调用成功时，返回HTTP状态码为“200”和Response信息。
    -   调试失败时，返回HTTP状态码为4_xx_或5_xx_。

5.  您可以通过调整请求参数与参数值，发送不同的请求，验证API服务。

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >如果需要修改API参数，请在右上角单击“编辑”，进入API编辑页面。


## 后续操作<a name="section122151752810"></a>

API调试成功后，您可以将API[发布API](发布API.md)，以便API调用者调用。

