# 校验CSR<a name="scm_02_0021"></a>

## 功能介绍<a name="zh-cn_topic_0000001122898803_s1731a14fb0144c79bf0fa90c694f34f7"></a>

校验证书请求文件（Certificate Signing Request，CSR）并解析域名。

## URI<a name="zh-cn_topic_0000001122898803_se70c3e5518a04f60b06032524dddfef4"></a>

-   URI格式

    POST /v2/\{project\_id\}/scm/check-csr

-   参数说明

    <a name="zh-cn_topic_0000001122898803_t982da1e0196d4ec1a28d1fbff2cc8191"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0000001122898803_r6e963322c1e740d181726d2f0e91df5a"><th class="cellrowborder" valign="top" width="20%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0000001122898803_a3b5bbe5a7f644fd3a74cecbfb3f7ed60"><a name="zh-cn_topic_0000001122898803_a3b5bbe5a7f644fd3a74cecbfb3f7ed60"></a><a name="zh-cn_topic_0000001122898803_a3b5bbe5a7f644fd3a74cecbfb3f7ed60"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="20%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0000001122898803_p84171140153917"><a name="zh-cn_topic_0000001122898803_p84171140153917"></a><a name="zh-cn_topic_0000001122898803_p84171140153917"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="20%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0000001122898803_p1859883763913"><a name="zh-cn_topic_0000001122898803_p1859883763913"></a><a name="zh-cn_topic_0000001122898803_p1859883763913"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="40%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0000001122898803_a6bb6f1fe56a2454982832e8d56d354d8"><a name="zh-cn_topic_0000001122898803_a6bb6f1fe56a2454982832e8d56d354d8"></a><a name="zh-cn_topic_0000001122898803_a6bb6f1fe56a2454982832e8d56d354d8"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0000001122898803_r69bf37b65d3f446eab7b3f4d1b2fcec0"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0000001122898803_ae42d73592f58424ea93a11e52d2478dd"><a name="zh-cn_topic_0000001122898803_ae42d73592f58424ea93a11e52d2478dd"></a><a name="zh-cn_topic_0000001122898803_ae42d73592f58424ea93a11e52d2478dd"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0000001122898803_p154181440173917"><a name="zh-cn_topic_0000001122898803_p154181440173917"></a><a name="zh-cn_topic_0000001122898803_p154181440173917"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0000001122898803_p4599537193912"><a name="zh-cn_topic_0000001122898803_p4599537193912"></a><a name="zh-cn_topic_0000001122898803_p4599537193912"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0000001122898803_a1314869d2dc147b38461e037d622f7b4"><a name="zh-cn_topic_0000001122898803_a1314869d2dc147b38461e037d622f7b4"></a><a name="zh-cn_topic_0000001122898803_a1314869d2dc147b38461e037d622f7b4"></a>项目ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="zh-cn_topic_0000001122898803_seb7b7901701247fab30a59b76f1c7f93"></a>

请求参数

<a name="zh-cn_topic_0000001122898803_table46221022101230"></a>
<table><thead align="left"><tr id="zh-cn_topic_0000001122898803_row9315574101230"><th class="cellrowborder" valign="top" width="20%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0000001122898803_p16364058101230"><a name="zh-cn_topic_0000001122898803_p16364058101230"></a><a name="zh-cn_topic_0000001122898803_p16364058101230"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0000001122898803_p18681345203916"><a name="zh-cn_topic_0000001122898803_p18681345203916"></a><a name="zh-cn_topic_0000001122898803_p18681345203916"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0000001122898803_p14956439391"><a name="zh-cn_topic_0000001122898803_p14956439391"></a><a name="zh-cn_topic_0000001122898803_p14956439391"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0000001122898803_p28146304101230"><a name="zh-cn_topic_0000001122898803_p28146304101230"></a><a name="zh-cn_topic_0000001122898803_p28146304101230"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0000001122898803_row2638193101722"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0000001122898803_p4481944111821"><a name="zh-cn_topic_0000001122898803_p4481944111821"></a><a name="zh-cn_topic_0000001122898803_p4481944111821"></a>csr</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0000001122898803_p1686844510399"><a name="zh-cn_topic_0000001122898803_p1686844510399"></a><a name="zh-cn_topic_0000001122898803_p1686844510399"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0000001122898803_p99512431398"><a name="zh-cn_topic_0000001122898803_p99512431398"></a><a name="zh-cn_topic_0000001122898803_p99512431398"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0000001122898803_p1164514065313"><a name="zh-cn_topic_0000001122898803_p1164514065313"></a><a name="zh-cn_topic_0000001122898803_p1164514065313"></a>证书请求文件CSR。</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="zh-cn_topic_0000001122898803_sfadd53a5f4714e8f87811818d62d0296"></a>

响应参数

