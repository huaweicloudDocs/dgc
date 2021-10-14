# 管理Agent<a name="dgc_01_0128"></a>

对于HDFS和关系型数据库类型的数据源，不方便暴露节点的场景，可选择在源端网络中部署Agent。CDM通过Agent拉取客户内部数据源的数据，但不支持写入数据。

**图 1**  场景图<a name="zh-cn_topic_0207402273_fig129235219507"></a>  
![](figures/场景图.jpg "场景图")

Agent的使用流程如[图2](#zh-cn_topic_0207402273_zh-cn_topic_0191978474_fig581611212343)所示。

**图 2**  Agent使用流程<a name="zh-cn_topic_0207402273_zh-cn_topic_0191978474_fig581611212343"></a>  
![](figures/Agent使用流程.jpg "Agent使用流程")

## 前提条件<a name="zh-cn_topic_0207402273_zh-cn_topic_0191978474_section165610530308"></a>

已具备CDM集群。

## 新建Agent<a name="zh-cn_topic_0207402273_zh-cn_topic_0191978474_section85334211067"></a>

1.  进入CDM主界面，单击左侧导航上的“集群管理“，选择集群后的“作业管理  \>  Agent管理  \>  新建Agent“，配置Agent相关信息，如[图3](#zh-cn_topic_0207402273_fig15586733165119)所示。

    **图 3**  配置Agent<a name="zh-cn_topic_0207402273_fig15586733165119"></a>  
    ![](figures/配置Agent.png "配置Agent")

    -   IP地址：配置为源端网络中部署Agent的机器IP。
    -   端口：Agent暴露的端口。建议范围：1024\~65535。
    -   启用压缩：是否对数据进行压缩传输。
    -   启用SSL：是否启用SSL双向认证，保证数据的安全性。
    -   限流：设置agent的最大下行速率，默认不限流。

2.  单击“确认“，完成Agent的创建。在Agent管理页面可查看已成功创建的Agent。

## 安装并启动Agent<a name="zh-cn_topic_0207402273_zh-cn_topic_0191978474_section98287153337"></a>

1.  在Agent管理页面，找到已成功创建的Agent。如[图4](#zh-cn_topic_0207402273_zh-cn_topic_0191978474_fig996512212404)所示，下载Agent。

    **图 4**  下载Agent<a name="zh-cn_topic_0207402273_zh-cn_topic_0191978474_fig996512212404"></a>  
    ![](figures/下载Agent.png "下载Agent")

2.  准备部署Agent的主机。该主机需要满足以下条件：
    -   需要已安装64位版本java 8并配置java环境变量。
    -   授予Ruby用户在/tmp目录下的写权限。

3.  将下载的Agent压缩包，上传至部署Agent的主机上。
4.  解压安装包后执行如下命令安装Agent。

    **sh sbin/install.sh**

5.  如果需要通过Agent连接关系数据库，则需要将对应的驱动（参考[管理驱动](管理驱动.md#dgc_01_0132)获取）上传至Agent安装目录下的/server/jdbc，并修改同目录下properties文件里对应数据库驱动的版本号。
6.  安装完成后，执行如下命令启动Agent。

    **su Ruby**

    **sh sbin/start.sh**

7.  执行如下命令检查Agent进程是否启动。

    **ps -ef | grep agent**

    如果命令执行完成后返回了正在运行的Agent进程，说明Agent进程已启动。


## 连接Agent<a name="zh-cn_topic_0207402273_zh-cn_topic_0191978474_section1072083564713"></a>

1.  在Agent管理页面，找到已成功创建的Agent。如[图5](#zh-cn_topic_0207402273_zh-cn_topic_0191978474_fig1282252673415)所示，连接Agent。

    **图 5**  连接Agent<a name="zh-cn_topic_0207402273_zh-cn_topic_0191978474_fig1282252673415"></a>  
    ![](figures/连接Agent.png "连接Agent")

2.  Agent连接成功后，即可在创建连接中选择Agent。

