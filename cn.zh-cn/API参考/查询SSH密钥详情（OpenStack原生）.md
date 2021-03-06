# 查询SSH密钥详情（OpenStack原生）<a name="ZH-CN_TOPIC_0060384659"></a>

## 功能介绍<a name="section59539732104217"></a>

根据SSH密钥名称查询指定SSH密钥。

## URI<a name="section52138884104217"></a>

GET /v2.1/\{project\_id\}/os-keypairs/\{keypair\_name\}

参数说明请参见[表1](#table1179423205514)。

**表 1**  参数说明

<a name="table1179423205514"></a>
<table><thead align="left"><tr id="row679693215558"><th class="cellrowborder" valign="top" width="24.662466246624664%" id="mcps1.2.4.1.1"><p id="p17653616104217"><a name="p17653616104217"></a><a name="p17653616104217"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="23.99239923992399%" id="mcps1.2.4.1.2"><p id="p20656767104217"><a name="p20656767104217"></a><a name="p20656767104217"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="51.34513451345134%" id="mcps1.2.4.1.3"><p id="p62585419104217"><a name="p62585419104217"></a><a name="p62585419104217"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row379623265513"><td class="cellrowborder" valign="top" width="24.662466246624664%" headers="mcps1.2.4.1.1 "><p id="p50904119104217"><a name="p50904119104217"></a><a name="p50904119104217"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="23.99239923992399%" headers="mcps1.2.4.1.2 "><p id="p29593000104217"><a name="p29593000104217"></a><a name="p29593000104217"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="51.34513451345134%" headers="mcps1.2.4.1.3 "><p id="p48222838104217"><a name="p48222838104217"></a><a name="p48222838104217"></a>项目ID。</p>
<p id="p652825144113"><a name="p652825144113"></a><a name="p652825144113"></a>获取方式请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="row1579623216550"><td class="cellrowborder" valign="top" width="24.662466246624664%" headers="mcps1.2.4.1.1 "><p id="p56513487104217"><a name="p56513487104217"></a><a name="p56513487104217"></a>keypair_name</p>
</td>
<td class="cellrowborder" valign="top" width="23.99239923992399%" headers="mcps1.2.4.1.2 "><p id="p14189698104217"><a name="p14189698104217"></a><a name="p14189698104217"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="51.34513451345134%" headers="mcps1.2.4.1.3 "><p id="p8514927104217"><a name="p8514927104217"></a><a name="p8514927104217"></a>密钥名称信息。</p>
<p id="p7466161413561"><a name="p7466161413561"></a><a name="p7466161413561"></a>可以通过<a href="查询SSH密钥列表（OpenStack原生）.md">查询SSH密钥列表（OpenStack原生）</a>API获取。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section18620476104217"></a>

-   请求参数

    无

-   请求样例

    ```
    GET https://{ECS Endpoint}/v2.1/bbf1946d374b44a0a2a95533562ba954/os-keypairs/keypair-test
    ```


## 响应消息<a name="section18336671104217"></a>

-   响应参数

    <a name="table47814565104217"></a>
    <table><thead align="left"><tr id="row50677205104217"><th class="cellrowborder" valign="top" width="23.45765423457654%" id="mcps1.1.4.1.1"><p id="p19987085"><a name="p19987085"></a><a name="p19987085"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="30.376962303769623%" id="mcps1.1.4.1.2"><p id="p4546697"><a name="p4546697"></a><a name="p4546697"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="46.16538346165384%" id="mcps1.1.4.1.3"><p id="p32738149"><a name="p32738149"></a><a name="p32738149"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row33037343104217"><td class="cellrowborder" valign="top" width="23.45765423457654%" headers="mcps1.1.4.1.1 "><p id="p58779125104217"><a name="p58779125104217"></a><a name="p58779125104217"></a>keypair</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.376962303769623%" headers="mcps1.1.4.1.2 "><p id="p63488655104217"><a name="p63488655104217"></a><a name="p63488655104217"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.16538346165384%" headers="mcps1.1.4.1.3 "><p id="p42307413104217"><a name="p42307413104217"></a><a name="p42307413104217"></a>SSH密钥信息，详情请参见<a href="#table39136185104217">表2</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 2**  keypair字段数据结构说明

    <a name="table39136185104217"></a>
    <table><thead align="left"><tr id="row60401722104217"><th class="cellrowborder" valign="top" width="23.45765423457654%" id="mcps1.2.4.1.1"><p id="p2384624132419"><a name="p2384624132419"></a><a name="p2384624132419"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="30.376962303769623%" id="mcps1.2.4.1.2"><p id="p23851124102419"><a name="p23851124102419"></a><a name="p23851124102419"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="46.16538346165384%" id="mcps1.2.4.1.3"><p id="p1388224162411"><a name="p1388224162411"></a><a name="p1388224162411"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row52495862104217"><td class="cellrowborder" valign="top" width="23.45765423457654%" headers="mcps1.2.4.1.1 "><p id="p24306447104217"><a name="p24306447104217"></a><a name="p24306447104217"></a>public_key</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.376962303769623%" headers="mcps1.2.4.1.2 "><p id="p22665160104217"><a name="p22665160104217"></a><a name="p22665160104217"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.16538346165384%" headers="mcps1.2.4.1.3 "><p id="p23938633104217"><a name="p23938633104217"></a><a name="p23938633104217"></a>密钥对应publicKey信息。</p>
    </td>
    </tr>
    <tr id="row14121108104217"><td class="cellrowborder" valign="top" width="23.45765423457654%" headers="mcps1.2.4.1.1 "><p id="p2959125104217"><a name="p2959125104217"></a><a name="p2959125104217"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.376962303769623%" headers="mcps1.2.4.1.2 "><p id="p38362611104217"><a name="p38362611104217"></a><a name="p38362611104217"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.16538346165384%" headers="mcps1.2.4.1.3 "><p id="p20363797104217"><a name="p20363797104217"></a><a name="p20363797104217"></a>密钥名称。</p>
    </td>
    </tr>
    <tr id="row49056452104217"><td class="cellrowborder" valign="top" width="23.45765423457654%" headers="mcps1.2.4.1.1 "><p id="p14149639104217"><a name="p14149639104217"></a><a name="p14149639104217"></a>fingerprint</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.376962303769623%" headers="mcps1.2.4.1.2 "><p id="p5270148104217"><a name="p5270148104217"></a><a name="p5270148104217"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.16538346165384%" headers="mcps1.2.4.1.3 "><p id="p24228833104217"><a name="p24228833104217"></a><a name="p24228833104217"></a>密钥对应指纹信息。</p>
    </td>
    </tr>
    <tr id="row16732907104217"><td class="cellrowborder" valign="top" width="23.45765423457654%" headers="mcps1.2.4.1.1 "><p id="p13188220104217"><a name="p13188220104217"></a><a name="p13188220104217"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.376962303769623%" headers="mcps1.2.4.1.2 "><p id="p61612865104217"><a name="p61612865104217"></a><a name="p61612865104217"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.16538346165384%" headers="mcps1.2.4.1.3 "><p id="p24586146104217"><a name="p24586146104217"></a><a name="p24586146104217"></a>密钥创建时间。</p>
    <p id="p8768130115818"><a name="p8768130115818"></a><a name="p8768130115818"></a>时间戳格式为ISO 8601，例如：2019-05-07T12:06:13.681238</p>
    </td>
    </tr>
    <tr id="row19948729104217"><td class="cellrowborder" valign="top" width="23.45765423457654%" headers="mcps1.2.4.1.1 "><p id="p5234385104217"><a name="p5234385104217"></a><a name="p5234385104217"></a>deleted</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.376962303769623%" headers="mcps1.2.4.1.2 "><p id="p21332025104217"><a name="p21332025104217"></a><a name="p21332025104217"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.16538346165384%" headers="mcps1.2.4.1.3 "><p id="p50172441104217"><a name="p50172441104217"></a><a name="p50172441104217"></a>密钥删除标记。</p>
    <a name="ul1594190135612"></a><a name="ul1594190135612"></a><ul id="ul1594190135612"><li>true：表示密钥已被删除。</li><li>false：表示密钥未被删除。</li></ul>
    </td>
    </tr>
    <tr id="row48898790104217"><td class="cellrowborder" valign="top" width="23.45765423457654%" headers="mcps1.2.4.1.1 "><p id="p1379054104217"><a name="p1379054104217"></a><a name="p1379054104217"></a>deleted_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.376962303769623%" headers="mcps1.2.4.1.2 "><p id="p44594563104217"><a name="p44594563104217"></a><a name="p44594563104217"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.16538346165384%" headers="mcps1.2.4.1.3 "><p id="p55389836104217"><a name="p55389836104217"></a><a name="p55389836104217"></a>密钥删除时间。</p>
    <p id="p03819116010"><a name="p03819116010"></a><a name="p03819116010"></a>时间戳格式为ISO 8601，例如：2019-05-07T12:06:13.681238</p>
    </td>
    </tr>
    <tr id="row28746480104217"><td class="cellrowborder" valign="top" width="23.45765423457654%" headers="mcps1.2.4.1.1 "><p id="p46763523104217"><a name="p46763523104217"></a><a name="p46763523104217"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.376962303769623%" headers="mcps1.2.4.1.2 "><p id="p29748990104217"><a name="p29748990104217"></a><a name="p29748990104217"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.16538346165384%" headers="mcps1.2.4.1.3 "><p id="p60857994104217"><a name="p60857994104217"></a><a name="p60857994104217"></a>密钥ID。</p>
    </td>
    </tr>
    <tr id="row10851038104217"><td class="cellrowborder" valign="top" width="23.45765423457654%" headers="mcps1.2.4.1.1 "><p id="p6518853104217"><a name="p6518853104217"></a><a name="p6518853104217"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.376962303769623%" headers="mcps1.2.4.1.2 "><p id="p58265105104217"><a name="p58265105104217"></a><a name="p58265105104217"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.16538346165384%" headers="mcps1.2.4.1.3 "><p id="p21853098104217"><a name="p21853098104217"></a><a name="p21853098104217"></a>密钥更新时间。</p>
    <p id="p63535230013"><a name="p63535230013"></a><a name="p63535230013"></a>时间戳格式为ISO 8601，例如：2019-05-07T12:06:13.681238</p>
    </td>
    </tr>
    <tr id="row62460159104217"><td class="cellrowborder" valign="top" width="23.45765423457654%" headers="mcps1.2.4.1.1 "><p id="p26108085104217"><a name="p26108085104217"></a><a name="p26108085104217"></a>user_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.376962303769623%" headers="mcps1.2.4.1.2 "><p id="p34380140104217"><a name="p34380140104217"></a><a name="p34380140104217"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.16538346165384%" headers="mcps1.2.4.1.3 "><p id="p33327947104217"><a name="p33327947104217"></a><a name="p33327947104217"></a>密钥所属用户信息。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "keypair": {
            "created_at": "2019-05-07T12:06:13.681238",
            "deleted": false,
            "deleted_at": null,
            "fingerprint": "9d:00:f4:d7:26:6e:52:06:4c:c1:d3:1d:fd:06:66:01",
            "id": 1,
            "name": "keypair-3582d8b7-e588-4aad-b7f7-f4e76f0e4314",
            "public_key": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDYJrTVpcMwFqQy/oMvtUSRofZdSRHEwrsX8AYkRvn2ZnCXM+b6+GZ2NQuuWj+ocznlnwiGFQDsL/yeE+/kurqcPJFKKp60mToXIMyzioFxW88fJtwEWawHKAclbHWpR1t4fQ4DS+/sIbX/Yd9btlVQ2tpQjodGDbM9Tr9/+/3i6rcR+EoLqmbgCgAiGiVV6VbM2Zx79yUwd+GnQejHX8BlYZoOjCnt3NREsITcmWE9FVFy6TnLmahs3FkEO/QGgWGkaohAJlsgaVvSWGgDn2AujKYwyDokK3dXyeX3m2Vmc3ejiqPa/C4nRrCOlko5nSgV/9IXRx1ERImsqZnE9usB Generated-by-Nova",
            "updated_at": null,
            "user_id": "fake"
        }
    }
    ```


## 返回值<a name="section7610951"></a>

正常返回值：

<a name="zh-cn_topic_0106040941_table753804619176"></a>
<table><thead align="left"><tr id="zh-cn_topic_0106040941_row10735134615172"><th class="cellrowborder" valign="top" width="42.42%" id="mcps1.1.3.1.1"><p id="zh-cn_topic_0106040941_p19735204616177"><a name="zh-cn_topic_0106040941_p19735204616177"></a><a name="zh-cn_topic_0106040941_p19735204616177"></a>返回值</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.1.3.1.2"><p id="zh-cn_topic_0106040941_p207355465176"><a name="zh-cn_topic_0106040941_p207355465176"></a><a name="zh-cn_topic_0106040941_p207355465176"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0106040941_row1473514621713"><td class="cellrowborder" valign="top" width="42.42%" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0106040941_p13735144611178"><a name="zh-cn_topic_0106040941_p13735144611178"></a><a name="zh-cn_topic_0106040941_p13735144611178"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.1.3.1.2 "><p id="zh-cn_topic_0106040941_p207351246161711"><a name="zh-cn_topic_0106040941_p207351246161711"></a><a name="zh-cn_topic_0106040941_p207351246161711"></a>服务器已成功处理了请求。</p>
</td>
</tr>
</tbody>
</table>

其他返回值请参考[状态码](状态码.md)。

## 错误码<a name="section14752650154917"></a>

请参考[错误码](错误码.md)。

