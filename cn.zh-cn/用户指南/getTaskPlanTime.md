# getTaskPlanTime<a name="dayu_01_0477"></a>

将作业计划运行的时间加偏移量之后，按照规定的日期格式返回。

## 函数格式<a name="zh-cn_topic_0126515630_section1644216138434"></a>

String  **getTaskPlanTime**\(Long planTime, String format, Integer offset\)

## 参数<a name="zh-cn_topic_0126515630_section16381557184317"></a>

-   planTime

    作业计划运行的时间。区分大小写，固定为全小写。

-   format

    返回值格式，合法的java日期格式化格式。

-   offset

    偏移量，以秒为单位的一个整数。如果偏移量数字为正，表示向未来偏移；如果偏移量数字为负，表示向过去偏移。


## 示例<a name="zh-cn_topic_0126515630_section20520313194417"></a>

示例一：

函数形式：$getTaskPlanTime\(plantime, @@yyyy/MM/dd HH:mm:ss@@, -24\*60\*60\)

返回值：假设作业计划运行的时间为“2018/08/18 18:00:00“，那么返回为“2018/08/17 18:00:00“

示例二：

函数形式：$getTaskPlanTime\(plantime, @@yyyy@@, -24\*60\*60\)

返回值：假设作业计划运行的时间为“2018/08/18 18:00:00“，那么返回为“2018“

