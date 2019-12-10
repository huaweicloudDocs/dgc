# OBS导入数据到SQL Server时出现Unable to execute the SQL statement怎么处理？<a name="dayu_01_0114"></a>

## 问题描述<a name="zh-cn_topic_0173586862_section146105598718"></a>

使用CDM从OBS导入数据到SQL Server时，作业运行失败，错误提示为：Unable to execute the SQL statement. Cause : 将截断字符串或二进制数据。

## 原因分析<a name="zh-cn_topic_0173586862_section122891983182"></a>

用户OBS中的数据超出了SQL Server数据库的字段长度限制。

## 解决方法<a name="zh-cn_topic_0173586862_section1131621151917"></a>

在SQL Server数据库中建表时，将数据库字段改大，长度不能小于源端OBS中的数据长度。

