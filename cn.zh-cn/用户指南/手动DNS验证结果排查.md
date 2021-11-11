# 手动DNS验证结果排查<a name="ZH-CN_TOPIC_0000001171367982"></a>

手动DNS验证操作完成后，如果您使用的是Windows操作系统，可通过以下方式进行排查：

## 操作步骤<a name="zh-cn_topic_0000001171009914_section456395912261"></a>

1.  在Windows系统中，单击“开始“，输入“cmd“，进入命令提示符对话框。
2.  在cmd中输入以下命令，查看DNS验证配置是否已经生效。

    **nslookup -q=TXT** _xxx_

    _xxx_代表域名服务商返回的“主机记录“值。

    -   如果界面回显的记录值（text的值）与域名服务商返回的“记录值“一致，如[图1](#zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_fig1141255248)所示，说明域名授权验证配置已经生效。

        **图 1**  域名授权验证配置生效<a name="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_fig1141255248"></a>  
        ![](figures/域名授权验证配置生效.png "域名授权验证配置生效")

    -   如果界面回显信息不存在TXT记录，显示为“Non-existent domain“，说明域名授权验证配置未生效。

        **图 2**  域名授权验证配置未生效<a name="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_fig9346102419212"></a>  
        ![](figures/域名授权验证配置未生效.png "域名授权验证配置未生效")

3.  如果DNS验证配置未生效，请根据以下可能原因进行排除修改，直至验证生效。

    **表 1**  排查处理

    <a name="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_table628812514416"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_row1828919251041"><th class="cellrowborder" valign="top" width="28.939999999999998%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_p1228919253413"><a name="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_p1228919253413"></a><a name="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_p1228919253413"></a>可能原因</p>
    </th>
    <th class="cellrowborder" valign="top" width="71.06%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_p528917253414"><a name="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_p528917253414"></a><a name="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_p528917253414"></a>处理方法</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_row62896252047"><td class="cellrowborder" valign="top" width="28.939999999999998%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_p162891625847"><a name="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_p162891625847"></a><a name="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_p162891625847"></a>记录配置出错</p>
    </td>
    <td class="cellrowborder" valign="top" width="71.06%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_p2028917251146"><a name="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_p2028917251146"></a><a name="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_p2028917251146"></a>请您检查<span class="parmname" id="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_parmname179218391043"><a name="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_parmname179218391043"></a><a name="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_parmname179218391043"></a>“主机记录”</span>或<span class="parmname" id="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_parmname11925391545"><a name="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_parmname11925391545"></a><a name="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_parmname11925391545"></a>“类型”</span>是否填写正确。</p>
    <p id="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_p551005218411"><a name="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_p551005218411"></a><a name="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_p551005218411"></a>如下以华为云的云解析服务中的配置为例进行说明：</p>
    <p id="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_p4605121414619"><a name="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_p4605121414619"></a><a name="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_p4605121414619"></a><a name="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_image19510352341"></a><a name="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_image19510352341"></a><span><img id="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_image19510352341" src="figures/配置检查.png" height="129.20005700000002" width="332.5"></span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_row1428962511415"><td class="cellrowborder" valign="top" width="28.939999999999998%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_p52891325940"><a name="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_p52891325940"></a><a name="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_p52891325940"></a>配置的生效时间过长，生效时间还未到，因此无法查询到数据。</p>
    </td>
    <td class="cellrowborder" valign="top" width="71.06%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_p1328919259410"><a name="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_p1328919259410"></a><a name="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_p1328919259410"></a>请您检查生效时间（TTL）是否设置过长，建议将生效时间修改为5分钟。不同的域名提供商的DNS配置不一样，如华为云的DNS（云解析服务）默认是5分钟后生效，如下图所示。</p>
    <p id="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_p189929331369"><a name="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_p189929331369"></a><a name="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_p189929331369"></a>若配置的生效时间未到，请等时间到了后再进行验证。</p>
    <p id="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_p92401953350"><a name="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_p92401953350"></a><a name="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_p92401953350"></a><a name="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_image8639239852"></a><a name="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_image8639239852"></a><span><img id="zh-cn_topic_0000001171009914_zh-cn_topic_0000001215578709_zh-cn_topic_0000001169740848_image8639239852" src="figures/配置时间.png" height="246.746654" width="266"></span></p>
    </td>
    </tr>
    </tbody>
    </table>


