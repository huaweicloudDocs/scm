# 上传已有SSL证书<a name="ZH-CN_TOPIC_0000001215904795"></a>

您可以将您所拥有的SSL证书（已在其他平台购买并签发的SSL证书）上传到云证书管理平台，以便在云证书管理平台中对您的证书进行统一管理。上传后，可将证书部署到华为云其他云产品，且支持设置证书到期前提醒。

该任务指导您如何在本地将外部SSL证书上传到云证书管理平台。

## 前提条件<a name="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_section2256777914731"></a>

已准备好需要上传证书的相关文件，具体如下：

-   PEM编码格式的证书文件（文件后缀是PEM或者CRT）
-   PEM编码格式的证书私钥文件（文件后缀是KEY）

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   目前SSL证书管理平台只支持上传PEM格式的证书。其他格式的证书需要转化成PEM格式后才能上传，具体操作请参见[如何将证书格式转换为PEM格式？](https://support.huaweicloud.com/ccm_faq/ccm_01_0128.html)。
>    更多关于证书链的相关配置请参见[证书链配置说明](https://support.huaweicloud.com/ccm_faq/ccm_01_0106.html)。
>-   证书私钥需要是无密码保护的，更多详细介绍请参见[为什么要使用无密码保护的私钥？](https://support.huaweicloud.com/ccm_faq/ccm_01_0274.html)。
>-   上传的证书，SCM会在证书到期前30天提醒您证书即将到期，同时还支持配置消息提醒，设置后SSL证书管理系统会在证书到期前两个月、一个月、一周和到期时，发送邮件和短信提醒用户，具体配置操作请参见[如何配置SSL证书到期提醒？](https://support.huaweicloud.com/ccm_faq/ccm_01_0204.html)。

## 操作步骤<a name="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_section2756238314925"></a>

1.  登录[管理控制台](https://console.huaweicloud.com/)。
2.  单击页面左上方的![](figures/icon-servicelist.png)，选择“安全与合规  \>  云证书管理服务“，进入云证书管理界面。
3.  在左侧导航栏选择“SSL证书管理“，进入SSL证书管理页面。
4.  在证书列表左上角，单击“上传原有证书“，进入“上传原有证书“界面。
5.  在“上传原有证书“对话框中，输入证书信息，如[图1](#zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_fig17246889161023)所示，各参数说明如[表1](#zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_table490517514292)所示。

    **图 1**  上传原有证书<a name="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_fig17246889161023"></a>  
    ![](figures/上传原有证书.png "上传原有证书")

    **表 1**  上传证书参数说明

    <a name="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_table490517514292"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_row12906135142916"><th class="cellrowborder" valign="top" width="18.8%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_p8907752297"><a name="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_p8907752297"></a><a name="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_p8907752297"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="81.2%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_p49075562918"><a name="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_p49075562918"></a><a name="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_p49075562918"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_row109081515297"><td class="cellrowborder" valign="top" width="18.8%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_p159096582912"><a name="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_p159096582912"></a><a name="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_p159096582912"></a>证书名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="81.2%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_p1891155122915"><a name="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_p1891155122915"></a><a name="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_p1891155122915"></a>用户自定义。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001170537394_row1223794417541"><td class="cellrowborder" valign="top" width="18.8%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0000001170537394_p7237194425414"><a name="zh-cn_topic_0000001170537394_p7237194425414"></a><a name="zh-cn_topic_0000001170537394_p7237194425414"></a>企业项目</p>
    </td>
    <td class="cellrowborder" valign="top" width="81.2%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0000001170537394_p14237184445411"><a name="zh-cn_topic_0000001170537394_p14237184445411"></a><a name="zh-cn_topic_0000001170537394_p14237184445411"></a>将上传的SSL证书分配至对应的企业项目中。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_row6911165182919"><td class="cellrowborder" valign="top" width="18.8%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_p891111514297"><a name="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_p891111514297"></a><a name="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_p891111514297"></a>证书文件</p>
    </td>
    <td class="cellrowborder" valign="top" width="81.2%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_p1991112562918"><a name="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_p1991112562918"></a><a name="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_p1991112562918"></a>以文本方式打开待上传证书里的PEM格式的文件（后缀名为<span class="parmvalue" id="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_parmvalue2091116562912"><a name="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_parmvalue2091116562912"></a><a name="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_parmvalue2091116562912"></a>“.pem”</span>），将证书内容复制到此处。</p>
    <p id="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_p9987151031310"><a name="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_p9987151031310"></a><a name="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_p9987151031310"></a>按照“服务器证书-证书链”的顺序依次排列上传。具体方法请参见<a href="https://support.huaweicloud.com/ccm_faq/ccm_01_0187.html" target="_blank" rel="noopener noreferrer">如何上传证书文件？</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_row1491212517291"><td class="cellrowborder" valign="top" width="18.8%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_p2912156299"><a name="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_p2912156299"></a><a name="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_p2912156299"></a>证书私钥</p>
    </td>
    <td class="cellrowborder" valign="top" width="81.2%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_p1191395182916"><a name="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_p1191395182916"></a><a name="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_p1191395182916"></a>以文本方式打开待上传证书里的KEY格式的文件（后缀名为<span class="parmvalue" id="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_parmvalue1291365142915"><a name="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_parmvalue1291365142915"></a><a name="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_parmvalue1291365142915"></a>“.key”</span>），将私钥复制到此处。</p>
    </td>
    </tr>
    </tbody>
    </table>

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >-   上传的原有证书和秘钥必须是一一对应的。
    >-   保证私钥无密码保护，更多详细介绍请参见[为什么要使用无密码保护的私钥？](https://support.huaweicloud.com/ccm_faq/ccm_01_0274.html)。

6.  单击“确定“，完成上传证书。

    证书上传成功，证书列表中新增一条状态为“托管中“的证书。

    上传的证书可以部署到云产品中。


## 相关操作<a name="zh-cn_topic_0000001170537394_zh-cn_topic_0000001124401715_zh-cn_topic_0110866194_section7740135116176"></a>

上传证书可部署到华为云其他云产品中，具体操作请参见[推送证书到云产品](推送SSL证书到云产品.md#ZH-CN_TOPIC_0000001216146277)。

