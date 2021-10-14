# 配置DIS Agent<a name="dgc_01_0222"></a>

DIS Agent配置文件格式为“YAML”，各配置项与值之间必须以英文格式的“冒号+空格”形式分隔。

agent.yml文件模板可从“dis-agent”压缩包中获取，内容示例如下。具体配置项说明请参见[表1](#table192441715172513)。

```
---
# cloud region id
region: cn-north-1
# you ak (get from 'My Credential')
ak: YOU_AK
# you sk (get from 'My Credential')
sk: YOU_SK
# you project id (get from 'My Credential')
projectId: YOU_PROJECTID
# the dis endpoint
endpoint: https://dis.cn-north-1.myhuaweicloud.com
# config each flow to monitor file.
flows:
  ### DIS Stream
  - DISStream: YOU_DIS_STREAM_1
    ## only support specified directory, filename can use * to match some files. eg. * means match all file, test*.log means match test1.log or test-12.log and so on.
    filePattern: /tmp/*.log
    ## from where to start: 'START_OF_FILE' or 'END_OF_FILE'
    initialPosition: START_OF_FILE
    ## upload max interval(ms)
    maxBufferAgeMillis: 5000

  ### If there are other monitor files, continue to follow the above configuration
  ### another dis stream monitor config, uncomment # if you want to use this feature
  #- DISStream: YOU_DIS_STREAM_2
  #  filePattern: /opt/*.log
  #  initialPosition: START_OF_FILE
  #  maxBufferAgeMillis: 5000

  ### OBS Stream: Upload the matching file to OBS and send the file name to DIS, uncomment # if you want to use this feature
  #- OBSStream: YOU_DIS_STREAM_3
  #  filePattern: /opt/*.log
  #  initialPosition: START_OF_FILE
  #  ## bucket name
  #  OBSBucket: YOU_OBS_BUCKET_NAME
  #  ## OBS endpoint
  #  OBSEndpoint: https://obs.cn-north-1.myhuaweicloud.com
  #  ## the directory(using / separated) where the files are stored under the bucket, automatically created if it does not exist
  #  dumpDirectory: example/dis/

```

>![](public_sys-resources/icon-note.gif) **说明：** 
>配置完成之后，请将agent.yml中flows下面无用的示例配置删除或者使用\#注释（比如只配置了一个DISStream，则将下面的CustomFileStream与另外的DISStream模块删除或者注释）。

## Linux服务器上配置DIS Agent<a name="zh-cn_topic_0194140722_section4916936311221"></a>

1.  使用PuTTY 工具登录日志所在服务器。
2.  执行**cd /opt/dis-agent-X.X.X/**命令，进入“dis-agent-X.X.X“文件夹。
3.  执行**vim conf/agent.yml**命令，打开DIS Agent配置文件“agent.yml“，根据实际情况修改各配置项的值并保存，配置项说明请参见[表1](#table192441715172513)。

    **表 1**  agent.yml配置文件说明

    <a name="table192441715172513"></a>
    <table><thead align="left"><tr id="row19244171514259"><th class="cellrowborder" valign="top" width="16.328367163283673%" id="mcps1.2.5.1.1"><p id="p1324414156252"><a name="p1324414156252"></a><a name="p1324414156252"></a>配置项</p>
    </th>
    <th class="cellrowborder" valign="top" width="8.159184081591842%" id="mcps1.2.5.1.2"><p id="p1524421572518"><a name="p1524421572518"></a><a name="p1524421572518"></a>是否必填</p>
    </th>
    <th class="cellrowborder" valign="top" width="37.75622437756224%" id="mcps1.2.5.1.3"><p id="p1824591572518"><a name="p1824591572518"></a><a name="p1824591572518"></a>说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="37.75622437756224%" id="mcps1.2.5.1.4"><p id="p224551582516"><a name="p224551582516"></a><a name="p224551582516"></a>默认值</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row172451515132517"><td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.1 "><p id="p3245315142515"><a name="p3245315142515"></a><a name="p3245315142515"></a>region</p>
    </td>
    <td class="cellrowborder" valign="top" width="8.159184081591842%" headers="mcps1.2.5.1.2 "><p id="p14245181582518"><a name="p14245181582518"></a><a name="p14245181582518"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.3 "><p id="p102453156259"><a name="p102453156259"></a><a name="p102453156259"></a>DIS服务所在区域。</p>
    <div class="note" id="note162452158258"><a name="note162452158258"></a><a name="note162452158258"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p624512154258"><a name="p624512154258"></a><a name="p624512154258"></a>获取DIS区域请参见<a href="https://developer.huaweicloud.com/endpoint?DIS" target="_blank" rel="noopener noreferrer">终端节点及区域说明</a>。</p>
    </div></div>
    </td>
    <td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.4 "><p id="p13245131513254"><a name="p13245131513254"></a><a name="p13245131513254"></a>cn-north-1</p>
    </td>
    </tr>
    <tr id="row16245815192515"><td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.1 "><p id="p182459153250"><a name="p182459153250"></a><a name="p182459153250"></a>ak</p>
    </td>
    <td class="cellrowborder" valign="top" width="8.159184081591842%" headers="mcps1.2.5.1.2 "><p id="p1524511514257"><a name="p1524511514257"></a><a name="p1524511514257"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.3 "><p id="p32467151258"><a name="p32467151258"></a><a name="p32467151258"></a>用户的Access Key。</p>
    <p id="p192468154253"><a name="p192468154253"></a><a name="p192468154253"></a>获取方式请参见<a href="安装前准备.md#zh-cn_topic_0194140940_s929153773cb54e1b801a8399b2ef9b2f">检查认证信息</a>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.4 "><p id="p17246191592510"><a name="p17246191592510"></a><a name="p17246191592510"></a>请根据实际情况配置</p>
    </td>
    </tr>
    <tr id="row102461115142512"><td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.1 "><p id="p1246171532517"><a name="p1246171532517"></a><a name="p1246171532517"></a>sk</p>
    </td>
    <td class="cellrowborder" valign="top" width="8.159184081591842%" headers="mcps1.2.5.1.2 "><p id="p17246101512516"><a name="p17246101512516"></a><a name="p17246101512516"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.3 "><p id="p152461515192516"><a name="p152461515192516"></a><a name="p152461515192516"></a>用户的Secret Key。</p>
    <p id="p18246115122519"><a name="p18246115122519"></a><a name="p18246115122519"></a>获取方式请参见<a href="安装前准备.md#zh-cn_topic_0194140940_s929153773cb54e1b801a8399b2ef9b2f">检查认证信息</a>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.4 "><p id="p1324631511251"><a name="p1324631511251"></a><a name="p1324631511251"></a>请根据实际情况配置</p>
    </td>
    </tr>
    <tr id="row6246201582518"><td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.1 "><p id="p1124691514253"><a name="p1124691514253"></a><a name="p1124691514253"></a>projectId</p>
    </td>
    <td class="cellrowborder" valign="top" width="8.159184081591842%" headers="mcps1.2.5.1.2 "><p id="p1924611513256"><a name="p1924611513256"></a><a name="p1924611513256"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.3 "><p id="p924691520254"><a name="p924691520254"></a><a name="p924691520254"></a>用户所属区域的项目ID。</p>
    <p id="p224681519250"><a name="p224681519250"></a><a name="p224681519250"></a>获取方式请参见<a href="安装前准备.md#zh-cn_topic_0194140940_s929153773cb54e1b801a8399b2ef9b2f">检查认证信息</a>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.4 "><p id="p122461515132510"><a name="p122461515132510"></a><a name="p122461515132510"></a>请根据实际情况配置</p>
    </td>
    </tr>
    <tr id="row8246201519258"><td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.1 "><p id="p52471215122519"><a name="p52471215122519"></a><a name="p52471215122519"></a>endpoint</p>
    </td>
    <td class="cellrowborder" valign="top" width="8.159184081591842%" headers="mcps1.2.5.1.2 "><p id="p20247141514254"><a name="p20247141514254"></a><a name="p20247141514254"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.3 "><p id="p13247315112513"><a name="p13247315112513"></a><a name="p13247315112513"></a>DIS数据网关地址。</p>
    <p id="p10247715182512"><a name="p10247715182512"></a><a name="p10247715182512"></a>格式：https://DIS终端节点。</p>
    <div class="note" id="note148471506534"><a name="note148471506534"></a><a name="note148471506534"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p9847150165319"><a name="p9847150165319"></a><a name="p9847150165319"></a>获取DIS终端节点请参见<a href="https://developer.huaweicloud.com/endpoint?DIS" target="_blank" rel="noopener noreferrer">终端节点及区域说明</a>。</p>
    </div></div>
    </td>
    <td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.4 "><p id="p92472159250"><a name="p92472159250"></a><a name="p92472159250"></a>https://dis.cn-north-1.myhuaweicloud.com</p>
    </td>
    </tr>
    <tr id="row20247181510251"><td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.1 "><p id="p124771572519"><a name="p124771572519"></a><a name="p124771572519"></a>body.serialize.type</p>
    </td>
    <td class="cellrowborder" valign="top" width="8.159184081591842%" headers="mcps1.2.5.1.2 "><p id="p19247315202511"><a name="p19247315202511"></a><a name="p19247315202511"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.3 "><div class="p" id="p1424712155251"><a name="p1424712155251"></a><a name="p1424712155251"></a>DIS数据包上传格式。（非原始数据格式）<a name="ul124891516255"></a><a name="ul124891516255"></a><ul id="ul124891516255"><li>json：DIS数据包封装为json格式，满足普通使用。</li><li>protobuf：DIS数据包封装为二进制格式，可以减少体积约1/3，在数据量较大的情况下推荐使用此格式。</li></ul>
    </div>
    </td>
    <td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.4 "><p id="p6248121516257"><a name="p6248121516257"></a><a name="p6248121516257"></a>json</p>
    </td>
    </tr>
    <tr id="row7248181513258"><td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.1 "><p id="p624819153252"><a name="p624819153252"></a><a name="p624819153252"></a>body.compress.enabled</p>
    </td>
    <td class="cellrowborder" valign="top" width="8.159184081591842%" headers="mcps1.2.5.1.2 "><p id="p10248191513256"><a name="p10248191513256"></a><a name="p10248191513256"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.3 "><p id="p624811542517"><a name="p624811542517"></a><a name="p624811542517"></a>是否开启传输数据压缩。</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.4 "><p id="p5248181519256"><a name="p5248181519256"></a><a name="p5248181519256"></a>false</p>
    </td>
    </tr>
    <tr id="row12248615142511"><td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.1 "><p id="p152481915192512"><a name="p152481915192512"></a><a name="p152481915192512"></a>body.compress.type</p>
    </td>
    <td class="cellrowborder" valign="top" width="8.159184081591842%" headers="mcps1.2.5.1.2 "><p id="p1824813159256"><a name="p1824813159256"></a><a name="p1824813159256"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.3 "><p id="p624861512520"><a name="p624861512520"></a><a name="p624861512520"></a>开启压缩时选择的数据压缩格式，目前支持的压缩格式如下：</p>
    <p id="p17248815142515"><a name="p17248815142515"></a><a name="p17248815142515"></a>lz4：综合来看效率最高的压缩算法,更加侧重压缩解压速度,压缩比并不是第一。</p>
    <p id="p15249121518253"><a name="p15249121518253"></a><a name="p15249121518253"></a>zstd：一种新的无损压缩算法，旨在提供快速压缩，并实现高压缩比。</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.4 "><p id="p12249141572515"><a name="p12249141572515"></a><a name="p12249141572515"></a>lz4</p>
    </td>
    </tr>
    <tr id="row1824912151259"><td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.1 "><p id="p182491115102520"><a name="p182491115102520"></a><a name="p182491115102520"></a>PROXY_HOST</p>
    </td>
    <td class="cellrowborder" valign="top" width="8.159184081591842%" headers="mcps1.2.5.1.2 "><p id="p1249101532510"><a name="p1249101532510"></a><a name="p1249101532510"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.3 "><p id="p324961542516"><a name="p324961542516"></a><a name="p324961542516"></a>配置代理IP，请求走代理服务器的需要配置。</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.4 "><p id="p12249201520251"><a name="p12249201520251"></a><a name="p12249201520251"></a>请根据实际情况配置</p>
    </td>
    </tr>
    <tr id="row1324911152255"><td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.1 "><p id="p2024919156253"><a name="p2024919156253"></a><a name="p2024919156253"></a>PROXY_PORT</p>
    </td>
    <td class="cellrowborder" valign="top" width="8.159184081591842%" headers="mcps1.2.5.1.2 "><p id="p192497154255"><a name="p192497154255"></a><a name="p192497154255"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.3 "><p id="p1624961522513"><a name="p1624961522513"></a><a name="p1624961522513"></a>配置代理端口。</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.4 "><p id="p1324971512516"><a name="p1324971512516"></a><a name="p1324971512516"></a>80</p>
    </td>
    </tr>
    <tr id="row924901517256"><td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.1 "><p id="p18249515182512"><a name="p18249515182512"></a><a name="p18249515182512"></a>PROXY_PROTOCOL</p>
    </td>
    <td class="cellrowborder" valign="top" width="8.159184081591842%" headers="mcps1.2.5.1.2 "><p id="p152501315122513"><a name="p152501315122513"></a><a name="p152501315122513"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.3 "><p id="p3250151512257"><a name="p3250151512257"></a><a name="p3250151512257"></a>配置代理协议。支持http和https。</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.4 "><p id="p62509151255"><a name="p62509151255"></a><a name="p62509151255"></a>http</p>
    </td>
    </tr>
    <tr id="row1525017151253"><td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.1 "><p id="p1725081572518"><a name="p1725081572518"></a><a name="p1725081572518"></a>PROXY_USERNAME</p>
    </td>
    <td class="cellrowborder" valign="top" width="8.159184081591842%" headers="mcps1.2.5.1.2 "><p id="p112501015152511"><a name="p112501015152511"></a><a name="p112501015152511"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.3 "><p id="p1325081516259"><a name="p1325081516259"></a><a name="p1325081516259"></a>配置代理用户名。</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.4 "><p id="p172501815202515"><a name="p172501815202515"></a><a name="p172501815202515"></a>请根据实际情况配置</p>
    </td>
    </tr>
    <tr id="row132501915192510"><td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.1 "><p id="p62501115112516"><a name="p62501115112516"></a><a name="p62501115112516"></a>PROXY_PASSWORD</p>
    </td>
    <td class="cellrowborder" valign="top" width="8.159184081591842%" headers="mcps1.2.5.1.2 "><p id="p625018158254"><a name="p625018158254"></a><a name="p625018158254"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.3 "><p id="p8250111532513"><a name="p8250111532513"></a><a name="p8250111532513"></a>配置代理密码。</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.75622437756224%" headers="mcps1.2.5.1.4 "><p id="p72512155257"><a name="p72512155257"></a><a name="p72512155257"></a>请根据实际情况配置</p>
    </td>
    </tr>
    <tr id="row10251915132518"><td class="cellrowborder" colspan="4" valign="top" headers="mcps1.2.5.1.1 mcps1.2.5.1.2 mcps1.2.5.1.3 mcps1.2.5.1.4 "><p id="p14251191582512"><a name="p14251191582512"></a><a name="p14251191582512"></a>[flows]</p>
    <p id="p142511015192518"><a name="p142511015192518"></a><a name="p142511015192518"></a>监控的文件信息，可同时配置多个监控文件信息。</p>
    <p id="p82518152256"><a name="p82518152256"></a><a name="p82518152256"></a>当前支持如下模式上传：</p>
    <p id="p6251121522518"><a name="p6251121522518"></a><a name="p6251121522518"></a>DISStream:持续监控文本文件，实时收集增量数据按分隔符解析并上传到DIS通道(通道源数据类型为BLOB/JSON/CSV)，配置项说明请参见<a href="#table4887181017263">表2</a>。</p>
    <p id="p16251615192513"><a name="p16251615192513"></a><a name="p16251615192513"></a>具体配置格式可以参见版本包中的“agent.yml”的样例。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 2**  DISStream配置项说明

    <a name="table4887181017263"></a>
    <table><thead align="left"><tr id="row98871710172619"><th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.1"><p id="p2088716101268"><a name="p2088716101268"></a><a name="p2088716101268"></a>配置项</p>
    </th>
    <th class="cellrowborder" valign="top" width="8%" id="mcps1.2.5.1.2"><p id="p488781022614"><a name="p488781022614"></a><a name="p488781022614"></a>是否必填</p>
    </th>
    <th class="cellrowborder" valign="top" width="62%" id="mcps1.2.5.1.3"><p id="p288731012269"><a name="p288731012269"></a><a name="p288731012269"></a>说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="14.000000000000002%" id="mcps1.2.5.1.4"><p id="p388761022612"><a name="p388761022612"></a><a name="p388761022612"></a>默认值</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row11888131062617"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="p1388861010265"><a name="p1388861010265"></a><a name="p1388861010265"></a>DISStream</p>
    </td>
    <td class="cellrowborder" valign="top" width="8%" headers="mcps1.2.5.1.2 "><p id="p18888131092616"><a name="p18888131092616"></a><a name="p18888131092616"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.5.1.3 "><p id="p1188871014262"><a name="p1188871014262"></a><a name="p1188871014262"></a>DIS 通道名称。</p>
    <p id="p9888121052618"><a name="p9888121052618"></a><a name="p9888121052618"></a>将<span class="parmname" id="parmname11888410122614"><a name="parmname11888410122614"></a><a name="parmname11888410122614"></a>“filePattern”</span>所匹配到的文件内容按分隔符解析并上传到此通道。</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.4 "><p id="p12888141062617"><a name="p12888141062617"></a><a name="p12888141062617"></a>请根据实际情况配置</p>
    </td>
    </tr>
    <tr id="row28887107264"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="p5888181052616"><a name="p5888181052616"></a><a name="p5888181052616"></a>filePattern</p>
    </td>
    <td class="cellrowborder" valign="top" width="8%" headers="mcps1.2.5.1.2 "><p id="p1488814103266"><a name="p1488814103266"></a><a name="p1488814103266"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.5.1.3 "><p id="p6888111020261"><a name="p6888111020261"></a><a name="p6888111020261"></a>文件监控路径，只能监控一个目录下的文件，无法递归目录监控。</p>
    <div class="p" id="p1888710192613"><a name="p1888710192613"></a><a name="p1888710192613"></a>如果要监控多个目录，可以在flows下面配置多个<span class="parmname" id="parmname588891019266"><a name="parmname588891019266"></a><a name="parmname588891019266"></a>“DISStream”</span>，文件名可使用“*”进行匹配。<a name="ul10888191020262"></a><a name="ul10888191020262"></a><ul id="ul10888191020262"><li><span class="parmname" id="parmname28898102267"><a name="parmname28898102267"></a><a name="parmname28898102267"></a>“/tmp/*.log”</span>表示匹配<span class="filepath" id="filepath1588971012267"><a name="filepath1588971012267"></a><a name="filepath1588971012267"></a>“/tmp”</span>目录下所有以<span class="parmvalue" id="parmvalue168898102267"><a name="parmvalue168898102267"></a><a name="parmvalue168898102267"></a>“.log”</span>结尾的文件。</li><li><span class="parmname" id="parmname1188911082620"><a name="parmname1188911082620"></a><a name="parmname1188911082620"></a>“/tmp/access-*.log”</span>表示匹配<span class="filepath" id="filepath7889191013264"><a name="filepath7889191013264"></a><a name="filepath7889191013264"></a>“/tmp”</span>目录下所有以<span class="parmvalue" id="parmvalue1888951012265"><a name="parmvalue1888951012265"></a><a name="parmvalue1888951012265"></a>“access-”</span>开头，以<span class="parmvalue" id="parmvalue158891910182612"><a name="parmvalue158891910182612"></a><a name="parmvalue158891910182612"></a>“.log”</span>结尾的文件。</li><li>Windows上路径范例为<span class="parmvalue" id="parmvalue58906106262"><a name="parmvalue58906106262"></a><a name="parmvalue58906106262"></a>“D:\logs\*.log”</span>。</li></ul>
    </div>
    </td>
    <td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.4 "><p id="p148901110142616"><a name="p148901110142616"></a><a name="p148901110142616"></a>请根据实际情况配置</p>
    </td>
    </tr>
    <tr id="row118901810192610"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="p19890171072618"><a name="p19890171072618"></a><a name="p19890171072618"></a>directoryRecursionEnabled</p>
    </td>
    <td class="cellrowborder" valign="top" width="8%" headers="mcps1.2.5.1.2 "><p id="p28901710172615"><a name="p28901710172615"></a><a name="p28901710172615"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.5.1.3 "><p id="p1789015109267"><a name="p1789015109267"></a><a name="p1789015109267"></a>是否查找子目录</p>
    <a name="ul1189031062620"></a><a name="ul1189031062620"></a><ul id="ul1189031062620"><li>false：不递归查找子目录，只匹配根目录下的文件</li><li>true： 递归查找所有子目录。如filePattern配置为/tmp/*.log，此时可以匹配到/tmp/one.log，/tmp/child/two.log，/tmp/child/child/three.log</li></ul>
    <p id="p38907102261"><a name="p38907102261"></a><a name="p38907102261"></a></p>
    </td>
    <td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.4 "><p id="p48901010132611"><a name="p48901010132611"></a><a name="p48901010132611"></a>false</p>
    </td>
    </tr>
    <tr id="row2891111092615"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="p14891111012620"><a name="p14891111012620"></a><a name="p14891111012620"></a>initialPosition</p>
    </td>
    <td class="cellrowborder" valign="top" width="8%" headers="mcps1.2.5.1.2 "><p id="p11891710102613"><a name="p11891710102613"></a><a name="p11891710102613"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.5.1.3 "><p id="p9891710132613"><a name="p9891710132613"></a><a name="p9891710132613"></a>监控起始位置。</p>
    <a name="ul489131082612"></a><a name="ul489131082612"></a><ul id="ul489131082612"><li>END_OF_FILE：开始启动时不解析当前匹配的文件，而是从新增文件或新增的内容开始按分隔符解析并上传。</li><li>START_OF_FILE：将“filePattern”配置的所有匹配文件按照修改时间，从旧到新按分隔符解析并上传到DIS服务。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.4 "><p id="p12891201015266"><a name="p12891201015266"></a><a name="p12891201015266"></a>START_OF_FILE</p>
    </td>
    </tr>
    <tr id="row289113107264"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="p1891131019263"><a name="p1891131019263"></a><a name="p1891131019263"></a>maxBufferAgeMillis</p>
    </td>
    <td class="cellrowborder" valign="top" width="8%" headers="mcps1.2.5.1.2 "><p id="p489141072612"><a name="p489141072612"></a><a name="p489141072612"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.5.1.3 "><p id="p4891310172612"><a name="p4891310172612"></a><a name="p4891310172612"></a>最长上传等待时间。</p>
    <p id="p178911810142615"><a name="p178911810142615"></a><a name="p178911810142615"></a>单位：毫秒</p>
    <a name="ul689121062617"></a><a name="ul689121062617"></a><ul id="ul689121062617"><li>记录队列满则立即上传。</li><li>记录队列未满，等待此配置项配置的时间后上传到DIS服务。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.4 "><p id="p3891161018261"><a name="p3891161018261"></a><a name="p3891161018261"></a>5000</p>
    </td>
    </tr>
    <tr id="row178911410132619"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="p17891810192617"><a name="p17891810192617"></a><a name="p17891810192617"></a>maxBufferSizeRecords</p>
    </td>
    <td class="cellrowborder" valign="top" width="8%" headers="mcps1.2.5.1.2 "><p id="p118921510182620"><a name="p118921510182620"></a><a name="p118921510182620"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.5.1.3 "><p id="p1489211002611"><a name="p1489211002611"></a><a name="p1489211002611"></a>记录队列缓存的最大记录数，如果队列达到此值则立刻上传这批数据。</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.4 "><p id="p989231042616"><a name="p989231042616"></a><a name="p989231042616"></a>500</p>
    </td>
    </tr>
    <tr id="row1489219105264"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="p1689211101261"><a name="p1689211101261"></a><a name="p1689211101261"></a>partitionKeyOption</p>
    </td>
    <td class="cellrowborder" valign="top" width="8%" headers="mcps1.2.5.1.2 "><p id="p108921410202617"><a name="p108921410202617"></a><a name="p108921410202617"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.5.1.3 "><div class="p" id="p14892151042617"><a name="p14892151042617"></a><a name="p14892151042617"></a>每条记录会携带一个PartitionKey，相同PartitionKey的记录会分配到同一个分区。此配置项可设置每条记录的PartitionKey值，取值如下：<a name="ul1189241062614"></a><a name="ul1189241062614"></a><ul id="ul1189241062614"><li>RANDOM_INT：PartitionKey的值为随机数字的字符串，记录均匀分布在每个分区。</li><li>FILE_NAME：PartitionKey的值为文件名称字符串，记录分布在特定的一个分区中。</li><li>FILE_NAME,RANDOM_INT：PartitionKey的值为文件名称字符串与随机数字字符串的组合体，以英文逗号分隔，记录携带所属的文件名并均匀分布在所有分区。</li></ul>
    </div>
    </td>
    <td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.4 "><p id="p12892110142616"><a name="p12892110142616"></a><a name="p12892110142616"></a>RANDOM_INT</p>
    </td>
    </tr>
    <tr id="row1789331013266"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="p138931910142613"><a name="p138931910142613"></a><a name="p138931910142613"></a>recordDelimiter</p>
    </td>
    <td class="cellrowborder" valign="top" width="8%" headers="mcps1.2.5.1.2 "><p id="p6893161082615"><a name="p6893161082615"></a><a name="p6893161082615"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.5.1.3 "><p id="p88931010112618"><a name="p88931010112618"></a><a name="p88931010112618"></a>每条记录之间的分隔符。</p>
    <p id="p389313101261"><a name="p389313101261"></a><a name="p389313101261"></a>取值范围：任意一个字符，且包含在双引号内。</p>
    <p id="p1189314107264"><a name="p1189314107264"></a><a name="p1189314107264"></a>取值不可为空，即该配置项不可配置为“”。</p>
    <div class="note" id="note11893111012261"><a name="note11893111012261"></a><a name="note11893111012261"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p1989341019264"><a name="p1989341019264"></a><a name="p1989341019264"></a>如果取值为特殊字符，使用反斜杠（\）转义，如分隔符为引号（"），可配置为"\""，如果为反斜杠（\），可配置为"\\"。</p>
    <p id="p1489315107263"><a name="p1489315107263"></a><a name="p1489315107263"></a>如果为控制字符如STX（正文开始），可配置为"\u0002"。</p>
    </div></div>
    </td>
    <td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.4 "><p id="p1289311105262"><a name="p1289311105262"></a><a name="p1289311105262"></a>"\n"</p>
    </td>
    </tr>
    <tr id="row1589371092615"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="p889313103262"><a name="p889313103262"></a><a name="p889313103262"></a>isRemainRecordDelimiter</p>
    </td>
    <td class="cellrowborder" valign="top" width="8%" headers="mcps1.2.5.1.2 "><p id="p8893191013262"><a name="p8893191013262"></a><a name="p8893191013262"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.5.1.3 "><div class="p" id="p1489311072613"><a name="p1489311072613"></a><a name="p1489311072613"></a>上传记录时，是否携带分隔符。<a name="ul1893111072618"></a><a name="ul1893111072618"></a><ul id="ul1893111072618"><li>true：携带分隔符。</li><li>false：不携带分隔符。</li></ul>
    </div>
    </td>
    <td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.4 "><p id="p19894191011268"><a name="p19894191011268"></a><a name="p19894191011268"></a>false</p>
    </td>
    </tr>
    <tr id="row198941610112611"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="p208946109269"><a name="p208946109269"></a><a name="p208946109269"></a>isFileAppendable</p>
    </td>
    <td class="cellrowborder" valign="top" width="8%" headers="mcps1.2.5.1.2 "><p id="p0894101052618"><a name="p0894101052618"></a><a name="p0894101052618"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.5.1.3 "><p id="p48949102265"><a name="p48949102265"></a><a name="p48949102265"></a>文件是否有追加内容的可能。</p>
    <a name="ul198941110192619"></a><a name="ul198941110192619"></a><ul id="ul198941110192619"><li>true：文件可能会追加内容。Agent持续监控文件，若文件追加了内容则根据recordDelimiter解析后上传记录。此时要保证文件以recordDelimiter结尾，否则Agent会认为文件追加未完成，继续等待recordDelimiter写入。</li><li>false：文件不会追加内容。文件最后一行不以recordDelimiter结尾，Agent仍会当做最后一条记录上传，上传完成后根据<span class="parmname" id="parmname789415104269"><a name="parmname789415104269"></a><a name="parmname789415104269"></a>“deletePolicy”</span>和<span class="parmname" id="parmname58943109266"><a name="parmname58943109266"></a><a name="parmname58943109266"></a>“fileSuffix”</span>的配置执行文件删除或重命名操作。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.4 "><p id="p198941710192611"><a name="p198941710192611"></a><a name="p198941710192611"></a>true</p>
    </td>
    </tr>
    <tr id="row0894310152611"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="p38951107261"><a name="p38951107261"></a><a name="p38951107261"></a>maxFileCheckingMillis</p>
    </td>
    <td class="cellrowborder" valign="top" width="8%" headers="mcps1.2.5.1.2 "><p id="p188952010112611"><a name="p188952010112611"></a><a name="p188952010112611"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.5.1.3 "><p id="p98953105261"><a name="p98953105261"></a><a name="p98953105261"></a>最长文件变动检查时间，如果文件在此时间内“大小”、“修改时间”和“文件ID”都没有变化，则认为文件已经完成并开始上传。</p>
    <p id="p138951810172617"><a name="p138951810172617"></a><a name="p138951810172617"></a>请根据实际文件变动的频率配置此值，避免文件未完成已开始上传的情况。</p>
    <p id="p1889511072617"><a name="p1889511072617"></a><a name="p1889511072617"></a>若文件上传后有变动，则会重新全量上传。</p>
    <p id="p789521014266"><a name="p789521014266"></a><a name="p789521014266"></a>单位：毫秒</p>
    <div class="note" id="note9895101013264"><a name="note9895101013264"></a><a name="note9895101013264"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p10895010182617"><a name="p10895010182617"></a><a name="p10895010182617"></a>“isFileAppendable”配置为“false”时该配置项生效。</p>
    </div></div>
    </td>
    <td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.4 "><p id="p9895710182611"><a name="p9895710182611"></a><a name="p9895710182611"></a>5000</p>
    </td>
    </tr>
    <tr id="row1895710152610"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="p16895141032618"><a name="p16895141032618"></a><a name="p16895141032618"></a>deletePolicy</p>
    </td>
    <td class="cellrowborder" valign="top" width="8%" headers="mcps1.2.5.1.2 "><p id="p489521052616"><a name="p489521052616"></a><a name="p489521052616"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.5.1.3 "><div class="p" id="p8895410132620"><a name="p8895410132620"></a><a name="p8895410132620"></a>文件内容上传完成之后的删除策略。<a name="ul2089561012615"></a><a name="ul2089561012615"></a><ul id="ul2089561012615"><li>never：文件内容上传完毕后不删除文件。</li><li>immediate：文件内容上传完毕后删除文件 。<div class="note" id="note0895141032619"><a name="note0895141032619"></a><a name="note0895141032619"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p14895410102615"><a name="p14895410102615"></a><a name="p14895410102615"></a><span class="parmname" id="parmname20896141012266"><a name="parmname20896141012266"></a><a name="parmname20896141012266"></a>“isFileAppendable”</span>配置为<span class="parmvalue" id="parmvalue1189661022613"><a name="parmvalue1189661022613"></a><a name="parmvalue1189661022613"></a>“false”</span>时该配置项生效。</p>
    </div></div>
    </li></ul>
    </div>
    </td>
    <td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.4 "><p id="p78966105268"><a name="p78966105268"></a><a name="p78966105268"></a>never</p>
    </td>
    </tr>
    <tr id="row19896141018269"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="p389631092614"><a name="p389631092614"></a><a name="p389631092614"></a>fileSuffix</p>
    </td>
    <td class="cellrowborder" valign="top" width="8%" headers="mcps1.2.5.1.2 "><p id="p289619102264"><a name="p289619102264"></a><a name="p289619102264"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.5.1.3 "><p id="p1789613108262"><a name="p1789613108262"></a><a name="p1789613108262"></a>文件内容上传完成之后添加的文件名后缀。</p>
    <p id="p1189631012268"><a name="p1189631012268"></a><a name="p1189631012268"></a>例如：原文件名为<span class="filepath" id="filepath1896111022614"><a name="filepath1896111022614"></a><a name="filepath1896111022614"></a>“x.txt”</span>，<span class="parmname" id="parmname15896141052616"><a name="parmname15896141052616"></a><a name="parmname15896141052616"></a>“fileSuffix”</span>配置为<span class="parmvalue" id="parmvalue3896141092612"><a name="parmvalue3896141092612"></a><a name="parmvalue3896141092612"></a>“.COMPLETED”</span>，则文件上传后的命名为<span class="filepath" id="filepath1789611013266"><a name="filepath1789611013266"></a><a name="filepath1789611013266"></a>“x.txt.COMPLETED”</span>。</p>
    <div class="note" id="note1089691019266"><a name="note1089691019266"></a><a name="note1089691019266"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p28961310182612"><a name="p28961310182612"></a><a name="p28961310182612"></a><span class="parmname" id="parmname10897131092611"><a name="parmname10897131092611"></a><a name="parmname10897131092611"></a>“isFileAppendable”</span>配置为<span class="parmvalue" id="parmvalue1289719105260"><a name="parmvalue1289719105260"></a><a name="parmvalue1289719105260"></a>“false”</span>，同时<span class="parmname" id="parmname589711101263"><a name="parmname589711101263"></a><a name="parmname589711101263"></a>“deletePolicy”</span>配置为<span class="parmvalue" id="parmvalue9897171012260"><a name="parmvalue9897171012260"></a><a name="parmvalue9897171012260"></a>“never”</span>，该配置项生效。</p>
    </div></div>
    </td>
    <td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.4 "><p id="p389711102262"><a name="p389711102262"></a><a name="p389711102262"></a>.COMPLETED</p>
    </td>
    </tr>
    <tr id="row1889715101264"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="p10897121032619"><a name="p10897121032619"></a><a name="p10897121032619"></a>sendingThreadSize</p>
    </td>
    <td class="cellrowborder" valign="top" width="8%" headers="mcps1.2.5.1.2 "><p id="p7897510192619"><a name="p7897510192619"></a><a name="p7897510192619"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.5.1.3 "><p id="p118978107268"><a name="p118978107268"></a><a name="p118978107268"></a>发送线程数。默认单线程发送。</p>
    <div class="notice" id="note189791018264"><a name="note189791018264"></a><a name="note189791018264"></a><span class="noticetitle"> 须知： </span><div class="noticebody"><p id="p789715105266"><a name="p789715105266"></a><a name="p789715105266"></a>使用多线程会导致如下问题：</p>
    <a name="ul289719106266"></a><a name="ul289719106266"></a><ul id="ul289719106266"><li>数据发送不保证顺序。</li><li>程序异常停止并重新启动时会丢失部分数据。</li></ul>
    </div></div>
    </td>
    <td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.4 "><p id="p19898181015267"><a name="p19898181015267"></a><a name="p19898181015267"></a>1</p>
    </td>
    </tr>
    <tr id="row198985108266"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="p5898610182614"><a name="p5898610182614"></a><a name="p5898610182614"></a>fileEncoding</p>
    </td>
    <td class="cellrowborder" valign="top" width="8%" headers="mcps1.2.5.1.2 "><p id="p88988101269"><a name="p88988101269"></a><a name="p88988101269"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.5.1.3 "><p id="p1589871014269"><a name="p1589871014269"></a><a name="p1589871014269"></a>文件编码格式，支持UTF8, GBK, GB2312, ISO-8859-1等</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.4 "><p id="p289821062616"><a name="p289821062616"></a><a name="p289821062616"></a>UTF8</p>
    </td>
    </tr>
    <tr id="row98984103267"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="p128982010172614"><a name="p128982010172614"></a><a name="p128982010172614"></a>resultLogLevel</p>
    </td>
    <td class="cellrowborder" valign="top" width="8%" headers="mcps1.2.5.1.2 "><p id="p8898410132617"><a name="p8898410132617"></a><a name="p8898410132617"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.5.1.3 "><p id="p1889811010264"><a name="p1889811010264"></a><a name="p1889811010264"></a>每次调用DIS数据发送接口后的结果日志级别。</p>
    <a name="ul189821011265"></a><a name="ul189821011265"></a><ul id="ul189821011265"><li>OFF：日志中不输出每次接口调用的结果。</li><li>INFO：每次接口调用的结果以INFO级别输出到日志。</li><li>WARN：每次接口调用的结果以WARN级别输出到日志。</li><li>ERROR：每次接口调用的结果以ERROR级别输出到日志。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.4 "><p id="p178998107264"><a name="p178998107264"></a><a name="p178998107264"></a>INFO</p>
    </td>
    </tr>
    </tbody>
    </table>


## Windows服务器上配置DIS Agent<a name="zh-cn_topic_0194140722_section59581866112340"></a>

1.  使用文件管理器进入安装包解压后的目录，例如“C:\\dis-agent-X.X.X”。
2.  使用编辑器打开“agent.yml”文件，根据实际情况修改各配置项的值并保存，配置项说明请参见[表1](#table192441715172513)。

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >“agent.yml“文件为linux格式，建议使用通用文本编辑器工具编辑文件。


## 上传性能调优<a name="section795372725913"></a>

本小节介绍DIS agent上传性能不足，如何进行调优，以避免出现数据上传不够及时，数据堆积的问题。

Agent 的内存配置在start-dis-agent.sh中：

```
JAVACMD="java"
JAVA_START_HEAP="256m" # 默认xms为256m
JAVA_MAX_HEAP="512m" # 默认xmx为512m
```

将这2个参数分别改成 1G、2G，然后把线程数调大，数值在60-70之间，最后把每次传输的数据量根据实际情况调小即可。

