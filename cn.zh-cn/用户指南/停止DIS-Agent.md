# 停止DIS Agent<a name="dgc_01_0225"></a>

## 在Linux服务器上停止DIS Agent<a name="zh-cn_topic_0194140649_section7023695163740"></a>

1.  使用PuTTY工具登录日志所在服务器。
2.  进入DIS Agent安装目录。

    **cd /opt/dis-agent-X.X.X/**

3.  停止DIS Agent。

    **bash bin/stop-dis-agent.sh**

    >![](public_sys-resources/icon-notice.gif) **须知：** 
    >请确保使用bash执行脚本，否则使用sh、./ 等方式启动脚本，可能由于系统默认shell的差异导致启动失败。

    显示类似如下内容，表示正在停止中。“xxxxx”表示进程ID。

    ```
    Stopping Agent [xxxxx].....
    ```

    显示类似如下内容，表示Agent进程已停止。

    ```
    Stopping Agent [xxxxx]............. Successfully.
    ```

    强制停止Agent进程操作如下。

    1.  执行**ps -ef | grep dis-agent | grep -v grep**命令，获取Agent的进程标识（PID）。输出的第二个字段即为PID。
    2.  执行**kill -9 PID**命令，强制停止Agent进程。


## 在Windows服务器上停止DIS Agent<a name="zh-cn_topic_0194140649_section2897118163841"></a>

1.  在控制台窗口按“Ctrl+C”键，提示如下内容。

    ```
    [INFO ] (Agent STOPPING) com.bigdata.dis.agent.Agent Agent: Shutting down...
    ```

2.  等待出现如下提示，则表示停止完成.输入“Y”，单击“回车”键即可正常关闭窗口。

    ```
    Terminate batch job (Y/N)?
    ```