<a name="zh-cn_topic_0000001122898803_t98d238e10953421e84a073707024c329"></a>
<table><thead align="left"><tr id="zh-cn_topic_0000001122898803_r144a2c52c5054c6d9243eb2ef3875a21"><th class="cellrowborder" valign="top" width="20%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0000001122898803_a9156e0b03f054d4e8547e0787f88a51b"><a name="zh-cn_topic_0000001122898803_a9156e0b03f054d4e8547e0787f88a51b"></a><a name="zh-cn_topic_0000001122898803_a9156e0b03f054d4e8547e0787f88a51b"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0000001122898803_p58822546391"><a name="zh-cn_topic_0000001122898803_p58822546391"></a><a name="zh-cn_topic_0000001122898803_p58822546391"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0000001122898803_p62425293914"><a name="zh-cn_topic_0000001122898803_p62425293914"></a><a name="zh-cn_topic_0000001122898803_p62425293914"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0000001122898803_a0097000016b14857972b7929bcaaa038"><a name="zh-cn_topic_0000001122898803_a0097000016b14857972b7929bcaaa038"></a><a name="zh-cn_topic_0000001122898803_a0097000016b14857972b7929bcaaa038"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0000001122898803_rf212a916c502452a8e151eba2f118272"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0000001122898803_p7216853205314"><a name="zh-cn_topic_0000001122898803_p7216853205314"></a><a name="zh-cn_topic_0000001122898803_p7216853205314"></a>domain_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0000001122898803_p158821154113914"><a name="zh-cn_topic_0000001122898803_p158821154113914"></a><a name="zh-cn_topic_0000001122898803_p158821154113914"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0000001122898803_p1024185212397"><a name="zh-cn_topic_0000001122898803_p1024185212397"></a><a name="zh-cn_topic_0000001122898803_p1024185212397"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0000001122898803_p61101369111935"><a name="zh-cn_topic_0000001122898803_p61101369111935"></a><a name="zh-cn_topic_0000001122898803_p61101369111935"></a>CSR中的域名。</p>
</td>
</tr>
</tbody>
</table>

## 示例<a name="zh-cn_topic_0000001122898803_section1683920202720"></a>

如下以校验某个CSR为例。

-   请求样例

    ```
    {
        "csr":"-----BEGIN NEW CERTIFICATE REQUEST-----******-----END NEW CERTIFICATE REQUEST-----"
    }
    ```

-   响应样例

    ```
    {
        "domain": "a.example1.com"
    }
    ```

    或

    ```
    { 
       "error_code": "SCM.XXXX",  
       "error_msg": "XXXX"   
     }
    ```


## 状态码<a name="zh-cn_topic_0000001122898803_section12126152083712"></a>

[表1](#zh-cn_topic_0000001122898803_scm_02_0014_zh-cn_topic_0079615001_table20596071)描述的是API返回的正常状态码。

**表 1**  状态码

<a name="zh-cn_topic_0000001122898803_scm_02_0014_zh-cn_topic_0079615001_table20596071"></a>
<table><thead align="left"><tr id="zh-cn_topic_0000001122898803_scm_02_0014_zh-cn_topic_0079615001_row9746163"><th class="cellrowborder" valign="top" width="22%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0000001122898803_scm_02_0014_p57545694203043"><a name="zh-cn_topic_0000001122898803_scm_02_0014_p57545694203043"></a><a name="zh-cn_topic_0000001122898803_scm_02_0014_p57545694203043"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="32%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0000001122898803_scm_02_0014_p4531342288"><a name="zh-cn_topic_0000001122898803_scm_02_0014_p4531342288"></a><a name="zh-cn_topic_0000001122898803_scm_02_0014_p4531342288"></a>编码</p>
</th>
<th class="cellrowborder" valign="top" width="46%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0000001122898803_scm_02_0014_p30689603203043"><a name="zh-cn_topic_0000001122898803_scm_02_0014_p30689603203043"></a><a name="zh-cn_topic_0000001122898803_scm_02_0014_p30689603203043"></a>状态说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0000001122898803_scm_02_0014_zh-cn_topic_0079615001_row48621261"><td class="cellrowborder" valign="top" width="22%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001122898803_scm_02_0014_zh-cn_topic_0079615001_p46008046"><a name="zh-cn_topic_0000001122898803_scm_02_0014_zh-cn_topic_0079615001_p46008046"></a><a name="zh-cn_topic_0000001122898803_scm_02_0014_zh-cn_topic_0079615001_p46008046"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001122898803_scm_02_0014_p7538425819"><a name="zh-cn_topic_0000001122898803_scm_02_0014_p7538425819"></a><a name="zh-cn_topic_0000001122898803_scm_02_0014_p7538425819"></a>OK</p>
</td>
<td class="cellrowborder" valign="top" width="46%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001122898803_scm_02_0014_zh-cn_topic_0079615001_p35664277"><a name="zh-cn_topic_0000001122898803_scm_02_0014_zh-cn_topic_0079615001_p35664277"></a><a name="zh-cn_topic_0000001122898803_scm_02_0014_zh-cn_topic_0079615001_p35664277"></a>请求已成功。</p>
</td>
</tr>
</tbody>
</table>

异常状态码，请参见[错误码](https://support.huaweicloud.com/api-scm/ErrorCode.html)。

