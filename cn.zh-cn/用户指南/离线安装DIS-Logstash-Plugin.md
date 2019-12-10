# 离线安装DIS Logstash Plugin<a name="dayu_01_0238"></a>

安装DIS Logstash Plugin有在线和离线安装两种方式：

离线安装需要获取插件包并执行安装脚本。

## 前提条件<a name="zh-cn_topic_0194140895_section13422180184114"></a>

已安装PuTTY工具。

## 操作步骤<a name="zh-cn_topic_0194140895_section161170025815"></a>

1.  使用PuTTY工具\(或其他终端工具\)远程登录Logstash服务器。
2.  进入到Logstash的安装目录。

    **_cd $\{LOGSTASH\_HOME\}_**

3.  上传“dis-logstash-plugins-_X.X.X_.zip”安装包到此目录下。
4.  解压安装包。

    **_unzip dis-logstash-plugins-X.X.X.zip_**

5.  进入安装包解压后的目录。

    **_cd logstash-plugins_**

6.  运行安装程序，需要指定Logstash的安装目录。

    **_bash install.sh –p $\{LOGSTASH\_HOME\}_**

    安装完成后，显示类似如下内容，表示安装成功。

    ```
    Install dis-logstash-plugins successfully.
    ```


