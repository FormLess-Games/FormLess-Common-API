# FormLess-Common-API

## 获取指定币种汇率 测试环境地址:http://118.113.15.73:3002
```text
暂无描述
```


#### 接口URL
> http://118.113.15.73:3002/formless-api/exchangeRate/getByCode?code=CNY

#### 请求方式
> GET

#### Content-Type
> form-data

#### 请求Query参数
参数名 | 示例值 | 参数类型 | 是否必填 | 参数描述
--- | --- | --- | --- | ---
code | CNY | Text | 是 | 币种名，参考所有币种中币种名

#### 成功响应示例
```javascript
{
	"status": 200,
	"msg": "",
	"data": {
		"id": 31,
		"fromCurrencyCode": "USD",
		"fromCurrencyName": "United States Dollar",
		"toCurrencyCode": "CNY",
		"toCurrencyName": "Chinese Yuan",
		"exchangeRate": "6.44410000",
		"createTime": "2021-09-22T10:59:42.000+00:00",
		"updateTime": "2021-10-11T00:22:09.000+00:00",
		"strikeOut": 0
	}
}
```

参数名 | 示例值 | 参数类型 | 参数描述
--- | --- | --- | ---
status | 200 | Text | 
msg | - | Text | 返回文字描述
data | - | Text | 返回数据
data.id | 31 | Text | 
data.fromCurrencyCode | USD | Text | 兑换币种
data.fromCurrencyName | United States Dollar | Text | 兑换币种详细名
data.toCurrencyCode | CNY | Text | 目标币种
data.toCurrencyName | Chinese Yuan | Text | 目标币种详细名
data.exchangeRate | 6.44410000 | Text | 汇率
data.createTime | 2021-09-22T10:59:42.000+00:00 | Text | 
data.updateTime | 2021-10-11T00:22:09.000+00:00 | Text | 时间
data.strikeOut | 0 | Text | 
## /链游api/获取所有实体币种汇率

#### 接口URL
> http://118.113.15.73:3002/formless-api/exchangeRate/list

#### 请求方式
> GET

#### Content-Type
> form-data

#### 成功响应示例
```javascript
{
	"status": 200,
	"msg": "",
	"data": [
		{
			"id": 1,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "AED",
			"toCurrencyName": "United Arab Emirates Dirham",
			"exchangeRate": "3.67280000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:27:14.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 2,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "AFN",
			"toCurrencyName": "Afghan Afghani",
			"exchangeRate": "90.61000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:26:15.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 3,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "ALL",
			"toCurrencyName": "Albanian Lek",
			"exchangeRate": "104.55000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:26:17.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 4,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "AMD",
			"toCurrencyName": "Armenian Dram",
			"exchangeRate": "478.80000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:27:02.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 5,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "ANG",
			"toCurrencyName": "Netherlands Antillean Guilder",
			"exchangeRate": "1.78500000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:27:07.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 6,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "AOA",
			"toCurrencyName": "Angolan Kwanza",
			"exchangeRate": "593.38800000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:26:12.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 7,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "ARS",
			"toCurrencyName": "Argentine Peso",
			"exchangeRate": "98.85000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:25:03.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 8,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "AUD",
			"toCurrencyName": "Australian Dollar",
			"exchangeRate": "1.36810000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:25:08.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 9,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "AWG",
			"toCurrencyName": "Aruban Florin",
			"exchangeRate": "1.78000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:25:07.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 10,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "AZN",
			"toCurrencyName": "Azerbaijani Manat",
			"exchangeRate": "1.69950000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:25:10.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 11,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "BAM",
			"toCurrencyName": "Bosnia-Herzegovina Convertible Mark",
			"exchangeRate": "1.69340000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:26:03.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 12,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "BBD",
			"toCurrencyName": "Barbadian Dollar",
			"exchangeRate": "2.00000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:26:09.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 13,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "BDT",
			"toCurrencyName": "Bangladeshi Taka",
			"exchangeRate": "84.72000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:22:08.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 14,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "BGN",
			"toCurrencyName": "Bulgarian Lev",
			"exchangeRate": "1.69058000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:23:03.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 15,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "BHD",
			"toCurrencyName": "Bahraini Dinar",
			"exchangeRate": "0.37700000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:23:08.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 16,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "BIF",
			"toCurrencyName": "Burundian Franc",
			"exchangeRate": "1976.61000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:23:13.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 17,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "BMD",
			"toCurrencyName": "Bermudan Dollar",
			"exchangeRate": "1.00000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:23:05.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 18,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "BND",
			"toCurrencyName": "Brunei Dollar",
			"exchangeRate": "1.35280000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:24:07.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 19,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "BOB",
			"toCurrencyName": "Bolivian Boliviano",
			"exchangeRate": "6.86000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:24:11.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 20,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "BRL",
			"toCurrencyName": "Brazilian Real",
			"exchangeRate": "5.50610000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:24:04.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 21,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "BSD",
			"toCurrencyName": "Bahamian Dollar",
			"exchangeRate": "1.00000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:24:15.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 22,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "BTN",
			"toCurrencyName": "Bhutanese Ngultrum",
			"exchangeRate": "74.82000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:24:13.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 23,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "BWP",
			"toCurrencyName": "Botswanan Pula",
			"exchangeRate": "11.29440000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:25:05.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 24,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "BZD",
			"toCurrencyName": "Belize Dollar",
			"exchangeRate": "1.99780000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:23:10.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 25,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "CAD",
			"toCurrencyName": "Canadian Dollar",
			"exchangeRate": "1.24715000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:21:04.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 26,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "CDF",
			"toCurrencyName": "Congolese Franc",
			"exchangeRate": "1980.58000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:22:02.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 27,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "CHF",
			"toCurrencyName": "Swiss Franc",
			"exchangeRate": "0.92620000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:21:06.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 28,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "CLF",
			"toCurrencyName": "Chilean Unit of Account UF",
			"exchangeRate": "0.02711000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:21:10.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 29,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "CLP",
			"toCurrencyName": "Chilean Peso",
			"exchangeRate": "824.00000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:22:06.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 30,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "CNH",
			"toCurrencyName": "Chinese Yuan Offshore",
			"exchangeRate": "6.44305000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:22:04.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 31,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "CNY",
			"toCurrencyName": "Chinese Yuan",
			"exchangeRate": "6.44410000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:22:09.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 32,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "COP",
			"toCurrencyName": "Colombian Peso",
			"exchangeRate": "3764.88000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:20:12.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 33,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "CUP",
			"toCurrencyName": "Cuban Peso",
			"exchangeRate": "25.00000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:20:05.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 34,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "CVE",
			"toCurrencyName": "Cape Verdean Escudo",
			"exchangeRate": "95.25000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:21:03.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 35,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "CZK",
			"toCurrencyName": "Czech Republic Koruna",
			"exchangeRate": "21.96920000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:20:01.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 36,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "DJF",
			"toCurrencyName": "Djiboutian Franc",
			"exchangeRate": "177.50000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:20:09.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 37,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "DKK",
			"toCurrencyName": "Danish Krone",
			"exchangeRate": "6.42850000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:21:02.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 38,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "DOP",
			"toCurrencyName": "Dominican Peso",
			"exchangeRate": "56.26000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:20:03.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 39,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "DZD",
			"toCurrencyName": "Algerian Dinar",
			"exchangeRate": "137.09300000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:19:02.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 40,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "EGP",
			"toCurrencyName": "Egyptian Pound",
			"exchangeRate": "15.66000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:19:10.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 41,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "ERN",
			"toCurrencyName": "Eritrean Nakfa",
			"exchangeRate": "15.07000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:19:06.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 42,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "ETB",
			"toCurrencyName": "Ethiopian Birr",
			"exchangeRate": "46.33000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:18:11.000+00:00",
			"strikeOut": 0
		}
	]
}
```
参数名 | 示例值 | 参数类型 | 参数描述
--- | --- | --- | ---
status | 200 | Text | 
msg | - | Text | 返回文字描述
data | - | Text | 返回数据
data.id | 1 | Text | 
data.fromCurrencyCode | USD | Text | 兑换币种
data.fromCurrencyName | United States Dollar | Text | 兑换币种详细名
data.toCurrencyCode | AED | Text | 目标币种
data.toCurrencyName | United Arab Emirates Dirham | Text | 目标币种详细名
data.exchangeRate | 3.67280000 | Text | 汇率
data.createTime | 2021-09-22T10:59:42.000+00:00 | Text | 
data.updateTime | 2021-10-11T00:27:14.000+00:00 | Text | 时间
data.strikeOut | 0 | Text | 
## /链游api/查看钱包默认币种
```text
暂无描述
```


