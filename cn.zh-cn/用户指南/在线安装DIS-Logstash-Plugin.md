# 在线安装DIS Logstash Plugin<a name="dayu_01_0237"></a>

安装DIS Logstash Plugin有在线和离线安装两种方式：

在线安装无需下载插件包，直接连接公网即可安装。

## 前提条件<a name="zh-cn_topic_0194140845_section13422180184114"></a>

已安装PuTTY工具。

## 安装logstash-input-dis<a name="zh-cn_topic_0194140845_section158925115333"></a>

1.  使用PuTTY工具\(或其他终端工具\)远程登录Logstash服务器。
2.  进入到Logstash的安装目录。

    **_cd $\{LOGSTASH\_HOME\}_**

3.  执行安装命令。

    bin/logstash-plugin install logstash-input-dis

    安装完成后，显示类似如下内容，表示安装成功。

    ```
    Validating logstash-input-dis
    Installing logstash-input-dis
    Installation successful
    ```


## 安装**logstash-output-dis**<a name="zh-cn_topic_0194140845_section36194933312"></a>

1.  使用PuTTY工具\(或其他终端工具\)远程登录Logstash服务器。
2.  进入到Logstash的安装目录。

    **_cd $\{LOGSTASH\_HOME\}_**

3.  执行安装命令。

    bin/logstash-plugin install logstash-output-dis

    安装完成后，显示类似如下内容，表示安装成功。

    ```
    Validating logstash-output-dis
    Installing logstash-output-dis
    Installation successful
    ```


