# 配置模式生成API<a name="dgc_01_0305"></a>

本节介绍如何通过配置模式生成API。

使用配置模式生成数据API简单且容易上手，您不需编写任何代码，通过产品界面进行勾选配置即可快速生成API。推荐对API功能的要求不高或者无代码开发经验的用户使用。

## 前提条件<a name="zh-cn_topic_0180012632_section154291641113819"></a>

已在“管理中心  \>  数据连接“页面，完成数据源的配置。

## 新建API目录<a name="zh-cn_topic_0180012632_section18624154416414"></a>

API目录是按一定次序编排记录的API索引，是反映类别、指导使用、检索API的工具，帮助API开发者对API服务进行有效的分类和管理。

1.  在DGC控制台首页，选择对应工作空间的“数据服务“模块，进入数据服务页面。

    **图 1**  选择数据服务<a name="dgc_01_0313_dgc_01_0009_fig1540042925813"></a>  
    ![](figures/选择数据服务.png "选择数据服务")


1.  在左侧导航栏选择服务版本（例如：专享版），进入总览页。
2.  进入“数据服务 \>   \>  API目录“页面，单击![](figures/新建.jpg)。

    输入新建API目录名称，可新建API目录。

3.  对应已成功创建的API目录的操作列，可重新编辑API目录或者管理API。

    单击“编辑“，可修改API目录名称信息。仅当API处于已创建、已驳回、已下线、已停用的情况下才能进行API修改。


## 配置API基本信息<a name="zh-cn_topic_0180012632_section579414314409"></a>

1.  在DGC控制台首页，选择对应工作空间的“数据服务“模块，进入数据服务页面。

    **图 2**  选择数据服务<a name="dgc_01_0313_dgc_01_0009_fig1540042925813_1"></a>  
    ![](figures/选择数据服务.png "选择数据服务")


