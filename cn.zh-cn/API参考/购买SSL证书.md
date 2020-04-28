# 购买SSL证书<a name="ZH-CN_TOPIC_0182547690"></a>

## 功能介绍<a name="s1731a14fb0144c79bf0fa90c694f34f7"></a>

购买SSL证书。

>![](public_sys-resources/icon-note.gif) **说明：**   
>请求参数“agree\_privacy\_protection“必须设置为“true“，才能成功提交购买证书申请。  

## URI<a name="se70c3e5518a04f60b06032524dddfef4"></a>

-   URI格式

    POST /v2/\{project\_id\}/scm/cert/purchase

-   参数说明

    <a name="t982da1e0196d4ec1a28d1fbff2cc8191"></a>
    <table><thead align="left"><tr id="r6e963322c1e740d181726d2f0e91df5a"><th class="cellrowborder" valign="top" width="20%" id="mcps1.1.5.1.1"><p id="a3b5bbe5a7f644fd3a74cecbfb3f7ed60"><a name="a3b5bbe5a7f644fd3a74cecbfb3f7ed60"></a><a name="a3b5bbe5a7f644fd3a74cecbfb3f7ed60"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="20%" id="mcps1.1.5.1.2"><p id="p478785352411"><a name="p478785352411"></a><a name="p478785352411"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="20%" id="mcps1.1.5.1.3"><p id="p698810431245"><a name="p698810431245"></a><a name="p698810431245"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="40%" id="mcps1.1.5.1.4"><p id="a6bb6f1fe56a2454982832e8d56d354d8"><a name="a6bb6f1fe56a2454982832e8d56d354d8"></a><a name="a6bb6f1fe56a2454982832e8d56d354d8"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="r69bf37b65d3f446eab7b3f4d1b2fcec0"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.1 "><p id="ae42d73592f58424ea93a11e52d2478dd"><a name="ae42d73592f58424ea93a11e52d2478dd"></a><a name="ae42d73592f58424ea93a11e52d2478dd"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p47871953182417"><a name="p47871953182417"></a><a name="p47871953182417"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p2989184311241"><a name="p2989184311241"></a><a name="p2989184311241"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.5.1.4 "><p id="a1314869d2dc147b38461e037d622f7b4"><a name="a1314869d2dc147b38461e037d622f7b4"></a><a name="a1314869d2dc147b38461e037d622f7b4"></a>项目ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="seb7b7901701247fab30a59b76f1c7f93"></a>

请求参数

