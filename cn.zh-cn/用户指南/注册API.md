# 注册API<a name="dayu_01_0307"></a>

本文将为您介绍如何注册API，与通过数据表生成的API统一管理和发布到API网关。

目前数据服务支持Restful风格的API注册，包含GET/POST常见请求方式。

**图 1**  注册API流程<a name="zh-cn_topic_0179716871_fig1983252154610"></a>  
![](figures/注册API流程.jpg "注册API流程")

## 配置API基本信息<a name="zh-cn_topic_0179716871_section1992120471923"></a>

1.  [登录DAYU控制台](https://console.huaweicloud.com/dayu/)，找到所需要的DAYU实例，单击实例卡片上的“进入控制台”，进入概览页面。

    选择“空间管理”页签，完成工作空间的创建。

    在工作空间列表中，找到所需要的工作空间。


1.  单击相应工作空间的“数据服务“。

    系统跳转至“数据服务“页面。


1.  进入“数据服务 \>  \>  总览  \>  开发API  \>  API管理“页面，单击“注册现有API“，填写API基本信息。

    **表 1**  API基本信息

    <a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_table8943152418215"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_row5944624142115"><th class="cellrowborder" valign="top" width="17.72%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p14944024102112"><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p14944024102112"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p14944024102112"></a>配置</p>
    </th>
    <th class="cellrowborder" valign="top" width="82.28%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p1994412244215"><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p1994412244215"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p1994412244215"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_row8944132412212"><td class="cellrowborder" valign="top" width="17.72%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p14944324122114"><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p14944324122114"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p14944324122114"></a>API名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="82.28%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p2094432432115"><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p2094432432115"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p2094432432115"></a>支持中文、英文、数字、下划线，且只能以英文或中文开头，3-64个字符。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_row159441924202111"><td class="cellrowborder" valign="top" width="17.72%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p139441124162110"><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p139441124162110"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p139441124162110"></a>API分组</p>
    </td>
    <td class="cellrowborder" valign="top" width="82.28%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p1794417249211"><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p1794417249211"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p1794417249211"></a>一个特定功能或场景的API集合，是数据服务中API的最小组织单元，也是API网关中的最小管理单元。</p>
    <p id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p0237181018261"><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p0237181018261"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p0237181018261"></a>您可单击<span class="uicontrol" id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_uicontrol179511519182615"><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_uicontrol179511519182615"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_uicontrol179511519182615"></a>“新建”</span>进行新建，也可选择<a href="向导模式生成API.md#zh-cn_topic_0180012632_section18624154416414">管理API分组</a>已创建的API分组。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_row19944122419211"><td class="cellrowborder" valign="top" width="17.72%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p09441624182110"><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p09441624182110"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p09441624182110"></a>请求Path</p>
    </td>
    <td class="cellrowborder" valign="top" width="82.28%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p199441124152112"><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p199441124152112"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p199441124152112"></a>资源路径，也即API访问路径。</p>
    <p id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p157144617114"><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p157144617114"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p157144617114"></a>示例：/v2/{project_id}/streams</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_row5944724132111"><td class="cellrowborder" valign="top" width="17.72%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p1894482414216"><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p1894482414216"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p1894482414216"></a>协议</p>
    </td>
    <td class="cellrowborder" valign="top" width="82.28%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p594432412116"><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p594432412116"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p594432412116"></a>用于传输请求的协议，支持HTTP和HTTPS协议。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_row4944624182114"><td class="cellrowborder" valign="top" width="17.72%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p1294432416216"><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p1294432416216"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p1294432416216"></a>请求方式</p>
    </td>
    <td class="cellrowborder" valign="top" width="82.28%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_zh-cn_topic_0121682347_p46347563325"><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_zh-cn_topic_0121682347_p46347563325"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_zh-cn_topic_0121682347_p46347563325"></a>HTTP请求方法（也称为操作或动词），它告诉服务你正在请求什么类型的操作。</p>
    <p id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p392117034119"><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p392117034119"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p392117034119"></a>GET：请求服务器返回指定资源。</p>
    <p id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p478642154112"><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p478642154112"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p478642154112"></a>POST：请求服务器新增资源或执行特殊操作。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_row894416245216"><td class="cellrowborder" valign="top" width="17.72%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p39447244210"><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p39447244210"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p39447244210"></a>描述</p>
    </td>
    <td class="cellrowborder" valign="top" width="82.28%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p1794482452113"><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p1794482452113"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p1794482452113"></a>对API进行简要描述。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_row14789201319239"><td class="cellrowborder" valign="top" width="17.72%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p479016137235"><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p479016137235"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p479016137235"></a>负责人</p>
    </td>
    <td class="cellrowborder" valign="top" width="82.28%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p879091315236"><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p879091315236"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p879091315236"></a>拥有API的审核权限。</p>
    <p id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p1560823194914"><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p1560823194914"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p1560823194914"></a>单击<span class="uicontrol" id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_uicontrol59411231144917"><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_uicontrol59411231144917"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_uicontrol59411231144917"></a>“新建”</span>，进入<span class="menucascade" id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_menucascade4679476507"><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_menucascade4679476507"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_menucascade4679476507"></a>“<span class="uicontrol" id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_uicontrol8679147205019"><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_uicontrol8679147205019"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_uicontrol8679147205019"></a>审核中心</span> &gt; <span class="uicontrol" id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_uicontrol3431311175015"><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_uicontrol3431311175015"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_uicontrol3431311175015"></a>审核人管理</span>”</span>页面，新建审核人。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_row1451110214238"><td class="cellrowborder" valign="top" width="17.72%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p9511192132313"><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p9511192132313"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p9511192132313"></a>是否公开</p>
    </td>
    <td class="cellrowborder" valign="top" width="82.28%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p65111521132316"><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p65111521132316"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p65111521132316"></a>勾选，则发布的API将在服务市场公开售卖。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_row19497130152315"><td class="cellrowborder" valign="top" width="17.72%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p9497330112317"><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p9497330112317"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p9497330112317"></a>入参定义</p>
    </td>
    <td class="cellrowborder" valign="top" width="82.28%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p194971030182316"><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p194971030182316"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p194971030182316"></a>配置API请求中的参数，包含资源路径中的动态参数，请求URI中的查询参数和Header参数。</p>
    <p id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p595114163011"><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p595114163011"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p595114163011"></a>以配置资源路径中的动态参数为例进行说明，例如资源路径（请求Path）设置为：</p>
    <p id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p375510579322"><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p375510579322"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_p375510579322"></a>/v2/{project_id}/streams，资源路径中的{project_id}为动态参数，需要在此进行配置。</p>
    <a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_ol15807165012339"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_ol15807165012339"></a><ol id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_ol15807165012339"><li>单击<span class="uicontrol" id="zh-cn_topic_0179716871_zh-cn_topic_0180012632_uicontrol598818352341"><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_uicontrol598818352341"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0180012632_uicontrol598818352341"></a>“添加”</span>，参数名配置为project_id。</li><li>参数位置选择PATH。</li><li>类型设置为STRING</li><li>选择性配置示例值和描述。</li></ol>
    </td>
    </tr>
    </tbody>
    </table>

2.  配置好API基本信息后，单击“下一步“，即可进入API取数逻辑页面。

## 配置API参数<a name="zh-cn_topic_0179716871_section1150143816315"></a>

配置API基本信息后，即可配置API参数。这里将配置API的后端服务和请求参数。

**表 2**  API参数配置说明

<a name="zh-cn_topic_0179716871_table06311401542"></a>
<table><thead align="left"><tr id="zh-cn_topic_0179716871_row46320406543"><th class="cellrowborder" valign="top" width="18.64%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0179716871_p15632104075413"><a name="zh-cn_topic_0179716871_p15632104075413"></a><a name="zh-cn_topic_0179716871_p15632104075413"></a>配置</p>
</th>
<th class="cellrowborder" valign="top" width="81.36%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0179716871_p13632134025416"><a name="zh-cn_topic_0179716871_p13632134025416"></a><a name="zh-cn_topic_0179716871_p13632134025416"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0179716871_row6632184014544"><td class="cellrowborder" valign="top" width="18.64%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0179716871_p963254015414"><a name="zh-cn_topic_0179716871_p963254015414"></a><a name="zh-cn_topic_0179716871_p963254015414"></a>协议</p>
</td>
<td class="cellrowborder" valign="top" width="81.36%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0179716871_p594432412116"><a name="zh-cn_topic_0179716871_p594432412116"></a><a name="zh-cn_topic_0179716871_p594432412116"></a>用于传输请求的协议，支持HTTP和HTTPS协议。</p>
<p id="zh-cn_topic_0179716871_p184791654017"><a name="zh-cn_topic_0179716871_p184791654017"></a><a name="zh-cn_topic_0179716871_p184791654017"></a>用于数据服务模块向待注册API服务传输请求。</p>
</td>
</tr>
<tr id="zh-cn_topic_0179716871_row863274015410"><td class="cellrowborder" valign="top" width="18.64%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0179716871_p6632184014543"><a name="zh-cn_topic_0179716871_p6632184014543"></a><a name="zh-cn_topic_0179716871_p6632184014543"></a>请求方式</p>
</td>
<td class="cellrowborder" valign="top" width="81.36%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0179716871_zh-cn_topic_0121682347_p46347563325"><a name="zh-cn_topic_0179716871_zh-cn_topic_0121682347_p46347563325"></a><a name="zh-cn_topic_0179716871_zh-cn_topic_0121682347_p46347563325"></a>HTTP请求方法（也称为操作或动词），它告诉服务你正在请求什么类型的操作。用于数据服务模块向待注册API服务传输请求。</p>
<p id="zh-cn_topic_0179716871_p392117034119"><a name="zh-cn_topic_0179716871_p392117034119"></a><a name="zh-cn_topic_0179716871_p392117034119"></a>GET：请求服务器返回指定资源。</p>
<p id="zh-cn_topic_0179716871_p478642154112"><a name="zh-cn_topic_0179716871_p478642154112"></a><a name="zh-cn_topic_0179716871_p478642154112"></a>POST：请求服务器新增资源或执行特殊操作。</p>
</td>
</tr>
<tr id="zh-cn_topic_0179716871_row116321940115410"><td class="cellrowborder" valign="top" width="18.64%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0179716871_p13632640195411"><a name="zh-cn_topic_0179716871_p13632640195411"></a><a name="zh-cn_topic_0179716871_p13632640195411"></a>后端服务HOST</p>
</td>
<td class="cellrowborder" valign="top" width="81.36%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0179716871_p85131816175819"><a name="zh-cn_topic_0179716871_p85131816175819"></a><a name="zh-cn_topic_0179716871_p85131816175819"></a>待注册API服务的Host，不能以http://或https://开头，并且不包含Path。</p>
</td>
</tr>
<tr id="zh-cn_topic_0179716871_row14632640195416"><td class="cellrowborder" valign="top" width="18.64%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0179716871_p263213403542"><a name="zh-cn_topic_0179716871_p263213403542"></a><a name="zh-cn_topic_0179716871_p263213403542"></a>后端服务PATH</p>
</td>
<td class="cellrowborder" valign="top" width="81.36%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0179716871_p4867201716114"><a name="zh-cn_topic_0179716871_p4867201716114"></a><a name="zh-cn_topic_0179716871_p4867201716114"></a>待注册API服务的Path，Path中支持参数，参数要放在{}中，如/user/{userid}。</p>
</td>
</tr>
<tr id="zh-cn_topic_0179716871_row1664784918560"><td class="cellrowborder" valign="top" width="18.64%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0179716871_p116481493569"><a name="zh-cn_topic_0179716871_p116481493569"></a><a name="zh-cn_topic_0179716871_p116481493569"></a>后端超时（ms）</p>
</td>
<td class="cellrowborder" valign="top" width="81.36%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0179716871_p141220918211"><a name="zh-cn_topic_0179716871_p141220918211"></a><a name="zh-cn_topic_0179716871_p141220918211"></a>设置后端超时时间。</p>
</td>
</tr>
<tr id="zh-cn_topic_0179716871_row174011835710"><td class="cellrowborder" valign="top" width="18.64%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0179716871_p1840117812574"><a name="zh-cn_topic_0179716871_p1840117812574"></a><a name="zh-cn_topic_0179716871_p1840117812574"></a>后端服务参数</p>
</td>
<td class="cellrowborder" valign="top" width="81.36%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0179716871_p1475101314318"><a name="zh-cn_topic_0179716871_p1475101314318"></a><a name="zh-cn_topic_0179716871_p1475101314318"></a>请求参数位置支持Path、Header、Query，不同的请求方式所支持的可选参数位置不一样，请根据产品上提供的可选项按需选择。</p>
</td>
</tr>
<tr id="zh-cn_topic_0179716871_row976991065715"><td class="cellrowborder" valign="top" width="18.64%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0179716871_p97691210155716"><a name="zh-cn_topic_0179716871_p97691210155716"></a><a name="zh-cn_topic_0179716871_p97691210155716"></a>常量参数</p>
</td>
<td class="cellrowborder" valign="top" width="81.36%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0179716871_p967923015312"><a name="zh-cn_topic_0179716871_p967923015312"></a><a name="zh-cn_topic_0179716871_p967923015312"></a>常量参数即参数值是固定的参数，对调用者不可见，API调用时不需传入常量参数，但后台服务始终接收这里定义好的常量参数及参数值。适用于当您希望把API的某个参数的取值固定为某个值以及要对调用者隐藏参数的场景。</p>
</td>
</tr>
</tbody>
</table>

## API测试<a name="zh-cn_topic_0179716871_section1134113251965"></a>

完成API参数的配置并保存后，单击左下角的“开始测试“，即可进入API测试环节。  填写参数值，单击“开始测试“，即可在线发送API请求，在右侧可以看到API请求详情及返回内容。如果测试失败，请仔细查看错误提示并做相应的修改重新测试。 配置过程中需要注意正常返回示例的设置。

完成API测试之后，单击“确定“，即成功生成了一个数据API。

