# CALCDATE<a name="dayu_01_0490"></a>

用户指定某一个时间按照规定的日期格式返回。

## 函数格式<a name="zh-cn_topic_0126539709_section1644216138434"></a>

String  **CALCDATE**\(Date date, int years, int months, int days, int hours, int minutes, int seconds\)

## 参数<a name="zh-cn_topic_0126539709_section16381557184317"></a>

-   date

    原始日期。

-   years、months、days、hours、minutes、seconds

    依次输入年、月、日、时、分、秒的偏移值，数字为正数时，表示向未来偏移；数字为负数时，表示向过去偏移。


## 示例<a name="zh-cn_topic_0126539709_section20520313194417"></a>

函数形式：$CALCDATE\(\[2008-08-08 12:30:00\], 2, 0, 0, 0, -30, 0\)

返回值：\[2010-08-08 12:00:00\]

