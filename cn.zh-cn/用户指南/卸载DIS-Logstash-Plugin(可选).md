# 卸载DIS Logstash Plugin\(可选\)<a name="dgc_01_0241"></a>

## 操作步骤<a name="zh-cn_topic_0194140939_section75029320585"></a>

1.  使用PuTTY工具远程登录Logstash所在服务器。
2.  停止Logstash程序。
3.  进入DIS Logstash Plugins插件所在的目录。

    **_**cd $\{LOGSTASH\_HOME\}**_**

    **_**cd logstash-plugins**_**

4.  卸载DIS Logstash Plugin。

    **_**bash uninstall.sh –p $\{LOGSTASH\_HOME\}**_**

    出现类似如下提示，表示卸载成功。

    ```
    Uninstall dis-logstash-plugins successfully.
    ```