#### 接口URL
> http://118.113.15.73:3002/formless-api/config/list

#### 请求方式
> GET

#### Content-Type
> form-data


#### 成功响应示例
```javascript
{
	"status": 200,
	"msg": "",
	"data": [
		{
			"cat_wllet": [
				{
					"ethereum": [
						{
							"coinName": " wbtc",
							"token": "0x2260fac5e5542a773aa44fbcfedf7c193bc2c599"
						},
						{
							"coinName": "usdt",
							"token": "0xdac17f958d2ee523a2206206994597c13d831ec7"
						},
						{
							"coinName": "xrp",
							"token": "以太查不到"
						},
						{
							"coinName": "link",
							"token": "0x514910771af9ca656af840dff83e8264ecf986ca"
						}
					]
				},
				{
					"ploygon": [
						{
							"coinName": " wbtc",
							"token": "0x1bfd67037b42cf73acf2047067bd4f2c47d9bfd6"
						},
						{
							"coinName": "weth",
							"token": "0x7ceb23fd6bc0add59e62ac25578270cff1b9f619"
						},
						{
							"coinName": "matic",
							"token": "REC-20查不到，具体问下合约web3查询方式"
						},
						{
							"coinName": "usdt",
							"token": "0xc2132d05d31c914a87c6611c10748aeb04b58e8f"
						},
						{
							"coinName": "usdc",
							"token": "0x2791bca1f2de4661ed88a30c99a7a9449aa84174"
						},
						{
							"coinName": "link",
							"token": "0x53e0bca35ec356bd5dddfebbd1fc0fd03fabad39"
						}
					]
				},
				{
					"flow": [
						{
							"coinName": " flow",
							"token": ""
						},
						{
							"coinName": "fusd",
							"token": ""
						},
						{
							"coinName": "tusdt",
							"token": ""
						}
					]
				}
			]
		}
	]
}
```
参数名 | 示例值 | 参数类型 | 参数描述
--- | --- | --- | ---
status | 200 | Text | 
msg | - | Text | 返回文字描述
data | - | Text | 返回数据
data.cat_wllet | - | Text | 查看钱包初始值
data.cat_wllet.ethereum | - | Text | 链类型
data.cat_wllet.ethereum.coinName |  wbtc | Text | 币种名
data.cat_wllet.ethereum.token | 0x2260fac5e5542a773aa44fbcfedf7c193bc2c599 | Text | 币种凭证id