1.  在左侧导航选择服务版本（例如：专享版），进入总览页。
2.  进入“API管理“页面，单击“新建“，填写API基本信息。

    **表 1**  API基本信息

    <a name="zh-cn_topic_0180012632_table8943152418215"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0180012632_row5944624142115"><th class="cellrowborder" valign="top" width="17.72%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0180012632_p14944024102112"><a name="zh-cn_topic_0180012632_p14944024102112"></a><a name="zh-cn_topic_0180012632_p14944024102112"></a>配置</p>
    </th>
    <th class="cellrowborder" valign="top" width="82.28%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0180012632_p1994412244215"><a name="zh-cn_topic_0180012632_p1994412244215"></a><a name="zh-cn_topic_0180012632_p1994412244215"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0180012632_row8944132412212"><td class="cellrowborder" valign="top" width="17.72%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180012632_p14944324122114"><a name="zh-cn_topic_0180012632_p14944324122114"></a><a name="zh-cn_topic_0180012632_p14944324122114"></a>API名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="82.28%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180012632_p2094432432115"><a name="zh-cn_topic_0180012632_p2094432432115"></a><a name="zh-cn_topic_0180012632_p2094432432115"></a>支持中文、英文、数字、下划线，且只能以英文或中文开头，3-64个字符。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180012632_row159441924202111"><td class="cellrowborder" valign="top" width="17.72%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180012632_p139441124162110"><a name="zh-cn_topic_0180012632_p139441124162110"></a><a name="zh-cn_topic_0180012632_p139441124162110"></a>API目录</p>
    </td>
    <td class="cellrowborder" valign="top" width="82.28%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180012632_p1794417249211"><a name="zh-cn_topic_0180012632_p1794417249211"></a><a name="zh-cn_topic_0180012632_p1794417249211"></a>一个特定功能或场景的API集合，类似文件夹，是数据服务中API的最小组织单元，也是API网关中的最小管理单元。</p>
    <p id="zh-cn_topic_0180012632_p0237181018261"><a name="zh-cn_topic_0180012632_p0237181018261"></a><a name="zh-cn_topic_0180012632_p0237181018261"></a>您可单击<span class="uicontrol" id="zh-cn_topic_0180012632_uicontrol179511519182615"><a name="zh-cn_topic_0180012632_uicontrol179511519182615"></a><a name="zh-cn_topic_0180012632_uicontrol179511519182615"></a>“新建”</span>进行新建，也可选择<a href="#zh-cn_topic_0180012632_section18624154416414">新建API目录</a>已创建的API分组。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180012632_row19944122419211"><td class="cellrowborder" valign="top" width="17.72%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180012632_p09441624182110"><a name="zh-cn_topic_0180012632_p09441624182110"></a><a name="zh-cn_topic_0180012632_p09441624182110"></a>请求Path</p>
    </td>
    <td class="cellrowborder" valign="top" width="82.28%" headers="mcps1.2.3.1.2 "><p id="p181510159221"><a name="p181510159221"></a><a name="p181510159221"></a>API访问路径，例如：/v2/{project_id}/streams。</p>
    <p id="p1018725172211"><a name="p1018725172211"></a><a name="p1018725172211"></a>请求Path即完整的url中，域名之后、查询参数之前的部分，如<a href="#fig12437742151811">图3</a>中的“/blogs/188138”。</p>
    <div class="fignone" id="fig12437742151811"><a name="fig12437742151811"></a><a name="fig12437742151811"></a><span class="figcap"><b>图1 </b>统一资源定位符url说明</span><br><a name="image18444131031716"></a><a name="image18444131031716"></a><span><img id="image18444131031716" src="figures/统一资源定位符url说明.png" width="325.185" height="46.317117"></span></div>
    <p id="p127834621618"><a name="p127834621618"></a><a name="p127834621618"></a>在请求路径中，可以使用大括号{}标识路径中的参数作为通配符。如“/blogs/{blog_id}”表示/blogs后可以携带任何参数，例如“/blogs/188138”和“/blogs/0”均会匹配至/blogs/{blog_id}，由此API统一处理。</p>
    <p id="p1378164611166"><a name="p1378164611166"></a><a name="p1378164611166"></a>此外，相同域名下，不允许重复的请求路径出现。路径参数作为通配符时，名称不具备唯一性，例如“/blogs/{blog_id}”和“/blogs/{xxxx}”，会被视作相同路径。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180012632_row5944724132111"><td class="cellrowborder" valign="top" width="17.72%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180012632_p1894482414216"><a name="zh-cn_topic_0180012632_p1894482414216"></a><a name="zh-cn_topic_0180012632_p1894482414216"></a>参数协议</p>
    </td>
    <td class="cellrowborder" valign="top" width="82.28%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180012632_p594432412116"><a name="zh-cn_topic_0180012632_p594432412116"></a><a name="zh-cn_topic_0180012632_p594432412116"></a>用于传输请求的协议，支持HTTP和HTTPS协议。</p>
    <a name="ul4812711122715"></a><a name="ul4812711122715"></a><ul id="ul4812711122715"><li>HTTP属于基础的网络传输协议，无状态、无连接、简单、快速、灵活、使用明文传输，在使用上较为便捷，但是安全性欠佳。</li><li>HTTPS是在HTTP协议上进行了SSL或TLS加密校验的协议，能够有效验证身份以及保护数据完整性。相对的，访问HTTPS的API，需要配置相关的SSL证书或跳过SSL校验，否则将无法访问。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180012632_row4944624182114"><td class="cellrowborder" valign="top" width="17.72%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180012632_p1294432416216"><a name="zh-cn_topic_0180012632_p1294432416216"></a><a name="zh-cn_topic_0180012632_p1294432416216"></a>请求方法</p>
    </td>
    <td class="cellrowborder" valign="top" width="82.28%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180012632_zh-cn_topic_0121682347_p46347563325"><a name="zh-cn_topic_0180012632_zh-cn_topic_0121682347_p46347563325"></a><a name="zh-cn_topic_0180012632_zh-cn_topic_0121682347_p46347563325"></a>HTTP请求方法（也称为操作或动词），表示请求什么类型的操作，包含GET、POST等，遵循resultful风格。</p>
    <a name="ul11795164411287"></a><a name="ul11795164411287"></a><ul id="ul11795164411287"><li>GET：请求服务器返回指定资源，推荐使用GET请求。</li><li>POST：请求服务器新增资源或执行特殊操作，仅在注册API时使用。POST请求当前不支持body体，而是直接透传。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180012632_row894416245216"><td class="cellrowborder" valign="top" width="17.72%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180012632_p39447244210"><a name="zh-cn_topic_0180012632_p39447244210"></a><a name="zh-cn_topic_0180012632_p39447244210"></a>描述</p>
    </td>
    <td class="cellrowborder" valign="top" width="82.28%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180012632_p1794482452113"><a name="zh-cn_topic_0180012632_p1794482452113"></a><a name="zh-cn_topic_0180012632_p1794482452113"></a>对API进行简要描述。</p>
    </td>
    </tr>
    <tr id="row385843612229"><td class="cellrowborder" valign="top" width="17.72%" headers="mcps1.2.3.1.1 "><p id="p68593365220"><a name="p68593365220"></a><a name="p68593365220"></a>标签</p>
    </td>
    <td class="cellrowborder" valign="top" width="82.28%" headers="mcps1.2.3.1.2 "><p id="p9859436102213"><a name="p9859436102213"></a><a name="p9859436102213"></a>对API设置标签。用于标记当前API的属性，创建后可以通过标签快速检索定位API。单个API最多可设置20个标签。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180012632_row14789201319239"><td class="cellrowborder" valign="top" width="17.72%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180012632_p479016137235"><a name="zh-cn_topic_0180012632_p479016137235"></a><a name="zh-cn_topic_0180012632_p479016137235"></a>审核人</p>
    </td>
    <td class="cellrowborder" valign="top" width="82.28%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180012632_p879091315236"><a name="zh-cn_topic_0180012632_p879091315236"></a><a name="zh-cn_topic_0180012632_p879091315236"></a>拥有API的审核权限。</p>
    <p id="zh-cn_topic_0180012632_p1560823194914"><a name="zh-cn_topic_0180012632_p1560823194914"></a><a name="zh-cn_topic_0180012632_p1560823194914"></a>单击<span class="uicontrol" id="zh-cn_topic_0180012632_uicontrol59411231144917"><a name="zh-cn_topic_0180012632_uicontrol59411231144917"></a><a name="zh-cn_topic_0180012632_uicontrol59411231144917"></a>“新建”</span>，进入<span class="menucascade" id="zh-cn_topic_0180012632_menucascade4679476507"><a name="zh-cn_topic_0180012632_menucascade4679476507"></a><a name="zh-cn_topic_0180012632_menucascade4679476507"></a>“<span class="uicontrol" id="zh-cn_topic_0180012632_uicontrol8679147205019"><a name="zh-cn_topic_0180012632_uicontrol8679147205019"></a><a name="zh-cn_topic_0180012632_uicontrol8679147205019"></a>审核中心</span> &gt; <span class="uicontrol" id="zh-cn_topic_0180012632_uicontrol3431311175015"><a name="zh-cn_topic_0180012632_uicontrol3431311175015"></a><a name="zh-cn_topic_0180012632_uicontrol3431311175015"></a>审核人管理</span>”</span>页面，新建审核人。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180012632_row1128545124219"><td class="cellrowborder" valign="top" width="17.72%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180012632_p0129145184217"><a name="zh-cn_topic_0180012632_p0129145184217"></a><a name="zh-cn_topic_0180012632_p0129145184217"></a>安全认证</p>
    </td>
    <td class="cellrowborder" valign="top" width="82.28%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180012632_p83993263315"><a name="zh-cn_topic_0180012632_p83993263315"></a><a name="zh-cn_topic_0180012632_p83993263315"></a>API认证方式：</p>
    <a name="zh-cn_topic_0180012632_ul1239910233312"></a><a name="zh-cn_topic_0180012632_ul1239910233312"></a><ul id="zh-cn_topic_0180012632_ul1239910233312"><li>APP认证：表示由API网关服务负责接口请求的安全认证，安全级别最高。</li><li>IAM认证：表示借助IAM服务进行安全认证，安全级别中等。</li><li>无认证：属于无防护的模式，无需认证即可访问，安全级别低，不推荐使用。</li></ul>
    </td>
    </tr>
    <tr id="row5776121204916"><td class="cellrowborder" valign="top" width="17.72%" headers="mcps1.2.3.1.1 "><p id="p7777111274915"><a name="p7777111274915"></a><a name="p7777111274915"></a>服务目录可见性</p>
    </td>
    <td class="cellrowborder" valign="top" width="82.28%" headers="mcps1.2.3.1.2 "><p id="p1177716123493"><a name="p1177716123493"></a><a name="p1177716123493"></a>发布后，所选范围内的用户均可以在服务目录中看到此API。</p>
    <a name="ul1261051712476"></a><a name="ul1261051712476"></a><ul id="ul1261051712476"><li>当前工作空间可见</li><li>当前项目可见</li><li>当前租户可见</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180012632_row124091155194218"><td class="cellrowborder" valign="top" width="17.72%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180012632_p1941013554422"><a name="zh-cn_topic_0180012632_p1941013554422"></a><a name="zh-cn_topic_0180012632_p1941013554422"></a>访问日志</p>
    </td>
    <td class="cellrowborder" valign="top" width="82.28%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180012632_p241013552428"><a name="zh-cn_topic_0180012632_p241013552428"></a><a name="zh-cn_topic_0180012632_p241013552428"></a>勾选，则此API的查询结果将会产生记录并被保留7天，可以在访问日志处进行查看。</p>
    </td>
    </tr>
    <tr id="row14181050122214"><td class="cellrowborder" valign="top" width="17.72%" headers="mcps1.2.3.1.1 "><p id="p14779121017198"><a name="p14779121017198"></a><a name="p14779121017198"></a>最低保留期限</p>
    </td>
    <td class="cellrowborder" valign="top" width="82.28%" headers="mcps1.2.3.1.2 "><p id="p2779171051910"><a name="p2779171051910"></a><a name="p2779171051910"></a>API解绑前预留的最低期限。 API进行停用/下线/取消授权时, 会通知已授权用户, 并为用户预留至少X小时, 直到所有授权用户均完成解除或处理，或者到达截止时间, API才会停用/下线/取消授权。0表示不设限制。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180012632_row19497130152315"><td class="cellrowborder" valign="top" width="17.72%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180012632_p9497330112317"><a name="zh-cn_topic_0180012632_p9497330112317"></a><a name="zh-cn_topic_0180012632_p9497330112317"></a>入参定义</p>
    </td>
    <td class="cellrowborder" valign="top" width="82.28%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180012632_p194971030182316"><a name="zh-cn_topic_0180012632_p194971030182316"></a><a name="zh-cn_topic_0180012632_p194971030182316"></a>配置API请求中的参数，包含资源路径中的动态参数，请求URI中的查询参数和Header参数。</p>
    <p id="p9224193383012"><a name="p9224193383012"></a><a name="p9224193383012"></a>添加入参定义时，如果参数设定为必填，则API在访问时，必须传入指定参数；如果非必填，则在API访问时，未传入的参数，会使用默认值进行代替。</p>
    <p id="p1347545456"><a name="p1347545456"></a><a name="p1347545456"></a>参数大小限制如下：</p>
    <a name="ul511616244462"></a><a name="ul511616244462"></a><ul id="ul511616244462"><li>query+path，url最大32KB</li><li>header，最大128KB</li><li>body， 最大128KB</li></ul>
    <p id="zh-cn_topic_0180012632_p595114163011"><a name="zh-cn_topic_0180012632_p595114163011"></a><a name="zh-cn_topic_0180012632_p595114163011"></a>以配置资源路径中的动态参数为例进行说明，例如资源路径（请求Path）设置为：</p>
    <p id="zh-cn_topic_0180012632_p375510579322"><a name="zh-cn_topic_0180012632_p375510579322"></a><a name="zh-cn_topic_0180012632_p375510579322"></a>/v2/{project_id}/streams，资源路径中的{project_id}为动态参数，需要在此进行配置。</p>
    <a name="zh-cn_topic_0180012632_ol15807165012339"></a><a name="zh-cn_topic_0180012632_ol15807165012339"></a><ol id="zh-cn_topic_0180012632_ol15807165012339"><li>单击<span class="uicontrol" id="zh-cn_topic_0180012632_uicontrol598818352341"><a name="zh-cn_topic_0180012632_uicontrol598818352341"></a><a name="zh-cn_topic_0180012632_uicontrol598818352341"></a>“添加”</span>，参数名配置为project_id。</li><li>参数位置选择PATH。</li><li>类型设置为STRING。</li><li>选择性配置示例值和描述。</li></ol>
    </td>
    </tr>
    </tbody>
    </table>

