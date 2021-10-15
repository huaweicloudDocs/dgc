# 实时数据接入API错误码<a name="dgc_02_0312"></a>

当您调用API时，如果遇到“APIGW”开头的错误码，请参见[API网关错误码](https://support.huaweicloud.com/devg-apisign/api-sign-errorcode.html)进行处理。

更多服务错误码请参见[API错误中心](https://apierrorcenter.developer.huaweicloud.com/apierrorcenter)。

<a name="ErrorCode"></a>
<table><thead align="left"><tr><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.6.1.1"><p>状态码 </p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.1.6.1.2"><p>错误码</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.1.6.1.3"><p>错误信息</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.1.6.1.4"><p>描述</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.1.6.1.5"><p>处理措施</p>
</th>
</tr>
</thead>
<tbody><tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4117</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>Invalid Project Id. %s</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>用户传入的projectId无效</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请检查传入的projectId是否有效，是否传入了其他project的id。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4200</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>Invalid request. %s</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>用户的请求无效</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请参考API文档检查请求。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4201</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>Invalid partition_id. %s</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>用户传入的partition_id无效</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请检查partition_id是否无效。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4202</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>Empty request.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>用户的请求为空</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请传入有效的请求。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4203</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>Invalid monitoring period. %s</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>查询监控信息的startTime无效</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请传入有效的时间戳。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4204</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>The monitoring period cannot be longer than 7 days.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>仅允许查询最近7天内的监控信息</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请查询最近7天内的监控信息。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4205</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>Stream is not running.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>通道状态不是运行中</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请检查通道状态。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4208</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>Mrs cluster is invalid. %s</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>创建MRS转储任务时，传入的MRS集群无效</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请检查传入的MRS集群名称和ID，集群状态是否为运行中，以及是否为安全模式的集群。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4209</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>Invalid metrics label. %s</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>查询监控信息时，传入的监控指标不合法</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请参考API文档检查监控指标并修正。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4215</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>Invalid cursor type. %s</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>获取数据游标时，传入的游标类型cursor-type不合法</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请参考API文档检查cursor-type字段的范围并修正。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4216</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>Invalid sequence_number. %s</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>获取数据游标时，传入的序列号starting-sequence-number不合法</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请传入有效的starting-sequence-number。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4217</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>Invalid partition cursor. %s</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>从DIS通道下载数据时，传入的数据游标partition-cursor无效</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请重新获取partition-cursor并下载数据。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4224</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>Sequence_number out of range. %s</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>获取数据游标时，传入的序列号starting-sequence-number不在有效范围</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请传入有效的starting-sequence-number。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4225</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>Expired partition cursor. %s</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>从DIS通道下载数据时，传入的数据游标partition-cursor过期</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请重新获取partition-cursor并下载数据。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4226</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>A partition iterator error occurred or a record to which the SN corresponds has expired. Try to obtain the partition iterator again.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>获取数据时，传入的数据游标partition-cursor对应的序列号starting-sequence-number过期</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请重新获取数据游标，并用新游标获取数据。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4300</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>Request error.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>请求体错误</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请对照API文档修正请求体。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4301</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>The stream does not exist. %s</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>通道不存在</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请检查传入的通道是否存在。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4302</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>Partition does not exist. %s</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>通道的分区不存在</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请检查用户传入的分区ID是否存在。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4303</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>Exceeded traffic control limit.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>超出流控</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请扩容通道或降低上传速率。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4305</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>Too many stream requests.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>同一时间内用户请求太多</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请降低请求频率并重试。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4306</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>Bucket does not exist. %s</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>传入的OBS桶不存在</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请检查OBS桶是否存在。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4307</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>The stream already exists.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>指定的通道已经存在</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请修改通道名称并重新创建通道</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4308</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>Insufficient quota.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>通道或分区的配额不足</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请释放配额或提工单修改账号的配额。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4309</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>Too many request failures. Please try again later.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>IP被加入黑名单</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>由于频繁的错误访问导致用户ip被加入黑名单，请检查认证信息和请求是否有效，并稍后重试。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4310</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>OBS access error.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>访问OBS失败</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请检查用户是否有访问OBS的权限。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4319</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>Partition is expired. %s</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>分区已过期</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>该分区已过期失效，主要针对缩容场景，检查该分区是否已失效，使用正确有效的分区。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4329</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>app quota exceeded.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>APP配额超出限制</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请释放APP的配额。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4330</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>app already exist.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>已经存在同名的APP</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请修改APP名称并重新创建APP。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4331</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>app is using.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>删除app时，当前app在使用中</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请确认app是否在使用中，如需删除请停止使用并重新删除。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4332</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>app not found.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>指定的APP不存在</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请检查指定的APP名称是否正确</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4335</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>Invalid IAM agency.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>创建转储任务时，使用的IAM委托无效</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>检查DIS创建的dis_admin_agency或用户自定义的IAM委托是否存在，权限是否完整。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4336</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>Invalid HDFS path.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>创建MRS转储任务时，传入的MRS HDFS路径无效</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请检查传入的MRS HDFS路径是否存在。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4337</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>The DLI database does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>创建DLI转储任务时，传入的DLI数据库不存在</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请检查传入的DLI数据库是否存在。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4338</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>The DLI table does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>创建DLI转储任务时，传入的DLI数据表不存在</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请检查传入的DLI表是否存在，并且是否为DLI内表。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4339</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>Consumer quota exceeded.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>消费组消费者配额不足</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>该消费组内的消费者数量已经超越最大配额，请合理分配消费者或者使用新消费组满足诉求。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4341</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>The CloudTable cluster does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>创建CloudTable转储任务时，传入的CloudTable集群不存在</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请检查传入的CloudTable集群是否存在，集群状态是否正常。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4342</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>The CloudTable table does not exist</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>创建CloudTable转储任务时，传入的CloudTable表不存在</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请检查传入的CloudTable表是否存在。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4343</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>The CloudTable table family does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>创建CloudTable转储任务时，传入的CloudTable表的列族不存在</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请检查传入的CloudTable表的列族名称是否存在。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4345</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>Invalid CloudTable schema.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>创建CloudTable转储任务时，传入的schema无效</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请根据返回的详细信息检查schema，例如配置的JSON属性名称是否存在，参数是否合法等。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4348</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>Invalid CloudTable openTSDB schema.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>创建CloudTable openTSDB转储任务时，传入的schema无效</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请根据返回的详细信息检查schema，例如配置的JSON属性名称是否存在，参数是否合法等。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4350</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>Invalid DWS cluster.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>创建DWS转储任务时，传入的DWS集群不存在</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请检查DWS集群是否存在，运行是否正常。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4351</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>Invalid KMS userKey.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>创建DWS转储任务时，传入的KMS秘钥信息无效</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请检查KMS密钥是否存在。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4354</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>The transfer task does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>删除或更新转储任务时，转储任务不存在</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请检查转储任务是否存在。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4355</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>The transfer task already exists.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>创建转储任务时，同一个通道下已存在同名的转储任务</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请修改新创建转储任务的名称并重新创建。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4357</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>Exceeded transfer task quota.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>单个通道仅允许同时存在5个转储任务，再创建新的转储任务会超出配额限制</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请删除废弃的转储任务释放配额。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4360</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>Invalid data schema.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>创建通道或更新通道时，传入的data_schema无效</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请检查data_schema的格式并重试。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4375</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>The app does not commit checkpoint</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>该app没有在通道中提交checkpoint操作</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请确认该app是否已在消费通道提交了checkpoint操作</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4601</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>The number of resource tags has reached the maximum.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>一个资源上最多有10个标签，添加标签时资源上已添加的标签数超出限制</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请删除废弃的标签并重新添加标签。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4602</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>Invalid resource type.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>资源类型不合法</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请检查资源类型是否合法。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4603</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>The resource does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>资源不存在</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请确认该资源是否已被删除。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4604</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>The key does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>标签Key不存在</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请确认标签Key是否存在。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>400</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4605</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>The action is not supported.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>当前标签操作不支持</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请确认当前标签操作是否合法，当前仅支持create和delete操作。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>403</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.4116</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>Invalid RBAC. %s</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>用户操作受限</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>请根据返回的具体信息判断账号是否未实名认证、欠费、无DIS服务的操作权限等。</p>
</td>
</tr>
<tr><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.1 "><p>500</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p>DIS.5000</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p>System error.</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p>系统错误，请联系客服或技术支持工程师处理。</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.6.1.5 "><p>系统错误，请联系客服或技术支持工程师处理。</p>
</td>
</tr>
</tbody>
</table>

