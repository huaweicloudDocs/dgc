# DIS服务端错误码<a name="dgc_06_0086"></a>

在使用SDK进行操作时如果遇到错误，会在控制台显示错误码描述错误信息。

<a name="zh-cn_topic_0080205353_table1074484417507"></a>
<table><thead align="left"><tr id="zh-cn_topic_0080205353_row4525174595018"><th class="cellrowborder" valign="top" width="7.219278072192781%" id="mcps1.1.6.1.1"><p id="zh-cn_topic_0080205353_p85252455500"><a name="zh-cn_topic_0080205353_p85252455500"></a><a name="zh-cn_topic_0080205353_p85252455500"></a>http状态码</p>
</th>
<th class="cellrowborder" valign="top" width="10.30896910308969%" id="mcps1.1.6.1.2"><p id="zh-cn_topic_0080205353_p55251145165013"><a name="zh-cn_topic_0080205353_p55251145165013"></a><a name="zh-cn_topic_0080205353_p55251145165013"></a>错误码</p>
</th>
<th class="cellrowborder" valign="top" width="27.83721627837216%" id="mcps1.1.6.1.3"><p id="zh-cn_topic_0080205353_p352524510505"><a name="zh-cn_topic_0080205353_p352524510505"></a><a name="zh-cn_topic_0080205353_p352524510505"></a>Error Message</p>
</th>
<th class="cellrowborder" valign="top" width="20.61793820617938%" id="mcps1.1.6.1.4"><p id="zh-cn_topic_0080205353_p1152614520503"><a name="zh-cn_topic_0080205353_p1152614520503"></a><a name="zh-cn_topic_0080205353_p1152614520503"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="34.016598340165984%" id="mcps1.1.6.1.5"><p id="zh-cn_topic_0080205353_p35269459509"><a name="zh-cn_topic_0080205353_p35269459509"></a><a name="zh-cn_topic_0080205353_p35269459509"></a>处理措施</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0080205353_row2526545125013"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p95264452501"><a name="zh-cn_topic_0080205353_p95264452501"></a><a name="zh-cn_topic_0080205353_p95264452501"></a>441</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p35266456507"><a name="zh-cn_topic_0080205353_p35266456507"></a><a name="zh-cn_topic_0080205353_p35266456507"></a>DIS.4100</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p15526164519509"><a name="zh-cn_topic_0080205353_p15526164519509"></a><a name="zh-cn_topic_0080205353_p15526164519509"></a>Authorization error.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p752764585014"><a name="zh-cn_topic_0080205353_p752764585014"></a><a name="zh-cn_topic_0080205353_p752764585014"></a>使用AKSK生成的签名信息错误</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p11527345205013"><a name="zh-cn_topic_0080205353_p11527345205013"></a><a name="zh-cn_topic_0080205353_p11527345205013"></a>请检查请求头里的签名信息是否无误。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row0527645105015"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p552754535016"><a name="zh-cn_topic_0080205353_p552754535016"></a><a name="zh-cn_topic_0080205353_p552754535016"></a>441</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p4527154535014"><a name="zh-cn_topic_0080205353_p4527154535014"></a><a name="zh-cn_topic_0080205353_p4527154535014"></a>DIS.4101</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p75276452506"><a name="zh-cn_topic_0080205353_p75276452506"></a><a name="zh-cn_topic_0080205353_p75276452506"></a>Authorization header cannot be empty.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p3527204575013"><a name="zh-cn_topic_0080205353_p3527204575013"></a><a name="zh-cn_topic_0080205353_p3527204575013"></a>使用AKSK生成的签名信息为空</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p18527245135017"><a name="zh-cn_topic_0080205353_p18527245135017"></a><a name="zh-cn_topic_0080205353_p18527245135017"></a>请求头里的签名信息为空，检查是否未生成签名信息。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row1652734565012"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p1652716458505"><a name="zh-cn_topic_0080205353_p1652716458505"></a><a name="zh-cn_topic_0080205353_p1652716458505"></a>441</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p152744513502"><a name="zh-cn_topic_0080205353_p152744513502"></a><a name="zh-cn_topic_0080205353_p152744513502"></a>DIS.4102</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p1652764519506"><a name="zh-cn_topic_0080205353_p1652764519506"></a><a name="zh-cn_topic_0080205353_p1652764519506"></a>Incorrectly parsed authorization header.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p85271245155011"><a name="zh-cn_topic_0080205353_p85271245155011"></a><a name="zh-cn_topic_0080205353_p85271245155011"></a>无法解析签名</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p352714519506"><a name="zh-cn_topic_0080205353_p352714519506"></a><a name="zh-cn_topic_0080205353_p352714519506"></a>请检查请求头里的签名信息。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row1452719456507"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p5527045105018"><a name="zh-cn_topic_0080205353_p5527045105018"></a><a name="zh-cn_topic_0080205353_p5527045105018"></a>441</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p18528154535014"><a name="zh-cn_topic_0080205353_p18528154535014"></a><a name="zh-cn_topic_0080205353_p18528154535014"></a>DIS.4103</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p7528945185011"><a name="zh-cn_topic_0080205353_p7528945185011"></a><a name="zh-cn_topic_0080205353_p7528945185011"></a>Empty X-Sdk-Date header.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p252874565016"><a name="zh-cn_topic_0080205353_p252874565016"></a><a name="zh-cn_topic_0080205353_p252874565016"></a>请求头里的X-Sdk-Date字段为空</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p25281345115013"><a name="zh-cn_topic_0080205353_p25281345115013"></a><a name="zh-cn_topic_0080205353_p25281345115013"></a>请检查请求头里的X-Sdk-Date字段并补齐。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row1652819454505"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p16528194511506"><a name="zh-cn_topic_0080205353_p16528194511506"></a><a name="zh-cn_topic_0080205353_p16528194511506"></a>441</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p1352874545016"><a name="zh-cn_topic_0080205353_p1352874545016"></a><a name="zh-cn_topic_0080205353_p1352874545016"></a>DIS.4104</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p17528845145011"><a name="zh-cn_topic_0080205353_p17528845145011"></a><a name="zh-cn_topic_0080205353_p17528845145011"></a>Error parsing X-Sdk-Date header.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p175288450508"><a name="zh-cn_topic_0080205353_p175288450508"></a><a name="zh-cn_topic_0080205353_p175288450508"></a>无法解析请求头里的X-Sdk-Date字段</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p175282451506"><a name="zh-cn_topic_0080205353_p175282451506"></a><a name="zh-cn_topic_0080205353_p175282451506"></a>请检查请求头里的X-Sdk-Date字段并修正。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row652844510505"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p2528114575015"><a name="zh-cn_topic_0080205353_p2528114575015"></a><a name="zh-cn_topic_0080205353_p2528114575015"></a>441</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p175287456504"><a name="zh-cn_topic_0080205353_p175287456504"></a><a name="zh-cn_topic_0080205353_p175287456504"></a>DIS.4105</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p205281245115013"><a name="zh-cn_topic_0080205353_p205281245115013"></a><a name="zh-cn_topic_0080205353_p205281245115013"></a>Invalid X-Sdk-Date header.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p12528345115012"><a name="zh-cn_topic_0080205353_p12528345115012"></a><a name="zh-cn_topic_0080205353_p12528345115012"></a>请求头里的X-Sdk-Date字段无效</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p1852917459505"><a name="zh-cn_topic_0080205353_p1852917459505"></a><a name="zh-cn_topic_0080205353_p1852917459505"></a>请检查请求头里的X-Sdk-Date字段并修正。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row2529845155014"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p18529245135018"><a name="zh-cn_topic_0080205353_p18529245135018"></a><a name="zh-cn_topic_0080205353_p18529245135018"></a>441</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p17529204595020"><a name="zh-cn_topic_0080205353_p17529204595020"></a><a name="zh-cn_topic_0080205353_p17529204595020"></a>DIS.4106</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p12529154510507"><a name="zh-cn_topic_0080205353_p12529154510507"></a><a name="zh-cn_topic_0080205353_p12529154510507"></a>Empty AcessKey header.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p8529545135011"><a name="zh-cn_topic_0080205353_p8529545135011"></a><a name="zh-cn_topic_0080205353_p8529545135011"></a>请求头里的签名信息Authorization字段中缺失AK</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p1252984535010"><a name="zh-cn_topic_0080205353_p1252984535010"></a><a name="zh-cn_topic_0080205353_p1252984535010"></a>请检查是否传入AK。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row17529164515504"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p165299451505"><a name="zh-cn_topic_0080205353_p165299451505"></a><a name="zh-cn_topic_0080205353_p165299451505"></a>441</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p145291445175010"><a name="zh-cn_topic_0080205353_p145291445175010"></a><a name="zh-cn_topic_0080205353_p145291445175010"></a>DIS.4107</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p115292459509"><a name="zh-cn_topic_0080205353_p115292459509"></a><a name="zh-cn_topic_0080205353_p115292459509"></a>Invalid AcessKey header.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p4529104518504"><a name="zh-cn_topic_0080205353_p4529104518504"></a><a name="zh-cn_topic_0080205353_p4529104518504"></a>请求头里的签名信息Authorization字段中的AK无效</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p125291345205017"><a name="zh-cn_topic_0080205353_p125291345205017"></a><a name="zh-cn_topic_0080205353_p125291345205017"></a>请检查是否传入有效的AK，避免AK填写错误、AK被删除、临时AK过期等。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row65295453503"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p152984505016"><a name="zh-cn_topic_0080205353_p152984505016"></a><a name="zh-cn_topic_0080205353_p152984505016"></a>441</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p1552984545012"><a name="zh-cn_topic_0080205353_p1552984545012"></a><a name="zh-cn_topic_0080205353_p1552984545012"></a>DIS.4108</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p145294458508"><a name="zh-cn_topic_0080205353_p145294458508"></a><a name="zh-cn_topic_0080205353_p145294458508"></a>Empty ServiceName header.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p95291745135017"><a name="zh-cn_topic_0080205353_p95291745135017"></a><a name="zh-cn_topic_0080205353_p95291745135017"></a>请求头里的签名信息Authorization字段中缺失服务名</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p55291545145010"><a name="zh-cn_topic_0080205353_p55291545145010"></a><a name="zh-cn_topic_0080205353_p55291545145010"></a>请检查请求头里的Authorization字段中是否包含服务名dis。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row253014518502"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p253016453506"><a name="zh-cn_topic_0080205353_p253016453506"></a><a name="zh-cn_topic_0080205353_p253016453506"></a>441</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p25303458509"><a name="zh-cn_topic_0080205353_p25303458509"></a><a name="zh-cn_topic_0080205353_p25303458509"></a>DIS.4109</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p35301145135019"><a name="zh-cn_topic_0080205353_p35301145135019"></a><a name="zh-cn_topic_0080205353_p35301145135019"></a>The Authorization header must contain the following field: {Credential,SignedHeaders,Signature;}</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p253054545014"><a name="zh-cn_topic_0080205353_p253054545014"></a><a name="zh-cn_topic_0080205353_p253054545014"></a>请求头里的签名信息Authorization字段有误</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p1453014545012"><a name="zh-cn_topic_0080205353_p1453014545012"></a><a name="zh-cn_topic_0080205353_p1453014545012"></a>请检查请求头里的Authorization字段是否包含Credential，SignedHeaders, Signature。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row45309451503"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p1453094516506"><a name="zh-cn_topic_0080205353_p1453094516506"></a><a name="zh-cn_topic_0080205353_p1453094516506"></a>441</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p1253018457505"><a name="zh-cn_topic_0080205353_p1253018457505"></a><a name="zh-cn_topic_0080205353_p1253018457505"></a>DIS.4110</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p8530945105020"><a name="zh-cn_topic_0080205353_p8530945105020"></a><a name="zh-cn_topic_0080205353_p8530945105020"></a>Empty Signature header.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p135306453509"><a name="zh-cn_topic_0080205353_p135306453509"></a><a name="zh-cn_topic_0080205353_p135306453509"></a>请求头里的签名信息Authorization字段中没有SignedHeaders</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p12530445145017"><a name="zh-cn_topic_0080205353_p12530445145017"></a><a name="zh-cn_topic_0080205353_p12530445145017"></a>请检查签名的生成方式是否有误。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row453011452501"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p1553015450507"><a name="zh-cn_topic_0080205353_p1553015450507"></a><a name="zh-cn_topic_0080205353_p1553015450507"></a>441</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p10530184517505"><a name="zh-cn_topic_0080205353_p10530184517505"></a><a name="zh-cn_topic_0080205353_p10530184517505"></a>DIS.4111</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p20530945135010"><a name="zh-cn_topic_0080205353_p20530945135010"></a><a name="zh-cn_topic_0080205353_p20530945135010"></a>Invalid Region header.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p753084510501"><a name="zh-cn_topic_0080205353_p753084510501"></a><a name="zh-cn_topic_0080205353_p753084510501"></a>请求头里的签名信息Authorization字段中的region无效</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p653015453508"><a name="zh-cn_topic_0080205353_p653015453508"></a><a name="zh-cn_topic_0080205353_p653015453508"></a>请检查是否传入有效的region。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row65309454501"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p553074565012"><a name="zh-cn_topic_0080205353_p553074565012"></a><a name="zh-cn_topic_0080205353_p553074565012"></a>441</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p10530164575016"><a name="zh-cn_topic_0080205353_p10530164575016"></a><a name="zh-cn_topic_0080205353_p10530164575016"></a>DIS.4112</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p25306458506"><a name="zh-cn_topic_0080205353_p25306458506"></a><a name="zh-cn_topic_0080205353_p25306458506"></a>Invalid authorization request.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p1653054519505"><a name="zh-cn_topic_0080205353_p1653054519505"></a><a name="zh-cn_topic_0080205353_p1653054519505"></a>使用AKSK生成的签名信息错误</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p0530174510506"><a name="zh-cn_topic_0080205353_p0530174510506"></a><a name="zh-cn_topic_0080205353_p0530174510506"></a>请检查签名的生成方式是否有误，检查AK、SK、region等信息。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row353017458507"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p105307452509"><a name="zh-cn_topic_0080205353_p105307452509"></a><a name="zh-cn_topic_0080205353_p105307452509"></a>441</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p1453034515010"><a name="zh-cn_topic_0080205353_p1453034515010"></a><a name="zh-cn_topic_0080205353_p1453034515010"></a>DIS.4113</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p8530164535013"><a name="zh-cn_topic_0080205353_p8530164535013"></a><a name="zh-cn_topic_0080205353_p8530164535013"></a>Empty Token header.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p13531345195016"><a name="zh-cn_topic_0080205353_p13531345195016"></a><a name="zh-cn_topic_0080205353_p13531345195016"></a>使用token认证时，请求头里的X-Auth-Token为空</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p17531174585011"><a name="zh-cn_topic_0080205353_p17531174585011"></a><a name="zh-cn_topic_0080205353_p17531174585011"></a>请检查请求头里的X-Auth-Token。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row453154520507"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p653114575011"><a name="zh-cn_topic_0080205353_p653114575011"></a><a name="zh-cn_topic_0080205353_p653114575011"></a>441</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p053104519501"><a name="zh-cn_topic_0080205353_p053104519501"></a><a name="zh-cn_topic_0080205353_p053104519501"></a>DIS.4114</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p55311845175016"><a name="zh-cn_topic_0080205353_p55311845175016"></a><a name="zh-cn_topic_0080205353_p55311845175016"></a>Invalid Token header.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p195318455509"><a name="zh-cn_topic_0080205353_p195318455509"></a><a name="zh-cn_topic_0080205353_p195318455509"></a>使用token认证时，请求头里的X-Auth-Token无效</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p653294535012"><a name="zh-cn_topic_0080205353_p653294535012"></a><a name="zh-cn_topic_0080205353_p653294535012"></a>请检查请求头里的X-Auth-Token是否过期。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row1532154575011"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p105325459504"><a name="zh-cn_topic_0080205353_p105325459504"></a><a name="zh-cn_topic_0080205353_p105325459504"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p2532845195010"><a name="zh-cn_topic_0080205353_p2532845195010"></a><a name="zh-cn_topic_0080205353_p2532845195010"></a>DIS.4116</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p205328452502"><a name="zh-cn_topic_0080205353_p205328452502"></a><a name="zh-cn_topic_0080205353_p205328452502"></a>Invalid RBAC.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p1453214515508"><a name="zh-cn_topic_0080205353_p1453214515508"></a><a name="zh-cn_topic_0080205353_p1453214515508"></a>用户操作受限</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p1353294511505"><a name="zh-cn_topic_0080205353_p1353294511505"></a><a name="zh-cn_topic_0080205353_p1353294511505"></a>请根据返回的具体信息判断帐号是否未实名认证、欠费、无DIS服务的操作权限等。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row1453212455505"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p13532134517506"><a name="zh-cn_topic_0080205353_p13532134517506"></a><a name="zh-cn_topic_0080205353_p13532134517506"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p1532745135016"><a name="zh-cn_topic_0080205353_p1532745135016"></a><a name="zh-cn_topic_0080205353_p1532745135016"></a>DIS.4117</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p253214453502"><a name="zh-cn_topic_0080205353_p253214453502"></a><a name="zh-cn_topic_0080205353_p253214453502"></a>Invalid Project Id.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p553214513505"><a name="zh-cn_topic_0080205353_p553214513505"></a><a name="zh-cn_topic_0080205353_p553214513505"></a>用户传入的projectId无效</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p10532174518503"><a name="zh-cn_topic_0080205353_p10532174518503"></a><a name="zh-cn_topic_0080205353_p10532174518503"></a>请检查传入的projectId是否有效，是否传入了其他project的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row17532645155011"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p1532164585018"><a name="zh-cn_topic_0080205353_p1532164585018"></a><a name="zh-cn_topic_0080205353_p1532164585018"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p3533164514505"><a name="zh-cn_topic_0080205353_p3533164514505"></a><a name="zh-cn_topic_0080205353_p3533164514505"></a>DIS.4200</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p65339455508"><a name="zh-cn_topic_0080205353_p65339455508"></a><a name="zh-cn_topic_0080205353_p65339455508"></a>Invalid request.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p155332454501"><a name="zh-cn_topic_0080205353_p155332454501"></a><a name="zh-cn_topic_0080205353_p155332454501"></a>用户的请求无效</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p135337457504"><a name="zh-cn_topic_0080205353_p135337457504"></a><a name="zh-cn_topic_0080205353_p135337457504"></a>请参考API文档检查请求。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row1053314510507"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p2533345165019"><a name="zh-cn_topic_0080205353_p2533345165019"></a><a name="zh-cn_topic_0080205353_p2533345165019"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p153384518503"><a name="zh-cn_topic_0080205353_p153384518503"></a><a name="zh-cn_topic_0080205353_p153384518503"></a>DIS.4201</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p6533134516501"><a name="zh-cn_topic_0080205353_p6533134516501"></a><a name="zh-cn_topic_0080205353_p6533134516501"></a>Invalid partition_id.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p155331245185013"><a name="zh-cn_topic_0080205353_p155331245185013"></a><a name="zh-cn_topic_0080205353_p155331245185013"></a>用户传入的partition_id无效</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p1453354510506"><a name="zh-cn_topic_0080205353_p1453354510506"></a><a name="zh-cn_topic_0080205353_p1453354510506"></a>请检查partition_id是否无效。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row115331845135018"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p553344585019"><a name="zh-cn_topic_0080205353_p553344585019"></a><a name="zh-cn_topic_0080205353_p553344585019"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p2533154525011"><a name="zh-cn_topic_0080205353_p2533154525011"></a><a name="zh-cn_topic_0080205353_p2533154525011"></a>DIS.4202</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p55331845105014"><a name="zh-cn_topic_0080205353_p55331845105014"></a><a name="zh-cn_topic_0080205353_p55331845105014"></a>Empty request.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p6533845115015"><a name="zh-cn_topic_0080205353_p6533845115015"></a><a name="zh-cn_topic_0080205353_p6533845115015"></a>用户的请求为空</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p1053412451500"><a name="zh-cn_topic_0080205353_p1053412451500"></a><a name="zh-cn_topic_0080205353_p1053412451500"></a>请传入有效的请求。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row75341445175014"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p45341454502"><a name="zh-cn_topic_0080205353_p45341454502"></a><a name="zh-cn_topic_0080205353_p45341454502"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p553414514508"><a name="zh-cn_topic_0080205353_p553414514508"></a><a name="zh-cn_topic_0080205353_p553414514508"></a>DIS.4203</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p18534154585012"><a name="zh-cn_topic_0080205353_p18534154585012"></a><a name="zh-cn_topic_0080205353_p18534154585012"></a>Invalid monitoring period.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p14534134513509"><a name="zh-cn_topic_0080205353_p14534134513509"></a><a name="zh-cn_topic_0080205353_p14534134513509"></a>查询监控信息的startTime无效</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p15534045165014"><a name="zh-cn_topic_0080205353_p15534045165014"></a><a name="zh-cn_topic_0080205353_p15534045165014"></a>请传入有效的时间戳。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row1753413459505"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p12534114545015"><a name="zh-cn_topic_0080205353_p12534114545015"></a><a name="zh-cn_topic_0080205353_p12534114545015"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p205347453503"><a name="zh-cn_topic_0080205353_p205347453503"></a><a name="zh-cn_topic_0080205353_p205347453503"></a>DIS.4204</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p6534145195012"><a name="zh-cn_topic_0080205353_p6534145195012"></a><a name="zh-cn_topic_0080205353_p6534145195012"></a>The monitoring period cannot be longer than 7 days.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p1253494565010"><a name="zh-cn_topic_0080205353_p1253494565010"></a><a name="zh-cn_topic_0080205353_p1253494565010"></a>仅允许查询最近7天内的监控信息</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p135341545175014"><a name="zh-cn_topic_0080205353_p135341545175014"></a><a name="zh-cn_topic_0080205353_p135341545175014"></a>请查询最近7天内的监控信息。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row35347453506"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p753484545018"><a name="zh-cn_topic_0080205353_p753484545018"></a><a name="zh-cn_topic_0080205353_p753484545018"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p1453414505014"><a name="zh-cn_topic_0080205353_p1453414505014"></a><a name="zh-cn_topic_0080205353_p1453414505014"></a>DIS.4208</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p14534124555013"><a name="zh-cn_topic_0080205353_p14534124555013"></a><a name="zh-cn_topic_0080205353_p14534124555013"></a>Invalid MRS cluster.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p115351345155019"><a name="zh-cn_topic_0080205353_p115351345155019"></a><a name="zh-cn_topic_0080205353_p115351345155019"></a>创建MRS转储任务时，传入的MRS集群无效</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p55351545105019"><a name="zh-cn_topic_0080205353_p55351545105019"></a><a name="zh-cn_topic_0080205353_p55351545105019"></a>请检查传入的MRS集群名称和ID，集群状态是否为运行中，以及是否为安全模式的集群。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row1253514545012"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p353574585019"><a name="zh-cn_topic_0080205353_p353574585019"></a><a name="zh-cn_topic_0080205353_p353574585019"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p1353519457505"><a name="zh-cn_topic_0080205353_p1353519457505"></a><a name="zh-cn_topic_0080205353_p1353519457505"></a>DIS.4209</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p1653519454507"><a name="zh-cn_topic_0080205353_p1653519454507"></a><a name="zh-cn_topic_0080205353_p1653519454507"></a>Invalid metrics label.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p153584519502"><a name="zh-cn_topic_0080205353_p153584519502"></a><a name="zh-cn_topic_0080205353_p153584519502"></a>查询监控信息时，传入的监控指标不合法</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p10535204514503"><a name="zh-cn_topic_0080205353_p10535204514503"></a><a name="zh-cn_topic_0080205353_p10535204514503"></a>请参考API文档检查监控指标并修正。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row8535164595016"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p18535164565012"><a name="zh-cn_topic_0080205353_p18535164565012"></a><a name="zh-cn_topic_0080205353_p18535164565012"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p9535104512505"><a name="zh-cn_topic_0080205353_p9535104512505"></a><a name="zh-cn_topic_0080205353_p9535104512505"></a>DIS.4215</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p195351645155016"><a name="zh-cn_topic_0080205353_p195351645155016"></a><a name="zh-cn_topic_0080205353_p195351645155016"></a>Invalid cursor type.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p18535144525013"><a name="zh-cn_topic_0080205353_p18535144525013"></a><a name="zh-cn_topic_0080205353_p18535144525013"></a>获取数据游标时，传入的游标类型cursor-type不合法</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p135351045115018"><a name="zh-cn_topic_0080205353_p135351045115018"></a><a name="zh-cn_topic_0080205353_p135351045115018"></a>请参考API文档检查cursor-type字段的范围并修正。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row953584513508"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p1653594512505"><a name="zh-cn_topic_0080205353_p1653594512505"></a><a name="zh-cn_topic_0080205353_p1653594512505"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p13536194515504"><a name="zh-cn_topic_0080205353_p13536194515504"></a><a name="zh-cn_topic_0080205353_p13536194515504"></a>DIS.4216</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p153664513503"><a name="zh-cn_topic_0080205353_p153664513503"></a><a name="zh-cn_topic_0080205353_p153664513503"></a>Invalid sequence_number.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p165364455502"><a name="zh-cn_topic_0080205353_p165364455502"></a><a name="zh-cn_topic_0080205353_p165364455502"></a>获取数据游标时，传入的序列号starting-sequence-number不合法</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p1953612451505"><a name="zh-cn_topic_0080205353_p1953612451505"></a><a name="zh-cn_topic_0080205353_p1953612451505"></a>请传入有效的starting-sequence-number。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row10536184516504"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p1353634545017"><a name="zh-cn_topic_0080205353_p1353634545017"></a><a name="zh-cn_topic_0080205353_p1353634545017"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p4536154519508"><a name="zh-cn_topic_0080205353_p4536154519508"></a><a name="zh-cn_topic_0080205353_p4536154519508"></a>DIS.4217</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p4536104510502"><a name="zh-cn_topic_0080205353_p4536104510502"></a><a name="zh-cn_topic_0080205353_p4536104510502"></a>Invalid partition cursor.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p195363458503"><a name="zh-cn_topic_0080205353_p195363458503"></a><a name="zh-cn_topic_0080205353_p195363458503"></a>从DIS通道下载数据时，传入的数据游标partition-cursor无效</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p55361345135010"><a name="zh-cn_topic_0080205353_p55361345135010"></a><a name="zh-cn_topic_0080205353_p55361345135010"></a>请重新获取partition-cursor并下载数据。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row1053614515010"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p1953616452500"><a name="zh-cn_topic_0080205353_p1953616452500"></a><a name="zh-cn_topic_0080205353_p1953616452500"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p753614512500"><a name="zh-cn_topic_0080205353_p753614512500"></a><a name="zh-cn_topic_0080205353_p753614512500"></a>DIS.4219</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p8536134525016"><a name="zh-cn_topic_0080205353_p8536134525016"></a><a name="zh-cn_topic_0080205353_p8536134525016"></a>The file is constantly resent.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p1153612454507"><a name="zh-cn_topic_0080205353_p1153612454507"></a><a name="zh-cn_topic_0080205353_p1153612454507"></a>该文件已经收到了</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p7536164595014"><a name="zh-cn_topic_0080205353_p7536164595014"></a><a name="zh-cn_topic_0080205353_p7536164595014"></a>文件已经收到不需要再上传。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row1753664505016"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p5536154515010"><a name="zh-cn_topic_0080205353_p5536154515010"></a><a name="zh-cn_topic_0080205353_p5536154515010"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p135361451503"><a name="zh-cn_topic_0080205353_p135361451503"></a><a name="zh-cn_topic_0080205353_p135361451503"></a>DIS.4220</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p1553614513503"><a name="zh-cn_topic_0080205353_p1553614513503"></a><a name="zh-cn_topic_0080205353_p1553614513503"></a>The block whose sequence number is %s needs to be resent.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p1053610454504"><a name="zh-cn_topic_0080205353_p1053610454504"></a><a name="zh-cn_topic_0080205353_p1053610454504"></a>文件块需要重新上传</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p3536124515505"><a name="zh-cn_topic_0080205353_p3536124515505"></a><a name="zh-cn_topic_0080205353_p3536124515505"></a>请按照指示上传对应的块。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row16536245205017"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p8536204575014"><a name="zh-cn_topic_0080205353_p8536204575014"></a><a name="zh-cn_topic_0080205353_p8536204575014"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p05366452508"><a name="zh-cn_topic_0080205353_p05366452508"></a><a name="zh-cn_topic_0080205353_p05366452508"></a>DIS.4221</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p953619459506"><a name="zh-cn_topic_0080205353_p953619459506"></a><a name="zh-cn_topic_0080205353_p953619459506"></a>Block seq %s is expected</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p1953618456509"><a name="zh-cn_topic_0080205353_p1953618456509"></a><a name="zh-cn_topic_0080205353_p1953618456509"></a>重复传入相同的文件块</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p115360451500"><a name="zh-cn_topic_0080205353_p115360451500"></a><a name="zh-cn_topic_0080205353_p115360451500"></a>请从系统期待的块开始上传。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row125361745185013"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p14537104585016"><a name="zh-cn_topic_0080205353_p14537104585016"></a><a name="zh-cn_topic_0080205353_p14537104585016"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p13537184517506"><a name="zh-cn_topic_0080205353_p13537184517506"></a><a name="zh-cn_topic_0080205353_p13537184517506"></a>DIS.4222</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p7537184525010"><a name="zh-cn_topic_0080205353_p7537184525010"></a><a name="zh-cn_topic_0080205353_p7537184525010"></a>Block seq %s is expected.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p753744585013"><a name="zh-cn_topic_0080205353_p753744585013"></a><a name="zh-cn_topic_0080205353_p753744585013"></a>传入的文件块不连续</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p653714457501"><a name="zh-cn_topic_0080205353_p653714457501"></a><a name="zh-cn_topic_0080205353_p653714457501"></a>从系统期待的块开始上传。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row65378455500"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p05377459505"><a name="zh-cn_topic_0080205353_p05377459505"></a><a name="zh-cn_topic_0080205353_p05377459505"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p0537645145010"><a name="zh-cn_topic_0080205353_p0537645145010"></a><a name="zh-cn_topic_0080205353_p0537645145010"></a>DIS.4223</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p1653704517505"><a name="zh-cn_topic_0080205353_p1653704517505"></a><a name="zh-cn_topic_0080205353_p1653704517505"></a>The file size exceeds the limit.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p05371745185012"><a name="zh-cn_topic_0080205353_p05371745185012"></a><a name="zh-cn_topic_0080205353_p05371745185012"></a>文件的容量超过了DIS的限制</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p17537134515010"><a name="zh-cn_topic_0080205353_p17537134515010"></a><a name="zh-cn_topic_0080205353_p17537134515010"></a>请拆分文件并再上传。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row135371545145016"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p15537144565019"><a name="zh-cn_topic_0080205353_p15537144565019"></a><a name="zh-cn_topic_0080205353_p15537144565019"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p7537145115010"><a name="zh-cn_topic_0080205353_p7537145115010"></a><a name="zh-cn_topic_0080205353_p7537145115010"></a>DIS.4224</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p6537124517502"><a name="zh-cn_topic_0080205353_p6537124517502"></a><a name="zh-cn_topic_0080205353_p6537124517502"></a>The sequence number is out of range.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p55371645135014"><a name="zh-cn_topic_0080205353_p55371645135014"></a><a name="zh-cn_topic_0080205353_p55371645135014"></a>获取数据游标时，传入的序列号starting-sequence-number不在有效范围</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p353711457508"><a name="zh-cn_topic_0080205353_p353711457508"></a><a name="zh-cn_topic_0080205353_p353711457508"></a>请传入有效的starting-sequence-number。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row6537134555010"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p353724575011"><a name="zh-cn_topic_0080205353_p353724575011"></a><a name="zh-cn_topic_0080205353_p353724575011"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p18537114510508"><a name="zh-cn_topic_0080205353_p18537114510508"></a><a name="zh-cn_topic_0080205353_p18537114510508"></a>DIS.4225</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p17537184517507"><a name="zh-cn_topic_0080205353_p17537184517507"></a><a name="zh-cn_topic_0080205353_p17537184517507"></a>Expired partition cursor.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p1953712453504"><a name="zh-cn_topic_0080205353_p1953712453504"></a><a name="zh-cn_topic_0080205353_p1953712453504"></a>从DIS通道下载数据时，传入的数据游标partition-cursor过期</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p35371045195015"><a name="zh-cn_topic_0080205353_p35371045195015"></a><a name="zh-cn_topic_0080205353_p35371045195015"></a>请重新获取partition-cursor并下载数据。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row753713451501"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p16537154511505"><a name="zh-cn_topic_0080205353_p16537154511505"></a><a name="zh-cn_topic_0080205353_p16537154511505"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p2537114545011"><a name="zh-cn_topic_0080205353_p2537114545011"></a><a name="zh-cn_topic_0080205353_p2537114545011"></a>DIS.4226</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p753714516509"><a name="zh-cn_topic_0080205353_p753714516509"></a><a name="zh-cn_topic_0080205353_p753714516509"></a>A partition iterator error occurred or a record to which the SN corresponds has expired. Try to obtain the partition iterator again.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p20537174545010"><a name="zh-cn_topic_0080205353_p20537174545010"></a><a name="zh-cn_topic_0080205353_p20537174545010"></a>获取数据时，传入的数据游标partition-cursor对应的序列号starting-sequence-number过期</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p75371045125013"><a name="zh-cn_topic_0080205353_p75371045125013"></a><a name="zh-cn_topic_0080205353_p75371045125013"></a>请获取获取数据游标，并用新游标获取数据。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row8537104516509"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p125388454508"><a name="zh-cn_topic_0080205353_p125388454508"></a><a name="zh-cn_topic_0080205353_p125388454508"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p15538124510507"><a name="zh-cn_topic_0080205353_p15538124510507"></a><a name="zh-cn_topic_0080205353_p15538124510507"></a>DIS.4300</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p1053854517504"><a name="zh-cn_topic_0080205353_p1053854517504"></a><a name="zh-cn_topic_0080205353_p1053854517504"></a>Request error.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p13538545125018"><a name="zh-cn_topic_0080205353_p13538545125018"></a><a name="zh-cn_topic_0080205353_p13538545125018"></a>请求体错误</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p1053834511508"><a name="zh-cn_topic_0080205353_p1053834511508"></a><a name="zh-cn_topic_0080205353_p1053834511508"></a>请对照API文档修正请求体。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row3538184512502"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p853804510501"><a name="zh-cn_topic_0080205353_p853804510501"></a><a name="zh-cn_topic_0080205353_p853804510501"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p4538445185012"><a name="zh-cn_topic_0080205353_p4538445185012"></a><a name="zh-cn_topic_0080205353_p4538445185012"></a>DIS.4301</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p12538134516509"><a name="zh-cn_topic_0080205353_p12538134516509"></a><a name="zh-cn_topic_0080205353_p12538134516509"></a>The stream does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p17538164535013"><a name="zh-cn_topic_0080205353_p17538164535013"></a><a name="zh-cn_topic_0080205353_p17538164535013"></a>通道不存在</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p1353824516503"><a name="zh-cn_topic_0080205353_p1353824516503"></a><a name="zh-cn_topic_0080205353_p1353824516503"></a>请检查传入的通道是否存在。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row85389453500"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p1053844512504"><a name="zh-cn_topic_0080205353_p1053844512504"></a><a name="zh-cn_topic_0080205353_p1053844512504"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p18538145125016"><a name="zh-cn_topic_0080205353_p18538145125016"></a><a name="zh-cn_topic_0080205353_p18538145125016"></a>DIS.4302</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p155380457504"><a name="zh-cn_topic_0080205353_p155380457504"></a><a name="zh-cn_topic_0080205353_p155380457504"></a>The partition does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p135384454507"><a name="zh-cn_topic_0080205353_p135384454507"></a><a name="zh-cn_topic_0080205353_p135384454507"></a>通道的分区不存在</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p125381845165010"><a name="zh-cn_topic_0080205353_p125381845165010"></a><a name="zh-cn_topic_0080205353_p125381845165010"></a>请检查用户传入的分区ID是否存在。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row353884514502"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p0538164517506"><a name="zh-cn_topic_0080205353_p0538164517506"></a><a name="zh-cn_topic_0080205353_p0538164517506"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p165389455504"><a name="zh-cn_topic_0080205353_p165389455504"></a><a name="zh-cn_topic_0080205353_p165389455504"></a>DIS.4303</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p195385457508"><a name="zh-cn_topic_0080205353_p195385457508"></a><a name="zh-cn_topic_0080205353_p195385457508"></a>Exceeded traffic control limit.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p10538845175016"><a name="zh-cn_topic_0080205353_p10538845175016"></a><a name="zh-cn_topic_0080205353_p10538845175016"></a>超出流控</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p8538184515012"><a name="zh-cn_topic_0080205353_p8538184515012"></a><a name="zh-cn_topic_0080205353_p8538184515012"></a>请扩容通道或降低上传速率。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row1153814457508"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p85381345185015"><a name="zh-cn_topic_0080205353_p85381345185015"></a><a name="zh-cn_topic_0080205353_p85381345185015"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p165381145185017"><a name="zh-cn_topic_0080205353_p165381145185017"></a><a name="zh-cn_topic_0080205353_p165381145185017"></a>DIS.4305</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p85381645175017"><a name="zh-cn_topic_0080205353_p85381645175017"></a><a name="zh-cn_topic_0080205353_p85381645175017"></a>Too many stream requests.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p8538134565018"><a name="zh-cn_topic_0080205353_p8538134565018"></a><a name="zh-cn_topic_0080205353_p8538134565018"></a>同一时间内用户请求太多</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p253819455508"><a name="zh-cn_topic_0080205353_p253819455508"></a><a name="zh-cn_topic_0080205353_p253819455508"></a>请降低请求频率并重试。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row3538164510504"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p25381145145016"><a name="zh-cn_topic_0080205353_p25381145145016"></a><a name="zh-cn_topic_0080205353_p25381145145016"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p10539164595017"><a name="zh-cn_topic_0080205353_p10539164595017"></a><a name="zh-cn_topic_0080205353_p10539164595017"></a>DIS.4306</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p55396457508"><a name="zh-cn_topic_0080205353_p55396457508"></a><a name="zh-cn_topic_0080205353_p55396457508"></a>The bucket does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p7539164535018"><a name="zh-cn_topic_0080205353_p7539164535018"></a><a name="zh-cn_topic_0080205353_p7539164535018"></a>传入的OBS桶不存在</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p165391245155010"><a name="zh-cn_topic_0080205353_p165391245155010"></a><a name="zh-cn_topic_0080205353_p165391245155010"></a>请检查OBS桶是否存在。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row12539184545011"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p353912459500"><a name="zh-cn_topic_0080205353_p353912459500"></a><a name="zh-cn_topic_0080205353_p353912459500"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p353904519503"><a name="zh-cn_topic_0080205353_p353904519503"></a><a name="zh-cn_topic_0080205353_p353904519503"></a>DIS.4307</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p1653934555013"><a name="zh-cn_topic_0080205353_p1653934555013"></a><a name="zh-cn_topic_0080205353_p1653934555013"></a>The stream already exists.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p105394458508"><a name="zh-cn_topic_0080205353_p105394458508"></a><a name="zh-cn_topic_0080205353_p105394458508"></a>指定的通道已经存在</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p145391645185011"><a name="zh-cn_topic_0080205353_p145391645185011"></a><a name="zh-cn_topic_0080205353_p145391645185011"></a>请修改通道名称并重新创建通道</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row18539164513508"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p1153924585015"><a name="zh-cn_topic_0080205353_p1153924585015"></a><a name="zh-cn_topic_0080205353_p1153924585015"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p4539104535015"><a name="zh-cn_topic_0080205353_p4539104535015"></a><a name="zh-cn_topic_0080205353_p4539104535015"></a>DIS.4308</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p0539945125015"><a name="zh-cn_topic_0080205353_p0539945125015"></a><a name="zh-cn_topic_0080205353_p0539945125015"></a>Insufficient quota.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p4539154525011"><a name="zh-cn_topic_0080205353_p4539154525011"></a><a name="zh-cn_topic_0080205353_p4539154525011"></a>通道或分区的配额不足</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p6539144514503"><a name="zh-cn_topic_0080205353_p6539144514503"></a><a name="zh-cn_topic_0080205353_p6539144514503"></a>请释放配额或提工单修改帐号的配额。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row5539145175017"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p105398451509"><a name="zh-cn_topic_0080205353_p105398451509"></a><a name="zh-cn_topic_0080205353_p105398451509"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p753974516509"><a name="zh-cn_topic_0080205353_p753974516509"></a><a name="zh-cn_topic_0080205353_p753974516509"></a>DIS.4309</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p1053914510508"><a name="zh-cn_topic_0080205353_p1053914510508"></a><a name="zh-cn_topic_0080205353_p1053914510508"></a>Too many request failures. Please try again later.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p11539145145010"><a name="zh-cn_topic_0080205353_p11539145145010"></a><a name="zh-cn_topic_0080205353_p11539145145010"></a>ip被加入黑名单</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p9539114516502"><a name="zh-cn_topic_0080205353_p9539114516502"></a><a name="zh-cn_topic_0080205353_p9539114516502"></a>由于频繁的错误访问导致用户ip被加入黑名单，请检查认证信息和请求是否有效，并稍后重试。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row9539114511504"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p19539134535016"><a name="zh-cn_topic_0080205353_p19539134535016"></a><a name="zh-cn_topic_0080205353_p19539134535016"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p253924512506"><a name="zh-cn_topic_0080205353_p253924512506"></a><a name="zh-cn_topic_0080205353_p253924512506"></a>DIS.4310</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p13539144511509"><a name="zh-cn_topic_0080205353_p13539144511509"></a><a name="zh-cn_topic_0080205353_p13539144511509"></a>OBS access error.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p5539194510508"><a name="zh-cn_topic_0080205353_p5539194510508"></a><a name="zh-cn_topic_0080205353_p5539194510508"></a>访问OBS失败</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p11539154510509"><a name="zh-cn_topic_0080205353_p11539154510509"></a><a name="zh-cn_topic_0080205353_p11539154510509"></a>请检查用户是否有访问OBS的权限。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row953964575014"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p354084515509"><a name="zh-cn_topic_0080205353_p354084515509"></a><a name="zh-cn_topic_0080205353_p354084515509"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p15401745155014"><a name="zh-cn_topic_0080205353_p15401745155014"></a><a name="zh-cn_topic_0080205353_p15401745155014"></a>DIS.4329</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p354074565016"><a name="zh-cn_topic_0080205353_p354074565016"></a><a name="zh-cn_topic_0080205353_p354074565016"></a>app quota exceeded.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p854054519501"><a name="zh-cn_topic_0080205353_p854054519501"></a><a name="zh-cn_topic_0080205353_p854054519501"></a>APP配额超出限制</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p55401459509"><a name="zh-cn_topic_0080205353_p55401459509"></a><a name="zh-cn_topic_0080205353_p55401459509"></a>请释放APP的配额。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row18540184525013"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p10540124518500"><a name="zh-cn_topic_0080205353_p10540124518500"></a><a name="zh-cn_topic_0080205353_p10540124518500"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p1540104535011"><a name="zh-cn_topic_0080205353_p1540104535011"></a><a name="zh-cn_topic_0080205353_p1540104535011"></a>DIS.4330</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p1654064516506"><a name="zh-cn_topic_0080205353_p1654064516506"></a><a name="zh-cn_topic_0080205353_p1654064516506"></a>app already exist.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p254018451507"><a name="zh-cn_topic_0080205353_p254018451507"></a><a name="zh-cn_topic_0080205353_p254018451507"></a>已经存在同名的APP</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p11540104515013"><a name="zh-cn_topic_0080205353_p11540104515013"></a><a name="zh-cn_topic_0080205353_p11540104515013"></a>请修改APP名称并重新创建APP。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row175401458506"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p654018457503"><a name="zh-cn_topic_0080205353_p654018457503"></a><a name="zh-cn_topic_0080205353_p654018457503"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p15401945125010"><a name="zh-cn_topic_0080205353_p15401945125010"></a><a name="zh-cn_topic_0080205353_p15401945125010"></a>DIS.4331</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p854054505013"><a name="zh-cn_topic_0080205353_p854054505013"></a><a name="zh-cn_topic_0080205353_p854054505013"></a>app is using.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p1754054505019"><a name="zh-cn_topic_0080205353_p1754054505019"></a><a name="zh-cn_topic_0080205353_p1754054505019"></a>删除app时，当前app在使用中</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p85401745205017"><a name="zh-cn_topic_0080205353_p85401745205017"></a><a name="zh-cn_topic_0080205353_p85401745205017"></a>请确认app是否在使用中，如需删除请停止使用并重新删除。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row0540114519509"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p115401345185011"><a name="zh-cn_topic_0080205353_p115401345185011"></a><a name="zh-cn_topic_0080205353_p115401345185011"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p154018452506"><a name="zh-cn_topic_0080205353_p154018452506"></a><a name="zh-cn_topic_0080205353_p154018452506"></a>DIS.4332</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p45401845135015"><a name="zh-cn_topic_0080205353_p45401845135015"></a><a name="zh-cn_topic_0080205353_p45401845135015"></a>app not found.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p4540144505014"><a name="zh-cn_topic_0080205353_p4540144505014"></a><a name="zh-cn_topic_0080205353_p4540144505014"></a>指定的APP不存在</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p195401245125015"><a name="zh-cn_topic_0080205353_p195401245125015"></a><a name="zh-cn_topic_0080205353_p195401245125015"></a>请检查指定的APP名称是否正确</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row135407453502"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p1654004595014"><a name="zh-cn_topic_0080205353_p1654004595014"></a><a name="zh-cn_topic_0080205353_p1654004595014"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p454134518501"><a name="zh-cn_topic_0080205353_p454134518501"></a><a name="zh-cn_topic_0080205353_p454134518501"></a>DIS.4335</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p11541144518503"><a name="zh-cn_topic_0080205353_p11541144518503"></a><a name="zh-cn_topic_0080205353_p11541144518503"></a>Invalid IAM agency.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p19541104575012"><a name="zh-cn_topic_0080205353_p19541104575012"></a><a name="zh-cn_topic_0080205353_p19541104575012"></a>创建转储任务时，使用的IAM委托无效</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p4541174520509"><a name="zh-cn_topic_0080205353_p4541174520509"></a><a name="zh-cn_topic_0080205353_p4541174520509"></a>检查DIS创建的dis_admin_agency或用户自定义的IAM委托是否存在，权限是否完整。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row165411045165017"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p18541144511504"><a name="zh-cn_topic_0080205353_p18541144511504"></a><a name="zh-cn_topic_0080205353_p18541144511504"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p1854112456505"><a name="zh-cn_topic_0080205353_p1854112456505"></a><a name="zh-cn_topic_0080205353_p1854112456505"></a>DIS.4336</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p454117459507"><a name="zh-cn_topic_0080205353_p454117459507"></a><a name="zh-cn_topic_0080205353_p454117459507"></a>Invalid HDFS path.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p154114515505"><a name="zh-cn_topic_0080205353_p154114515505"></a><a name="zh-cn_topic_0080205353_p154114515505"></a>创建MRS转储任务时，传入的MRS HDFS路径无效</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p15541445205010"><a name="zh-cn_topic_0080205353_p15541445205010"></a><a name="zh-cn_topic_0080205353_p15541445205010"></a>请检查传入的MRS HDFS路径是否存在。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row1254113456500"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p654114453504"><a name="zh-cn_topic_0080205353_p654114453504"></a><a name="zh-cn_topic_0080205353_p654114453504"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p7541745135018"><a name="zh-cn_topic_0080205353_p7541745135018"></a><a name="zh-cn_topic_0080205353_p7541745135018"></a>DIS.4337</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p15417459508"><a name="zh-cn_topic_0080205353_p15417459508"></a><a name="zh-cn_topic_0080205353_p15417459508"></a>The DLI database does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p15413456505"><a name="zh-cn_topic_0080205353_p15413456505"></a><a name="zh-cn_topic_0080205353_p15413456505"></a>创建DLI转储任务时，传入的DLI数据库不存在</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p55410455509"><a name="zh-cn_topic_0080205353_p55410455509"></a><a name="zh-cn_topic_0080205353_p55410455509"></a>请检查传入的DLI数据库是否存在。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row1754112453506"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p1454154517500"><a name="zh-cn_topic_0080205353_p1454154517500"></a><a name="zh-cn_topic_0080205353_p1454154517500"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p65411745105010"><a name="zh-cn_topic_0080205353_p65411745105010"></a><a name="zh-cn_topic_0080205353_p65411745105010"></a>DIS.4338</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p1754234575014"><a name="zh-cn_topic_0080205353_p1754234575014"></a><a name="zh-cn_topic_0080205353_p1754234575014"></a>The DLI table does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p1454284511508"><a name="zh-cn_topic_0080205353_p1454284511508"></a><a name="zh-cn_topic_0080205353_p1454284511508"></a>创建DLI转储任务时，传入的DLI数据表不存在</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p35421145185017"><a name="zh-cn_topic_0080205353_p35421145185017"></a><a name="zh-cn_topic_0080205353_p35421145185017"></a>请检查传入的DLI表是否存在，并且是否为DLI内表。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row18542345155011"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p1154294511507"><a name="zh-cn_topic_0080205353_p1154294511507"></a><a name="zh-cn_topic_0080205353_p1154294511507"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p25421458507"><a name="zh-cn_topic_0080205353_p25421458507"></a><a name="zh-cn_topic_0080205353_p25421458507"></a>DIS.4341</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p45421450506"><a name="zh-cn_topic_0080205353_p45421450506"></a><a name="zh-cn_topic_0080205353_p45421450506"></a>The CloudTable cluster does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p9542104535011"><a name="zh-cn_topic_0080205353_p9542104535011"></a><a name="zh-cn_topic_0080205353_p9542104535011"></a>创建CloudTable转储任务时，传入的CloudTable集群不存在</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p854264575017"><a name="zh-cn_topic_0080205353_p854264575017"></a><a name="zh-cn_topic_0080205353_p854264575017"></a>请检查传入的CloudTable集群是否存在，集群状态是否正常。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row1454217459500"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p3542245165012"><a name="zh-cn_topic_0080205353_p3542245165012"></a><a name="zh-cn_topic_0080205353_p3542245165012"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p85421045155018"><a name="zh-cn_topic_0080205353_p85421045155018"></a><a name="zh-cn_topic_0080205353_p85421045155018"></a>DIS.4342</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p9542114575014"><a name="zh-cn_topic_0080205353_p9542114575014"></a><a name="zh-cn_topic_0080205353_p9542114575014"></a>The CloudTable table does not exist</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p9543245185015"><a name="zh-cn_topic_0080205353_p9543245185015"></a><a name="zh-cn_topic_0080205353_p9543245185015"></a>创建CloudTable转储任务时，传入的CloudTable表不存在</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p15543184525012"><a name="zh-cn_topic_0080205353_p15543184525012"></a><a name="zh-cn_topic_0080205353_p15543184525012"></a>请检查传入的CloudTable表是否存在。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row7543145125016"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p13543124515012"><a name="zh-cn_topic_0080205353_p13543124515012"></a><a name="zh-cn_topic_0080205353_p13543124515012"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p1954374512506"><a name="zh-cn_topic_0080205353_p1954374512506"></a><a name="zh-cn_topic_0080205353_p1954374512506"></a>DIS.4343</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p7547645125019"><a name="zh-cn_topic_0080205353_p7547645125019"></a><a name="zh-cn_topic_0080205353_p7547645125019"></a>The CloudTable table family does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p9547184565017"><a name="zh-cn_topic_0080205353_p9547184565017"></a><a name="zh-cn_topic_0080205353_p9547184565017"></a>创建CloudTable转储任务时，传入的CloudTable表的列族不存在</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p16547114515500"><a name="zh-cn_topic_0080205353_p16547114515500"></a><a name="zh-cn_topic_0080205353_p16547114515500"></a>请检查传入的CloudTable表的列族名称是否存在。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row17547145105019"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p254764585013"><a name="zh-cn_topic_0080205353_p254764585013"></a><a name="zh-cn_topic_0080205353_p254764585013"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p1454714505019"><a name="zh-cn_topic_0080205353_p1454714505019"></a><a name="zh-cn_topic_0080205353_p1454714505019"></a>DIS.4345</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p1054784513509"><a name="zh-cn_topic_0080205353_p1054784513509"></a><a name="zh-cn_topic_0080205353_p1054784513509"></a>Invalid CloudTable schema.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p55471245205017"><a name="zh-cn_topic_0080205353_p55471245205017"></a><a name="zh-cn_topic_0080205353_p55471245205017"></a>创建CloudTable转储任务时，传入的schema无效</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p25472045165013"><a name="zh-cn_topic_0080205353_p25472045165013"></a><a name="zh-cn_topic_0080205353_p25472045165013"></a>请根据返回的详细信息检查schema，例如配置的JSON属性名称是否存在，参数是否合法等。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row55478458507"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p11547124514502"><a name="zh-cn_topic_0080205353_p11547124514502"></a><a name="zh-cn_topic_0080205353_p11547124514502"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p145471245145017"><a name="zh-cn_topic_0080205353_p145471245145017"></a><a name="zh-cn_topic_0080205353_p145471245145017"></a>DIS.4348</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p154716455505"><a name="zh-cn_topic_0080205353_p154716455505"></a><a name="zh-cn_topic_0080205353_p154716455505"></a>Invalid CloudTable openTSDB schema.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p754718455503"><a name="zh-cn_topic_0080205353_p754718455503"></a><a name="zh-cn_topic_0080205353_p754718455503"></a>创建CloudTable openTSDB转储任务时，传入的schema无效</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p195475452505"><a name="zh-cn_topic_0080205353_p195475452505"></a><a name="zh-cn_topic_0080205353_p195475452505"></a>请根据返回的详细信息检查schema，例如配置的JSON属性名称是否存在，参数是否合法等。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row854811459500"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p954810456508"><a name="zh-cn_topic_0080205353_p954810456508"></a><a name="zh-cn_topic_0080205353_p954810456508"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p135481145135011"><a name="zh-cn_topic_0080205353_p135481145135011"></a><a name="zh-cn_topic_0080205353_p135481145135011"></a>DIS.4350</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p17548194516507"><a name="zh-cn_topic_0080205353_p17548194516507"></a><a name="zh-cn_topic_0080205353_p17548194516507"></a>Invalid DWS cluster.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p19548174515505"><a name="zh-cn_topic_0080205353_p19548174515505"></a><a name="zh-cn_topic_0080205353_p19548174515505"></a>创建DWS转储任务时，传入的DWS集群不存在</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p18548104525010"><a name="zh-cn_topic_0080205353_p18548104525010"></a><a name="zh-cn_topic_0080205353_p18548104525010"></a>请检查DWS集群是否存在，运行是否正常。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row1854884545012"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p654816454505"><a name="zh-cn_topic_0080205353_p654816454505"></a><a name="zh-cn_topic_0080205353_p654816454505"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p5548845125013"><a name="zh-cn_topic_0080205353_p5548845125013"></a><a name="zh-cn_topic_0080205353_p5548845125013"></a>DIS.4351</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p14548645145019"><a name="zh-cn_topic_0080205353_p14548645145019"></a><a name="zh-cn_topic_0080205353_p14548645145019"></a>Invalid KMS userKey.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p35481245185020"><a name="zh-cn_topic_0080205353_p35481245185020"></a><a name="zh-cn_topic_0080205353_p35481245185020"></a>创建DWS转储任务时，传入的KMS秘钥信息无效</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p20548154555018"><a name="zh-cn_topic_0080205353_p20548154555018"></a><a name="zh-cn_topic_0080205353_p20548154555018"></a>请检查KMS密钥是否存在。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row4548174555017"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p15548144515501"><a name="zh-cn_topic_0080205353_p15548144515501"></a><a name="zh-cn_topic_0080205353_p15548144515501"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p14548145205015"><a name="zh-cn_topic_0080205353_p14548145205015"></a><a name="zh-cn_topic_0080205353_p14548145205015"></a>DIS.4354</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p3548104535015"><a name="zh-cn_topic_0080205353_p3548104535015"></a><a name="zh-cn_topic_0080205353_p3548104535015"></a>The transfer task does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p15548545105017"><a name="zh-cn_topic_0080205353_p15548545105017"></a><a name="zh-cn_topic_0080205353_p15548545105017"></a>删除或更新转储任务时，转储任务不存在</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p35481445165018"><a name="zh-cn_topic_0080205353_p35481445165018"></a><a name="zh-cn_topic_0080205353_p35481445165018"></a>请检查转储任务是否存在。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row18548174510508"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p145491445175013"><a name="zh-cn_topic_0080205353_p145491445175013"></a><a name="zh-cn_topic_0080205353_p145491445175013"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p75498456504"><a name="zh-cn_topic_0080205353_p75498456504"></a><a name="zh-cn_topic_0080205353_p75498456504"></a>DIS.4355</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p115497451504"><a name="zh-cn_topic_0080205353_p115497451504"></a><a name="zh-cn_topic_0080205353_p115497451504"></a>The transfer task already exists.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p18549184595017"><a name="zh-cn_topic_0080205353_p18549184595017"></a><a name="zh-cn_topic_0080205353_p18549184595017"></a>创建转储任务时，同一个通道下已存在同名的转储任务</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p1549945105015"><a name="zh-cn_topic_0080205353_p1549945105015"></a><a name="zh-cn_topic_0080205353_p1549945105015"></a>请修改新创建转储任务的名称并重新创建。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row1754912457505"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p6549164565016"><a name="zh-cn_topic_0080205353_p6549164565016"></a><a name="zh-cn_topic_0080205353_p6549164565016"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p1654918458507"><a name="zh-cn_topic_0080205353_p1654918458507"></a><a name="zh-cn_topic_0080205353_p1654918458507"></a>DIS.4357</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p1254964512502"><a name="zh-cn_topic_0080205353_p1254964512502"></a><a name="zh-cn_topic_0080205353_p1254964512502"></a>Exceeded transfer task quota.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p55495457508"><a name="zh-cn_topic_0080205353_p55495457508"></a><a name="zh-cn_topic_0080205353_p55495457508"></a>单个通道仅允许同时存在5个转储任务，再创建新的转储任务会超出配额限制</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p2054964510503"><a name="zh-cn_topic_0080205353_p2054964510503"></a><a name="zh-cn_topic_0080205353_p2054964510503"></a>请删除废弃的转储任务释放配额。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row15549194517507"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p1154964512503"><a name="zh-cn_topic_0080205353_p1154964512503"></a><a name="zh-cn_topic_0080205353_p1154964512503"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p55492450508"><a name="zh-cn_topic_0080205353_p55492450508"></a><a name="zh-cn_topic_0080205353_p55492450508"></a>DIS.4358</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p15549154555013"><a name="zh-cn_topic_0080205353_p15549154555013"></a><a name="zh-cn_topic_0080205353_p15549154555013"></a>The stream supports specific transfer tasks. Check the data type of the stream.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p1254934520502"><a name="zh-cn_topic_0080205353_p1254934520502"></a><a name="zh-cn_topic_0080205353_p1254934520502"></a>小文件转储的通道不支持创建普通转储任务</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p1954914518509"><a name="zh-cn_topic_0080205353_p1954914518509"></a><a name="zh-cn_topic_0080205353_p1954914518509"></a>请创建新的通道并创建转储任务。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row13549124595013"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p1155024514507"><a name="zh-cn_topic_0080205353_p1155024514507"></a><a name="zh-cn_topic_0080205353_p1155024514507"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p2550124595016"><a name="zh-cn_topic_0080205353_p2550124595016"></a><a name="zh-cn_topic_0080205353_p2550124595016"></a>DIS.4360</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p1355044555019"><a name="zh-cn_topic_0080205353_p1355044555019"></a><a name="zh-cn_topic_0080205353_p1355044555019"></a>Invalid data schema.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p355014518502"><a name="zh-cn_topic_0080205353_p355014518502"></a><a name="zh-cn_topic_0080205353_p355014518502"></a>创建通道或更新通道时，传入的data_schema无效</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p1555044512508"><a name="zh-cn_topic_0080205353_p1555044512508"></a><a name="zh-cn_topic_0080205353_p1555044512508"></a>请检查data_schema的格式并重试。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row145502455502"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p1055044565012"><a name="zh-cn_topic_0080205353_p1055044565012"></a><a name="zh-cn_topic_0080205353_p1055044565012"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p155501145135010"><a name="zh-cn_topic_0080205353_p155501145135010"></a><a name="zh-cn_topic_0080205353_p155501145135010"></a>DIS.4601</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p8550154515504"><a name="zh-cn_topic_0080205353_p8550154515504"></a><a name="zh-cn_topic_0080205353_p8550154515504"></a>The number of resource tags has reached the maximum.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p155014454505"><a name="zh-cn_topic_0080205353_p155014454505"></a><a name="zh-cn_topic_0080205353_p155014454505"></a>一个资源上最多有10个标签，添加标签时资源上已添加的标签数超出限制</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p1055014453501"><a name="zh-cn_topic_0080205353_p1055014453501"></a><a name="zh-cn_topic_0080205353_p1055014453501"></a>请删除废弃的标签并重新添加标签。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row12550174510504"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p5550745185011"><a name="zh-cn_topic_0080205353_p5550745185011"></a><a name="zh-cn_topic_0080205353_p5550745185011"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p45508451501"><a name="zh-cn_topic_0080205353_p45508451501"></a><a name="zh-cn_topic_0080205353_p45508451501"></a>DIS.4602</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p3550194525010"><a name="zh-cn_topic_0080205353_p3550194525010"></a><a name="zh-cn_topic_0080205353_p3550194525010"></a>Invalid resource type.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p655064519503"><a name="zh-cn_topic_0080205353_p655064519503"></a><a name="zh-cn_topic_0080205353_p655064519503"></a>资源类型不合法</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p2550145135015"><a name="zh-cn_topic_0080205353_p2550145135015"></a><a name="zh-cn_topic_0080205353_p2550145135015"></a>请检查资源类型是否合法。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row555012451509"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p755034515500"><a name="zh-cn_topic_0080205353_p755034515500"></a><a name="zh-cn_topic_0080205353_p755034515500"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p1155144512503"><a name="zh-cn_topic_0080205353_p1155144512503"></a><a name="zh-cn_topic_0080205353_p1155144512503"></a>DIS.4603</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p16551045155013"><a name="zh-cn_topic_0080205353_p16551045155013"></a><a name="zh-cn_topic_0080205353_p16551045155013"></a>The resource does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p10551134515013"><a name="zh-cn_topic_0080205353_p10551134515013"></a><a name="zh-cn_topic_0080205353_p10551134515013"></a>资源不存在</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p555117451503"><a name="zh-cn_topic_0080205353_p555117451503"></a><a name="zh-cn_topic_0080205353_p555117451503"></a>请确认该资源是否已被删除。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row555134512509"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p1155111453502"><a name="zh-cn_topic_0080205353_p1155111453502"></a><a name="zh-cn_topic_0080205353_p1155111453502"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p3551194585018"><a name="zh-cn_topic_0080205353_p3551194585018"></a><a name="zh-cn_topic_0080205353_p3551194585018"></a>DIS.4604</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p1655124555018"><a name="zh-cn_topic_0080205353_p1655124555018"></a><a name="zh-cn_topic_0080205353_p1655124555018"></a>The key does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p165511845185018"><a name="zh-cn_topic_0080205353_p165511845185018"></a><a name="zh-cn_topic_0080205353_p165511845185018"></a>标签Key不存在</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p1355104517501"><a name="zh-cn_topic_0080205353_p1355104517501"></a><a name="zh-cn_topic_0080205353_p1355104517501"></a>请确认标签Key是否存在。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row1755164555018"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p55511445135010"><a name="zh-cn_topic_0080205353_p55511445135010"></a><a name="zh-cn_topic_0080205353_p55511445135010"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p14551104517504"><a name="zh-cn_topic_0080205353_p14551104517504"></a><a name="zh-cn_topic_0080205353_p14551104517504"></a>DIS.4605</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p19551345155018"><a name="zh-cn_topic_0080205353_p19551345155018"></a><a name="zh-cn_topic_0080205353_p19551345155018"></a>The action is not supported.</p>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p1755115453507"><a name="zh-cn_topic_0080205353_p1755115453507"></a><a name="zh-cn_topic_0080205353_p1755115453507"></a>当前标签操作不支持</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p18551845175011"><a name="zh-cn_topic_0080205353_p18551845175011"></a><a name="zh-cn_topic_0080205353_p18551845175011"></a>请确认当前标签操作是否合法，当前仅支持create和delete操作。</p>
</td>
</tr>
<tr id="zh-cn_topic_0080205353_row145511456502"><td class="cellrowborder" valign="top" width="7.219278072192781%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0080205353_p155515454501"><a name="zh-cn_topic_0080205353_p155515454501"></a><a name="zh-cn_topic_0080205353_p155515454501"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="10.30896910308969%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0080205353_p455119455508"><a name="zh-cn_topic_0080205353_p455119455508"></a><a name="zh-cn_topic_0080205353_p455119455508"></a>DIS.5000~DIS.5999</p>
</td>
<td class="cellrowborder" valign="top" width="27.83721627837216%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0080205353_p1955264545017"><a name="zh-cn_topic_0080205353_p1955264545017"></a><a name="zh-cn_topic_0080205353_p1955264545017"></a>System error.</p>
<div class="note" id="zh-cn_topic_0080205353_note1142184511502"><a name="zh-cn_topic_0080205353_note1142184511502"></a><a name="zh-cn_topic_0080205353_note1142184511502"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0080205353_p13552145125015"><a name="zh-cn_topic_0080205353_p13552145125015"></a><a name="zh-cn_topic_0080205353_p13552145125015"></a>系统错误，请联系技术支持工程师处理。</p>
</div></div>
</td>
<td class="cellrowborder" valign="top" width="20.61793820617938%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0080205353_p145525457508"><a name="zh-cn_topic_0080205353_p145525457508"></a><a name="zh-cn_topic_0080205353_p145525457508"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="34.016598340165984%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0080205353_p19552445105017"><a name="zh-cn_topic_0080205353_p19552445105017"></a><a name="zh-cn_topic_0080205353_p19552445105017"></a>-</p>
</td>
</tr>
</tbody>
</table>