3.  配置好API基本信息后，单击“下一步“，即可进入API取数逻辑页面。

## 配置取数逻辑<a name="zh-cn_topic_0180012632_section294754991217"></a>

“取数方式“选择“配置方式“：

1.  选择数据源、数据连接、数据库和数据表，获取到需要配置的表。

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >数据服务仅支持部分数据源，详情请参见[DGC支持的数据源](DGC支持的数据源.md)。您需提前在DGC管理中心中配置好数据源，数据表支持表名搜索。

2.  配置参数字段

    选择好数据表之后，单击“参数设置“后的“添加“，添加参数页面自动列出这个表的所有字段，分别勾选需要设置为请求参数、返回参数和排序参数的字段，分别添加到请求参数、返回参数和排序参数列表当中。

    **图 4**  添加参数<a name="zh-cn_topic_0180012632_fig16705194594812"></a>  
    ![](figures/添加参数.png "添加参数")

3.  编辑请求参数信息

    请求参数主要分为三部分，绑定参数、绑定字段、操作符。在请求参数列表中，需要设置绑定参数和操作符。

    -   绑定参数对外开放，是用户访问API时，直接使用的参数。
    -   绑定字段对外不可见，是API调用时，实际访问的内容。
    -   操作符则是用户访问时，对参数的的处理方式。当前支持的操作符及含义如下：

        **表 2**  支持的操作符

        <a name="table3361128679"></a>
        <table><thead align="left"><tr id="row036111281977"><th class="cellrowborder" valign="top" width="24.87%" id="mcps1.2.3.1.1"><p id="p1749065811716"><a name="p1749065811716"></a><a name="p1749065811716"></a><strong id="b1640810129814"><a name="b1640810129814"></a><a name="b1640810129814"></a>操作符</strong></p>
        </th>
        <th class="cellrowborder" valign="top" width="75.13%" id="mcps1.2.3.1.2"><p id="p24901858777"><a name="p24901858777"></a><a name="p24901858777"></a><strong id="b54217121689"><a name="b54217121689"></a><a name="b54217121689"></a>描述</strong></p>
        </th>
        </tr>
        </thead>
        <tbody><tr id="row163611928771"><td class="cellrowborder" valign="top" width="24.87%" headers="mcps1.2.3.1.1 "><p id="p19490115820716"><a name="p19490115820716"></a><a name="p19490115820716"></a>=</p>
        </td>
        <td class="cellrowborder" valign="top" width="75.13%" headers="mcps1.2.3.1.2 "><p id="p1049095814715"><a name="p1049095814715"></a><a name="p1049095814715"></a>检查两个操作数的值是否相等，如果相等则条件为真。</p>
        </td>
        </tr>
        <tr id="row19361728277"><td class="cellrowborder" valign="top" width="24.87%" headers="mcps1.2.3.1.1 "><p id="p124901558877"><a name="p124901558877"></a><a name="p124901558877"></a>&lt;&gt;</p>
        </td>
        <td class="cellrowborder" valign="top" width="75.13%" headers="mcps1.2.3.1.2 "><p id="p3490958771"><a name="p3490958771"></a><a name="p3490958771"></a>检查两个操作数的值是否相等，如果不相等则条件为真。</p>
        </td>
        </tr>
        <tr id="row53615281575"><td class="cellrowborder" valign="top" width="24.87%" headers="mcps1.2.3.1.1 "><p id="p114904582078"><a name="p114904582078"></a><a name="p114904582078"></a>&gt;</p>
        </td>
        <td class="cellrowborder" valign="top" width="75.13%" headers="mcps1.2.3.1.2 "><p id="p44908584712"><a name="p44908584712"></a><a name="p44908584712"></a>检查左操作数的值是否大于右操作数的值，如果是则条件为真。</p>
        </td>
        </tr>
        <tr id="row8361128278"><td class="cellrowborder" valign="top" width="24.87%" headers="mcps1.2.3.1.1 "><p id="p134901558876"><a name="p134901558876"></a><a name="p134901558876"></a>&gt;=</p>
        </td>
        <td class="cellrowborder" valign="top" width="75.13%" headers="mcps1.2.3.1.2 "><p id="p94905581477"><a name="p94905581477"></a><a name="p94905581477"></a>检查左操作数的值是否大于等于右操作数的值，如果是则条件为真。</p>
        </td>
        </tr>
        <tr id="row2056233316913"><td class="cellrowborder" valign="top" width="24.87%" headers="mcps1.2.3.1.1 "><p id="p4490105816711"><a name="p4490105816711"></a><a name="p4490105816711"></a>&lt;</p>
        </td>
        <td class="cellrowborder" valign="top" width="75.13%" headers="mcps1.2.3.1.2 "><p id="p10490125816716"><a name="p10490125816716"></a><a name="p10490125816716"></a>检查左操作数的值是否小于右操作数的值，如果是则条件为真。</p>
        </td>
        </tr>
        <tr id="row93612281170"><td class="cellrowborder" valign="top" width="24.87%" headers="mcps1.2.3.1.1 "><p id="p1049014581577"><a name="p1049014581577"></a><a name="p1049014581577"></a>&lt;=</p>
        </td>
        <td class="cellrowborder" valign="top" width="75.13%" headers="mcps1.2.3.1.2 "><p id="p1049075819719"><a name="p1049075819719"></a><a name="p1049075819719"></a>检查左操作数的值是否小于等于右操作数的值，如果是则条件为真。</p>
        </td>
        </tr>
        <tr id="row11361102815716"><td class="cellrowborder" valign="top" width="24.87%" headers="mcps1.2.3.1.1 "><p id="p10490135816714"><a name="p10490135816714"></a><a name="p10490135816714"></a>%like%</p>
        </td>
        <td class="cellrowborder" valign="top" width="75.13%" headers="mcps1.2.3.1.2 "><p id="p8386101021017"><a name="p8386101021017"></a><a name="p8386101021017"></a>%like%表示忽略前后缀，进行字符匹配。</p>
        </td>
        </tr>
        <tr id="row7787142851012"><td class="cellrowborder" valign="top" width="24.87%" headers="mcps1.2.3.1.1 "><p id="p1134318548108"><a name="p1134318548108"></a><a name="p1134318548108"></a>%like</p>
        </td>
        <td class="cellrowborder" valign="top" width="75.13%" headers="mcps1.2.3.1.2 "><p id="p1787928101018"><a name="p1787928101018"></a><a name="p1787928101018"></a>%like表示忽略前缀，进行字符匹配。</p>
        </td>
        </tr>
        <tr id="row12343113141013"><td class="cellrowborder" valign="top" width="24.87%" headers="mcps1.2.3.1.1 "><p id="p535735414101"><a name="p535735414101"></a><a name="p535735414101"></a>like%</p>
        </td>
        <td class="cellrowborder" valign="top" width="75.13%" headers="mcps1.2.3.1.2 "><p id="p173434316103"><a name="p173434316103"></a><a name="p173434316103"></a>like%表示忽略后缀，进行字符匹配。</p>
        </td>
        </tr>
        <tr id="row1435216342106"><td class="cellrowborder" valign="top" width="24.87%" headers="mcps1.2.3.1.1 "><p id="p10352103410106"><a name="p10352103410106"></a><a name="p10352103410106"></a>in</p>
        </td>
        <td class="cellrowborder" valign="top" width="75.13%" headers="mcps1.2.3.1.2 "><p id="p235273411106"><a name="p235273411106"></a><a name="p235273411106"></a>in运算符用于把某个值与一系列指定列表的值进行比较。</p>
        </td>
        </tr>
        <tr id="row330374720109"><td class="cellrowborder" valign="top" width="24.87%" headers="mcps1.2.3.1.1 "><p id="p1030394717103"><a name="p1030394717103"></a><a name="p1030394717103"></a>not in</p>
        </td>
        <td class="cellrowborder" valign="top" width="75.13%" headers="mcps1.2.3.1.2 "><p id="p7303247191012"><a name="p7303247191012"></a><a name="p7303247191012"></a>in运算符的对立面，用于把某个值与不在一系列指定列表的值进行比较。</p>
        </td>
        </tr>
        </tbody>
        </table>

