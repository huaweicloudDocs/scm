# 下载SSL证书<a name="ZH-CN_TOPIC_0000001215904793"></a>

该任务指导用户在SSL证书管理平台下载证书。

## 前提条件<a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_section556861155951"></a>

“证书状态“为“已签发“或“托管中“。

## 约束条件<a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_section121106283812"></a>

-   仅支持在证书有效期内，不限次数的下载证书，下载后即可在服务器（华为云的或非华为云的均可）上进行部署。
-   “证书请求文件“选择的是“系统生成CSR“，下载的文件包含了“Apache“、“IIS“、“Nginx“、“Tomcat“4个文件夹和1个“domain.csr“文件。
-   “证书请求文件“选择的是“自己生成CSR“，下载的证书仅包含一个名为“server.pem“的文件。文件中已经包含两段证书代码，分别是服务器证书和CA中间证书。私钥为用户自行保存的，华为云SSL证书管理不提供。

## 操作步骤<a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_section408105191602"></a>

1.  登录[管理控制台](https://console.huaweicloud.com/)。
2.  单击页面左上方的![](figures/icon-servicelist.png)，选择“安全与合规  \>  云证书管理服务“，进入云证书管理界面。
3.  在左侧导航栏选择“SSL证书管理“，进入SSL证书管理页面。
4.  在需要下载的证书所在行的“操作“列，单击“下载“，如[图1](#zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_fig121926536132)所示。

    **图 1**  下载证书<a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_fig121926536132"></a>  
    ![](figures/下载证书.png "下载证书")

5.  请根据您需要的服务类型，在对应的“操作“列单击“下载证书“，进行证书下载操作。
6.  证书下载后，需要安装到对应的服务器上。
    -   在Tomcat上安装SSL证书的详细指导操作请参见[如何在Tomcat上安装SSL证书？](在Tomcat服务器上安装SSL证书.md#ZH-CN_TOPIC_0000001170585006)。
    -   在Nginx上安装SSL证书的详细指导操作请参见[如何在Nginx上安装SSL证书？](在Nginx服务器上安装SSL证书.md#ZH-CN_TOPIC_0000001170744950)。
    -   在Apache上安装SSL证书的详细指导操作请参见[如何在Apache上安装SSL证书？](在Apache服务器上安装SSL证书.md#ZH-CN_TOPIC_0000001216026323)。
    -   在IIS上安装SSL证书的详细指导操作请参见[如何在IIS上安装SSL证书？](在IIS服务器上安装SSL证书.md#ZH-CN_TOPIC_0000001170426454)。
    -   在Weblogic上安装SSL证书的详细指导操作请参见[在Weblogic服务器上安装SSL证书](在Weblogic服务器上安装SSL证书.md#ZH-CN_TOPIC_0000001170266470)。


## 下载的证书文件说明<a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_section7206183218592"></a>

下载文件说明：根据申请证书时，选择的“证书请求文件“方式的不同，下载文件也有所不同。

-   申请证书时，如果“证书请求文件“选择的是“系统生成CSR“，则下载文件说明如下：

    下载的文件包含了“Apache“、“IIS“、“Nginx“、“Tomcat“4个文件夹和1个“domain.csr“文件，如[图2](#zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_fig4414184151010)所示，具体文件说明如[表1](#zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_table116635101410)所示。

    **图 2**  解压SSL证书<a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_fig4414184151010"></a>  
    ![](figures/解压SSL证书.png "解压SSL证书")

    **表 1**  下载文件说明

    <a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_table116635101410"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_row966491019412"><th class="cellrowborder" valign="top" width="36.04%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p1966412101044"><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p1966412101044"></a><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p1966412101044"></a>文件夹/文件名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="63.959999999999994%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p56640101413"><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p56640101413"></a><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p56640101413"></a>文件夹内容</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_row966411101347"><td class="cellrowborder" valign="top" width="36.04%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p96641110443"><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p96641110443"></a><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p96641110443"></a>Tomcat</p>
    </td>
    <td class="cellrowborder" valign="top" width="63.959999999999994%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p15664101015419"><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p15664101015419"></a><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p15664101015419"></a>keystorePass.txt：证书密码。</p>
    <p id="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p22234920512"><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p22234920512"></a><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p22234920512"></a>server.jks：证书文件。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_row366413101949"><td class="cellrowborder" valign="top" width="36.04%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p13664410345"><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p13664410345"></a><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p13664410345"></a>Nginx</p>
    </td>
    <td class="cellrowborder" valign="top" width="63.959999999999994%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p1066410101742"><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p1066410101742"></a><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p1066410101742"></a>server.crt：证书文件，包含两段证书代码，分别为服务器证书和CA中间证书。</p>
    <p id="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p8859111815518"><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p8859111815518"></a><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p8859111815518"></a>server.key：证书私钥文件，包含一段证书私钥代码。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_row1065383320412"><td class="cellrowborder" valign="top" width="36.04%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p7654333442"><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p7654333442"></a><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p7654333442"></a>Apache</p>
    </td>
    <td class="cellrowborder" valign="top" width="63.959999999999994%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p116546338415"><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p116546338415"></a><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p116546338415"></a>ca.crt：证书链文件，包含一段中级CA代码。</p>
    <p id="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p611218531515"><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p611218531515"></a><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p611218531515"></a>server.crt：证书文件，包含一段服务器证书代码。</p>
    <p id="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p1959755610"><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p1959755610"></a><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p1959755610"></a>server.key：证书私钥文件，包含一段证书私钥代码。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_row1286419431648"><td class="cellrowborder" valign="top" width="36.04%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p586414312416"><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p586414312416"></a><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p586414312416"></a>IIS</p>
    </td>
    <td class="cellrowborder" valign="top" width="63.959999999999994%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p1086410431647"><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p1086410431647"></a><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p1086410431647"></a>keystorePass.txt：证书密码。</p>
    <p id="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p11134104213517"><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p11134104213517"></a><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p11134104213517"></a>server.pfx：证书文件。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_row35741610193613"><td class="cellrowborder" valign="top" width="36.04%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p1457481053613"><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p1457481053613"></a><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p1457481053613"></a>domain.csr</p>
    </td>
    <td class="cellrowborder" valign="top" width="63.959999999999994%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p75741210103616"><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p75741210103616"></a><a name="zh-cn_topic_0000001170218848_zh-cn_topic_0000001124217619_zh-cn_topic_0110866214_p75741210103616"></a>证书请求文件。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   申请证书时，如果“证书请求文件“选择的是“自己生成CSR“，则下载文件说明如下：

    下载的证书仅包含一个名为“server.pem“的文件。文件中已经包含两段证书代码，分别是服务器证书和CA中间证书。

    私钥为用户自行保存的，华为云SSL证书管理不提供。在各个服务器上安装证书时，需要填写对应私钥的位置。

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >“自己生成CSR“的证书不支持推送到云产品。


