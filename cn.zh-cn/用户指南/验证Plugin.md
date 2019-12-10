# 验证Plugin<a name="dayu_01_0231"></a>

## 验证DIS Source<a name="zh-cn_topic_0120206107_sa69aadf601894e5baed1e6d07eedd07a"></a>

1.  使用PuTTY工具远程登录Flume所在服务器。
2.  <a name="zh-cn_topic_0120206107_li136991938437"></a>确认已配置好包含dis source的配置文件

    可基于Flume自带的flume-conf.properties.template修改，文件样例如下所示：

    ```
    agent.sources = dissource
    agent.channels = memoryChannel
    agent.sinks = loggerSink
    # 定义 Source (使用dis source，从DIS读取数据)
    agent.sources.dissource.channels = memoryChannel
    agent.sources.dissource.type = com.huaweicloud.dis.adapter.flume.source.DISSource 
    agent.sources.dissource.streams = YOU_DIS_STREAM_NAME
    agent.sources.dissource.ak = YOU_ACCESS_KEY_ID
    agent.sources.dissource.sk = YOU_SECRET_KEY_ID
    agent.sources.dissource.region = ${region}
    agent.sources.dissource.projectId = YOU_PROJECT_ID
    agent.sources.dissource.endpoint = https://dis.${region}.myhuaweicloud.com
    agent.sources.dissource.group.id = YOU_APP_NAME
    # 定义 Channel
    agent.channels.memoryChannel.type = memory
    agent.channels.memoryChannel.capacity = 10000
    # 定义 Sink (使用logger sink，输出到控制台)
    agent.sinks.loggerSink.type = logger
    agent.sinks.loggerSink.channel = memoryChannel
    ```

3.  启动Flume程序，启动命令请参考Apache Flume官网指导。

    如果从Flume安装目录启动，示例命令如下所示：

    ```
    bin/flume-ng agent --conf-file conf/flume-conf.properties.template --name agent --conf conf/ -Dflume.root.logger=INFO,console
    ```

    其中bin/flume-ng agent表示启动Flume Agent；--conf-file 为用户编写的配置文件路径； --name 为配置文件中agent的名称, --conf 为Flume自带的conf/路径

    启动之后查看日志，若日志中有类似“source disSource started.”内容，表示DIS Source正常启动，其中“disSource”是用户配置的source名称。

4.  检查DIS Source下载数据是否正常。

    向source指向的通道上传数据，如果flume没有报错且sink端能正常获取到数据，表示下载正常。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >如果使用[2](#zh-cn_topic_0120206107_li136991938437)中示例的配置，则从DIS获取的数据会输出到控制台上，其内容显示为字节数组格式。  

5.  登录DIS控制台，等待2分钟后，查看[表1](配置Plugin.md#zh-cn_topic_0120206024_table57792315343)中“streams”配置的通道的监控。如果显示有数据下载\(蓝色线条\)，表示DIS Source运行成功。

## 验证DIS Sink<a name="zh-cn_topic_0120206107_section13261163275410"></a>

1.  使用PuTTY工具远程登录Flume所在服务器。
2.  <a name="zh-cn_topic_0120206107_li7637814185518"></a>确认已配置好包含dis sink的配置文件

    可基于Flume自带的flume-conf.properties.template修改，文件样例如下所示：

    ```
    agent.sources = exec
    agent.channels = memoryChannel
    agent.sinks = dissink
    # 定义 Source (使用exec source，监控/tmp/dis.txt文件)
    agent.sources.exec.type = exec
    agent.sources.exec.command = tail -F /tmp/dis.txt
    agent.sources.exec.shell = /bin/bash -c
    agent.sources.exec.channels = memoryChannel
    # 定义 Channel
    agent.channels.memoryChannel.type = memory
    agent.channels.memoryChannel.capacity = 10000
    # 定义 Sink (使用dis sink，输出到dis通道)
    agent.sinks.dissink.channel = memoryChannel
    agent.sinks.dissink.type = com.huaweicloud.dis.adapter.flume.sink.DISSink
    agent.sinks.dissink.streamName = YOU_DIS_STREAM_NAME
    agent.sinks.dissink.ak = YOU_ACCESS_KEY_ID
    agent.sinks.dissink.sk = YOU_SECRET_KEY_ID
    agent.sinks.dissink.region = ${region}
    agent.sinks.dissink.projectId = YOU_PROJECT_ID
    agent.sinks.dissink.endpoint = https://dis.${region}.myhuaweicloud.com
    agent.sinks.dissink.resultLogLevel = INFO
    ```

3.  启动Flume程序，启动命令请参考Apache Flume官网指导。

    如果从Flume安装目录启动，示例命令如下所示

    ```
    bin/flume-ng agent --conf-file conf/flume-conf.properties.template --name agent --conf conf/ -Dflume.root.logger=INFO,console
    ```

    其中bin/flume-ng agent表示启动Flume Agent；--conf-file 为用户编写的配置文件路径； --name 为配置文件中agent的名称, --conf 为Flume自带的conf/路径。

    查看日志，若日志中有类似“Dis flume sink \[dissink\] start.”内容，表示DIS Sink正常启动，其中“dissink”是用户配置的sink名称。

4.  检查DIS Sink上传数据是否正常。

    向Flume的source端输入数据，在DIS Sink的resultLogLevel级别不为OFF且不低于log4j配置的值，查看日志输出类似如下结果，表示DIS Sink上传数据正常。

    ```
    CurrentPut 5 events[success 5 / failed 0] spend 131 ms.
    ```

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >如果使用[2](#zh-cn_topic_0120206107_li7637814185518)中示例的配置，您可创建/tmp/dis.txt文件，并在此文件中追加内容。则启动Flume之后，追加的每行内容会被Flume读取并通过dis sink插件发动到DIS通道中。  

5.  登录DIS控制台，等待2分钟后，查看[表2](配置Plugin.md#zh-cn_topic_0120206024_table1440315456433)中“streamName”配置的通道的监控。如果显示有数据上传\(绿色线条\)，表示DIS Sink运行成功。