4.  编辑返回参数信息

    在返回参数列表中，设置参数的名称、参数类型、示例值和描述。

    返回参数主要分为三部分，参数名、绑定字段、参数类型。参数名对外开放，是API返回时，最终展示给用户的参数名称；绑定字段对外不可见，是API调用时，实际返回的内容；参数类型则是API调用时，数据的呈现格式，分为数值型和字符型两类。

5.  编辑排序参数信息

    在排序参数列表中，设置排序字段是否可选，排序方式和描述。

    排序参数主要分为四部分，参数名、字段名称、是否可选以及排序方式。参数名对外开放，是API返回时，最终展示给用户的参数名称；字段名称对外不可见，是API调用时，实际访问的内容；是否可选决定了当前排序条件是否允许移除，勾选则表示可以不使用此参数；排序方式分为升序、降序以及自定义，表示了当前参数允许使用的排序形式。

    通过排序参数列表中的操作列的向上、向下和删除按钮，可调整排序参数的顺序或者删除某排序参数。

6.  单击“下一步“，设置pre\_order\_by的值为所有排序参数的描述，以“英文分号“进行分隔。

    以如下样例数据为例进行说明：

    **表 3**  排序字段对应的参数描述

    <a name="zh-cn_topic_0180012632_table1357619134165"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0180012632_row15761313181618"><th class="cellrowborder" valign="top" width="27.33%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0180012632_p13576191301611"><a name="zh-cn_topic_0180012632_p13576191301611"></a><a name="zh-cn_topic_0180012632_p13576191301611"></a>排序字段</p>
    </th>
    <th class="cellrowborder" valign="top" width="72.67%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0180012632_p1557651314162"><a name="zh-cn_topic_0180012632_p1557651314162"></a><a name="zh-cn_topic_0180012632_p1557651314162"></a>对应的排序参数描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0180012632_row1457681381619"><td class="cellrowborder" valign="top" width="27.33%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180012632_p16576213161610"><a name="zh-cn_topic_0180012632_p16576213161610"></a><a name="zh-cn_topic_0180012632_p16576213161610"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="72.67%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180012632_p1457661331612"><a name="zh-cn_topic_0180012632_p1457661331612"></a><a name="zh-cn_topic_0180012632_p1457661331612"></a>a:asc</p>
    <p id="zh-cn_topic_0180012632_p31611261720"><a name="zh-cn_topic_0180012632_p31611261720"></a><a name="zh-cn_topic_0180012632_p31611261720"></a>其中，a是参数名，asc代表升序。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180012632_row195772013191613"><td class="cellrowborder" valign="top" width="27.33%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180012632_p35775138161"><a name="zh-cn_topic_0180012632_p35775138161"></a><a name="zh-cn_topic_0180012632_p35775138161"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="72.67%" headers="mcps1.2.3.1.2 "><a name="zh-cn_topic_0180012632_ul12458416170"></a><a name="zh-cn_topic_0180012632_ul12458416170"></a><ul id="zh-cn_topic_0180012632_ul12458416170"><li>b:asc</li><li>b</li><li>b:desc</li></ul>
    <p id="zh-cn_topic_0180012632_p59121941191917"><a name="zh-cn_topic_0180012632_p59121941191917"></a><a name="zh-cn_topic_0180012632_p59121941191917"></a>其中，b是参数名，因为排序方式是自定义，所以有如上三种参数描述。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180012632_row135775137164"><td class="cellrowborder" valign="top" width="27.33%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180012632_p0577131321612"><a name="zh-cn_topic_0180012632_p0577131321612"></a><a name="zh-cn_topic_0180012632_p0577131321612"></a>age</p>
    </td>
    <td class="cellrowborder" valign="top" width="72.67%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180012632_p115771013141620"><a name="zh-cn_topic_0180012632_p115771013141620"></a><a name="zh-cn_topic_0180012632_p115771013141620"></a>c:desc</p>
    <p id="zh-cn_topic_0180012632_p1826219172015"><a name="zh-cn_topic_0180012632_p1826219172015"></a><a name="zh-cn_topic_0180012632_p1826219172015"></a>其中，c是参数名，desc代表降序。</p>
    </td>
    </tr>
    </tbody>
    </table>

    依据[表3](#zh-cn_topic_0180012632_table1357619134165)，分析得出各个字段对应的排序参数描述，则pre\_order\_by的设置方式有如下几种情况，包含所有排序参数的描述。

    **表 4**  配置pre\_order\_by

    <a name="zh-cn_topic_0180012632_table3977115012240"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0180012632_row1897755082415"><th class="cellrowborder" valign="top" width="24.98%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0180012632_p1897835052414"><a name="zh-cn_topic_0180012632_p1897835052414"></a><a name="zh-cn_topic_0180012632_p1897835052414"></a>pre_order_by</p>
    </th>
    <th class="cellrowborder" valign="top" width="42.08%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0180012632_p1297813504244"><a name="zh-cn_topic_0180012632_p1297813504244"></a><a name="zh-cn_topic_0180012632_p1297813504244"></a>对应的后端order by 语句</p>
    </th>
    <th class="cellrowborder" valign="top" width="32.940000000000005%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0180012632_p973113447263"><a name="zh-cn_topic_0180012632_p973113447263"></a><a name="zh-cn_topic_0180012632_p973113447263"></a>备注</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0180012632_row10978195010248"><td class="cellrowborder" valign="top" width="24.98%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0180012632_p997818505247"><a name="zh-cn_topic_0180012632_p997818505247"></a><a name="zh-cn_topic_0180012632_p997818505247"></a>a:asc;b;c:desc</p>
    </td>
    <td class="cellrowborder" valign="top" width="42.08%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0180012632_p129781950112412"><a name="zh-cn_topic_0180012632_p129781950112412"></a><a name="zh-cn_topic_0180012632_p129781950112412"></a>order by id ASC, name, age DESC</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.940000000000005%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0180012632_p87311944122620"><a name="zh-cn_topic_0180012632_p87311944122620"></a><a name="zh-cn_topic_0180012632_p87311944122620"></a>-</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180012632_row16978350122411"><td class="cellrowborder" valign="top" width="24.98%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0180012632_p1978165016242"><a name="zh-cn_topic_0180012632_p1978165016242"></a><a name="zh-cn_topic_0180012632_p1978165016242"></a>b;c:desc</p>
    </td>
    <td class="cellrowborder" valign="top" width="42.08%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0180012632_p4978850112410"><a name="zh-cn_topic_0180012632_p4978850112410"></a><a name="zh-cn_topic_0180012632_p4978850112410"></a>order by name, age DESC</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.940000000000005%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0180012632_p14731644162614"><a name="zh-cn_topic_0180012632_p14731644162614"></a><a name="zh-cn_topic_0180012632_p14731644162614"></a>因a是可选排序字段，所以可以不填。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180012632_row297845032413"><td class="cellrowborder" valign="top" width="24.98%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0180012632_p18978125052418"><a name="zh-cn_topic_0180012632_p18978125052418"></a><a name="zh-cn_topic_0180012632_p18978125052418"></a>b:asc;c:desc</p>
    </td>
    <td class="cellrowborder" valign="top" width="42.08%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0180012632_p159781350122413"><a name="zh-cn_topic_0180012632_p159781350122413"></a><a name="zh-cn_topic_0180012632_p159781350122413"></a>order by name ASC; age DESC</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.940000000000005%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0180012632_p2731154414267"><a name="zh-cn_topic_0180012632_p2731154414267"></a><a name="zh-cn_topic_0180012632_p2731154414267"></a>b排序方式是自定义，排序时可选择升序。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180012632_row1497845092419"><td class="cellrowborder" valign="top" width="24.98%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0180012632_p49784507247"><a name="zh-cn_topic_0180012632_p49784507247"></a><a name="zh-cn_topic_0180012632_p49784507247"></a>b:desc;c:desc</p>
    </td>
    <td class="cellrowborder" valign="top" width="42.08%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0180012632_p1097814506242"><a name="zh-cn_topic_0180012632_p1097814506242"></a><a name="zh-cn_topic_0180012632_p1097814506242"></a>order by name DESC; age DESC</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.940000000000005%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0180012632_p197311744132615"><a name="zh-cn_topic_0180012632_p197311744132615"></a><a name="zh-cn_topic_0180012632_p197311744132615"></a>b排序方式是自定义，排序时可选择降序。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **图 5**  配置排序参数值<a name="zh-cn_topic_0180012632_fig1337415324911"></a>  
    ![](figures/配置排序参数值.png "配置排序参数值")

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >-   pre\_order\_by是非必填参数，当未配置pre\_order\_by参数值时，则选取非可选排序字段作为排序的依据。
    >-   当配置pre\_order\_by参数值时，配置类API需严格按照排序参数顺序进行设置。例如
    >    a:asc;b;c:desc ，可行。当设置为b;a:asc;c:desc，则报错。


## 测试API<a name="zh-cn_topic_0180012632_section1265617232818"></a>

完成API参数的配置并保存后，单击左下角的“开始测试“，可进入API测试环节。

填写参数值，单击“开始测试“，即可在线发送API请求，在右侧可以看到API请求详情及返回内容。如果测试失败，请仔细查看错误提示并做相应的修改重新测试。 配置过程中需要注意正常返回示例的设置。

完成API测试之后，单击“确定“，即成功生成了一个数据API。

## 修改API<a name="section144814229434"></a>

生成API后，如果您需要修改API内容，可在“开发API \> API目录”或“开发API \> API管理”处选择对应API，点击“编辑”按钮进行修改API的相关操作。

>![](public_sys-resources/icon-note.gif) **说明：** 
>仅当API处于已创建、已驳回、已下线、已停用的情况下才能进行API修改。

