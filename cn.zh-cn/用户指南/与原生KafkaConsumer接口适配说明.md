# 与原生KafkaConsumer接口适配说明<a name="dayu_01_0249"></a>

**表 1**  接口适配说明

<a name="zh-cn_topic_0142797207_table59817209306"></a>
<table><thead align="left"><tr id="zh-cn_topic_0142797207_row198182019308"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0142797207_p28761618133113"><a name="zh-cn_topic_0142797207_p28761618133113"></a><a name="zh-cn_topic_0142797207_p28761618133113"></a>原生KafkaConsumer</p>
</th>
<th class="cellrowborder" valign="top" width="13.370000000000001%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0142797207_p1387691811312"><a name="zh-cn_topic_0142797207_p1387691811312"></a><a name="zh-cn_topic_0142797207_p1387691811312"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="20.630000000000003%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0142797207_p198761918193114"><a name="zh-cn_topic_0142797207_p198761918193114"></a><a name="zh-cn_topic_0142797207_p198761918193114"></a>DISKafkaConsumer</p>
</th>
<th class="cellrowborder" valign="top" width="41%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0142797207_p14876121823112"><a name="zh-cn_topic_0142797207_p14876121823112"></a><a name="zh-cn_topic_0142797207_p14876121823112"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0142797207_row109812205301"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p11859125883118"><a name="zh-cn_topic_0142797207_p11859125883118"></a><a name="zh-cn_topic_0142797207_p11859125883118"></a>Set&lt;TopicPartition&gt; assignment()</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p11859258173114"><a name="zh-cn_topic_0142797207_p11859258173114"></a><a name="zh-cn_topic_0142797207_p11859258173114"></a>接口</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p9859175811313"><a name="zh-cn_topic_0142797207_p9859175811313"></a><a name="zh-cn_topic_0142797207_p9859175811313"></a>支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p13859145813120"><a name="zh-cn_topic_0142797207_p13859145813120"></a><a name="zh-cn_topic_0142797207_p13859145813120"></a>获取consumer消费的通道与分区信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0142797207_row129816203303"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p15747954320"><a name="zh-cn_topic_0142797207_p15747954320"></a><a name="zh-cn_topic_0142797207_p15747954320"></a>Set&lt;String&gt; subscription()</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p127471759322"><a name="zh-cn_topic_0142797207_p127471759322"></a><a name="zh-cn_topic_0142797207_p127471759322"></a>接口</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p77478523216"><a name="zh-cn_topic_0142797207_p77478523216"></a><a name="zh-cn_topic_0142797207_p77478523216"></a>支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p67472533212"><a name="zh-cn_topic_0142797207_p67472533212"></a><a name="zh-cn_topic_0142797207_p67472533212"></a>获取consumer已订阅的通道名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0142797207_row8981202093015"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p6747124263213"><a name="zh-cn_topic_0142797207_p6747124263213"></a><a name="zh-cn_topic_0142797207_p6747124263213"></a>void assign(Collection&lt;TopicPartition&gt; var1)</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p2747134211329"><a name="zh-cn_topic_0142797207_p2747134211329"></a><a name="zh-cn_topic_0142797207_p2747134211329"></a>接口</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p137471424326"><a name="zh-cn_topic_0142797207_p137471424326"></a><a name="zh-cn_topic_0142797207_p137471424326"></a>支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p12747174273215"><a name="zh-cn_topic_0142797207_p12747174273215"></a><a name="zh-cn_topic_0142797207_p12747174273215"></a>分配指定的分区</p>
</td>
</tr>
<tr id="zh-cn_topic_0142797207_row1098142013302"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p75361554193218"><a name="zh-cn_topic_0142797207_p75361554193218"></a><a name="zh-cn_topic_0142797207_p75361554193218"></a>void subscribe(Collection&lt;String&gt; var1)</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p145366543326"><a name="zh-cn_topic_0142797207_p145366543326"></a><a name="zh-cn_topic_0142797207_p145366543326"></a>接口</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p195364548320"><a name="zh-cn_topic_0142797207_p195364548320"></a><a name="zh-cn_topic_0142797207_p195364548320"></a>支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p353655473218"><a name="zh-cn_topic_0142797207_p353655473218"></a><a name="zh-cn_topic_0142797207_p353655473218"></a>订阅指定的通道</p>
</td>
</tr>
<tr id="zh-cn_topic_0142797207_row1999022012303"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p136813514336"><a name="zh-cn_topic_0142797207_p136813514336"></a><a name="zh-cn_topic_0142797207_p136813514336"></a>void subscribe(Collection&lt;String&gt; var1, ConsumerRebalanceListener var2)</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p196811858336"><a name="zh-cn_topic_0142797207_p196811858336"></a><a name="zh-cn_topic_0142797207_p196811858336"></a>接口</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p15681115133319"><a name="zh-cn_topic_0142797207_p15681115133319"></a><a name="zh-cn_topic_0142797207_p15681115133319"></a>支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p1681135183313"><a name="zh-cn_topic_0142797207_p1681135183313"></a><a name="zh-cn_topic_0142797207_p1681135183313"></a>订阅指定的通道并支持ConsumerRebalanceListener回调</p>
</td>
</tr>
<tr id="zh-cn_topic_0142797207_row1990020203018"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p437732215339"><a name="zh-cn_topic_0142797207_p437732215339"></a><a name="zh-cn_topic_0142797207_p437732215339"></a>void subscribe(Pattern var1, ConsumerRebalanceListener var2)</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p203771222183311"><a name="zh-cn_topic_0142797207_p203771222183311"></a><a name="zh-cn_topic_0142797207_p203771222183311"></a>接口</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p637717225336"><a name="zh-cn_topic_0142797207_p637717225336"></a><a name="zh-cn_topic_0142797207_p637717225336"></a>支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p4377422103320"><a name="zh-cn_topic_0142797207_p4377422103320"></a><a name="zh-cn_topic_0142797207_p4377422103320"></a>订阅所有匹配通配符的通道并支持ConsumerRebalanceListener回调</p>
</td>
</tr>
<tr id="zh-cn_topic_0142797207_row17830211183312"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p8259531183313"><a name="zh-cn_topic_0142797207_p8259531183313"></a><a name="zh-cn_topic_0142797207_p8259531183313"></a>void unsubscribe()</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p10259143111335"><a name="zh-cn_topic_0142797207_p10259143111335"></a><a name="zh-cn_topic_0142797207_p10259143111335"></a>接口</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p625973173317"><a name="zh-cn_topic_0142797207_p625973173317"></a><a name="zh-cn_topic_0142797207_p625973173317"></a>支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p1325963115335"><a name="zh-cn_topic_0142797207_p1325963115335"></a><a name="zh-cn_topic_0142797207_p1325963115335"></a>取消所有订阅</p>
</td>
</tr>
<tr id="zh-cn_topic_0142797207_row197916333"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p1569733911333"><a name="zh-cn_topic_0142797207_p1569733911333"></a><a name="zh-cn_topic_0142797207_p1569733911333"></a>ConsumerRecords&lt;K, V&gt; poll(long var1)</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p136978392331"><a name="zh-cn_topic_0142797207_p136978392331"></a><a name="zh-cn_topic_0142797207_p136978392331"></a>接口</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p7697239143319"><a name="zh-cn_topic_0142797207_p7697239143319"></a><a name="zh-cn_topic_0142797207_p7697239143319"></a>支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p1669753933312"><a name="zh-cn_topic_0142797207_p1669753933312"></a><a name="zh-cn_topic_0142797207_p1669753933312"></a>获取消息，但消息当中未实现</p>
<p id="zh-cn_topic_0142797207_p10697133933315"><a name="zh-cn_topic_0142797207_p10697133933315"></a><a name="zh-cn_topic_0142797207_p10697133933315"></a>checksum(消息的CRC32校验值)、serializedKeySize(key序列化后的字节长度)、serializedValueSize(key序列化后的字节长度)。</p>
</td>
</tr>
<tr id="zh-cn_topic_0142797207_row1299012063019"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p208101918347"><a name="zh-cn_topic_0142797207_p208101918347"></a><a name="zh-cn_topic_0142797207_p208101918347"></a>void commitSync()</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p1381012983412"><a name="zh-cn_topic_0142797207_p1381012983412"></a><a name="zh-cn_topic_0142797207_p1381012983412"></a>接口</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p1081012914341"><a name="zh-cn_topic_0142797207_p1081012914341"></a><a name="zh-cn_topic_0142797207_p1081012914341"></a>支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p168102917348"><a name="zh-cn_topic_0142797207_p168102917348"></a><a name="zh-cn_topic_0142797207_p168102917348"></a>同步提交当前消费的offset</p>
</td>
</tr>
<tr id="zh-cn_topic_0142797207_row97361423333"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p7295617123417"><a name="zh-cn_topic_0142797207_p7295617123417"></a><a name="zh-cn_topic_0142797207_p7295617123417"></a>void commitSync(final Map&lt;TopicPartition, OffsetAndMetadata&gt; offsets)</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p162951217173414"><a name="zh-cn_topic_0142797207_p162951217173414"></a><a name="zh-cn_topic_0142797207_p162951217173414"></a>接口</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p122951517143418"><a name="zh-cn_topic_0142797207_p122951517143418"></a><a name="zh-cn_topic_0142797207_p122951517143418"></a>支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p1829541718341"><a name="zh-cn_topic_0142797207_p1829541718341"></a><a name="zh-cn_topic_0142797207_p1829541718341"></a>同步提交指定的offset</p>
</td>
</tr>
<tr id="zh-cn_topic_0142797207_row276718475333"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p16811266341"><a name="zh-cn_topic_0142797207_p16811266341"></a><a name="zh-cn_topic_0142797207_p16811266341"></a>void commitAsync()</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p56802615341"><a name="zh-cn_topic_0142797207_p56802615341"></a><a name="zh-cn_topic_0142797207_p56802615341"></a>接口</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p1068326193417"><a name="zh-cn_topic_0142797207_p1068326193417"></a><a name="zh-cn_topic_0142797207_p1068326193417"></a>支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p176812663413"><a name="zh-cn_topic_0142797207_p176812663413"></a><a name="zh-cn_topic_0142797207_p176812663413"></a>异步提交当前消费的offset</p>
</td>
</tr>
<tr id="zh-cn_topic_0142797207_row29535015339"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p44641136163418"><a name="zh-cn_topic_0142797207_p44641136163418"></a><a name="zh-cn_topic_0142797207_p44641136163418"></a>public void commitAsync(OffsetCommitCallback callback)</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p0464163615349"><a name="zh-cn_topic_0142797207_p0464163615349"></a><a name="zh-cn_topic_0142797207_p0464163615349"></a>接口</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p18464136103417"><a name="zh-cn_topic_0142797207_p18464136103417"></a><a name="zh-cn_topic_0142797207_p18464136103417"></a>支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p1946473617349"><a name="zh-cn_topic_0142797207_p1946473617349"></a><a name="zh-cn_topic_0142797207_p1946473617349"></a>异步提交当前消费的offset并支持OffsetCommitCallback回调</p>
</td>
</tr>
<tr id="zh-cn_topic_0142797207_row13228852113320"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p1621685663410"><a name="zh-cn_topic_0142797207_p1621685663410"></a><a name="zh-cn_topic_0142797207_p1621685663410"></a>void commitAsync(Map&lt;TopicPartition, OffsetAndMetadata&gt; offsets, OffsetCommitCallback callback)</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p9216195610341"><a name="zh-cn_topic_0142797207_p9216195610341"></a><a name="zh-cn_topic_0142797207_p9216195610341"></a>接口</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p721635623411"><a name="zh-cn_topic_0142797207_p721635623411"></a><a name="zh-cn_topic_0142797207_p721635623411"></a>支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p13216456173411"><a name="zh-cn_topic_0142797207_p13216456173411"></a><a name="zh-cn_topic_0142797207_p13216456173411"></a>异步提交指定的offset并支持OffsetCommitCallback回调</p>
</td>
</tr>
<tr id="zh-cn_topic_0142797207_row12356174720341"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p62601520183510"><a name="zh-cn_topic_0142797207_p62601520183510"></a><a name="zh-cn_topic_0142797207_p62601520183510"></a>void seek(TopicPartition partition, long offset)</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p32601120153510"><a name="zh-cn_topic_0142797207_p32601120153510"></a><a name="zh-cn_topic_0142797207_p32601120153510"></a>接口</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p3260620153517"><a name="zh-cn_topic_0142797207_p3260620153517"></a><a name="zh-cn_topic_0142797207_p3260620153517"></a>支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p1326013201351"><a name="zh-cn_topic_0142797207_p1326013201351"></a><a name="zh-cn_topic_0142797207_p1326013201351"></a>给分区设置指定的offset</p>
</td>
</tr>
<tr id="zh-cn_topic_0142797207_row1151045173418"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p10666430153512"><a name="zh-cn_topic_0142797207_p10666430153512"></a><a name="zh-cn_topic_0142797207_p10666430153512"></a>void seekToBeginning(Collection&lt;TopicPartition&gt; partitions)</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p46661330163513"><a name="zh-cn_topic_0142797207_p46661330163513"></a><a name="zh-cn_topic_0142797207_p46661330163513"></a>接口</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p666683093514"><a name="zh-cn_topic_0142797207_p666683093514"></a><a name="zh-cn_topic_0142797207_p666683093514"></a>支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p1166618301351"><a name="zh-cn_topic_0142797207_p1166618301351"></a><a name="zh-cn_topic_0142797207_p1166618301351"></a>分区的offset设置为最旧的值</p>
</td>
</tr>
<tr id="zh-cn_topic_0142797207_row6309104293414"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p196515586359"><a name="zh-cn_topic_0142797207_p196515586359"></a><a name="zh-cn_topic_0142797207_p196515586359"></a>void seekToEnd(Collection&lt;TopicPartition&gt; partitions)</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p19651858123516"><a name="zh-cn_topic_0142797207_p19651858123516"></a><a name="zh-cn_topic_0142797207_p19651858123516"></a>接口</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p1465358143513"><a name="zh-cn_topic_0142797207_p1465358143513"></a><a name="zh-cn_topic_0142797207_p1465358143513"></a>支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p76555813520"><a name="zh-cn_topic_0142797207_p76555813520"></a><a name="zh-cn_topic_0142797207_p76555813520"></a>分区的offset设置为最新的值</p>
</td>
</tr>
<tr id="zh-cn_topic_0142797207_row1213584943511"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p59211677369"><a name="zh-cn_topic_0142797207_p59211677369"></a><a name="zh-cn_topic_0142797207_p59211677369"></a>long position(TopicPartition partition)</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p692111763611"><a name="zh-cn_topic_0142797207_p692111763611"></a><a name="zh-cn_topic_0142797207_p692111763611"></a>接口</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p492116713615"><a name="zh-cn_topic_0142797207_p492116713615"></a><a name="zh-cn_topic_0142797207_p492116713615"></a>支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p11921172363"><a name="zh-cn_topic_0142797207_p11921172363"></a><a name="zh-cn_topic_0142797207_p11921172363"></a>获取分区当前已消费数据的offset</p>
</td>
</tr>
<tr id="zh-cn_topic_0142797207_row1180613467358"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p690520159365"><a name="zh-cn_topic_0142797207_p690520159365"></a><a name="zh-cn_topic_0142797207_p690520159365"></a>OffsetAndMetadata committed(TopicPartition partition)</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p1790512153369"><a name="zh-cn_topic_0142797207_p1790512153369"></a><a name="zh-cn_topic_0142797207_p1790512153369"></a>接口</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p8905111593612"><a name="zh-cn_topic_0142797207_p8905111593612"></a><a name="zh-cn_topic_0142797207_p8905111593612"></a>支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p11905915183614"><a name="zh-cn_topic_0142797207_p11905915183614"></a><a name="zh-cn_topic_0142797207_p11905915183614"></a>获取分区已提交的offset</p>
</td>
</tr>
<tr id="zh-cn_topic_0142797207_row131811344123515"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p12702202263618"><a name="zh-cn_topic_0142797207_p12702202263618"></a><a name="zh-cn_topic_0142797207_p12702202263618"></a>List&lt;PartitionInfo&gt; partitionsFor(String topic)</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p1570282216369"><a name="zh-cn_topic_0142797207_p1570282216369"></a><a name="zh-cn_topic_0142797207_p1570282216369"></a>接口</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p107021422143613"><a name="zh-cn_topic_0142797207_p107021422143613"></a><a name="zh-cn_topic_0142797207_p107021422143613"></a>支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p1570262211364"><a name="zh-cn_topic_0142797207_p1570262211364"></a><a name="zh-cn_topic_0142797207_p1570262211364"></a>获取通道的分区信息，但PartitionInfo里面的leader, replicas, inSyncReplicas未实现。</p>
</td>
</tr>
<tr id="zh-cn_topic_0142797207_row1833104219358"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p360113323368"><a name="zh-cn_topic_0142797207_p360113323368"></a><a name="zh-cn_topic_0142797207_p360113323368"></a>Map&lt;String, List&lt;PartitionInfo&gt;&gt; listTopics()</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p12601123219368"><a name="zh-cn_topic_0142797207_p12601123219368"></a><a name="zh-cn_topic_0142797207_p12601123219368"></a>接口</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p14601163211362"><a name="zh-cn_topic_0142797207_p14601163211362"></a><a name="zh-cn_topic_0142797207_p14601163211362"></a>支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p66011432143613"><a name="zh-cn_topic_0142797207_p66011432143613"></a><a name="zh-cn_topic_0142797207_p66011432143613"></a>获取所有的通道信息，但PartitionInfo里面的leader, replicas, inSyncReplicas未实现。</p>
</td>
</tr>
<tr id="zh-cn_topic_0142797207_row10869103953518"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p125451140193616"><a name="zh-cn_topic_0142797207_p125451140193616"></a><a name="zh-cn_topic_0142797207_p125451140193616"></a>void pause(Collection&lt;TopicPartition&gt; partitions)</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p15455400366"><a name="zh-cn_topic_0142797207_p15455400366"></a><a name="zh-cn_topic_0142797207_p15455400366"></a>接口</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p354594020368"><a name="zh-cn_topic_0142797207_p354594020368"></a><a name="zh-cn_topic_0142797207_p354594020368"></a>支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p1654544011365"><a name="zh-cn_topic_0142797207_p1654544011365"></a><a name="zh-cn_topic_0142797207_p1654544011365"></a>暂停消费分区</p>
</td>
</tr>
<tr id="zh-cn_topic_0142797207_row136903723513"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p896025683619"><a name="zh-cn_topic_0142797207_p896025683619"></a><a name="zh-cn_topic_0142797207_p896025683619"></a>void resume(Collection&lt;TopicPartition&gt; partitions)</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p39601656103617"><a name="zh-cn_topic_0142797207_p39601656103617"></a><a name="zh-cn_topic_0142797207_p39601656103617"></a>接口</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p1896015683613"><a name="zh-cn_topic_0142797207_p1896015683613"></a><a name="zh-cn_topic_0142797207_p1896015683613"></a>支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p3960185611363"><a name="zh-cn_topic_0142797207_p3960185611363"></a><a name="zh-cn_topic_0142797207_p3960185611363"></a>恢复消费分区</p>
</td>
</tr>
<tr id="zh-cn_topic_0142797207_row43849458330"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p114191411370"><a name="zh-cn_topic_0142797207_p114191411370"></a><a name="zh-cn_topic_0142797207_p114191411370"></a>Set&lt;TopicPartition&gt; paused()</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p154161443714"><a name="zh-cn_topic_0142797207_p154161443714"></a><a name="zh-cn_topic_0142797207_p154161443714"></a>接口</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p1641161420376"><a name="zh-cn_topic_0142797207_p1641161420376"></a><a name="zh-cn_topic_0142797207_p1641161420376"></a>支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p44141443717"><a name="zh-cn_topic_0142797207_p44141443717"></a><a name="zh-cn_topic_0142797207_p44141443717"></a>获取所有已暂停消费的分区</p>
</td>
</tr>
<tr id="zh-cn_topic_0142797207_row27841113713"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p128942143720"><a name="zh-cn_topic_0142797207_p128942143720"></a><a name="zh-cn_topic_0142797207_p128942143720"></a>close()</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p1189112193718"><a name="zh-cn_topic_0142797207_p1189112193718"></a><a name="zh-cn_topic_0142797207_p1189112193718"></a>接口</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p68919215378"><a name="zh-cn_topic_0142797207_p68919215378"></a><a name="zh-cn_topic_0142797207_p68919215378"></a>支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p289132114374"><a name="zh-cn_topic_0142797207_p289132114374"></a><a name="zh-cn_topic_0142797207_p289132114374"></a>关闭consumer</p>
</td>
</tr>
<tr id="zh-cn_topic_0142797207_row3640175913617"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p1472914479379"><a name="zh-cn_topic_0142797207_p1472914479379"></a><a name="zh-cn_topic_0142797207_p1472914479379"></a>Map&lt;MetricName, ? extends Metric&gt; metrics()</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p472944733716"><a name="zh-cn_topic_0142797207_p472944733716"></a><a name="zh-cn_topic_0142797207_p472944733716"></a>接口</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p1772924717372"><a name="zh-cn_topic_0142797207_p1772924717372"></a><a name="zh-cn_topic_0142797207_p1772924717372"></a>不支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p57291547103713"><a name="zh-cn_topic_0142797207_p57291547103713"></a><a name="zh-cn_topic_0142797207_p57291547103713"></a>获取统计信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0142797207_row19948133616370"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p19870125519378"><a name="zh-cn_topic_0142797207_p19870125519378"></a><a name="zh-cn_topic_0142797207_p19870125519378"></a>wakeup()</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p1870205563716"><a name="zh-cn_topic_0142797207_p1870205563716"></a><a name="zh-cn_topic_0142797207_p1870205563716"></a>接口</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p1787085510373"><a name="zh-cn_topic_0142797207_p1787085510373"></a><a name="zh-cn_topic_0142797207_p1787085510373"></a>不支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p68709559373"><a name="zh-cn_topic_0142797207_p68709559373"></a><a name="zh-cn_topic_0142797207_p68709559373"></a>内部实现原理不一样，不需要。</p>
</td>
</tr>
<tr id="zh-cn_topic_0142797207_row7542629123714"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p17429536384"><a name="zh-cn_topic_0142797207_p17429536384"></a><a name="zh-cn_topic_0142797207_p17429536384"></a>group.id</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p2043812343813"><a name="zh-cn_topic_0142797207_p2043812343813"></a><a name="zh-cn_topic_0142797207_p2043812343813"></a>参数</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p194383393816"><a name="zh-cn_topic_0142797207_p194383393816"></a><a name="zh-cn_topic_0142797207_p194383393816"></a>支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p54382333819"><a name="zh-cn_topic_0142797207_p54382333819"></a><a name="zh-cn_topic_0142797207_p54382333819"></a>消费组ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0142797207_row11206152773710"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p11421201193816"><a name="zh-cn_topic_0142797207_p11421201193816"></a><a name="zh-cn_topic_0142797207_p11421201193816"></a>client.id</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p16421121163815"><a name="zh-cn_topic_0142797207_p16421121163815"></a><a name="zh-cn_topic_0142797207_p16421121163815"></a>参数</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p64219115381"><a name="zh-cn_topic_0142797207_p64219115381"></a><a name="zh-cn_topic_0142797207_p64219115381"></a>支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p5421191120387"><a name="zh-cn_topic_0142797207_p5421191120387"></a><a name="zh-cn_topic_0142797207_p5421191120387"></a>每个consumer的client.id必须唯一，如果不配置client.id, dis kafka consumer会生成一个uuid作为client.id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0142797207_row10948172413370"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p14960152913818"><a name="zh-cn_topic_0142797207_p14960152913818"></a><a name="zh-cn_topic_0142797207_p14960152913818"></a>key.deserializer</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p89684295387"><a name="zh-cn_topic_0142797207_p89684295387"></a><a name="zh-cn_topic_0142797207_p89684295387"></a>参数</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p1296802973817"><a name="zh-cn_topic_0142797207_p1296802973817"></a><a name="zh-cn_topic_0142797207_p1296802973817"></a>支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p5968102913386"><a name="zh-cn_topic_0142797207_p5968102913386"></a><a name="zh-cn_topic_0142797207_p5968102913386"></a>含义与kafka设置相同，但默认值为StringDeserializer (kafka必须配置)。</p>
</td>
</tr>
<tr id="zh-cn_topic_0142797207_row3742202113815"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p12421134173812"><a name="zh-cn_topic_0142797207_p12421134173812"></a><a name="zh-cn_topic_0142797207_p12421134173812"></a>value.deserializer</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p1442115414383"><a name="zh-cn_topic_0142797207_p1442115414383"></a><a name="zh-cn_topic_0142797207_p1442115414383"></a>参数</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p13421124113382"><a name="zh-cn_topic_0142797207_p13421124113382"></a><a name="zh-cn_topic_0142797207_p13421124113382"></a>支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p5421641183817"><a name="zh-cn_topic_0142797207_p5421641183817"></a><a name="zh-cn_topic_0142797207_p5421641183817"></a>含义与kafka设置相同，但默认值为StringDeserializer (kafka必须配置)。</p>
</td>
</tr>
<tr id="zh-cn_topic_0142797207_row2359171918385"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p156185112388"><a name="zh-cn_topic_0142797207_p156185112388"></a><a name="zh-cn_topic_0142797207_p156185112388"></a>enable.auto.commit</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p1614510384"><a name="zh-cn_topic_0142797207_p1614510384"></a><a name="zh-cn_topic_0142797207_p1614510384"></a>参数</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p1561851163815"><a name="zh-cn_topic_0142797207_p1561851163815"></a><a name="zh-cn_topic_0142797207_p1561851163815"></a>支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p66175113817"><a name="zh-cn_topic_0142797207_p66175113817"></a><a name="zh-cn_topic_0142797207_p66175113817"></a>同kafka的默认设置，默认为true</p>
<a name="zh-cn_topic_0142797207_ul4160211104819"></a><a name="zh-cn_topic_0142797207_ul4160211104819"></a><ul id="zh-cn_topic_0142797207_ul4160211104819"><li>true表示启用自动提交，每隔${auto.commit.interval.ms}的时间提交一次offset；</li><li>false表示不自动提交offset</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0142797207_row11265121763817"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p196712582380"><a name="zh-cn_topic_0142797207_p196712582380"></a><a name="zh-cn_topic_0142797207_p196712582380"></a>auto.commit.interval.ms</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p86714587383"><a name="zh-cn_topic_0142797207_p86714587383"></a><a name="zh-cn_topic_0142797207_p86714587383"></a>参数</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p136712058193814"><a name="zh-cn_topic_0142797207_p136712058193814"></a><a name="zh-cn_topic_0142797207_p136712058193814"></a>支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p126718587387"><a name="zh-cn_topic_0142797207_p126718587387"></a><a name="zh-cn_topic_0142797207_p126718587387"></a>自动提交offset的周期(毫秒)，默认值5000。</p>
</td>
</tr>
<tr id="zh-cn_topic_0142797207_row6602151413385"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p23311166393"><a name="zh-cn_topic_0142797207_p23311166393"></a><a name="zh-cn_topic_0142797207_p23311166393"></a>auto.offset.reset</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p2033151618391"><a name="zh-cn_topic_0142797207_p2033151618391"></a><a name="zh-cn_topic_0142797207_p2033151618391"></a>参数</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p153311916183910"><a name="zh-cn_topic_0142797207_p153311916183910"></a><a name="zh-cn_topic_0142797207_p153311916183910"></a>支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p033111610392"><a name="zh-cn_topic_0142797207_p033111610392"></a><a name="zh-cn_topic_0142797207_p033111610392"></a>同Kafka的默认配置，默认为latest。</p>
<p id="zh-cn_topic_0142797207_p1033151643917"><a name="zh-cn_topic_0142797207_p1033151643917"></a><a name="zh-cn_topic_0142797207_p1033151643917"></a>此值用于没有初始偏移量或者偏移量不正确的情况下，自动设置offset位置：</p>
<a name="zh-cn_topic_0142797207_ul13561123114485"></a><a name="zh-cn_topic_0142797207_ul13561123114485"></a><ul id="zh-cn_topic_0142797207_ul13561123114485"><li>earliest 将偏移量自动重置为最旧的值;</li><li>latest将偏移量自动重置为最新的值;</li><li>none 如果在消费者组中没有发现前一个偏移量，就向消费者抛出一个异常;</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0142797207_row8175127143914"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0142797207_p20206163818392"><a name="zh-cn_topic_0142797207_p20206163818392"></a><a name="zh-cn_topic_0142797207_p20206163818392"></a>其他参数</p>
</td>
<td class="cellrowborder" valign="top" width="13.370000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0142797207_p020614383397"><a name="zh-cn_topic_0142797207_p020614383397"></a><a name="zh-cn_topic_0142797207_p020614383397"></a>参数</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0142797207_p620616383392"><a name="zh-cn_topic_0142797207_p620616383392"></a><a name="zh-cn_topic_0142797207_p620616383392"></a>不支持</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0142797207_p1420620387395"><a name="zh-cn_topic_0142797207_p1420620387395"></a><a name="zh-cn_topic_0142797207_p1420620387395"></a>-</p>
</td>
</tr>
</tbody>
</table>

