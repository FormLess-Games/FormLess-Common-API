# FormLess-Common-API

## 获取指定币种汇率
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
		},
		{
			"id": 43,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "EUR",
			"toCurrencyName": "Euro",
			"exchangeRate": "0.86370000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:19:03.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 44,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "FJD",
			"toCurrencyName": "Fijian Dollar",
			"exchangeRate": "2.07500000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:19:05.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 45,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "FKP",
			"toCurrencyName": "Falkland Islands Pound",
			"exchangeRate": "0.73400000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:18:03.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 46,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "GBP",
			"toCurrencyName": "British Pound Sterling",
			"exchangeRate": "0.73340000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:17:08.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 47,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "GEL",
			"toCurrencyName": "Georgian Lari",
			"exchangeRate": "3.11980000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:18:08.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 48,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "GHS",
			"toCurrencyName": "Ghanaian Cedi",
			"exchangeRate": "5.97950000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:18:06.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 49,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "GIP",
			"toCurrencyName": "Gibraltar Pound",
			"exchangeRate": "0.73420000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:17:02.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 50,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "GMD",
			"toCurrencyName": "Gambian Dalasi",
			"exchangeRate": "51.25000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:18:09.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 51,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "GNF",
			"toCurrencyName": "Guinean Franc",
			"exchangeRate": "9703.00000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:16:09.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 52,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "GTQ",
			"toCurrencyName": "Guatemalan Quetzal",
			"exchangeRate": "7.73100000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:16:04.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 53,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "GYD",
			"toCurrencyName": "Guyanaese Dollar",
			"exchangeRate": "207.98000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:16:10.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 54,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "HKD",
			"toCurrencyName": "Hong Kong Dollar",
			"exchangeRate": "7.78420000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:17:07.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 55,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "HNL",
			"toCurrencyName": "Honduran Lempira",
			"exchangeRate": "24.04340000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:17:04.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 56,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "HRK",
			"toCurrencyName": "Croatian Kuna",
			"exchangeRate": "6.48990000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:17:06.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 57,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "HTG",
			"toCurrencyName": "Haitian Gourde",
			"exchangeRate": "98.00000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:16:02.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 58,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "HUF",
			"toCurrencyName": "Hungarian Forint",
			"exchangeRate": "311.67000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:15:07.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 60,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "IDR",
			"toCurrencyName": "Indonesian Rupiah",
			"exchangeRate": "14220.00000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:15:05.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 61,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "ILS",
			"toCurrencyName": "Israeli New Sheqel",
			"exchangeRate": "3.23100000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:15:04.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 62,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "INR",
			"toCurrencyName": "Indian Rupee",
			"exchangeRate": "75.11700000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:16:05.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 63,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "IQD",
			"toCurrencyName": "Iraqi Dinar",
			"exchangeRate": "1459.00000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:15:09.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 64,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "IRR",
			"toCurrencyName": "Iranian Rial",
			"exchangeRate": "42000.00000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:11:13.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 65,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "ISK",
			"toCurrencyName": "Icelandic Krona",
			"exchangeRate": "129.00000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:10:02.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 67,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "JMD",
			"toCurrencyName": "Jamaican Dollar",
			"exchangeRate": "147.41000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:11:09.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 68,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "JOD",
			"toCurrencyName": "Jordanian Dinar",
			"exchangeRate": "0.70780000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:10:09.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 69,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "JPY",
			"toCurrencyName": "Japanese Yen",
			"exchangeRate": "112.23800000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:10:10.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 70,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "KES",
			"toCurrencyName": "Kenyan Shilling",
			"exchangeRate": "110.65000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:12:12.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 71,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "KGS",
			"toCurrencyName": "Kyrgystani Som",
			"exchangeRate": "84.76690000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:11:02.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 72,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "KHR",
			"toCurrencyName": "Cambodian Riel",
			"exchangeRate": "4067.00000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:11:10.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 73,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "KMF",
			"toCurrencyName": "Comorian Franc",
			"exchangeRate": "425.33000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:12:08.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 74,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "KPW",
			"toCurrencyName": "North Korean Won",
			"exchangeRate": "900.00000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:13:08.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 75,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "KRW",
			"toCurrencyName": "South Korean Won",
			"exchangeRate": "1196.49000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:12:04.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 76,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "KWD",
			"toCurrencyName": "Kuwaiti Dinar",
			"exchangeRate": "0.30110000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:12:10.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 77,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "KYD",
			"toCurrencyName": "Cayman Islands Dollar",
			"exchangeRate": "0.82000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:13:05.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 78,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "KZT",
			"toCurrencyName": "Kazakhstani Tenge",
			"exchangeRate": "424.98000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:15:02.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 79,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "LAK",
			"toCurrencyName": "Laotian Kip",
			"exchangeRate": "10013.59960000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:13:02.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 80,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "LBP",
			"toCurrencyName": "Lebanese Pound",
			"exchangeRate": "1505.70000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:13:07.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 81,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "LKR",
			"toCurrencyName": "Sri Lankan Rupee",
			"exchangeRate": "199.50000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:14:07.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 82,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "LRD",
			"toCurrencyName": "Liberian Dollar",
			"exchangeRate": "169.52000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:14:11.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 83,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "LSL",
			"toCurrencyName": "Lesotho Loti",
			"exchangeRate": "14.93000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:14:02.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 84,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "LYD",
			"toCurrencyName": "Libyan Dinar",
			"exchangeRate": "4.54690000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:14:08.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 85,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "MAD",
			"toCurrencyName": "Moroccan Dirham",
			"exchangeRate": "9.06700000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:14:04.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 86,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "MDL",
			"toCurrencyName": "Moldovan Leu",
			"exchangeRate": "17.31500000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:13:03.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 87,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "MGA",
			"toCurrencyName": "Malagasy Ariary",
			"exchangeRate": "3870.00000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:12:05.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 88,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "MKD",
			"toCurrencyName": "Macedonian Denar",
			"exchangeRate": "53.09000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:11:06.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 89,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "MMK",
			"toCurrencyName": "Myanma Kyat",
			"exchangeRate": "1930.00000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:09:03.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 90,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "MNT",
			"toCurrencyName": "Mongolian Tugrik",
			"exchangeRate": "2848.89000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:09:04.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 91,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "MOP",
			"toCurrencyName": "Macanese Pataca",
			"exchangeRate": "8.01740000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:10:03.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 92,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "MRO",
			"toCurrencyName": "Mauritanian Ouguiya (pre-2018)",
			"exchangeRate": "355.00000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:08:09.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 93,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "MRU",
			"toCurrencyName": "Mauritanian Ouguiya",
			"exchangeRate": "36.03000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:08:04.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 94,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "MUR",
			"toCurrencyName": "Mauritian Rupee",
			"exchangeRate": "42.45000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:09:06.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 95,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "MVR",
			"toCurrencyName": "Maldivian Rufiyaa",
			"exchangeRate": "15.57000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:09:08.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 96,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "MWK",
			"toCurrencyName": "Malawian Kwacha",
			"exchangeRate": "807.51000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:10:07.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 97,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "MXN",
			"toCurrencyName": "Mexican Peso",
			"exchangeRate": "20.71500000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:09:02.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 98,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "MYR",
			"toCurrencyName": "Malaysian Ringgit",
			"exchangeRate": "4.17600000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:06:04.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 99,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "MZN",
			"toCurrencyName": "Mozambican Metical",
			"exchangeRate": "63.23000000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:07:02.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 100,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "NAD",
			"toCurrencyName": "Namibian Dollar",
			"exchangeRate": "14.95320000",
			"createTime": "2021-09-22T10:59:42.000+00:00",
			"updateTime": "2021-10-11T00:06:07.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 101,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "NGN",
			"toCurrencyName": "Nigerian Naira",
			"exchangeRate": "409.81000000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:07:04.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 102,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "NOK",
			"toCurrencyName": "Norwegian Krone",
			"exchangeRate": "8.55410000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:06:08.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 103,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "NPR",
			"toCurrencyName": "Nepalese Rupee",
			"exchangeRate": "119.90000000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:07:10.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 104,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "NZD",
			"toCurrencyName": "New Zealand Dollar",
			"exchangeRate": "1.44330000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:06:09.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 105,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "OMR",
			"toCurrencyName": "Omani Rial",
			"exchangeRate": "0.38500000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:08:02.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 106,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "PAB",
			"toCurrencyName": "Panamanian Balboa",
			"exchangeRate": "1.00000000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:07:08.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 107,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "PEN",
			"toCurrencyName": "Peruvian Nuevo Sol",
			"exchangeRate": "4.11980000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:08:07.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 108,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "PGK",
			"toCurrencyName": "Papua New Guinean Kina",
			"exchangeRate": "3.51610000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:08:06.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 109,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "PHP",
			"toCurrencyName": "Philippine Peso",
			"exchangeRate": "50.57000000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:07:05.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 110,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "PKR",
			"toCurrencyName": "Pakistani Rupee",
			"exchangeRate": "170.26000000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:01:03.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 111,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "PLN",
			"toCurrencyName": "Polish Zloty",
			"exchangeRate": "3.97890000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:01:10.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 112,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "PYG",
			"toCurrencyName": "Paraguayan Guarani",
			"exchangeRate": "6896.02000000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:02:08.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 113,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "QAR",
			"toCurrencyName": "Qatari Rial",
			"exchangeRate": "3.64000000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:02:05.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 114,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "RON",
			"toCurrencyName": "Romanian Leu",
			"exchangeRate": "4.27570000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:01:05.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 115,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "RSD",
			"toCurrencyName": "Serbian Dinar",
			"exchangeRate": "101.46920000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:02:02.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 116,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "RUB",
			"toCurrencyName": "Russian Ruble",
			"exchangeRate": "71.60000000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:03:02.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 118,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "RWF",
			"toCurrencyName": "Rwandan Franc",
			"exchangeRate": "989.29000000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:02:03.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 119,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "SAR",
			"toCurrencyName": "Saudi Riyal",
			"exchangeRate": "3.75020000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:03:05.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 121,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "SCR",
			"toCurrencyName": "Seychellois Rupee",
			"exchangeRate": "14.18280000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:02:09.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 122,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "SDG",
			"toCurrencyName": "Sudanese Pound",
			"exchangeRate": "439.00200000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:03:04.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 124,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "SEK",
			"toCurrencyName": "Swedish Krona",
			"exchangeRate": "8.74038000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:03:07.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 125,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "SGD",
			"toCurrencyName": "Singapore Dollar",
			"exchangeRate": "1.35492000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:03:06.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 127,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "SHP",
			"toCurrencyName": "Saint Helena Pound",
			"exchangeRate": "0.73420000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:04:04.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 128,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "SLL",
			"toCurrencyName": "Sierra Leonean Leone",
			"exchangeRate": "10540.10000000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:04:02.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 129,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "SOS",
			"toCurrencyName": "Somali Shilling",
			"exchangeRate": "571.00000000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:04:10.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 130,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "SRD",
			"toCurrencyName": "Surinamese Dollar",
			"exchangeRate": "21.29000000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:05:02.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 131,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "SYP",
			"toCurrencyName": "Syrian Pound",
			"exchangeRate": "2510.00000000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:04:06.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 132,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "SZL",
			"toCurrencyName": "Swazi Lilangeni",
			"exchangeRate": "14.93600000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:05:08.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 133,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "THB",
			"toCurrencyName": "Thai Baht",
			"exchangeRate": "33.87100000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:04:07.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 134,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "TJS",
			"toCurrencyName": "Tajikistani Somoni",
			"exchangeRate": "11.29450000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:05:05.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 135,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "TMT",
			"toCurrencyName": "Turkmenistani Manat",
			"exchangeRate": "3.36000000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:05:12.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 136,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "TND",
			"toCurrencyName": "Tunisian Dinar",
			"exchangeRate": "2.82750000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:05:10.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 137,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "TOP",
			"toCurrencyName": "Tongan Pa'anga",
			"exchangeRate": "2.26150000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:06:02.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 138,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "TRY",
			"toCurrencyName": "Turkish Lira",
			"exchangeRate": "8.95940000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:01:02.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 139,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "TTD",
			"toCurrencyName": "Trinidad and Tobago Dollar",
			"exchangeRate": "6.75440000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:28:17.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 140,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "TWD",
			"toCurrencyName": "New Taiwan Dollar",
			"exchangeRate": "28.08000000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:29:11.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 141,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "TZS",
			"toCurrencyName": "Tanzanian Shilling",
			"exchangeRate": "2295.00000000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:28:14.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 142,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "UAH",
			"toCurrencyName": "Ukrainian Hryvnia",
			"exchangeRate": "26.32000000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:29:02.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 143,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "UGX",
			"toCurrencyName": "Ugandan Shilling",
			"exchangeRate": "3573.80000000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:29:08.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 144,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "USD",
			"toCurrencyName": "United States Dollar",
			"exchangeRate": "1.00000000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:00:10.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 145,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "UYU",
			"toCurrencyName": "Uruguayan Peso",
			"exchangeRate": "43.29600000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:29:15.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 146,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "UZS",
			"toCurrencyName": "Uzbekistan Som",
			"exchangeRate": "10672.89000000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:01:09.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 147,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "VND",
			"toCurrencyName": "Vietnamese Dong",
			"exchangeRate": "22755.00000000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:30:21.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 148,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "VUV",
			"toCurrencyName": "Vanuatu Vatu",
			"exchangeRate": "110.35000000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:30:32.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 150,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "WST",
			"toCurrencyName": "Samoan Tala",
			"exchangeRate": "2.57280000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:00:13.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 151,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "XAF",
			"toCurrencyName": "CFA Franc BEAC",
			"exchangeRate": "566.65000000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:29:10.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 152,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "XCD",
			"toCurrencyName": "East Caribbean Dollar",
			"exchangeRate": "2.70000000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:00:16.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 153,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "XDR",
			"toCurrencyName": "Special Drawing Rights",
			"exchangeRate": "0.70878400",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:28:03.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 154,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "XOF",
			"toCurrencyName": "CFA Franc BCEAO",
			"exchangeRate": "566.65000000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:28:11.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 155,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "XPF",
			"toCurrencyName": "CFP Franc",
			"exchangeRate": "102.80000000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:27:16.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 156,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "YER",
			"toCurrencyName": "Yemeni Rial",
			"exchangeRate": "250.00000000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:00:06.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 157,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "ZAR",
			"toCurrencyName": "South African Rand",
			"exchangeRate": "14.92725000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:27:09.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 158,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "ZMW",
			"toCurrencyName": "Zambian Kwacha",
			"exchangeRate": "17.05000000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:28:08.000+00:00",
			"strikeOut": 0
		},
		{
			"id": 159,
			"fromCurrencyCode": "USD",
			"fromCurrencyName": "United States Dollar",
			"toCurrencyCode": "ZWL",
			"toCurrencyName": "Zimbabwean Dollar",
			"exchangeRate": "321.00000000",
			"createTime": "2021-09-22T10:59:43.000+00:00",
			"updateTime": "2021-10-11T00:00:18.000+00:00",
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
