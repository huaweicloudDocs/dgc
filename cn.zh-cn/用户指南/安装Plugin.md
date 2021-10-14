# 安装Plugin<a name="dgc_01_0229"></a>

## 前提条件<a name="zh-cn_topic_0120206099_section63502565"></a>

已安装PuTTY工具。

## 操作步骤<a name="zh-cn_topic_0120206099_section34652178"></a>

1.  使用PuTTY工具\(或其他终端工具\)远程登录Flume服务器。
2.  进入到Flume的安装目录。

    **cd $\{FLUME\_HOME\}**

3.  上传“dis-flume-plugin-_X.X.X_.zip”安装包到此目录下。
4.  解压安装包。

    **unzip dis-flume-plugin-X.X.X.zip**

5.  进入安装包解压后的目录。

    **cd dis-flume-plugin**

6.  运行安装程序。

    **bash install.sh**

    **DIS Flume Plugin**安装在“$\{FLUME\_HOME\}/plugin.d/dis-flume-plugin“目录下，安装完成后，显示类似如下内容，表示安装成功。

    ```
    Install dis-flume-plugin successfully.
    ```


