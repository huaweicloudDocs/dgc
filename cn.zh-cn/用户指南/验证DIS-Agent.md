# 验证DIS Agent<a name="dayu_01_0224"></a>

## Linux服务器上验证DIS Agent<a name="zh-cn_topic_0194140856_section52583644132848"></a>

1.  使用PuTTY工具登录日志所在服务器。
2.  进入DIS Agent的日志目录。

    **cd /opt/dis-agent-X.X.X/logs**

3.  查看日志。

    **tail -100f dis-agent.log**

    -   显示如下信息，表示Agent正常运行。

        ```
        Agent: Startup completed in xx ms
        ```

    -   Agent运行异常，常见问题原因和处理方法如下：
        -   **HttpClientErrorException: 400 Bad Request**

            可能原因：[配置DIS Agent](配置DIS-Agent.md#dayu_01_0222)中“DISStream”或“projectId”的配置不正确。

            处理方法：停止Agent进程后检查配置。

        -   **HttpClientErrorException: 403 Forbidden**

            可能原因：DIS网关将服务器IP加入黑名单，导致请求被拦截。列入黑名单通常由于多次使用错误的配置重复调用DIS接口导致。

            处理方法：停止Agent进程，修改[配置DIS Agent](配置DIS-Agent.md#dayu_01_0222)中“agent.yml“配置文件的配置。停止Agent30分钟后重启Agent。

        -   **UnknownHttpStatusCodeException: Unknown status code \[441\]**

            可能原因： AK/SK配置错误。

            处理方法：停止Agent进程检查AK/SK配置。

        -   **ConnectTimeoutException: Connect to DOMAIN\[DOMAIN/IP\] failed: connect timed out**

            可能原因：服务器连接DIS网关超时。

            处理方法：检查Agent所在日志服务器的网络配置是否可以连接公网。


4.  查看Agent是否上传日志。
    -   “agent.yml”中配置的监控目录下有匹配的文件，日志中会输出类似如下日志，表示解析了\[N1行\(B1字节数\)/N2文件\(B2字节数\)\]，成功上传了\[N3行/N4文件\]。

        ```
        Agent: Progress: [N1 records (B1 bytes) / N2 files (B2 bytes)] parsed, and [N3 records / N4 files] sent successfully to destinations. Uptime: 30146ms
        ```

    -   若监控目录下没有匹配文件，则执行如下命令生成日志文件。

        **echo "\`date\` Hello world." \>\> /tmp/test.log**

5.  登录DIS控制台，查看[配置DIS Agent](配置DIS-Agent.md#dayu_01_0222)中“DISStream“或“CustomFileStream“通道的监控。有数据上传，表示DIS服务接收正常，Agent安装成功。

## Windows服务器上验证DIS Agent<a name="zh-cn_topic_0194140856_section51063719153510"></a>

1.  使用文件管理器进入“logs“目录。
2.  使用编辑器打开“dis-agent.log“文件查看日志。
    -   显示如下信息，表示Agent正常运行。

        ```
        Agent: Startup completed in xx ms
        ```

    -   Agent运行异常，常见问题原因和处理方法如下：
        -   **HttpClientErrorException: 400 Bad Request**

            可能原因：[配置DIS Agent](配置DIS-Agent.md#dayu_01_0222)中“DISStream”或“projectId”的配置不正确。

            处理方法：停止Agent进程后检查配置。

        -   **HttpClientErrorException: 403 Forbidden**

            可能原因：DIS网关将服务器IP加入黑名单，导致请求被拦截。列入黑名单通常由于多次使用错误的配置重复调用DIS接口导致。

            处理方法：停止Agent进程，修改[配置DIS Agent](配置DIS-Agent.md#dayu_01_0222)中“agent.yml“配置文件的配置。停止Agent30分钟后重启Agent。

        -   **UnknownHttpStatusCodeException: Unknown status code \[441\]**

            可能原因： AK/SK配置错误。

            处理方法：停止Agent进程检查AK/SK配置。

        -   **ConnectTimeoutException: Connect to DOMAIN\[DOMAIN/IP\] failed: connect timed out**

            可能原因：服务器连接DIS网关超时。

            处理方法：检查Agent所在日志服务器的网络配置是否可以连接公网。


3.  查看Agent是否上传日志。
    -   “agent.yml”中配置的监控目录下有匹配的文件，日志中会输出类似如下日志，表示解析了\[N1行\(B1字节数\)/N2文件\(B2字节数\)\]，成功上传了\[N3行/N4文件\]。

        ```
        Agent: Progress: [N1 records (B1 bytes) / N2 files (B2 bytes)] parsed, and [N3 records / N4 files] sent successfully to destinations. Uptime: 30146ms
        ```

    -   若监控目录下没有匹配文件，则执行如下命令生成日志文件。

        **echo %date%time%Hello world. \>\> C:\\test.log**

4.  登录DIS控制台，查看[配置DIS Agent](配置DIS-Agent.md#dayu_01_0222)中“DISStream“或“CustomFileStream“通道的监控。有数据上传，表示DIS服务接收正常，Agent安装成功。

