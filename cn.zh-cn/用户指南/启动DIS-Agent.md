# 启动DIS Agent<a name="dayu_01_0223"></a>

## Linux服务器上启动DIS Agent<a name="zh-cn_topic_0194140639_sd4ef67de79d947c6934da764e73cb549"></a>

1.  使用PuTTY工具登录日志所在服务器。
2.  进入DIS Agent安装目录。其中_**“x.x.x**_”表示版本号。

    **cd /opt/dis-agent-x.x.x/**

3.  启动DIS Agent。

    **bash bin/start-dis-agent.sh**

    如果需要启动多个DIS Agent进程，则新启的Agent进程需要通过-c指定配置文件以及-n参数指定名称。

    **bash bin/start-dis-agent.sh -c config/anotherAgent.yml -n anotherAgent**

    >![](public_sys-resources/icon-notice.gif) **须知：**   
    >请确保使用bash执行脚本，否则使用sh、./ 等方式启动脚本，可能由于系统默认shell的差异导致启动失败。  

    显示类似如下信息，表示Agent启动成功。

    ```
    Success to start DIS Agent [xxxxx].
    ```

    如果启动出现java变量找不到的情况，执行**source /etc/profile**后重新启动Agent。


## Windows服务器上启动DIS Agent<a name="zh-cn_topic_0194140639_section38534633132034"></a>

1.  进入DIS Agent程序的bin目录，例如“C:\\dis-agent-X.X.X\\bin”。
2.  双击“start-dis-agent.bat”，启动DIS Agent。

    若控制台前几行中打印出如下日志表示启动成功。

    ```
    [INFO ] (main) com.bigdata.dis.agent.Agent Agent: Startup completed in XXX ms.
    ```


