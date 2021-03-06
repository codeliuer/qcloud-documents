
## 密钥管理服务

### 加解密相关接口
| 接口功能 | Action ID | 功能描述
|---------|---------|---------|
| [加密](https://www.qcloud.com/document/product/573/8889) | Encrypt|用于加密最多为4KB任意数据，诸如RSA密钥，数据库密钥，或者其他敏感的客户信息。|
| [解密](https://www.qcloud.com/document/product/573/8890) | Decrypt|用于解密密文数据，得到明文数据。|



### 密钥管理相关接口
| 接口功能 | Action ID | 功能描述|
|---------|---------|---------|
| [创建主密钥](https://www.qcloud.com/document/product/573/8893) |CreateKey |创建用户管理数据秘钥的主秘钥CMK（Custom Master Key）。|
| [获取主密钥列表](https://www.qcloud.com/document/product/573/8897) | ListKey | 用于获取用户所有的keyId。|
|[获取主密钥属性](https://www.qcloud.com/document/product/573/8898)  | GetKeyAttributes| 用于获取指定keyId的属性信息。|
| [禁用主密钥](https://www.qcloud.com/document/product/573/8896) | DisableKey |用于禁用一个指定的keyId。|
| [启用主密钥](https://www.qcloud.com/document/product/573/8894) | EnableKey | 用于启用一个指定的keyId。|
| [生成数据密钥](https://www.qcloud.com/document/product/573/8895) |GenerateDataKey| 用于生成一个密钥，用户可以使用该密钥用于本地数据的加密。|
| [修改主密钥属性](https://www.qcloud.com/document/product/573/8892)|SetKeyAttributes|用于修改指定keyId的属性信息。|


