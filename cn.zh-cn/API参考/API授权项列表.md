# API授权项列表<a name="ZH-CN_TOPIC_0183644077"></a>

<a name="table17904541184618"></a>
<table><thead align="left"><tr id="row990434134614"><th class="cellrowborder" valign="top" width="15.58%" id="mcps1.1.7.1.1"><p id="p12905341114619"><a name="p12905341114619"></a><a name="p12905341114619"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="34.42%" id="mcps1.1.7.1.2"><p id="p53051820144715"><a name="p53051820144715"></a><a name="p53051820144715"></a>对应API接口</p>
</th>
<th class="cellrowborder" valign="top" width="16%" id="mcps1.1.7.1.3"><p id="p390510419461"><a name="p390510419461"></a><a name="p390510419461"></a>授权项（Action）</p>
</th>
<th class="cellrowborder" valign="top" width="16%" id="mcps1.1.7.1.4"><p id="p16559185513472"><a name="p16559185513472"></a><a name="p16559185513472"></a>依赖的授权项</p>
</th>
<th class="cellrowborder" valign="top" width="9%" id="mcps1.1.7.1.5"><p id="p18181050174813"><a name="p18181050174813"></a><a name="p18181050174813"></a>IAM项目</p>
<p id="p1018265014811"><a name="p1018265014811"></a><a name="p1018265014811"></a>(Project)</p>
</th>
<th class="cellrowborder" valign="top" width="9%" id="mcps1.1.7.1.6"><p id="p8748195614484"><a name="p8748195614484"></a><a name="p8748195614484"></a>企业项目</p>
<p id="p127481256174817"><a name="p127481256174817"></a><a name="p127481256174817"></a>(Enterprise Project)</p>
</th>
</tr>
</thead>
<tbody><tr id="row17905941134613"><td class="cellrowborder" valign="top" width="15.58%" headers="mcps1.1.7.1.1 "><p id="p5905441114612"><a name="p5905441114612"></a><a name="p5905441114612"></a>查询证书列表</p>
</td>
<td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.1.7.1.2 "><p id="p1130562044714"><a name="p1130562044714"></a><a name="p1130562044714"></a>GET /v2/{project_id}/scm/certlist</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.3 "><p id="p3905134114465"><a name="p3905134114465"></a><a name="p3905134114465"></a>scm:cert:list</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.4 "><p id="p1255916554474"><a name="p1255916554474"></a><a name="p1255916554474"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.5 "><p id="p11546132134813"><a name="p11546132134813"></a><a name="p11546132134813"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.6 "><p id="p36331236204818"><a name="p36331236204818"></a><a name="p36331236204818"></a>x</p>
</td>
</tr>
<tr id="row3905174184615"><td class="cellrowborder" valign="top" width="15.58%" headers="mcps1.1.7.1.1 "><p id="p2905184117466"><a name="p2905184117466"></a><a name="p2905184117466"></a>查询证书详情</p>
</td>
<td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.1.7.1.2 "><p id="p16305162044713"><a name="p16305162044713"></a><a name="p16305162044713"></a>GET /v2/{project_id}/scm/cert/{cert_id}</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.3 "><p id="p15905341164617"><a name="p15905341164617"></a><a name="p15905341164617"></a>scm:cert:get</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.4 "><p id="p1955915552473"><a name="p1955915552473"></a><a name="p1955915552473"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.5 "><p id="p434118593490"><a name="p434118593490"></a><a name="p434118593490"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.6 "><p id="p33429594494"><a name="p33429594494"></a><a name="p33429594494"></a>x</p>
</td>
</tr>
<tr id="row79063419461"><td class="cellrowborder" valign="top" width="15.58%" headers="mcps1.1.7.1.1 "><p id="p290644119467"><a name="p290644119467"></a><a name="p290644119467"></a>查询证书产品类型</p>
</td>
<td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.1.7.1.2 "><p id="p530642044711"><a name="p530642044711"></a><a name="p530642044711"></a>GET /v2/{project_id}/scm/cert/product</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.3 "><p id="p890684120462"><a name="p890684120462"></a><a name="p890684120462"></a>scm:certType:get</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.4 "><p id="p355925516476"><a name="p355925516476"></a><a name="p355925516476"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.5 "><p id="p16975218507"><a name="p16975218507"></a><a name="p16975218507"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.6 "><p id="p1269810217504"><a name="p1269810217504"></a><a name="p1269810217504"></a>x</p>
</td>
</tr>
<tr id="row9906174194619"><td class="cellrowborder" valign="top" width="15.58%" headers="mcps1.1.7.1.1 "><p id="p109061841104613"><a name="p109061841104613"></a><a name="p109061841104613"></a>查询证书产品详情</p>
</td>
<td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.1.7.1.2 "><p id="p133068206474"><a name="p133068206474"></a><a name="p133068206474"></a>GET /v2/{project_id}/scm/product/{product_id}</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.3 "><p id="p9907144114463"><a name="p9907144114463"></a><a name="p9907144114463"></a>scm:certProduct:get</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.4 "><p id="p175595559479"><a name="p175595559479"></a><a name="p175595559479"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.5 "><p id="p153769615013"><a name="p153769615013"></a><a name="p153769615013"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.6 "><p id="p1137611625012"><a name="p1137611625012"></a><a name="p1137611625012"></a>x</p>
</td>
</tr>
<tr id="row9907114118466"><td class="cellrowborder" valign="top" width="15.58%" headers="mcps1.1.7.1.1 "><p id="p0907144174610"><a name="p0907144174610"></a><a name="p0907144174610"></a>取消申请</p>
</td>
<td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.1.7.1.2 "><p id="p133061120124717"><a name="p133061120124717"></a><a name="p133061120124717"></a>POST /v2/{project_id}/scm/cert/{cert_id}/cancel-cert</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.3 "><p id="p17907204112464"><a name="p17907204112464"></a><a name="p17907204112464"></a>scm:cert:cancel</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.4 "><p id="p1155955515478"><a name="p1155955515478"></a><a name="p1155955515478"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.5 "><p id="p14240111120504"><a name="p14240111120504"></a><a name="p14240111120504"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.6 "><p id="p10241171135019"><a name="p10241171135019"></a><a name="p10241171135019"></a>x</p>
</td>
</tr>
<tr id="row19151341114619"><td class="cellrowborder" valign="top" width="15.58%" headers="mcps1.1.7.1.1 "><p id="p10915104114616"><a name="p10915104114616"></a><a name="p10915104114616"></a>购买证书</p>
</td>
<td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.1.7.1.2 "><p id="p630632019471"><a name="p630632019471"></a><a name="p630632019471"></a>POST /v2/{project_id}/scm/cert/purchase</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.3 "><p id="p18915184113469"><a name="p18915184113469"></a><a name="p18915184113469"></a>scm:cert:purchase</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.4 "><p id="p9559055204716"><a name="p9559055204716"></a><a name="p9559055204716"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.5 "><p id="p17564111619504"><a name="p17564111619504"></a><a name="p17564111619504"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.6 "><p id="p20565181615017"><a name="p20565181615017"></a><a name="p20565181615017"></a>x</p>
</td>
</tr>
<tr id="row1291624113462"><td class="cellrowborder" valign="top" width="15.58%" headers="mcps1.1.7.1.1 "><p id="p991624119461"><a name="p991624119461"></a><a name="p991624119461"></a>申请证书</p>
</td>
<td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.1.7.1.2 "><p id="p153063202477"><a name="p153063202477"></a><a name="p153063202477"></a>POST /v2/{project_id}/scm/cert/{cert_id}/complete</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.3 "><p id="p1791724111469"><a name="p1791724111469"></a><a name="p1791724111469"></a>scm:cert:complete</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.4 "><p id="p255913558479"><a name="p255913558479"></a><a name="p255913558479"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.5 "><p id="p1657441865012"><a name="p1657441865012"></a><a name="p1657441865012"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.6 "><p id="p145741218145012"><a name="p145741218145012"></a><a name="p145741218145012"></a>x</p>
</td>
</tr>
<tr id="row79178411460"><td class="cellrowborder" valign="top" width="15.58%" headers="mcps1.1.7.1.1 "><p id="p13917241174616"><a name="p13917241174616"></a><a name="p13917241174616"></a>保存申请证书填写的信息</p>
</td>
<td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.1.7.1.2 "><p id="p530610208474"><a name="p530610208474"></a><a name="p530610208474"></a>POST /v2/{project_id}/scm/cert/{cert_id}/save</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.3 "><p id="p129171241174612"><a name="p129171241174612"></a><a name="p129171241174612"></a>scm:cert:complete</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.4 "><p id="p855917558470"><a name="p855917558470"></a><a name="p855917558470"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.5 "><p id="p10497132075018"><a name="p10497132075018"></a><a name="p10497132075018"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.6 "><p id="p18497132017502"><a name="p18497132017502"></a><a name="p18497132017502"></a>x</p>
</td>
</tr>
<tr id="row13917194112465"><td class="cellrowborder" valign="top" width="15.58%" headers="mcps1.1.7.1.1 "><p id="p9917341194614"><a name="p9917341194614"></a><a name="p9917341194614"></a>读取申请证书填写的信息</p>
</td>
<td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.1.7.1.2 "><p id="p5306132015476"><a name="p5306132015476"></a><a name="p5306132015476"></a>POST /v2/{project_id}/scm/cert/{cert_id}/read</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.3 "><p id="p2917164154616"><a name="p2917164154616"></a><a name="p2917164154616"></a>scm:cert:complete</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.4 "><p id="p19560145524713"><a name="p19560145524713"></a><a name="p19560145524713"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.5 "><p id="p15312422175020"><a name="p15312422175020"></a><a name="p15312422175020"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.6 "><p id="p331212212506"><a name="p331212212506"></a><a name="p331212212506"></a>x</p>
</td>
</tr>
<tr id="row1791824111468"><td class="cellrowborder" valign="top" width="15.58%" headers="mcps1.1.7.1.1 "><p id="p109180411462"><a name="p109180411462"></a><a name="p109180411462"></a>修改证书</p>
</td>
<td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.1.7.1.2 "><p id="p2307202034713"><a name="p2307202034713"></a><a name="p2307202034713"></a>PUT /v2/{project_id}/scm/cert/{cert_id}</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.3 "><p id="p15918141114616"><a name="p15918141114616"></a><a name="p15918141114616"></a>scm:cert:edit</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.4 "><p id="p17560255104717"><a name="p17560255104717"></a><a name="p17560255104717"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.5 "><p id="p146816240503"><a name="p146816240503"></a><a name="p146816240503"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.6 "><p id="p1468152495017"><a name="p1468152495017"></a><a name="p1468152495017"></a>x</p>
</td>
</tr>
<tr id="row19191241104617"><td class="cellrowborder" valign="top" width="15.58%" headers="mcps1.1.7.1.1 "><p id="p6919194118461"><a name="p6919194118461"></a><a name="p6919194118461"></a>删除证书</p>
</td>
<td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.1.7.1.2 "><p id="p6307182074710"><a name="p6307182074710"></a><a name="p6307182074710"></a>DELETE /v2/{project_id}/scm/cert/{cert_id}</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.3 "><p id="p9919194117467"><a name="p9919194117467"></a><a name="p9919194117467"></a>scm:cert:delete</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.4 "><p id="p145601455184711"><a name="p145601455184711"></a><a name="p145601455184711"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.5 "><p id="p0461278508"><a name="p0461278508"></a><a name="p0461278508"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.6 "><p id="p13467275506"><a name="p13467275506"></a><a name="p13467275506"></a>x</p>
</td>
</tr>
<tr id="row4919184114618"><td class="cellrowborder" valign="top" width="15.58%" headers="mcps1.1.7.1.1 "><p id="p139198419461"><a name="p139198419461"></a><a name="p139198419461"></a>下载证书</p>
</td>
<td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.1.7.1.2 "><p id="p11307220194719"><a name="p11307220194719"></a><a name="p11307220194719"></a>GET /v2/{project_id}/scm/cert/{cert_id}/cert_file</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.3 "><p id="p79196411468"><a name="p79196411468"></a><a name="p79196411468"></a>scm:cert:download</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.4 "><p id="p856095524711"><a name="p856095524711"></a><a name="p856095524711"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.5 "><p id="p19941928115018"><a name="p19941928115018"></a><a name="p19941928115018"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.6 "><p id="p15994152815016"><a name="p15994152815016"></a><a name="p15994152815016"></a>x</p>
</td>
</tr>
<tr id="row19201841174620"><td class="cellrowborder" valign="top" width="15.58%" headers="mcps1.1.7.1.1 "><p id="p1492004117461"><a name="p1492004117461"></a><a name="p1492004117461"></a>上传认证信息</p>
</td>
<td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.1.7.1.2 "><p id="p830718203473"><a name="p830718203473"></a><a name="p830718203473"></a>POST /v2/{project_id}/scm/cert/{cert_id}/info/{type}/upload_authentication</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.3 "><p id="p17920141124619"><a name="p17920141124619"></a><a name="p17920141124619"></a>scm:cert:complete</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.4 "><p id="p18560145512473"><a name="p18560145512473"></a><a name="p18560145512473"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.5 "><p id="p1927503117501"><a name="p1927503117501"></a><a name="p1927503117501"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.6 "><p id="p12751131165012"><a name="p12751131165012"></a><a name="p12751131165012"></a>x</p>
</td>
</tr>
<tr id="row1792010411466"><td class="cellrowborder" valign="top" width="15.58%" headers="mcps1.1.7.1.1 "><p id="p7920174114465"><a name="p7920174114465"></a><a name="p7920174114465"></a>吊销证书</p>
</td>
<td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.1.7.1.2 "><p id="p23071420104718"><a name="p23071420104718"></a><a name="p23071420104718"></a>POST /v2/{project_id}/scm/cert/{cert_id}/revoke</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.3 "><p id="p149203418462"><a name="p149203418462"></a><a name="p149203418462"></a>scm:cert:revoke</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.4 "><p id="p115607558479"><a name="p115607558479"></a><a name="p115607558479"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.5 "><p id="p226217334502"><a name="p226217334502"></a><a name="p226217334502"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.6 "><p id="p132627332502"><a name="p132627332502"></a><a name="p132627332502"></a>x</p>
</td>
</tr>
<tr id="row169218412468"><td class="cellrowborder" valign="top" width="15.58%" headers="mcps1.1.7.1.1 "><p id="p14921154114619"><a name="p14921154114619"></a><a name="p14921154114619"></a>推送证书</p>
</td>
<td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.1.7.1.2 "><p id="p113071120124718"><a name="p113071120124718"></a><a name="p113071120124718"></a>POST /v2/{project_id}/scm/cert/{cert_id}/push</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.3 "><p id="p69211241204614"><a name="p69211241204614"></a><a name="p69211241204614"></a>scm:cert:push</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.4 "><p id="p192118411461"><a name="p192118411461"></a><a name="p192118411461"></a>推送至CDN时，还需要添加如下授权项：</p>
<p id="p13921441154616"><a name="p13921441154616"></a><a name="p13921441154616"></a>cdn:configuration:queryHttpsConf</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.5 "><p id="p79706347506"><a name="p79706347506"></a><a name="p79706347506"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.6 "><p id="p109701034145012"><a name="p109701034145012"></a><a name="p109701034145012"></a>x</p>
</td>
</tr>
<tr id="row13922164104611"><td class="cellrowborder" valign="top" width="15.58%" headers="mcps1.1.7.1.1 "><p id="p1992274134611"><a name="p1992274134611"></a><a name="p1992274134611"></a>查询推送记录</p>
</td>
<td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.1.7.1.2 "><p id="p19307152014476"><a name="p19307152014476"></a><a name="p19307152014476"></a>GET /v2/{project_id}/scm/cert/{cert_id}/push-history</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.3 "><p id="p19221141204618"><a name="p19221141204618"></a><a name="p19221141204618"></a>scm:pushHistory:list</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.4 "><p id="p856085514718"><a name="p856085514718"></a><a name="p856085514718"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.5 "><p id="p111331337165020"><a name="p111331337165020"></a><a name="p111331337165020"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.6 "><p id="p41349370500"><a name="p41349370500"></a><a name="p41349370500"></a>x</p>
</td>
</tr>
<tr id="row1592254144611"><td class="cellrowborder" valign="top" width="15.58%" headers="mcps1.1.7.1.1 "><p id="p5922184120466"><a name="p5922184120466"></a><a name="p5922184120466"></a>上传证书</p>
</td>
<td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.1.7.1.2 "><p id="p5307420194712"><a name="p5307420194712"></a><a name="p5307420194712"></a>POST /v2/{project_id}/scm/cert/upload</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.3 "><p id="p139221141174612"><a name="p139221141174612"></a><a name="p139221141174612"></a>scm:cert:upload</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.4 "><p id="p256015554710"><a name="p256015554710"></a><a name="p256015554710"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.5 "><p id="p37861438195014"><a name="p37861438195014"></a><a name="p37861438195014"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.6 "><p id="p07861438105019"><a name="p07861438105019"></a><a name="p07861438105019"></a>x</p>
</td>
</tr>
<tr id="row892344114616"><td class="cellrowborder" valign="top" width="15.58%" headers="mcps1.1.7.1.1 "><p id="p18923114117461"><a name="p18923114117461"></a><a name="p18923114117461"></a>校验CSR</p>
</td>
<td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.1.7.1.2 "><p id="p1230812207479"><a name="p1230812207479"></a><a name="p1230812207479"></a>POST /v2/{project_id}/scm/check-csr</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.3 "><p id="p192354154613"><a name="p192354154613"></a><a name="p192354154613"></a>scm:cert:complete</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.4 "><p id="p125601355204713"><a name="p125601355204713"></a><a name="p125601355204713"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.5 "><p id="p177331440105014"><a name="p177331440105014"></a><a name="p177331440105014"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.6 "><p id="p67331040195012"><a name="p67331040195012"></a><a name="p67331040195012"></a>x</p>
</td>
</tr>
<tr id="row1923641184615"><td class="cellrowborder" valign="top" width="15.58%" headers="mcps1.1.7.1.1 "><p id="p2924141194617"><a name="p2924141194617"></a><a name="p2924141194617"></a>新增附加域名</p>
</td>
<td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.1.7.1.2 "><p id="p6308620104717"><a name="p6308620104717"></a><a name="p6308620104717"></a>POST /v2/{project_id}/scm/cert/{cert_id}/supplement</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.3 "><p id="p192417412466"><a name="p192417412466"></a><a name="p192417412466"></a>scm:cert:supplement</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.4 "><p id="p9560115510478"><a name="p9560115510478"></a><a name="p9560115510478"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.5 "><p id="p31861542135015"><a name="p31861542135015"></a><a name="p31861542135015"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.6 "><p id="p718694220502"><a name="p718694220502"></a><a name="p718694220502"></a>x</p>
</td>
</tr>
<tr id="row79252411465"><td class="cellrowborder" valign="top" width="15.58%" headers="mcps1.1.7.1.1 "><p id="p592564134616"><a name="p592564134616"></a><a name="p592564134616"></a>取消隐私授权</p>
</td>
<td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.1.7.1.2 "><p id="p730812205474"><a name="p730812205474"></a><a name="p730812205474"></a>DELETE /v2/{project_id}/scm/privacy-protection/{cert_id}</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.3 "><p id="p15925134117466"><a name="p15925134117466"></a><a name="p15925134117466"></a>scm:privacyProtection:delete</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.7.1.4 "><p id="p1256085574716"><a name="p1256085574716"></a><a name="p1256085574716"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.5 "><p id="p399414314506"><a name="p399414314506"></a><a name="p399414314506"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.1.7.1.6 "><p id="p17994144317500"><a name="p17994144317500"></a><a name="p17994144317500"></a>x</p>
</td>
</tr>
</tbody>
</table>

