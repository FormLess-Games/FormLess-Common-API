#### 公共Header参数
参数名 | 示例值 | 参数描述
--- | --- | ---
暂无参数
#### 公共Query参数
参数名 | 示例值 | 参数描述
--- | --- | ---
暂无参数
#### 公共Body参数
参数名 | 示例值 | 参数描述
--- | --- | ---
暂无参数
#### 预执行脚本
```javascript
暂无预执行脚本
```
#### 后执行脚本
```javascript
暂无后执行脚本
```
## /fromless/钱包交易与合约交易信息保存
```text
暂无描述
```
#### 接口状态
> 开发中

#### 接口URL
> 测试环境：http://118.113.15.73:3002/formless-api/nft/market/tra/contract/save
> 
> 正式环境：https://formless.me/api/nft/market/tra/contract/save(完全交付时更改)
#### 请求方式
> POST

#### Content-Type
> json

#### 请求Header参数
参数名 | 示例值 | 参数类型 | 是否必填 | 参数描述
--- | --- | --- | --- | ---
#### 请求Body参数
```javascript
{
    "traFrom": "address",//0x***
    "traTo": "address",//0x***
    "txhash": "0x171096e1a06967d96027677b7c5eb14e44961d9cf5303c95fa691d3bbe914d3f",
    "amount": "6554.1561651651",
    "tokenDecimal":10,
    "methods": "approve",
    "network": "network",//
    "rpc": "https://rinkeby.infura.io/v3/60e51d66a38e4624bfb90643cff08d0b",
    "chainid":"61",
    "traType": "WALLET_TRA"
}
```
参数名 | 示例值 | 参数类型 | 参数描述
--- | --- | --- | ---
traFrom | 0x**** | Text | 发起方
traTo | 0x**** | Text | 接收方
txhash | 0x171096e1a06967d96027677b7c5eb14e44961d9cf5303c95fa691d3bbe914d3f | Text | txHash
amount | 6554.1561651651 | Text | 金额
tokenDecimal | 18 | Text | token精度(非必填)
methods | approve/mint | Text | 方法
network | network | Text | 网络
rpc | rpc | Text | rpc地址
chainid | 61 | Text | 链Id
traType | WALLET_TRA | Text | 交易类型(WALLET_TRA:钱包交易,CONTRACT_TRA:合约交易)
#### 预执行脚本
```javascript
暂无预执行脚本
```
#### 后执行脚本
```javascript
暂无后执行脚本
```
#### 成功响应示例
```javascript
{
	"status": 200,
	"msg": "",
	"data": null
}
```
