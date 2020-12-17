# 在Nginx服务器上安装SSL证书<a name="ZH-CN_TOPIC_0171809251"></a>

本章节介绍如何将下载的证书安装到Nginx服务器上。安装好证书后，您的Web服务器将能支持SSL通信，从而保证您Web服务器的通信安全。

>![](public_sys-resources/icon-note.gif) **说明：** 
>如果证书安装过程中遇到问题，请在证书下载页面右方的“一对一咨询“中，单击“立即咨询“，联系工程师进行处理。
>您还可以直接单击[HTTPS服务配置全站加密SSL优化检测](https://market.huaweicloud.com/product/00301-120142-0--0)进行购买，购买服务后，联系工程师进行处理。

## 前提条件<a name="section171927174218"></a>

-   已获取管理控制台的登录账号与密码。
-   “证书状态“为“已签发“。
-   已下载SSL证书，具体操作请参见[下载证书](下载证书.md)。

## 约束条件<a name="section13500821131513"></a>

-   证书安装前，务必在Tomcat服务器上开启“443“端口，避免安装后仍然无法启用HTTPS。
-   如果一个域名有多个服务器，则每一个服务器上都要部署。
-   待安装证书的服务器上需要运行的域名，必须与证书的域名一一对应，即购买的是哪个域名的证书，则用于哪个域名。否则安装部署后，浏览器将提示不安全。

## 操作步骤<a name="section6411655151013"></a>

在Nginx服务器上安装SSL证书的流程如下所示：

[①获取文件](#section1695131981311)  →  [②创建目录](#section12396955146)  →  [③修改配置文件](#section107625153145)  →  [④验证配置是否正确](#section9969162141410)  →  [⑤重启Nginx](#section1334319226163)  →  [⑥效果验证](#section17691911165112)

## 步骤一：获取文件<a name="section1695131981311"></a>

安装证书前，需要获取证书文件和密码文件，请根据申请证书时选择的“证书请求文件“生成方式来选择操作步骤：

-   如果申请证书时，“证书请求文件“选择“系统生成CSR“，具体操作请参见：[系统生成CSR](#li132139219148)。
-   如果申请证书时，“证书请求文件“选择“自己生成CSR“，具体操作请参见：[自己生成CSR](#li12143211413)。

具体操作如下：

-   <a name="li132139219148"></a>系统生成CSR
    1.  在本地解压已下载的证书文件。

        下载的文件包含了“Apache“、“IIS“、“Nginx“、“Tomcat“4个文件夹和1个“domain.csr“文件，如[图1](#zh-cn_topic_0171809250_zh-cn_topic_0110866190_fdd76c20249e24d95b7a52872f72f84fd)所示。

        **图 1**  本地解压SSL证书<a name="zh-cn_topic_0171809250_zh-cn_topic_0110866190_fdd76c20249e24d95b7a52872f72f84fd"></a>  
        ![](figures/本地解压SSL证书.png "本地解压SSL证书")

    2.  从“Nginx“文件夹内获得证书文件“server.crt“和私钥文件“server.key“。
        -   “server.crt“文件包括两段证书代码“-----BEGIN CERTIFICATE-----“和“-----END CERTIFICATE-----“，分别为服务器证书和中级CA。
        -   “server.key“文件包括一段私钥代码“-----BEGIN RSA PRIVATE KEY-----“和“-----END RSA PRIVATE KEY-----“。


-   <a name="li12143211413"></a>自己生成CSR
    1.  解压已下载的证书压缩包，获得“server.pem“文件。

        “server.pem“文件包括两段证书代码“-----BEGIN CERTIFICATE-----“和“-----END CERTIFICATE-----“，分别为服务器证书和中级CA证书。

    2.  将“server.pem“的后缀名修改为“crt”，即“server.crt“。
    3.  将“server.crt“和生成CSR时的私钥“server.key“放在任意文件夹内。


## 步骤二：创建目录<a name="section12396955146"></a>

在Nginx的安装目录下创建“cert“目录，并且将“server.key“和“server.crt“拷贝到“cert“目录下。

## 步骤三：修改配置文件<a name="section107625153145"></a>

配置Nginx中“conf“目录下的“nginx.conf“文件。

1.  找到如下配置内容：

    ```
    #server {
    #    listen       443 ssl;
    #    server_name  localhost;
    #    ssl_certificate      cert.pem;
    #    ssl_certificate_key  cert.key;
    #    ssl_session_cache    shared:SSL:1m;
    #    ssl_session_timeout  5m;
    #    ssl_ciphers  HIGH:!aNULL:!MD5;
    #    ssl_prefer_server_ciphers  on;
    #    location / {
    #        root   html;
    #        index  index.html index.htm;
    #    }
    #}
    ```

2.  删除行首的配置语句注释符号\#。

    ```
    server {  
                 listen              443 ssl;  
                 server_name         localhost;
                 ssl_certificate     cert.pem;  
                 ssl_certificate_key cert.key;
                 ssl_session_cache   shared:SSL:1m;  
                 ssl_session_timeout 5m;  
                 ssl_ciphers         HIGH:!aNULL:!MD5;         
                 ssl_prefer_server_ciphers  on;  
                 location / {  
                            root     html; 
                            index    index.html index.htm;  
                             }  
    }
    ```

3.  修改如下参数，具体参数修改说明如[表1](#table4462648181517)所示。

    ```
    ssl_certificate          cert/server.crt;    
    ssl_certificate_key      cert/server.key;   
    ```

    完整的配置如下，其余参数根据实际情况修改：

    ```
    server {
            listen       443 ssl;
            server_name  www.domain.com; #修改为您证书绑定的域名。
            ssl_certificate      cert/server.crt; #替换成您的证书文件的路径。
            ssl_certificate_key  cert/server.key; #替换成您的私钥文件的路径。
            ssl_session_cache    shared:SSL:1m;
            ssl_session_timeout  5m;
            ssl_ciphers  HIGH:!aNULL:!MD5; #加密套件。
            ssl_prefer_server_ciphers  on;
            location / {
                root   html; #站点目录。
                index  index.html index.htm; #添加属性。
                       }  
    }
    ```

    >![](public_sys-resources/icon-notice.gif) **须知：** 
    >不要直接拷贝所有配置，参数中“ssl“开头的属性与证书配置有直接关系，其它参数请根据自己的实际情况修改。

    **表 1**  参数说明

    <a name="table4462648181517"></a>
    <table><thead align="left"><tr id="row1446274819154"><th class="cellrowborder" valign="top" width="25.619999999999997%" id="mcps1.2.3.1.1"><p id="p144628487152"><a name="p144628487152"></a><a name="p144628487152"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="74.38%" id="mcps1.2.3.1.2"><p id="p16462104814154"><a name="p16462104814154"></a><a name="p16462104814154"></a>参数说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row2462154818156"><td class="cellrowborder" valign="top" width="25.619999999999997%" headers="mcps1.2.3.1.1 "><p id="p13462194817156"><a name="p13462194817156"></a><a name="p13462194817156"></a>listen</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.38%" headers="mcps1.2.3.1.2 "><p id="p1146244815153"><a name="p1146244815153"></a><a name="p1146244815153"></a>SSL访问端口号，设置为<span class="parmvalue" id="parmvalue9462348151514"><a name="parmvalue9462348151514"></a><a name="parmvalue9462348151514"></a>“443”</span>。</p>
    </td>
    </tr>
    <tr id="row1146216480154"><td class="cellrowborder" valign="top" width="25.619999999999997%" headers="mcps1.2.3.1.1 "><p id="p5462164801519"><a name="p5462164801519"></a><a name="p5462164801519"></a>server_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.38%" headers="mcps1.2.3.1.2 "><p id="p24621348171514"><a name="p24621348171514"></a><a name="p24621348171514"></a>证书绑定的域名。示例：www.domain.com</p>
    </td>
    </tr>
    <tr id="row11462848191514"><td class="cellrowborder" valign="top" width="25.619999999999997%" headers="mcps1.2.3.1.1 "><p id="p1246254871516"><a name="p1246254871516"></a><a name="p1246254871516"></a>ssl_certificate</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.38%" headers="mcps1.2.3.1.2 "><p id="p546274811520"><a name="p546274811520"></a><a name="p546274811520"></a>证书文件<span class="filepath" id="filepath34621448161519"><a name="filepath34621448161519"></a><a name="filepath34621448161519"></a>“server.crt”</span>。</p>
    <p id="p1746312483156"><a name="p1746312483156"></a><a name="p1746312483156"></a>设置为<span class="filepath" id="filepath94632048151517"><a name="filepath94632048151517"></a><a name="filepath94632048151517"></a>“server.crt”</span>文件的路径，且路径中不能包含中文字符，例如<span class="filepath" id="filepath1146316483152"><a name="filepath1146316483152"></a><a name="filepath1146316483152"></a>“cert/server.crt”</span>。</p>
    </td>
    </tr>
    <tr id="row94639482156"><td class="cellrowborder" valign="top" width="25.619999999999997%" headers="mcps1.2.3.1.1 "><p id="p18463164831514"><a name="p18463164831514"></a><a name="p18463164831514"></a>ssl_certificate_key</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.38%" headers="mcps1.2.3.1.2 "><p id="p16463154812157"><a name="p16463154812157"></a><a name="p16463154812157"></a>私钥文件<span class="filepath" id="filepath1946313481155"><a name="filepath1946313481155"></a><a name="filepath1946313481155"></a>“server.key”</span>。</p>
    <p id="p146324871517"><a name="p146324871517"></a><a name="p146324871517"></a>设置为<span class="filepath" id="filepath0463144816155"><a name="filepath0463144816155"></a><a name="filepath0463144816155"></a>“server.key”</span>的路径，且路径中不能包含中文字符，例如<span class="filepath" id="filepath3463184817155"><a name="filepath3463184817155"></a><a name="filepath3463184817155"></a>“cert/server.key”</span>。</p>
    </td>
    </tr>
    </tbody>
    </table>

4.  修改完成后保存配置文件。

## 步骤四：验证配置是否正确<a name="section9969162141410"></a>

进入Nginx执行目录下，执行以下命令：

****sbin/nginx -t****

当回显信息如下所示时，则表示配置正确：

```
nginx.conf syntax is ok
nginx.conf test is successful
```

## 步骤五：重启Nginx<a name="section1334319226163"></a>

执行以下操作重启Nginx。

在Nginx安装目录下执行**nginx -s quit**命令，停止Nginx服务；

在Nginx安装目录下执行****start nginx****命令，启动Nginx服务。

## 效果验证<a name="section17691911165112"></a>

部署成功后，可在浏览器的地址栏中输入“https://域名“，按“Enter“。

如果浏览器地址栏显示安全锁标识，则说明证书安装成功。

-   如果网站仍然出现不安全提示，请参见[为什么部署了SSL证书后，网站仍然出现不安全提示？](https://support.huaweicloud.com/scm_faq/scm_01_0098.html)进行处理。
-   如果通过域名访问网站时，无法打开网站，请参见[为什么部署了SSL证书后，通过域名访问网站时，无法打开网站？](https://support.huaweicloud.com/scm_faq/scm_01_0099.html)进行处理。

