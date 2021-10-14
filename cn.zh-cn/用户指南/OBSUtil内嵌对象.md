# OBSUtil内嵌对象<a name="dgc_01_0553"></a>

OBSUtil内嵌对象提供了一系列针对OBS的操作方法，例如判断OBS文件或目录是否存在。

## 方法<a name="section1305173518816"></a>

**表 1**  方法说明

<a name="table124871918198"></a>
<table><thead align="left"><tr id="row24881718491"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p1448813184910"><a name="p1448813184910"></a><a name="p1448813184910"></a>方法</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p19488101819911"><a name="p19488101819911"></a><a name="p19488101819911"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row248818181297"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p651195712712"><a name="p651195712712"></a><a name="p651195712712"></a>boolean isExistOBSPath(String obsPath)</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p8511105718717"><a name="p8511105718717"></a><a name="p8511105718717"></a>判断OBS文件或目录（目录请以“/”结尾）是否存在，存在返回true，不存在返回false。</p>
</td>
</tr>
</tbody>
</table>

## 举例<a name="section146218581191"></a>

-   判断OBS目录是否存在，目录请以“/”结尾，EL表达式如下：

    \#\{OBSUtil.isExistOBSPath\("obs://test/jobs/"\)\}


-   判断OBS文件是否存在，EL表达式如下：

    \#\{OBSUtil.isExistOBSPath\("obs://test/jobs/job.log"\)\}


