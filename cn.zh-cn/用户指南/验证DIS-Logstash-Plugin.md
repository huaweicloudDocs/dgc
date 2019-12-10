# 验证DIS Logstash Plugin<a name="dayu_01_0240"></a>

## 验证DIS Logstash Input<a name="zh-cn_topic_0194140783_section51995384541"></a>

1.  使用PuTTY工具远程登录Logstash所在服务器。
2.  启动Logstash程序。

    ```
    bin/logstash -f dis_to_local.conf
    ```

    其中 -f 为用户编写的配置文件路径。

3.  检查DIS Logstash Input下载数据是否正常。

    向input指向的通道上传数据，如果Logstash没有报错且output端能正常获取到数据，表示下载正常。

4.  登录DIS控制台，等待2分钟后，查看[表1](配置DIS-Logstash-Plugin.md#zh-cn_topic_0194140892_table57792315343)中“streams”配置的通道的监控。如果显示有数据下载\(蓝色线条\)，表示DIS Logstash Input运行成功。

## 验证DIS Logstash Output<a name="zh-cn_topic_0194140783_section865661316574"></a>

1.  使用PuTTY工具远程登录Logstash所在服务器。
2.  启动Logstash程序。

    ```
    bin/logstash -f local_to_dis.conf
    ```

    其中 -f 为用户编写的配置文件路径。

3.  检查DIS Logstash Output上传数据是否正常。

    向Logstash的input端输入数据，如果Logstash没有报错数据可以正常上传到指向的通道，表示上传正常。

4.  登录DIS控制台，等待2分钟后，查看[表2](配置DIS-Logstash-Plugin.md#zh-cn_topic_0194140892_table151821388539)中“streamName”配置的通道的监控。如果显示有数据上传\(绿色线条\)，表示DIS Logstash Output运行成功。

