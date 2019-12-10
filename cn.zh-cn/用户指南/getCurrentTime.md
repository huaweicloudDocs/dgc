# getCurrentTime<a name="dayu_01_0472"></a>

用户获取系统当前时间，按照规定的日期格式返回。

## 函数格式<a name="zh-cn_topic_0126423659_section57840345152"></a>

String  **getCurrentTime**\(String format, Integer offset\)

## 参数<a name="zh-cn_topic_0126423659_section954910288167"></a>

-   format

    返回值格式，合法的java日期格式化格式。

-   offset

    偏移量，以秒为单位的一个整数。如果偏移量数字为正，表示向未来偏移；如果偏移量数字为负，表示向过去偏移。


## 示例<a name="zh-cn_topic_0126423659_section1033315913339"></a>

函数形式：$getCurrentTime\(@@yyyy-MM-dd HH:mm@@, -24\*60\*60\)

返回值：假设系统当前时间为“2018-08-16 17:30“，那么返回为“2018-08-15 17:30“

