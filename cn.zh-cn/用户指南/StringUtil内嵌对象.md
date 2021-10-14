# StringUtil内嵌对象<a name="dgc_01_0499"></a>

StringUtil内嵌对象提供了一系列字符串操作方法，例如从一个字符串中截取一个子字符串。

StringUtil内部是由org.apache.commons.lang3.StringUtils实现的，具体使用方法请参考[appache commons文档](https://commons.apache.org/proper/commons-lang/apidocs/org/apache/commons/lang3/StringUtils.html)。

## 举例<a name="zh-cn_topic_0132846498_section781015577112"></a>

假设变量a为字符串No.0010，返回“.“后面的子字符串，EL表达式如下：

```
#{StringUtil.substringAfter(a,".")}
```