<a name="table46221022101230"></a>
<table><thead align="left"><tr id="row9315574101230"><th class="cellrowborder" valign="top" width="20%" id="mcps1.1.5.1.1"><p id="p16364058101230"><a name="p16364058101230"></a><a name="p16364058101230"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.1.5.1.2"><p id="p57514295101230"><a name="p57514295101230"></a><a name="p57514295101230"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.1.5.1.3"><p id="p50420322101230"><a name="p50420322101230"></a><a name="p50420322101230"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.1.5.1.4"><p id="p28146304101230"><a name="p28146304101230"></a><a name="p28146304101230"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row65258150101230"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.1 "><p id="p652324423817"><a name="p652324423817"></a><a name="p652324423817"></a>cert_brand</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p1052317449382"><a name="p1052317449382"></a><a name="p1052317449382"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p557810495386"><a name="p557810495386"></a><a name="p557810495386"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.5.1.4 "><p id="p052314419383"><a name="p052314419383"></a><a name="p052314419383"></a>证书品牌。</p>
<p id="p165237446381"><a name="p165237446381"></a><a name="p165237446381"></a>如：GLOBALSIGN</p>
</td>
</tr>
<tr id="row2245699720624"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.1 "><p id="p1952310448382"><a name="p1952310448382"></a><a name="p1952310448382"></a>cert_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p14850192913404"><a name="p14850192913404"></a><a name="p14850192913404"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p2578115203813"><a name="p2578115203813"></a><a name="p2578115203813"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.5.1.4 "><p id="p168361850143915"><a name="p168361850143915"></a><a name="p168361850143915"></a>证书类型，取值如下：</p>
<a name="ul18803152212387"></a><a name="ul18803152212387"></a><ul id="ul18803152212387"><li>OV_SSL_CERT：企业型SSL证书。</li><li>EV_SSL_CERT：增强型SSL证书。</li></ul>
</td>
</tr>
<tr id="row56396726142438"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.1 "><p id="p1952484418388"><a name="p1952484418388"></a><a name="p1952484418388"></a>domain_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p19793133118401"><a name="p19793133118401"></a><a name="p19793133118401"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p13132105515386"><a name="p13132105515386"></a><a name="p13132105515386"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.5.1.4 "><p id="p1524134463814"><a name="p1524134463814"></a><a name="p1524134463814"></a>域名类型，取值如下：</p>
<a name="ul1396204812395"></a><a name="ul1396204812395"></a><ul id="ul1396204812395"><li>SINGLE_DOMAIN：单域名类型。</li><li>MULTI_DOMAIN：多域名类型。</li><li>WILDCARD：泛域名类型。</li></ul>
</td>
</tr>
<tr id="row35142504101726"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.1 "><p id="p1452424412385"><a name="p1452424412385"></a><a name="p1452424412385"></a>effective_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p7524184413384"><a name="p7524184413384"></a><a name="p7524184413384"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p125001117113919"><a name="p125001117113919"></a><a name="p125001117113919"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.5.1.4 "><p id="p11524104419386"><a name="p11524104419386"></a><a name="p11524104419386"></a>证书有效期（年），取值如下：</p>
<a name="ul9783191534215"></a><a name="ul9783191534215"></a><ul id="ul9783191534215"><li>1：购买有效期为1年的证书。</li><li>2：购买有效期为2年的证书。</li></ul>
</td>
</tr>
<tr id="row138451589499"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.1 "><p id="p384511818498"><a name="p384511818498"></a><a name="p384511818498"></a>domain_numbers</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p384515864919"><a name="p384515864919"></a><a name="p384515864919"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p17845118134914"><a name="p17845118134914"></a><a name="p17845118134914"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.5.1.4 "><p id="p1845108194919"><a name="p1845108194919"></a><a name="p1845108194919"></a>域名数量。</p>
<a name="ul1691485334214"></a><a name="ul1691485334214"></a><ul id="ul1691485334214"><li>当<span class="parmvalue" id="parmvalue1576113974511"><a name="parmvalue1576113974511"></a><a name="parmvalue1576113974511"></a>“domain_type”</span>选择的是<span class="parmvalue" id="parmvalue093141674519"><a name="parmvalue093141674519"></a><a name="parmvalue093141674519"></a>“SINGLE_DOMAIN”</span>或<span class="parmvalue" id="parmvalue51001421124520"><a name="parmvalue51001421124520"></a><a name="parmvalue51001421124520"></a>“WILDCARD”</span>类型的证书时，域名数量取值为<span class="parmvalue" id="parmvalue1983113324497"><a name="parmvalue1983113324497"></a><a name="parmvalue1983113324497"></a>“1”</span>。</li><li>当<span class="parmvalue" id="parmvalue6923191394513"><a name="parmvalue6923191394513"></a><a name="parmvalue6923191394513"></a>“domain_type”</span>选择的是<span class="parmvalue" id="parmvalue814912416458"><a name="parmvalue814912416458"></a><a name="parmvalue814912416458"></a>“MULTI_DOMAIN”</span>类型的证书是，域名数量取值范围为<span class="parmvalue" id="parmvalue114626363490"><a name="parmvalue114626363490"></a><a name="parmvalue114626363490"></a>“2~100”</span>。</li></ul>
</td>
</tr>
<tr id="row755496164919"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.1 "><p id="p13524444163819"><a name="p13524444163819"></a><a name="p13524444163819"></a>order_number</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p2554146164911"><a name="p2554146164911"></a><a name="p2554146164911"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p185549664919"><a name="p185549664919"></a><a name="p185549664919"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.5.1.4 "><p id="p13941173554912"><a name="p13941173554912"></a><a name="p13941173554912"></a>购买的证书数量。取值范围为1~1000。</p>
</td>
</tr>
<tr id="row19652143174912"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.1 "><p id="p4652332490"><a name="p4652332490"></a><a name="p4652332490"></a>agree_privacy_protection</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p126521835495"><a name="p126521835495"></a><a name="p126521835495"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p1029911284498"><a name="p1029911284498"></a><a name="p1029911284498"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.5.1.4 "><p id="p791011372496"><a name="p791011372496"></a><a name="p791011372496"></a>是否同意隐私协议。</p>
<a name="ul12414554234"></a><a name="ul12414554234"></a><ul id="ul12414554234"><li>true：同意隐私协议。</li><li>false：不同意隐私协议。</li></ul>
<p id="p16999143163216"><a name="p16999143163216"></a><a name="p16999143163216"></a>此处仅能设置为true才能成功购买证书。</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="sfadd53a5f4714e8f87811818d62d0296"></a>

响应参数

