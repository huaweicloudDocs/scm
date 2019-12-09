# API授权项列表<a name="ZH-CN_TOPIC_0183644077"></a>

<a name="table15642105118238"></a>
<table><thead align="left"><tr id="row16642125122310"><th class="cellrowborder" valign="top" width="20.23%" id="mcps1.1.5.1.1"><p id="p48811517242"><a name="p48811517242"></a><a name="p48811517242"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="21.21%" id="mcps1.1.5.1.2"><p id="p988671152417"><a name="p988671152417"></a><a name="p988671152417"></a>授权项</p>
</th>
<th class="cellrowborder" valign="top" width="21.89%" id="mcps1.1.5.1.3"><p id="p1834910910535"><a name="p1834910910535"></a><a name="p1834910910535"></a>授权范围</p>
</th>
<th class="cellrowborder" valign="top" width="36.67%" id="mcps1.1.5.1.4"><p id="p767919205315"><a name="p767919205315"></a><a name="p767919205315"></a>对应API接口</p>
</th>
</tr>
</thead>
<tbody><tr id="row76421513237"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.1.5.1.1 "><p id="p1793833014261"><a name="p1793833014261"></a><a name="p1793833014261"></a>查询证书列表</p>
</td>
<td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.1.5.1.2 "><p id="p196421651202310"><a name="p196421651202310"></a><a name="p196421651202310"></a>scm:cert:list</p>
</td>
<td class="cellrowborder" valign="top" width="21.89%" headers="mcps1.1.5.1.3 "><a name="ul1337941311558"></a><a name="ul1337941311558"></a><ul id="ul1337941311558"><li>支持：<p id="p1837931315550"><a name="p1837931315550"></a><a name="p1837931315550"></a>项目(Project)</p>
</li></ul>
<a name="ul15379413115514"></a><a name="ul15379413115514"></a><ul id="ul15379413115514"><li>不支持：<p id="p537921315559"><a name="p537921315559"></a><a name="p537921315559"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="36.67%" headers="mcps1.1.5.1.4 "><p id="p8311193815241"><a name="p8311193815241"></a><a name="p8311193815241"></a>GET /v2/{project_id}/scm/certlist</p>
</td>
</tr>
<tr id="row202041242184413"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.1.5.1.1 "><p id="p771135654415"><a name="p771135654415"></a><a name="p771135654415"></a>查询证书详情</p>
</td>
<td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.1.5.1.2 "><p id="p1571375619443"><a name="p1571375619443"></a><a name="p1571375619443"></a>scm:cert:get</p>
</td>
<td class="cellrowborder" valign="top" width="21.89%" headers="mcps1.1.5.1.3 "><a name="ul65275411556"></a><a name="ul65275411556"></a><ul id="ul65275411556"><li>支持：<p id="p1352734135517"><a name="p1352734135517"></a><a name="p1352734135517"></a>项目(Project)</p>
</li></ul>
<a name="ul195270411554"></a><a name="ul195270411554"></a><ul id="ul195270411554"><li>不支持：<p id="p3527741175515"><a name="p3527741175515"></a><a name="p3527741175515"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="36.67%" headers="mcps1.1.5.1.4 "><p id="p1570925614412"><a name="p1570925614412"></a><a name="p1570925614412"></a>GET /v2/{project_id}/scm/cert/{cert_id}</p>
</td>
</tr>
<tr id="row71614715444"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.1.5.1.1 "><p id="p1123971194518"><a name="p1123971194518"></a><a name="p1123971194518"></a>查询证书产品类型</p>
</td>
<td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.1.5.1.2 "><p id="p10244416453"><a name="p10244416453"></a><a name="p10244416453"></a>scm:certType:get</p>
</td>
<td class="cellrowborder" valign="top" width="21.89%" headers="mcps1.1.5.1.3 "><a name="ul1574416429553"></a><a name="ul1574416429553"></a><ul id="ul1574416429553"><li>支持：<p id="p9744184212557"><a name="p9744184212557"></a><a name="p9744184212557"></a>项目(Project)</p>
</li></ul>
<a name="ul127441421559"></a><a name="ul127441421559"></a><ul id="ul127441421559"><li>不支持：<p id="p10744142105511"><a name="p10744142105511"></a><a name="p10744142105511"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="36.67%" headers="mcps1.1.5.1.4 "><p id="p82362119452"><a name="p82362119452"></a><a name="p82362119452"></a>GET /v2/{project_id}/scm/cert/product</p>
</td>
</tr>
<tr id="row7285027184511"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.1.5.1.1 "><p id="p79311928174520"><a name="p79311928174520"></a><a name="p79311928174520"></a>查询证书产品详情</p>
</td>
<td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.1.5.1.2 "><p id="p149351128174512"><a name="p149351128174512"></a><a name="p149351128174512"></a>scm:certProduct:get</p>
</td>
<td class="cellrowborder" valign="top" width="21.89%" headers="mcps1.1.5.1.3 "><a name="ul115611744125510"></a><a name="ul115611744125510"></a><ul id="ul115611744125510"><li>支持：<p id="p85611644135515"><a name="p85611644135515"></a><a name="p85611644135515"></a>项目(Project)</p>
</li></ul>
<a name="ul35618442554"></a><a name="ul35618442554"></a><ul id="ul35618442554"><li>不支持：<p id="p155624443553"><a name="p155624443553"></a><a name="p155624443553"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="36.67%" headers="mcps1.1.5.1.4 "><p id="p1925128104513"><a name="p1925128104513"></a><a name="p1925128104513"></a>GET /v2/{project_id}/scm/product/{product_id}</p>
</td>
</tr>
<tr id="row1610754234515"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.1.5.1.1 "><p id="p8807195316454"><a name="p8807195316454"></a><a name="p8807195316454"></a>取消申请</p>
</td>
<td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.1.5.1.2 "><p id="p180905312455"><a name="p180905312455"></a><a name="p180905312455"></a>scm:cert:cancel</p>
</td>
<td class="cellrowborder" valign="top" width="21.89%" headers="mcps1.1.5.1.3 "><a name="ul13863245175512"></a><a name="ul13863245175512"></a><ul id="ul13863245175512"><li>支持：<p id="p186354505515"><a name="p186354505515"></a><a name="p186354505515"></a>项目(Project)</p>
</li></ul>
<a name="ul58631345105513"></a><a name="ul58631345105513"></a><ul id="ul58631345105513"><li>不支持：<p id="p138641245105517"><a name="p138641245105517"></a><a name="p138641245105517"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="36.67%" headers="mcps1.1.5.1.4 "><p id="p68051853124511"><a name="p68051853124511"></a><a name="p68051853124511"></a>POST /v2/{project_id}/scm/cert/{cert_id}/cancel-cert</p>
</td>
</tr>
<tr id="row164225114236"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.1.5.1.1 "><p id="p1393816306264"><a name="p1393816306264"></a><a name="p1393816306264"></a>购买证书</p>
</td>
<td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.1.5.1.2 "><p id="p56421151192319"><a name="p56421151192319"></a><a name="p56421151192319"></a>scm:cert:purchase</p>
</td>
<td class="cellrowborder" valign="top" width="21.89%" headers="mcps1.1.5.1.3 "><a name="ul8348647185510"></a><a name="ul8348647185510"></a><ul id="ul8348647185510"><li>支持：<p id="p15348747185518"><a name="p15348747185518"></a><a name="p15348747185518"></a>项目(Project)</p>
</li></ul>
<a name="ul53481247165520"></a><a name="ul53481247165520"></a><ul id="ul53481247165520"><li>不支持：<p id="p5348154715557"><a name="p5348154715557"></a><a name="p5348154715557"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="36.67%" headers="mcps1.1.5.1.4 "><p id="p20311638142417"><a name="p20311638142417"></a><a name="p20311638142417"></a>POST /v2/{project_id}/scm/cert/purchase</p>
</td>
</tr>
<tr id="row1642185182313"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.1.5.1.1 "><p id="p7938103013265"><a name="p7938103013265"></a><a name="p7938103013265"></a>申请证书</p>
</td>
<td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.1.5.1.2 "><p id="p16643351112317"><a name="p16643351112317"></a><a name="p16643351112317"></a>scm:cert:complete</p>
</td>
<td class="cellrowborder" valign="top" width="21.89%" headers="mcps1.1.5.1.3 "><a name="ul583524835510"></a><a name="ul583524835510"></a><ul id="ul583524835510"><li>支持：<p id="p08351048125516"><a name="p08351048125516"></a><a name="p08351048125516"></a>项目(Project)</p>
</li></ul>
<a name="ul08351048185511"></a><a name="ul08351048185511"></a><ul id="ul08351048185511"><li>不支持：<p id="p10835194825513"><a name="p10835194825513"></a><a name="p10835194825513"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="36.67%" headers="mcps1.1.5.1.4 "><p id="p12311338162411"><a name="p12311338162411"></a><a name="p12311338162411"></a>POST /v2/{project_id}/scm/cert/{cert_id}/complete</p>
</td>
</tr>
<tr id="row7643115116233"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.1.5.1.1 "><p id="p159415300264"><a name="p159415300264"></a><a name="p159415300264"></a>保存申请证书填写的信息</p>
</td>
<td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.1.5.1.2 "><p id="p9643135102314"><a name="p9643135102314"></a><a name="p9643135102314"></a>scm:cert:complete</p>
</td>
<td class="cellrowborder" valign="top" width="21.89%" headers="mcps1.1.5.1.3 "><a name="ul5460195110554"></a><a name="ul5460195110554"></a><ul id="ul5460195110554"><li>支持：<p id="p5460185135518"><a name="p5460185135518"></a><a name="p5460185135518"></a>项目(Project)</p>
</li></ul>
<a name="ul15460205115517"></a><a name="ul15460205115517"></a><ul id="ul15460205115517"><li>不支持：<p id="p154601451125514"><a name="p154601451125514"></a><a name="p154601451125514"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="36.67%" headers="mcps1.1.5.1.4 "><p id="p18312183872413"><a name="p18312183872413"></a><a name="p18312183872413"></a>POST /v2/{project_id}/scm/cert/{cert_id}/save</p>
</td>
</tr>
<tr id="row15643175119238"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.1.5.1.1 "><p id="p5941183014266"><a name="p5941183014266"></a><a name="p5941183014266"></a>读取申请证书填写的信息</p>
</td>
<td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.1.5.1.2 "><p id="p2643151162313"><a name="p2643151162313"></a><a name="p2643151162313"></a>scm:cert:complete</p>
</td>
<td class="cellrowborder" valign="top" width="21.89%" headers="mcps1.1.5.1.3 "><a name="ul3408530553"></a><a name="ul3408530553"></a><ul id="ul3408530553"><li>支持：<p id="p1640453155514"><a name="p1640453155514"></a><a name="p1640453155514"></a>项目(Project)</p>
</li></ul>
<a name="ul1040653115520"></a><a name="ul1040653115520"></a><ul id="ul1040653115520"><li>不支持：<p id="p1641953115518"><a name="p1641953115518"></a><a name="p1641953115518"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="36.67%" headers="mcps1.1.5.1.4 "><p id="p2312238192418"><a name="p2312238192418"></a><a name="p2312238192418"></a>POST /v2/{project_id}/scm/cert/{cert_id}/read</p>
</td>
</tr>
<tr id="row16643551192319"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.1.5.1.1 "><p id="p199419308267"><a name="p199419308267"></a><a name="p199419308267"></a>修改证书</p>
</td>
<td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.1.5.1.2 "><p id="p86431851112319"><a name="p86431851112319"></a><a name="p86431851112319"></a>scm:cert:edit</p>
</td>
<td class="cellrowborder" valign="top" width="21.89%" headers="mcps1.1.5.1.3 "><a name="ul14204125405515"></a><a name="ul14204125405515"></a><ul id="ul14204125405515"><li>支持：<p id="p1820414548558"><a name="p1820414548558"></a><a name="p1820414548558"></a>项目(Project)</p>
</li></ul>
<a name="ul42046549555"></a><a name="ul42046549555"></a><ul id="ul42046549555"><li>不支持：<p id="p2020435414553"><a name="p2020435414553"></a><a name="p2020435414553"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="36.67%" headers="mcps1.1.5.1.4 "><p id="p1331216384249"><a name="p1331216384249"></a><a name="p1331216384249"></a>PUT /v2/{project_id}/scm/cert/{cert_id}</p>
</td>
</tr>
<tr id="row19643351192319"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.1.5.1.1 "><p id="p99413305266"><a name="p99413305266"></a><a name="p99413305266"></a>删除证书</p>
</td>
<td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.1.5.1.2 "><p id="p8766011122914"><a name="p8766011122914"></a><a name="p8766011122914"></a>scm:cert:delete</p>
</td>
<td class="cellrowborder" valign="top" width="21.89%" headers="mcps1.1.5.1.3 "><a name="ul139755552556"></a><a name="ul139755552556"></a><ul id="ul139755552556"><li>支持：<p id="p49751755135510"><a name="p49751755135510"></a><a name="p49751755135510"></a>项目(Project)</p>
</li></ul>
<a name="ul6975125565515"></a><a name="ul6975125565515"></a><ul id="ul6975125565515"><li>不支持：<p id="p1797519551553"><a name="p1797519551553"></a><a name="p1797519551553"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="36.67%" headers="mcps1.1.5.1.4 "><p id="p1312203872419"><a name="p1312203872419"></a><a name="p1312203872419"></a>DELETE /v2/{project_id}/scm/cert/{cert_id}</p>
</td>
</tr>
<tr id="row16434516233"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.1.5.1.1 "><p id="p18941193012263"><a name="p18941193012263"></a><a name="p18941193012263"></a>下载证书</p>
</td>
<td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.1.5.1.2 "><p id="p10766131112298"><a name="p10766131112298"></a><a name="p10766131112298"></a>scm:cert:download</p>
</td>
<td class="cellrowborder" valign="top" width="21.89%" headers="mcps1.1.5.1.3 "><a name="ul13493175710557"></a><a name="ul13493175710557"></a><ul id="ul13493175710557"><li>支持：<p id="p17493145717558"><a name="p17493145717558"></a><a name="p17493145717558"></a>项目(Project)</p>
</li></ul>
<a name="ul84931557145513"></a><a name="ul84931557145513"></a><ul id="ul84931557145513"><li>不支持：<p id="p1549310573553"><a name="p1549310573553"></a><a name="p1549310573553"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="36.67%" headers="mcps1.1.5.1.4 "><p id="p1731283812243"><a name="p1731283812243"></a><a name="p1731283812243"></a>GET /v2/{project_id}/scm/cert/{cert_id}/cert_file</p>
</td>
</tr>
<tr id="row0643115113238"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.1.5.1.1 "><p id="p59411630102619"><a name="p59411630102619"></a><a name="p59411630102619"></a>上传认证信息</p>
</td>
<td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.1.5.1.2 "><p id="p196432051132312"><a name="p196432051132312"></a><a name="p196432051132312"></a>scm:cert:complete</p>
</td>
<td class="cellrowborder" valign="top" width="21.89%" headers="mcps1.1.5.1.3 "><a name="ul49561822566"></a><a name="ul49561822566"></a><ul id="ul49561822566"><li>支持：<p id="p1895762195615"><a name="p1895762195615"></a><a name="p1895762195615"></a>项目(Project)</p>
</li></ul>
<a name="ul895717295615"></a><a name="ul895717295615"></a><ul id="ul895717295615"><li>不支持：<p id="p11957720569"><a name="p11957720569"></a><a name="p11957720569"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="36.67%" headers="mcps1.1.5.1.4 "><p id="p3312038152411"><a name="p3312038152411"></a><a name="p3312038152411"></a>POST /v2/{project_id}/scm/cert/{cert_id}/info/{type}/upload_authentication</p>
</td>
</tr>
<tr id="row36431351142310"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.1.5.1.1 "><p id="p69411930192610"><a name="p69411930192610"></a><a name="p69411930192610"></a>吊销证书</p>
</td>
<td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.1.5.1.2 "><p id="p864475102315"><a name="p864475102315"></a><a name="p864475102315"></a>scm:cert:revoke</p>
</td>
<td class="cellrowborder" valign="top" width="21.89%" headers="mcps1.1.5.1.3 "><a name="ul1212314455616"></a><a name="ul1212314455616"></a><ul id="ul1212314455616"><li>支持：<p id="p16124043568"><a name="p16124043568"></a><a name="p16124043568"></a>项目(Project)</p>
</li></ul>
<a name="ul312417411561"></a><a name="ul312417411561"></a><ul id="ul312417411561"><li>不支持：<p id="p20124164145612"><a name="p20124164145612"></a><a name="p20124164145612"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="36.67%" headers="mcps1.1.5.1.4 "><p id="p031211386247"><a name="p031211386247"></a><a name="p031211386247"></a>POST /v2/{project_id}/scm/cert/{cert_id}/revoke</p>
</td>
</tr>
<tr id="row164465114234"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.1.5.1.1 "><p id="p14619142518118"><a name="p14619142518118"></a><a name="p14619142518118"></a>推送证书</p>
</td>
<td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.1.5.1.2 "><p id="p8644195122315"><a name="p8644195122315"></a><a name="p8644195122315"></a>scm:cert:push</p>
<p id="p5873131231612"><a name="p5873131231612"></a><a name="p5873131231612"></a>推送至CDN时，还需要添加如下授权项：</p>
<p id="p13584195210172"><a name="p13584195210172"></a><a name="p13584195210172"></a>cdn:configuration:queryHttpsConf</p>
</td>
<td class="cellrowborder" valign="top" width="21.89%" headers="mcps1.1.5.1.3 "><a name="ul63301752561"></a><a name="ul63301752561"></a><ul id="ul63301752561"><li>支持：<p id="p183301258562"><a name="p183301258562"></a><a name="p183301258562"></a>项目(Project)</p>
</li></ul>
<a name="ul18330165115619"></a><a name="ul18330165115619"></a><ul id="ul18330165115619"><li>不支持：<p id="p633005125619"><a name="p633005125619"></a><a name="p633005125619"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="36.67%" headers="mcps1.1.5.1.4 "><p id="p1731213818242"><a name="p1731213818242"></a><a name="p1731213818242"></a>POST /v2/{project_id}/scm/cert/{cert_id}/push</p>
</td>
</tr>
<tr id="row1964425192316"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.1.5.1.1 "><p id="p19941193082615"><a name="p19941193082615"></a><a name="p19941193082615"></a>查询推送记录</p>
</td>
<td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.1.5.1.2 "><p id="p56441512239"><a name="p56441512239"></a><a name="p56441512239"></a>scm:pushHistory:list</p>
</td>
<td class="cellrowborder" valign="top" width="21.89%" headers="mcps1.1.5.1.3 "><a name="ul2859162825619"></a><a name="ul2859162825619"></a><ul id="ul2859162825619"><li>支持：<p id="p10859132815612"><a name="p10859132815612"></a><a name="p10859132815612"></a>项目(Project)</p>
</li></ul>
<a name="ul16859172811567"></a><a name="ul16859172811567"></a><ul id="ul16859172811567"><li>不支持：<p id="p685952816567"><a name="p685952816567"></a><a name="p685952816567"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="36.67%" headers="mcps1.1.5.1.4 "><p id="p173121338142411"><a name="p173121338142411"></a><a name="p173121338142411"></a>GET /v2/{project_id}/scm/cert/{cert_id}/push-history</p>
</td>
</tr>
<tr id="row5644145119236"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.1.5.1.1 "><p id="p1194120306265"><a name="p1194120306265"></a><a name="p1194120306265"></a>上传证书</p>
</td>
<td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.1.5.1.2 "><p id="p106441351112313"><a name="p106441351112313"></a><a name="p106441351112313"></a>scm:cert:upload</p>
</td>
<td class="cellrowborder" valign="top" width="21.89%" headers="mcps1.1.5.1.3 "><a name="ul1915017308562"></a><a name="ul1915017308562"></a><ul id="ul1915017308562"><li>支持：<p id="p10151133095611"><a name="p10151133095611"></a><a name="p10151133095611"></a>项目(Project)</p>
</li></ul>
<a name="ul12151330165619"></a><a name="ul12151330165619"></a><ul id="ul12151330165619"><li>不支持：<p id="p815143014564"><a name="p815143014564"></a><a name="p815143014564"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="36.67%" headers="mcps1.1.5.1.4 "><p id="p1531316387246"><a name="p1531316387246"></a><a name="p1531316387246"></a>POST /v2/{project_id}/scm/cert/upload</p>
</td>
</tr>
<tr id="row16644651122313"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.1.5.1.1 "><p id="p694113010268"><a name="p694113010268"></a><a name="p694113010268"></a>校验CSR</p>
</td>
<td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.1.5.1.2 "><p id="p3644105110238"><a name="p3644105110238"></a><a name="p3644105110238"></a>scm:cert:complete</p>
</td>
<td class="cellrowborder" valign="top" width="21.89%" headers="mcps1.1.5.1.3 "><a name="ul2531173155618"></a><a name="ul2531173155618"></a><ul id="ul2531173155618"><li>支持：<p id="p25323311561"><a name="p25323311561"></a><a name="p25323311561"></a>项目(Project)</p>
</li></ul>
<a name="ul11532431185615"></a><a name="ul11532431185615"></a><ul id="ul11532431185615"><li>不支持：<p id="p953213165619"><a name="p953213165619"></a><a name="p953213165619"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="36.67%" headers="mcps1.1.5.1.4 "><p id="p133135387240"><a name="p133135387240"></a><a name="p133135387240"></a>POST /v2/{project_id}/scm/check-csr</p>
</td>
</tr>
<tr id="row364415517239"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.1.5.1.1 "><p id="p1994119304261"><a name="p1994119304261"></a><a name="p1994119304261"></a>新增附加域名</p>
</td>
<td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.1.5.1.2 "><p id="p1644105115232"><a name="p1644105115232"></a><a name="p1644105115232"></a>scm:cert:supplement</p>
</td>
<td class="cellrowborder" valign="top" width="21.89%" headers="mcps1.1.5.1.3 "><a name="ul1623522610563"></a><a name="ul1623522610563"></a><ul id="ul1623522610563"><li>支持：<p id="p2235122635611"><a name="p2235122635611"></a><a name="p2235122635611"></a>项目(Project)</p>
</li></ul>
<a name="ul5235132675618"></a><a name="ul5235132675618"></a><ul id="ul5235132675618"><li>不支持：<p id="p12352262565"><a name="p12352262565"></a><a name="p12352262565"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="36.67%" headers="mcps1.1.5.1.4 "><p id="p7313123815244"><a name="p7313123815244"></a><a name="p7313123815244"></a>POST /v2/{project_id}/scm/cert/{cert_id}/supplement</p>
</td>
</tr>
<tr id="row9644165172313"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.1.5.1.1 "><p id="p494113032610"><a name="p494113032610"></a><a name="p494113032610"></a>取消隐私授权</p>
</td>
<td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.1.5.1.2 "><p id="p9644135182314"><a name="p9644135182314"></a><a name="p9644135182314"></a>scm:privacyProtection:delete</p>
</td>
<td class="cellrowborder" valign="top" width="21.89%" headers="mcps1.1.5.1.3 "><a name="ul17410102518561"></a><a name="ul17410102518561"></a><ul id="ul17410102518561"><li>支持：<p id="p174101925185614"><a name="p174101925185614"></a><a name="p174101925185614"></a>项目(Project)</p>
</li></ul>
<a name="ul1241002512566"></a><a name="ul1241002512566"></a><ul id="ul1241002512566"><li>不支持：<p id="p204111225125611"><a name="p204111225125611"></a><a name="p204111225125611"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="36.67%" headers="mcps1.1.5.1.4 "><p id="p1731318388248"><a name="p1731318388248"></a><a name="p1731318388248"></a>DELETE /v2/{project_id}/scm/privacy-protection/{cert_id}</p>
</td>
</tr>
</tbody>
</table>

