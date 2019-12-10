# 配置DIS Agent<a name="dayu_01_0222"></a>

## Linux服务器上配置DIS Agent<a name="zh-cn_topic_0194140722_section4916936311221"></a>

1.  使用PuTTY 工具登录日志所在服务器。
2.  执行**cd /opt/dis-agent-X.X.X/**命令，进入“dis-agent-X.X.X“文件夹。
3.  执行**vim conf/agent.yml**命令，打开DIS Agent配置文件“agent.yml“，根据实际情况修改各配置项的值并保存，配置项说明请参见[表1](#zh-cn_topic_0194140722_zh-cn_topic_0077812210_table31093287)。

## Windows服务器上配置DIS Agent<a name="zh-cn_topic_0194140722_section59581866112340"></a>

1.  使用文件管理器进入安装包解压后的目录，例如“C:\\dis-agent-X.X.X”。
2.  使用编辑器打开“agent.yml”文件，根据实际情况修改各配置项的值并保存，配置项说明请参见[表1](#zh-cn_topic_0194140722_zh-cn_topic_0077812210_table31093287)。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >“agent.yml“文件为linux格式，建议使用“Notepad++“工具编辑文件。  


## 配置文件说明<a name="zh-cn_topic_0194140722_section6170167112511"></a>

DIS Agent配置文件格式为“YAML”，各配置项与值之间必须以英文格式的“冒号+空格”形式分隔。具体配置项说明请参见[表1](#zh-cn_topic_0194140722_zh-cn_topic_0077812210_table31093287)。

>![](public_sys-resources/icon-note.gif) **说明：**   
>配置完成之后，请将agent.yml中flows下面无用的示例配置删除或者使用\#注释（比如只配置了一个DISStream，则将下面的CustomFileStream与另外的DISStream模块删除或者注释）。  

**表 1**  agent.yml配置文件说明

<a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_table31093287"></a>
<table><thead align="left"><tr id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_row24129853"><th class="cellrowborder" valign="top" width="16.328367163283673%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p8361080"><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p8361080"></a><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p8361080"></a>配置项</p>
</th>
<th class="cellrowborder" valign="top" width="8.159184081591842%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p6158855"><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p6158855"></a><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p6158855"></a>是否必填</p>
</th>
<th class="cellrowborder" valign="top" width="37.75622437756224%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p29105235"><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p29105235"></a><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p29105235"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="37.75622437756224%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p8713795"><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p8713795"></a><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p8713795"></a>默认值</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_row34728767"><td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p61566768"><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p61566768"></a><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p61566768"></a>region</p>
</td>
<td class="cellrowborder" valign="top" width="8.159184081591842%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p20852350"><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p20852350"></a><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p20852350"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p11318800"><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p11318800"></a><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p11318800"></a>DIS服务所在区域。</p>
<div class="note" id="zh-cn_topic_0194140722_note16149114305512"><a name="zh-cn_topic_0194140722_note16149114305512"></a><a name="zh-cn_topic_0194140722_note16149114305512"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0194140722_p91495438556"><a name="zh-cn_topic_0194140722_p91495438556"></a><a name="zh-cn_topic_0194140722_p91495438556"></a>获取DIS区域请参见<a href="http://developer.huaweicloud.com/dev/endpoint?DIS" target="_blank" rel="noopener noreferrer">终端节点及区域说明</a>。</p>
</div></div>
</td>
<td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p44407631"><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p44407631"></a><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p44407631"></a>cn-north-1</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_row64124362"><td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p26690871"><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p26690871"></a><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p26690871"></a>ak</p>
</td>
<td class="cellrowborder" valign="top" width="8.159184081591842%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p14476932"><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p14476932"></a><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p14476932"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p31780825"><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p31780825"></a><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p31780825"></a>用户的Access Key。</p>
<p id="zh-cn_topic_0194140722_a7a5004ef7cc145c7b1bba1788deb2e72"><a name="zh-cn_topic_0194140722_a7a5004ef7cc145c7b1bba1788deb2e72"></a><a name="zh-cn_topic_0194140722_a7a5004ef7cc145c7b1bba1788deb2e72"></a>获取方式请参见<a href="安装前准备.md#zh-cn_topic_0194140940_s929153773cb54e1b801a8399b2ef9b2f">检查认证信息</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p15663836"><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p15663836"></a><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p15663836"></a>请根据实际情况配置</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_row6756797"><td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p10429724"><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p10429724"></a><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p10429724"></a>sk</p>
</td>
<td class="cellrowborder" valign="top" width="8.159184081591842%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p39501348"><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p39501348"></a><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p39501348"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140722_a8df70f1b132f4c21819ac41552d67b8d"><a name="zh-cn_topic_0194140722_a8df70f1b132f4c21819ac41552d67b8d"></a><a name="zh-cn_topic_0194140722_a8df70f1b132f4c21819ac41552d67b8d"></a>用户的Secret Key。</p>
<p id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p45492604"><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p45492604"></a><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p45492604"></a>获取方式请参见<a href="安装前准备.md#zh-cn_topic_0194140940_s929153773cb54e1b801a8399b2ef9b2f">检查认证信息</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p61022284"><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p61022284"></a><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p61022284"></a>请根据实际情况配置</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_row12329649"><td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p59177513"><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p59177513"></a><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p59177513"></a>projectId</p>
</td>
<td class="cellrowborder" valign="top" width="8.159184081591842%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p28649262"><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p28649262"></a><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p28649262"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p538322511400"><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p538322511400"></a><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p538322511400"></a>用户所属区域的项目ID。</p>
<p id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p38888871"><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p38888871"></a><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p38888871"></a>获取方式请参见<a href="安装前准备.md#zh-cn_topic_0194140940_s929153773cb54e1b801a8399b2ef9b2f">检查认证信息</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p62990845"><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p62990845"></a><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p62990845"></a>请根据实际情况配置</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_row30046694"><td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p17863121"><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p17863121"></a><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p17863121"></a>endpoint</p>
</td>
<td class="cellrowborder" valign="top" width="8.159184081591842%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p37626701"><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p37626701"></a><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p37626701"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p27863937"><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p27863937"></a><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p27863937"></a>DIS数据网关地址。</p>
<p id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p49448848"><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p49448848"></a><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p49448848"></a>格式：https://DIS终端节点。</p>
<div class="note" id="zh-cn_topic_0194140722_note18471843544"><a name="zh-cn_topic_0194140722_note18471843544"></a><a name="zh-cn_topic_0194140722_note18471843544"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0194140722_p34879412545"><a name="zh-cn_topic_0194140722_p34879412545"></a><a name="zh-cn_topic_0194140722_p34879412545"></a>获取DIS终端节点请参见<a href="http://developer.huaweicloud.com/dev/endpoint?DIS" target="_blank" rel="noopener noreferrer">终端节点及区域说明</a>。</p>
</div></div>
</td>
<td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p10750772"><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p10750772"></a><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p10750772"></a>https://dis.cn-north-1.myhuaweicloud.com</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140722_row8911914598"><td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140722_p6847141218598"><a name="zh-cn_topic_0194140722_p6847141218598"></a><a name="zh-cn_topic_0194140722_p6847141218598"></a>body.serialize.type</p>
</td>
<td class="cellrowborder" valign="top" width="8.159184081591842%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140722_p48478128597"><a name="zh-cn_topic_0194140722_p48478128597"></a><a name="zh-cn_topic_0194140722_p48478128597"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.3 "><div class="p" id="zh-cn_topic_0194140722_p284711212599"><a name="zh-cn_topic_0194140722_p284711212599"></a><a name="zh-cn_topic_0194140722_p284711212599"></a>DIS数据包上传格式。（非原始数据格式）<a name="zh-cn_topic_0194140722_ul0847612195914"></a><a name="zh-cn_topic_0194140722_ul0847612195914"></a><ul id="zh-cn_topic_0194140722_ul0847612195914"><li>json：DIS数据包封装为json格式，满足普通使用。</li><li>protobuf：DIS数据包封装为二进制格式，可以减少体积约1/3，在数据量较大的情况下推荐使用此格式。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140722_p784751295915"><a name="zh-cn_topic_0194140722_p784751295915"></a><a name="zh-cn_topic_0194140722_p784751295915"></a>json</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140722_row9766109132419"><td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140722_p1376611916244"><a name="zh-cn_topic_0194140722_p1376611916244"></a><a name="zh-cn_topic_0194140722_p1376611916244"></a>body.compress.enabled</p>
</td>
<td class="cellrowborder" valign="top" width="8.159184081591842%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140722_p1576717917247"><a name="zh-cn_topic_0194140722_p1576717917247"></a><a name="zh-cn_topic_0194140722_p1576717917247"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140722_p47679972415"><a name="zh-cn_topic_0194140722_p47679972415"></a><a name="zh-cn_topic_0194140722_p47679972415"></a>是否开启传输数据压缩。</p>
</td>
<td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140722_p1476713942417"><a name="zh-cn_topic_0194140722_p1476713942417"></a><a name="zh-cn_topic_0194140722_p1476713942417"></a>false</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140722_row3972159246"><td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140722_p89861515245"><a name="zh-cn_topic_0194140722_p89861515245"></a><a name="zh-cn_topic_0194140722_p89861515245"></a>body.compress.type</p>
</td>
<td class="cellrowborder" valign="top" width="8.159184081591842%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140722_p1198115142416"><a name="zh-cn_topic_0194140722_p1198115142416"></a><a name="zh-cn_topic_0194140722_p1198115142416"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140722_p15981215162415"><a name="zh-cn_topic_0194140722_p15981215162415"></a><a name="zh-cn_topic_0194140722_p15981215162415"></a>开启压缩时选择的数据压缩格式，目前支持的压缩格式如下：</p>
<p id="zh-cn_topic_0194140722_p173731511152816"><a name="zh-cn_topic_0194140722_p173731511152816"></a><a name="zh-cn_topic_0194140722_p173731511152816"></a>lz4：综合来看效率最高的压缩算法,更加侧重压缩解压速度,压缩比并不是第一。</p>
<p id="zh-cn_topic_0194140722_p15968538102811"><a name="zh-cn_topic_0194140722_p15968538102811"></a><a name="zh-cn_topic_0194140722_p15968538102811"></a>zstd：一种新的无损压缩算法，旨在提供快速压缩，并实现高压缩比。</p>
</td>
<td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140722_p1858881712253"><a name="zh-cn_topic_0194140722_p1858881712253"></a><a name="zh-cn_topic_0194140722_p1858881712253"></a>lz4</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140722_row1916519644612"><td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140722_p15166196154613"><a name="zh-cn_topic_0194140722_p15166196154613"></a><a name="zh-cn_topic_0194140722_p15166196154613"></a>PROXY_HOST</p>
</td>
<td class="cellrowborder" valign="top" width="8.159184081591842%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140722_p16166863462"><a name="zh-cn_topic_0194140722_p16166863462"></a><a name="zh-cn_topic_0194140722_p16166863462"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140722_p15167365461"><a name="zh-cn_topic_0194140722_p15167365461"></a><a name="zh-cn_topic_0194140722_p15167365461"></a>配置代理IP，请求走代理服务器的需要配置。</p>
</td>
<td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140722_p316766174617"><a name="zh-cn_topic_0194140722_p316766174617"></a><a name="zh-cn_topic_0194140722_p316766174617"></a>请根据实际情况配置</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140722_row4757181354816"><td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140722_p175781316483"><a name="zh-cn_topic_0194140722_p175781316483"></a><a name="zh-cn_topic_0194140722_p175781316483"></a>PROXY_PORT</p>
</td>
<td class="cellrowborder" valign="top" width="8.159184081591842%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140722_p13757101344813"><a name="zh-cn_topic_0194140722_p13757101344813"></a><a name="zh-cn_topic_0194140722_p13757101344813"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140722_p12757913184815"><a name="zh-cn_topic_0194140722_p12757913184815"></a><a name="zh-cn_topic_0194140722_p12757913184815"></a>配置代理端口。</p>
</td>
<td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140722_p1875751374818"><a name="zh-cn_topic_0194140722_p1875751374818"></a><a name="zh-cn_topic_0194140722_p1875751374818"></a>80</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140722_row126687220508"><td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140722_p16668102217505"><a name="zh-cn_topic_0194140722_p16668102217505"></a><a name="zh-cn_topic_0194140722_p16668102217505"></a>PROXY_PROTOCOL</p>
</td>
<td class="cellrowborder" valign="top" width="8.159184081591842%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140722_p6668162212505"><a name="zh-cn_topic_0194140722_p6668162212505"></a><a name="zh-cn_topic_0194140722_p6668162212505"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140722_p966872218504"><a name="zh-cn_topic_0194140722_p966872218504"></a><a name="zh-cn_topic_0194140722_p966872218504"></a>配置代理协议。支持http和https。</p>
</td>
<td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140722_p11668142219502"><a name="zh-cn_topic_0194140722_p11668142219502"></a><a name="zh-cn_topic_0194140722_p11668142219502"></a>http</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140722_row10513141820499"><td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140722_p1851381814496"><a name="zh-cn_topic_0194140722_p1851381814496"></a><a name="zh-cn_topic_0194140722_p1851381814496"></a>PROXY_USERNAME</p>
</td>
<td class="cellrowborder" valign="top" width="8.159184081591842%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140722_p1251321814910"><a name="zh-cn_topic_0194140722_p1251321814910"></a><a name="zh-cn_topic_0194140722_p1251321814910"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140722_p1751371814498"><a name="zh-cn_topic_0194140722_p1751371814498"></a><a name="zh-cn_topic_0194140722_p1751371814498"></a>配置代理用户名。</p>
</td>
<td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140722_p17513201814493"><a name="zh-cn_topic_0194140722_p17513201814493"></a><a name="zh-cn_topic_0194140722_p17513201814493"></a>请根据实际情况配置</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140722_row146151321174914"><td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140722_p7615152164914"><a name="zh-cn_topic_0194140722_p7615152164914"></a><a name="zh-cn_topic_0194140722_p7615152164914"></a>PROXY_PASSWORD</p>
</td>
<td class="cellrowborder" valign="top" width="8.159184081591842%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140722_p861572113492"><a name="zh-cn_topic_0194140722_p861572113492"></a><a name="zh-cn_topic_0194140722_p861572113492"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140722_p196158219492"><a name="zh-cn_topic_0194140722_p196158219492"></a><a name="zh-cn_topic_0194140722_p196158219492"></a>配置代理密码。</p>
</td>
<td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140722_p18615182111492"><a name="zh-cn_topic_0194140722_p18615182111492"></a><a name="zh-cn_topic_0194140722_p18615182111492"></a>请根据实际情况配置</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_row21574462"><td class="cellrowborder" colspan="4" valign="top" headers="mcps1.2.5.1.1 mcps1.2.5.1.2 mcps1.2.5.1.3 mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p2701015"><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p2701015"></a><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p2701015"></a>[flows]</p>
<p id="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p24309136"><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p24309136"></a><a name="zh-cn_topic_0194140722_zh-cn_topic_0077812210_p24309136"></a>监控的文件信息，可同时配置多个监控文件信息。</p>
<p id="zh-cn_topic_0194140722_p20049024114312"><a name="zh-cn_topic_0194140722_p20049024114312"></a><a name="zh-cn_topic_0194140722_p20049024114312"></a>当前支持如下模式上传：</p>
<p id="zh-cn_topic_0194140722_p2588636184712"><a name="zh-cn_topic_0194140722_p2588636184712"></a><a name="zh-cn_topic_0194140722_p2588636184712"></a>DISStream:持续监控文本文件，实时收集增量数据按分隔符解析并上传到DIS通道(通道源数据类型为BLOB/JSON/CSV)，配置项说明请参见<a href="#zh-cn_topic_0194140722_table491818012236">表2</a>。</p>
<p id="zh-cn_topic_0194140722_p8273036114312"><a name="zh-cn_topic_0194140722_p8273036114312"></a><a name="zh-cn_topic_0194140722_p8273036114312"></a>具体配置格式可以参见版本包中的“agent.yml”的样例。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  DISStream配置项说明

<a name="zh-cn_topic_0194140722_table491818012236"></a>
<table><thead align="left"><tr id="zh-cn_topic_0194140722_row622406912236"><th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0194140722_p5266559612255"><a name="zh-cn_topic_0194140722_p5266559612255"></a><a name="zh-cn_topic_0194140722_p5266559612255"></a>配置项</p>
</th>
<th class="cellrowborder" valign="top" width="8%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0194140722_p3805490812255"><a name="zh-cn_topic_0194140722_p3805490812255"></a><a name="zh-cn_topic_0194140722_p3805490812255"></a>是否必填</p>
</th>
<th class="cellrowborder" valign="top" width="62%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0194140722_p6254872512255"><a name="zh-cn_topic_0194140722_p6254872512255"></a><a name="zh-cn_topic_0194140722_p6254872512255"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="14.000000000000002%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0194140722_p3328193412255"><a name="zh-cn_topic_0194140722_p3328193412255"></a><a name="zh-cn_topic_0194140722_p3328193412255"></a>默认值</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0194140722_row6271560912236"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140722_p5763449712255"><a name="zh-cn_topic_0194140722_p5763449712255"></a><a name="zh-cn_topic_0194140722_p5763449712255"></a>DISStream</p>
</td>
<td class="cellrowborder" valign="top" width="8%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140722_p3788266712255"><a name="zh-cn_topic_0194140722_p3788266712255"></a><a name="zh-cn_topic_0194140722_p3788266712255"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140722_p4859720612255"><a name="zh-cn_topic_0194140722_p4859720612255"></a><a name="zh-cn_topic_0194140722_p4859720612255"></a>DIS 通道名称。</p>
<p id="zh-cn_topic_0194140722_p3472167512255"><a name="zh-cn_topic_0194140722_p3472167512255"></a><a name="zh-cn_topic_0194140722_p3472167512255"></a>将<span class="parmname" id="zh-cn_topic_0194140722_parmname3362171210482"><a name="zh-cn_topic_0194140722_parmname3362171210482"></a><a name="zh-cn_topic_0194140722_parmname3362171210482"></a>“filePattern”</span>所匹配到的文件内容按分隔符解析并上传到此通道。</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140722_p6099231412255"><a name="zh-cn_topic_0194140722_p6099231412255"></a><a name="zh-cn_topic_0194140722_p6099231412255"></a>请根据实际情况配置</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140722_row3137436512236"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140722_p3732925812255"><a name="zh-cn_topic_0194140722_p3732925812255"></a><a name="zh-cn_topic_0194140722_p3732925812255"></a>filePattern</p>
</td>
<td class="cellrowborder" valign="top" width="8%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140722_p377104712255"><a name="zh-cn_topic_0194140722_p377104712255"></a><a name="zh-cn_topic_0194140722_p377104712255"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140722_p854214355547"><a name="zh-cn_topic_0194140722_p854214355547"></a><a name="zh-cn_topic_0194140722_p854214355547"></a>文件监控路径，只能监控一个目录下的文件，无法递归目录监控。</p>
<div class="p" id="zh-cn_topic_0194140722_p82152875011"><a name="zh-cn_topic_0194140722_p82152875011"></a><a name="zh-cn_topic_0194140722_p82152875011"></a>如果要监控多个目录，可以在flows下面配置多个<span class="parmname" id="zh-cn_topic_0194140722_parmname1583731085515"><a name="zh-cn_topic_0194140722_parmname1583731085515"></a><a name="zh-cn_topic_0194140722_parmname1583731085515"></a>“DISStream”</span>，文件名可使用“*”进行匹配。<a name="zh-cn_topic_0194140722_ul68535395119"></a><a name="zh-cn_topic_0194140722_ul68535395119"></a><ul id="zh-cn_topic_0194140722_ul68535395119"><li><span class="parmname" id="zh-cn_topic_0194140722_parmname727331115218"><a name="zh-cn_topic_0194140722_parmname727331115218"></a><a name="zh-cn_topic_0194140722_parmname727331115218"></a>“/tmp/*.log”</span>表示匹配<span class="filepath" id="zh-cn_topic_0194140722_filepath13245163615517"><a name="zh-cn_topic_0194140722_filepath13245163615517"></a><a name="zh-cn_topic_0194140722_filepath13245163615517"></a>“/tmp”</span>目录下所有以<span class="parmvalue" id="zh-cn_topic_0194140722_parmvalue115516535614"><a name="zh-cn_topic_0194140722_parmvalue115516535614"></a><a name="zh-cn_topic_0194140722_parmvalue115516535614"></a>“.log”</span>结尾的文件。</li><li><span class="parmname" id="zh-cn_topic_0194140722_parmname184701158525"><a name="zh-cn_topic_0194140722_parmname184701158525"></a><a name="zh-cn_topic_0194140722_parmname184701158525"></a>“/tmp/access-*.log”</span>表示匹配<span class="filepath" id="zh-cn_topic_0194140722_filepath9571175214511"><a name="zh-cn_topic_0194140722_filepath9571175214511"></a><a name="zh-cn_topic_0194140722_filepath9571175214511"></a>“/tmp”</span>目录下所有以<span class="parmvalue" id="zh-cn_topic_0194140722_parmvalue69781592569"><a name="zh-cn_topic_0194140722_parmvalue69781592569"></a><a name="zh-cn_topic_0194140722_parmvalue69781592569"></a>“access-”</span>开头，以<span class="parmvalue" id="zh-cn_topic_0194140722_parmvalue12260513195616"><a name="zh-cn_topic_0194140722_parmvalue12260513195616"></a><a name="zh-cn_topic_0194140722_parmvalue12260513195616"></a>“.log”</span>结尾的文件。</li><li>Windows上路径范例为<span class="parmvalue" id="zh-cn_topic_0194140722_parmvalue545792095620"><a name="zh-cn_topic_0194140722_parmvalue545792095620"></a><a name="zh-cn_topic_0194140722_parmvalue545792095620"></a>“D:\logs\*.log”</span>。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140722_p4577917012255"><a name="zh-cn_topic_0194140722_p4577917012255"></a><a name="zh-cn_topic_0194140722_p4577917012255"></a>请根据实际情况配置</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140722_row17720162413207"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140722_p169019466208"><a name="zh-cn_topic_0194140722_p169019466208"></a><a name="zh-cn_topic_0194140722_p169019466208"></a>directoryRecursionEnabled</p>
</td>
<td class="cellrowborder" valign="top" width="8%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140722_p1169064642012"><a name="zh-cn_topic_0194140722_p1169064642012"></a><a name="zh-cn_topic_0194140722_p1169064642012"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140722_p7690154613200"><a name="zh-cn_topic_0194140722_p7690154613200"></a><a name="zh-cn_topic_0194140722_p7690154613200"></a>是否查找子目录</p>
<a name="zh-cn_topic_0194140722_ul12690134615205"></a><a name="zh-cn_topic_0194140722_ul12690134615205"></a><ul id="zh-cn_topic_0194140722_ul12690134615205"><li>false：不递归查找子目录，只匹配根目录下的文件</li><li>true： 递归查找所有子目录。如filePattern配置为/tmp/*.log，此时可以匹配到/tmp/one.log，/tmp/child/two.log，/tmp/child/child/three.log</li></ul>
<p id="zh-cn_topic_0194140722_p1690124682010"><a name="zh-cn_topic_0194140722_p1690124682010"></a><a name="zh-cn_topic_0194140722_p1690124682010"></a></p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140722_p4690184614202"><a name="zh-cn_topic_0194140722_p4690184614202"></a><a name="zh-cn_topic_0194140722_p4690184614202"></a>false</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140722_row6211962212236"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140722_p1990994412255"><a name="zh-cn_topic_0194140722_p1990994412255"></a><a name="zh-cn_topic_0194140722_p1990994412255"></a>initialPosition</p>
</td>
<td class="cellrowborder" valign="top" width="8%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140722_p209279912255"><a name="zh-cn_topic_0194140722_p209279912255"></a><a name="zh-cn_topic_0194140722_p209279912255"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140722_p3529899312255"><a name="zh-cn_topic_0194140722_p3529899312255"></a><a name="zh-cn_topic_0194140722_p3529899312255"></a>监控起始位置。</p>
<a name="zh-cn_topic_0194140722_ul4925548712255"></a><a name="zh-cn_topic_0194140722_ul4925548712255"></a><ul id="zh-cn_topic_0194140722_ul4925548712255"><li>END_OF_FILE：开始启动时不解析当前匹配的文件，而是从新增文件或新增的内容开始按分隔符解析并上传。</li><li>START_OF_FILE：将“filePattern”配置的所有匹配文件按照修改时间，从旧到新按分隔符解析并上传到DIS服务。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140722_p3607139212255"><a name="zh-cn_topic_0194140722_p3607139212255"></a><a name="zh-cn_topic_0194140722_p3607139212255"></a>START_OF_FILE</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140722_row2587299712236"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140722_p5647932112255"><a name="zh-cn_topic_0194140722_p5647932112255"></a><a name="zh-cn_topic_0194140722_p5647932112255"></a>maxBufferAgeMillis</p>
</td>
<td class="cellrowborder" valign="top" width="8%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140722_p1142227412255"><a name="zh-cn_topic_0194140722_p1142227412255"></a><a name="zh-cn_topic_0194140722_p1142227412255"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140722_p5278900012255"><a name="zh-cn_topic_0194140722_p5278900012255"></a><a name="zh-cn_topic_0194140722_p5278900012255"></a>最长上传等待时间。</p>
<p id="zh-cn_topic_0194140722_p533895312255"><a name="zh-cn_topic_0194140722_p533895312255"></a><a name="zh-cn_topic_0194140722_p533895312255"></a>单位：毫秒</p>
<a name="zh-cn_topic_0194140722_ul4805057812255"></a><a name="zh-cn_topic_0194140722_ul4805057812255"></a><ul id="zh-cn_topic_0194140722_ul4805057812255"><li>记录队列满则立即上传。</li><li>记录队列未满，等待此配置项配置的时间后上传到DIS服务。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140722_p4950990812255"><a name="zh-cn_topic_0194140722_p4950990812255"></a><a name="zh-cn_topic_0194140722_p4950990812255"></a>5000</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140722_row4806425103817"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140722_p92364488715"><a name="zh-cn_topic_0194140722_p92364488715"></a><a name="zh-cn_topic_0194140722_p92364488715"></a>maxBufferSizeRecords</p>
</td>
<td class="cellrowborder" valign="top" width="8%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140722_p023616485711"><a name="zh-cn_topic_0194140722_p023616485711"></a><a name="zh-cn_topic_0194140722_p023616485711"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140722_p2023644817712"><a name="zh-cn_topic_0194140722_p2023644817712"></a><a name="zh-cn_topic_0194140722_p2023644817712"></a>记录队列缓存的最大记录数，如果队列达到此值则立刻上传这批数据。</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140722_p42361848174"><a name="zh-cn_topic_0194140722_p42361848174"></a><a name="zh-cn_topic_0194140722_p42361848174"></a>500</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140722_row2859323612236"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140722_p15356171912417"><a name="zh-cn_topic_0194140722_p15356171912417"></a><a name="zh-cn_topic_0194140722_p15356171912417"></a>partitionKeyOption</p>
</td>
<td class="cellrowborder" valign="top" width="8%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140722_p33568193412"><a name="zh-cn_topic_0194140722_p33568193412"></a><a name="zh-cn_topic_0194140722_p33568193412"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.5.1.3 "><div class="p" id="zh-cn_topic_0194140722_p16356619248"><a name="zh-cn_topic_0194140722_p16356619248"></a><a name="zh-cn_topic_0194140722_p16356619248"></a>每条记录会携带一个PartitionKey，相同PartitionKey的记录会分配到同一个分区。此配置项可设置每条记录的PartitionKey值，取值如下：<a name="zh-cn_topic_0194140722_ul93566195419"></a><a name="zh-cn_topic_0194140722_ul93566195419"></a><ul id="zh-cn_topic_0194140722_ul93566195419"><li>RANDOM_INT：PartitionKey的值为随机数字的字符串，记录均匀分布在每个分区。</li><li>FILE_NAME：PartitionKey的值为文件名称字符串，记录分布在特定的一个分区中。</li><li>FILE_NAME,RANDOM_INT：PartitionKey的值为文件名称字符串与随机数字字符串的组合体，以英文逗号分隔，记录携带所属的文件名并均匀分布在所有分区。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140722_p93560191648"><a name="zh-cn_topic_0194140722_p93560191648"></a><a name="zh-cn_topic_0194140722_p93560191648"></a>RANDOM_INT</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140722_row8871154436"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140722_p11356119244"><a name="zh-cn_topic_0194140722_p11356119244"></a><a name="zh-cn_topic_0194140722_p11356119244"></a>recordDelimiter</p>
</td>
<td class="cellrowborder" valign="top" width="8%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140722_p435651910415"><a name="zh-cn_topic_0194140722_p435651910415"></a><a name="zh-cn_topic_0194140722_p435651910415"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140722_p377619495158"><a name="zh-cn_topic_0194140722_p377619495158"></a><a name="zh-cn_topic_0194140722_p377619495158"></a>每条记录之间的分隔符。</p>
<p id="zh-cn_topic_0194140722_p13561191148"><a name="zh-cn_topic_0194140722_p13561191148"></a><a name="zh-cn_topic_0194140722_p13561191148"></a>取值范围：任意一个字符，且包含在双引号内。</p>
<p id="zh-cn_topic_0194140722_p73649320306"><a name="zh-cn_topic_0194140722_p73649320306"></a><a name="zh-cn_topic_0194140722_p73649320306"></a>取值不可为空，即该配置项不可配置为“”。</p>
<div class="note" id="zh-cn_topic_0194140722_note080712251132"><a name="zh-cn_topic_0194140722_note080712251132"></a><a name="zh-cn_topic_0194140722_note080712251132"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0194140722_p1480714251137"><a name="zh-cn_topic_0194140722_p1480714251137"></a><a name="zh-cn_topic_0194140722_p1480714251137"></a>如果取值为特殊字符，使用反斜杠（\）转义，如分隔符为引号（"），可配置为"\""，如果为反斜杠（\），可配置为"\\"。</p>
<p id="zh-cn_topic_0194140722_p1229145374611"><a name="zh-cn_topic_0194140722_p1229145374611"></a><a name="zh-cn_topic_0194140722_p1229145374611"></a>如果为控制字符如STX（正文开始），可配置为"\u0002"。</p>
</div></div>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140722_p1535712191944"><a name="zh-cn_topic_0194140722_p1535712191944"></a><a name="zh-cn_topic_0194140722_p1535712191944"></a>"\n"</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140722_row1278710581230"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140722_p1535713191247"><a name="zh-cn_topic_0194140722_p1535713191247"></a><a name="zh-cn_topic_0194140722_p1535713191247"></a>isRemainRecordDelimiter</p>
</td>
<td class="cellrowborder" valign="top" width="8%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140722_p33571419543"><a name="zh-cn_topic_0194140722_p33571419543"></a><a name="zh-cn_topic_0194140722_p33571419543"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.5.1.3 "><div class="p" id="zh-cn_topic_0194140722_p17357161918417"><a name="zh-cn_topic_0194140722_p17357161918417"></a><a name="zh-cn_topic_0194140722_p17357161918417"></a>上传记录时，是否携带分隔符。<a name="zh-cn_topic_0194140722_ul103571319140"></a><a name="zh-cn_topic_0194140722_ul103571319140"></a><ul id="zh-cn_topic_0194140722_ul103571319140"><li>true：携带分隔符。</li><li>false：不携带分隔符。</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140722_p15359919144"><a name="zh-cn_topic_0194140722_p15359919144"></a><a name="zh-cn_topic_0194140722_p15359919144"></a>false</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140722_row4938173846"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140722_p1335913195419"><a name="zh-cn_topic_0194140722_p1335913195419"></a><a name="zh-cn_topic_0194140722_p1335913195419"></a>isFileAppendable</p>
</td>
<td class="cellrowborder" valign="top" width="8%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140722_p13596191741"><a name="zh-cn_topic_0194140722_p13596191741"></a><a name="zh-cn_topic_0194140722_p13596191741"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140722_p835918191145"><a name="zh-cn_topic_0194140722_p835918191145"></a><a name="zh-cn_topic_0194140722_p835918191145"></a>文件是否有追加内容的可能。</p>
<a name="zh-cn_topic_0194140722_ul83591819041"></a><a name="zh-cn_topic_0194140722_ul83591819041"></a><ul id="zh-cn_topic_0194140722_ul83591819041"><li>true：文件可能会追加内容。Agent持续监控文件，若文件追加了内容则根据recordDelimiter解析后上传记录。此时要保证文件以recordDelimiter结尾，否则Agent会认为文件追加未完成，继续等待recordDelimiter写入。</li><li>false：文件不会追加内容。文件最后一行不以recordDelimiter结尾，Agent仍会当做最后一条记录上传，上传完成后根据<span class="parmname" id="zh-cn_topic_0194140722_parmname5444154031413"><a name="zh-cn_topic_0194140722_parmname5444154031413"></a><a name="zh-cn_topic_0194140722_parmname5444154031413"></a>“deletePolicy”</span>和<span class="parmname" id="zh-cn_topic_0194140722_parmname18929163991512"><a name="zh-cn_topic_0194140722_parmname18929163991512"></a><a name="zh-cn_topic_0194140722_parmname18929163991512"></a>“fileSuffix”</span>的配置执行文件删除或重命名操作。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140722_p1135915191746"><a name="zh-cn_topic_0194140722_p1135915191746"></a><a name="zh-cn_topic_0194140722_p1135915191746"></a>true</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140722_row1439717389567"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140722_p1664883115715"><a name="zh-cn_topic_0194140722_p1664883115715"></a><a name="zh-cn_topic_0194140722_p1664883115715"></a>maxFileCheckingMillis</p>
</td>
<td class="cellrowborder" valign="top" width="8%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140722_p064815315579"><a name="zh-cn_topic_0194140722_p064815315579"></a><a name="zh-cn_topic_0194140722_p064815315579"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140722_p196489318570"><a name="zh-cn_topic_0194140722_p196489318570"></a><a name="zh-cn_topic_0194140722_p196489318570"></a>最长文件变动检查时间，如果文件在此时间内“大小”、“修改时间”和“文件ID”都没有变化，则认为文件已经完成并开始上传。</p>
<p id="zh-cn_topic_0194140722_p1464818335720"><a name="zh-cn_topic_0194140722_p1464818335720"></a><a name="zh-cn_topic_0194140722_p1464818335720"></a>请根据实际文件变动的频率配置此值，避免文件未完成已开始上传的情况。</p>
<p id="zh-cn_topic_0194140722_p16648143205714"><a name="zh-cn_topic_0194140722_p16648143205714"></a><a name="zh-cn_topic_0194140722_p16648143205714"></a>若文件上传后有变动，则会重新全量上传。</p>
<p id="zh-cn_topic_0194140722_p96484314578"><a name="zh-cn_topic_0194140722_p96484314578"></a><a name="zh-cn_topic_0194140722_p96484314578"></a>单位：毫秒</p>
<div class="note" id="zh-cn_topic_0194140722_note0584333574"><a name="zh-cn_topic_0194140722_note0584333574"></a><a name="zh-cn_topic_0194140722_note0584333574"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0194140722_p156481534576"><a name="zh-cn_topic_0194140722_p156481534576"></a><a name="zh-cn_topic_0194140722_p156481534576"></a>“isFileAppendable”配置为“false”时该配置项生效。</p>
</div></div>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140722_p186482315571"><a name="zh-cn_topic_0194140722_p186482315571"></a><a name="zh-cn_topic_0194140722_p186482315571"></a>5000</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140722_row11911774419"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140722_p1635910191844"><a name="zh-cn_topic_0194140722_p1635910191844"></a><a name="zh-cn_topic_0194140722_p1635910191844"></a>deletePolicy</p>
</td>
<td class="cellrowborder" valign="top" width="8%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140722_p1135917191242"><a name="zh-cn_topic_0194140722_p1135917191242"></a><a name="zh-cn_topic_0194140722_p1135917191242"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.5.1.3 "><div class="p" id="zh-cn_topic_0194140722_p9359131911413"><a name="zh-cn_topic_0194140722_p9359131911413"></a><a name="zh-cn_topic_0194140722_p9359131911413"></a>文件内容上传完成之后的删除策略。<a name="zh-cn_topic_0194140722_ul13597191540"></a><a name="zh-cn_topic_0194140722_ul13597191540"></a><ul id="zh-cn_topic_0194140722_ul13597191540"><li>never：文件内容上传完毕后不删除文件。</li><li>immediate：文件内容上传完毕后删除文件 。<div class="note" id="zh-cn_topic_0194140722_note22638471617"><a name="zh-cn_topic_0194140722_note22638471617"></a><a name="zh-cn_topic_0194140722_note22638471617"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0194140722_p142637413169"><a name="zh-cn_topic_0194140722_p142637413169"></a><a name="zh-cn_topic_0194140722_p142637413169"></a><span class="parmname" id="zh-cn_topic_0194140722_parmname17901317111612"><a name="zh-cn_topic_0194140722_parmname17901317111612"></a><a name="zh-cn_topic_0194140722_parmname17901317111612"></a>“isFileAppendable”</span>配置为<span class="parmvalue" id="zh-cn_topic_0194140722_parmvalue951832151615"><a name="zh-cn_topic_0194140722_parmvalue951832151615"></a><a name="zh-cn_topic_0194140722_parmvalue951832151615"></a>“false”</span>时该配置项生效。</p>
</div></div>
</li></ul>
</div>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140722_p1835920191941"><a name="zh-cn_topic_0194140722_p1835920191941"></a><a name="zh-cn_topic_0194140722_p1835920191941"></a>never</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140722_row20434151118419"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140722_p53593191412"><a name="zh-cn_topic_0194140722_p53593191412"></a><a name="zh-cn_topic_0194140722_p53593191412"></a>fileSuffix</p>
</td>
<td class="cellrowborder" valign="top" width="8%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140722_p1535915191342"><a name="zh-cn_topic_0194140722_p1535915191342"></a><a name="zh-cn_topic_0194140722_p1535915191342"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140722_p26591357122110"><a name="zh-cn_topic_0194140722_p26591357122110"></a><a name="zh-cn_topic_0194140722_p26591357122110"></a>文件内容上传完成之后添加的文件名后缀。</p>
<p id="zh-cn_topic_0194140722_p102681051191818"><a name="zh-cn_topic_0194140722_p102681051191818"></a><a name="zh-cn_topic_0194140722_p102681051191818"></a>例如：原文件名为<span class="filepath" id="zh-cn_topic_0194140722_filepath78318516204"><a name="zh-cn_topic_0194140722_filepath78318516204"></a><a name="zh-cn_topic_0194140722_filepath78318516204"></a>“x.txt”</span>，<span class="parmname" id="zh-cn_topic_0194140722_parmname1891865716208"><a name="zh-cn_topic_0194140722_parmname1891865716208"></a><a name="zh-cn_topic_0194140722_parmname1891865716208"></a>“fileSuffix”</span>配置为<span class="parmvalue" id="zh-cn_topic_0194140722_parmvalue128708110213"><a name="zh-cn_topic_0194140722_parmvalue128708110213"></a><a name="zh-cn_topic_0194140722_parmvalue128708110213"></a>“.COMPLETED”</span>，则文件上传后的命名为<span class="filepath" id="zh-cn_topic_0194140722_filepath17100171211"><a name="zh-cn_topic_0194140722_filepath17100171211"></a><a name="zh-cn_topic_0194140722_filepath17100171211"></a>“x.txt.COMPLETED”</span>。</p>
<div class="note" id="zh-cn_topic_0194140722_note14281103914188"><a name="zh-cn_topic_0194140722_note14281103914188"></a><a name="zh-cn_topic_0194140722_note14281103914188"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0194140722_p1281193918186"><a name="zh-cn_topic_0194140722_p1281193918186"></a><a name="zh-cn_topic_0194140722_p1281193918186"></a><span class="parmname" id="zh-cn_topic_0194140722_parmname155418442188"><a name="zh-cn_topic_0194140722_parmname155418442188"></a><a name="zh-cn_topic_0194140722_parmname155418442188"></a>“isFileAppendable”</span>配置为<span class="parmvalue" id="zh-cn_topic_0194140722_parmvalue35684413189"><a name="zh-cn_topic_0194140722_parmvalue35684413189"></a><a name="zh-cn_topic_0194140722_parmvalue35684413189"></a>“false”</span>，同时<span class="parmname" id="zh-cn_topic_0194140722_parmname2063432691913"><a name="zh-cn_topic_0194140722_parmname2063432691913"></a><a name="zh-cn_topic_0194140722_parmname2063432691913"></a>“deletePolicy”</span>配置为<span class="parmvalue" id="zh-cn_topic_0194140722_parmvalue19519185716199"><a name="zh-cn_topic_0194140722_parmvalue19519185716199"></a><a name="zh-cn_topic_0194140722_parmvalue19519185716199"></a>“never”</span>，该配置项生效。</p>
</div></div>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140722_p1536081911415"><a name="zh-cn_topic_0194140722_p1536081911415"></a><a name="zh-cn_topic_0194140722_p1536081911415"></a>.COMPLETED</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140722_row5933361812236"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140722_p514995312255"><a name="zh-cn_topic_0194140722_p514995312255"></a><a name="zh-cn_topic_0194140722_p514995312255"></a>sendingThreadSize</p>
</td>
<td class="cellrowborder" valign="top" width="8%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140722_p1449306612255"><a name="zh-cn_topic_0194140722_p1449306612255"></a><a name="zh-cn_topic_0194140722_p1449306612255"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140722_p39847201121525"><a name="zh-cn_topic_0194140722_p39847201121525"></a><a name="zh-cn_topic_0194140722_p39847201121525"></a>发送线程数。默认单线程发送。</p>
<div class="notice" id="zh-cn_topic_0194140722_note6132691121654"><a name="zh-cn_topic_0194140722_note6132691121654"></a><a name="zh-cn_topic_0194140722_note6132691121654"></a><span class="noticetitle"> 须知： </span><div class="noticebody"><p id="zh-cn_topic_0194140722_p2440497112194"><a name="zh-cn_topic_0194140722_p2440497112194"></a><a name="zh-cn_topic_0194140722_p2440497112194"></a>使用多线程会导致如下问题：</p>
<a name="zh-cn_topic_0194140722_ul52849325121724"></a><a name="zh-cn_topic_0194140722_ul52849325121724"></a><ul id="zh-cn_topic_0194140722_ul52849325121724"><li>数据发送不保证顺序。</li><li>程序异常停止并重新启动时会丢失部分数据。</li></ul>
</div></div>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140722_p6285533212255"><a name="zh-cn_topic_0194140722_p6285533212255"></a><a name="zh-cn_topic_0194140722_p6285533212255"></a>1</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140722_row463678144816"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140722_p182819281487"><a name="zh-cn_topic_0194140722_p182819281487"></a><a name="zh-cn_topic_0194140722_p182819281487"></a>fileEncoding</p>
</td>
<td class="cellrowborder" valign="top" width="8%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140722_p162811288488"><a name="zh-cn_topic_0194140722_p162811288488"></a><a name="zh-cn_topic_0194140722_p162811288488"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140722_p1528152816481"><a name="zh-cn_topic_0194140722_p1528152816481"></a><a name="zh-cn_topic_0194140722_p1528152816481"></a>文件编码格式，支持UTF8, GBK, GB2312, ISO-8859-1等</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140722_p19281282486"><a name="zh-cn_topic_0194140722_p19281282486"></a><a name="zh-cn_topic_0194140722_p19281282486"></a>UTF8</p>
</td>
</tr>
<tr id="zh-cn_topic_0194140722_row88242944715"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0194140722_p930204311475"><a name="zh-cn_topic_0194140722_p930204311475"></a><a name="zh-cn_topic_0194140722_p930204311475"></a>resultLogLevel</p>
</td>
<td class="cellrowborder" valign="top" width="8%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0194140722_p630234374714"><a name="zh-cn_topic_0194140722_p630234374714"></a><a name="zh-cn_topic_0194140722_p630234374714"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0194140722_p430294354710"><a name="zh-cn_topic_0194140722_p430294354710"></a><a name="zh-cn_topic_0194140722_p430294354710"></a>每次调用DIS数据发送接口后的结果日志级别。</p>
<a name="zh-cn_topic_0194140722_ul9302243204718"></a><a name="zh-cn_topic_0194140722_ul9302243204718"></a><ul id="zh-cn_topic_0194140722_ul9302243204718"><li>OFF：日志中不输出每次接口调用的结果。</li><li>INFO：每次接口调用的结果以INFO级别输出到日志。</li><li>WARN：每次接口调用的结果以WARN级别输出到日志。</li><li>ERROR：每次接口调用的结果以ERROR级别输出到日志。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0194140722_p3302743144710"><a name="zh-cn_topic_0194140722_p3302743144710"></a><a name="zh-cn_topic_0194140722_p3302743144710"></a>INFO</p>
</td>
</tr>
</tbody>
</table>