<a name="t98d238e10953421e84a073707024c329"></a>
<table><thead align="left"><tr id="r144a2c52c5054c6d9243eb2ef3875a21"><th class="cellrowborder" valign="top" width="20%" id="mcps1.1.5.1.1"><p id="a9156e0b03f054d4e8547e0787f88a51b"><a name="a9156e0b03f054d4e8547e0787f88a51b"></a><a name="a9156e0b03f054d4e8547e0787f88a51b"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.1.5.1.2"><p id="a39360acf5daf4c01a1ebddeff5d68a1c"><a name="a39360acf5daf4c01a1ebddeff5d68a1c"></a><a name="a39360acf5daf4c01a1ebddeff5d68a1c"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.1.5.1.3"><p id="p1364012288483"><a name="p1364012288483"></a><a name="p1364012288483"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.1.5.1.4"><p id="a0097000016b14857972b7929bcaaa038"><a name="a0097000016b14857972b7929bcaaa038"></a><a name="a0097000016b14857972b7929bcaaa038"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="r3c4af7b36e9240d197ab56255e37b83c"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.1 "><p id="p5718161011500"><a name="p5718161011500"></a><a name="p5718161011500"></a>order_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p7713193415920"><a name="p7713193415920"></a><a name="p7713193415920"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p133020292093"><a name="p133020292093"></a><a name="p133020292093"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.5.1.4 "><p id="p33891398102713"><a name="p33891398102713"></a><a name="p33891398102713"></a>订单号。</p>
</td>
</tr>
<tr id="rf212a916c502452a8e151eba2f118272"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.1 "><p id="p0602131418506"><a name="p0602131418506"></a><a name="p0602131418506"></a>cert</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p972910369912"><a name="p972910369912"></a><a name="p972910369912"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p130162913913"><a name="p130162913913"></a><a name="p130162913913"></a>Array of cert objects</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.5.1.4 "><p id="p79539366500"><a name="p79539366500"></a><a name="p79539366500"></a>证书列表，详情请参见<a href="#table197767634419">表1</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 1**  cert

<a name="table197767634419"></a>
<table><thead align="left"><tr id="row13776668449"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p1481771118446"><a name="p1481771118446"></a><a name="p1481771118446"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p1067011516913"><a name="p1067011516913"></a><a name="p1067011516913"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p481731114419"><a name="p481731114419"></a><a name="p481731114419"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p4818111134417"><a name="p4818111134417"></a><a name="p4818111134417"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row157769694412"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p11818121120442"><a name="p11818121120442"></a><a name="p11818121120442"></a>cert_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p174518481991"><a name="p174518481991"></a><a name="p174518481991"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p10818911154410"><a name="p10818911154410"></a><a name="p10818911154410"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p158184118444"><a name="p158184118444"></a><a name="p158184118444"></a>证书ID。</p>
</td>
</tr>
</tbody>
</table>

## 示例<a name="section1079019295212"></a>

如下以购买1张品牌为Globalsign，域名类型为多域名，域名数量为5，有效期为1年的OV证书为例。

-   请求样例

    ```
    { 
     "cert_brand":"GLOBALSIGN", 
     "cert_type":"OV_SSL_CERT ", 
     "domain_type":"MULTI_DOMAIN", 
     "effective_time": 1, 
     "domain_numbers": 5, 
     "order_number": 1, 
     "agree_privacy_protection":true 
     }
    ```

-   响应样例

    ```
    {  
    "order_id": "CS1803192259ROA8U" 
    "cert": [{ 
             "cert_id": "scs1481110651012", 
           }] 
    }
    ```

    或

    ```
    { 
       "error_code": "SCM.XXXX",  
       "error_msg": "XXXX"   
     }
    ```


## 状态码<a name="s811d1a98cd5242509abd6671a9959d55"></a>

[表2](#zh-cn_topic_0079615001_table20596071)描述的是API返回的正常状态码。

**表 2**  状态码

<a name="zh-cn_topic_0079615001_table20596071"></a>
<table><thead align="left"><tr id="zh-cn_topic_0079615001_row9746163"><th class="cellrowborder" valign="top" width="22%" id="mcps1.2.4.1.1"><p id="p57545694203043"><a name="p57545694203043"></a><a name="p57545694203043"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="32%" id="mcps1.2.4.1.2"><p id="p4531342288"><a name="p4531342288"></a><a name="p4531342288"></a>编码</p>
</th>
<th class="cellrowborder" valign="top" width="46%" id="mcps1.2.4.1.3"><p id="p30689603203043"><a name="p30689603203043"></a><a name="p30689603203043"></a>状态说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0079615001_row48621261"><td class="cellrowborder" valign="top" width="22%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0079615001_p46008046"><a name="zh-cn_topic_0079615001_p46008046"></a><a name="zh-cn_topic_0079615001_p46008046"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.4.1.2 "><p id="p7538425819"><a name="p7538425819"></a><a name="p7538425819"></a>OK</p>
</td>
<td class="cellrowborder" valign="top" width="46%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0079615001_p35664277"><a name="zh-cn_topic_0079615001_p35664277"></a><a name="zh-cn_topic_0079615001_p35664277"></a>请求已成功。</p>
</td>
</tr>
</tbody>
</table>

异常状态码，请参见[状态码](状态码.md)。

