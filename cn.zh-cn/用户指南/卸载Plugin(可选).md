# 卸载Plugin\(可选\)<a name="dgc_01_0232"></a>

## 操作步骤<a name="zh-cn_topic_0120206062_s532b45faacb147a4adbafdbe092376ef"></a>

1.  使用PuTTY工具远程登录Flume所在服务器。
2.  停止Flume程序。
3.  进入DIS Flume Plugin插件所在的目录。

    **cd $\{FLUME\_HOME\}**

    **cd dis-flume-plugin**

4.  卸载DIS Flume Plugin。

    **dos2unix install.sh**

    **bash install.sh uninstall**

    出现类似如下提示，表示卸载成功。

    ```
    Uninstall dis-flume-plugin successfully.
    ```


