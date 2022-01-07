## 一 ：BaseURL:https://formless.me/api/

# 一 ：游戏列表


**接口地址**:`/openApi/game/list`


**请求方式**:`POST`


**请求数据类型**:`application/x-www-form-urlencoded,application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>支持的排序字段 act_yield;yield;act_score;score;act_player_count;player_count ;review_count ;article_count ;sub_count </p>
act真实数据
无act干扰后的排序
* yield 收益率干扰值
* act_yield 真实收益率
* score 评分干扰值
* act_score 真实评分
* player_count 干扰玩家总计
* act_player_count 真实玩家总计
* review_count 评论数
* article_count 贴子数
* sub_count 预约数



**请求示例**:


```javascript
{
  "current": 0,
  "link_type": "",
  "order_items": [
    {
      "asc": true,
      "column": ""
    }
  ],
  "platform_type": "",
  "size": 0,
  "title": "",
  "type_id": 0
}
```


**请求参数**:


**请求参数**:


| 参数名称                       | 参数说明             | 请求类型 | 是否必须 | 数据类型        | schema          |
| ------------------------------ | -------------------- | -------- | -------- | --------------- | --------------- |
| gameInfoQueryVO                | game发行属性         | body     | true     | GameInfoQueryVO | GameInfoQueryVO |
| &emsp;&emsp;current            | 页码                 |          | true    | integer(int64)  |                 |
| &emsp;&emsp;link_type          | 所在链               |          | false    | string          |                 |
| &emsp;&emsp;order_items        | 排序字段列表         |          | false    | array           | OrderItem       |
| &emsp;&emsp;&emsp;&emsp;asc    | 是否是升序           |          | false    | boolean         |                 |
| &emsp;&emsp;&emsp;&emsp;column | 排序字段             |          | false    | string          |                 |
| &emsp;&emsp;platform_type      | 游戏平台             |          | false    | string          |                 |
| &emsp;&emsp;size               | 每页显示结果条目数量 |          | true    | integer(int64)  |                 |
| &emsp;&emsp;title              | 游戏名称             |          | false    | string          |                 |
| &emsp;&emsp;type_id            | 游戏类型             |          | false    | integer(int64)  |                 |


**响应状态**:


| 状态码 | 说明         | schema                    |
| ------ | ------------ | ------------------------- |
| 200    | OK           | RD«IPage«GameInfoListBO»» |
| 201    | Created      |                           |
| 401    | Unauthorized |                           |
| 403    | Forbidden    |                           |
| 404    | Not Found    |                           |


**响应参数**:


| 参数名称                                 | 参数说明                   | 类型                  | schema                |
| ---------------------------------------- | -------------------------- | --------------------- | --------------------- |
| data                                     |                            | IPage«GameInfoListBO» | IPage«GameInfoListBO» |
| &emsp;&emsp;current                      |                            | integer(int64)        |                       |
| &emsp;&emsp;pages                        |                            | integer(int64)        |                       |
| &emsp;&emsp;records                      |                            | array                 | GameInfoListBO        |
| &emsp;&emsp;&emsp;&emsp;act_player_count | 实际玩家数                 | integer               |                       |
| &emsp;&emsp;&emsp;&emsp;act_score        | 实际评分                   | number                |                       |
| &emsp;&emsp;&emsp;&emsp;act_weight       | 实际排序权重               | integer               |                       |
| &emsp;&emsp;&emsp;&emsp;act_yield        | 实际收益率                 | number                |                       |
| &emsp;&emsp;&emsp;&emsp;article_count    | 帖子数                     | integer               |                       |
| &emsp;&emsp;&emsp;&emsp;creator_id       | 发布人ID                   | integer               |                       |
| &emsp;&emsp;&emsp;&emsp;creator_name     | 发布人用户名               | string                |                       |
| &emsp;&emsp;&emsp;&emsp;gid              |                            | integer               |                       |
| &emsp;&emsp;&emsp;&emsp;image_url        | 游戏图标url                | string                |                       |
| &emsp;&emsp;&emsp;&emsp;is_able          | 是否启用,可用值:FALSE,TRUE | string                |                       |
| &emsp;&emsp;&emsp;&emsp;link_type        | 所在链                     | array                 | string                |
| &emsp;&emsp;&emsp;&emsp;platform_type    | 游戏平台                   | array                 | string                |
| &emsp;&emsp;&emsp;&emsp;player_count     | 玩家数                     | integer               |                       |
| &emsp;&emsp;&emsp;&emsp;review_count     | 评论数                     | integer               |                       |
| &emsp;&emsp;&emsp;&emsp;score            | 评分                       | number                |                       |
| &emsp;&emsp;&emsp;&emsp;source           | 来源                       | integer               |                       |
| &emsp;&emsp;&emsp;&emsp;sub_count        | 预约数                     | integer               |                       |
| &emsp;&emsp;&emsp;&emsp;title            | 游戏名称                   | string                |                       |
| &emsp;&emsp;&emsp;&emsp;types            | 游戏类型                   | array                 | string                |
| &emsp;&emsp;&emsp;&emsp;website          | 官网链接                   | string                |                       |
| &emsp;&emsp;&emsp;&emsp;weight           | 排序权重                   | integer               |                       |
| &emsp;&emsp;&emsp;&emsp;yield            | 收益率                     | number                |                       |
| &emsp;&emsp;&emsp;&emsp;zh_CN            |                            | GameInfoListBO        | GameInfoListBO        |
| &emsp;&emsp;size                         |                            | integer(int64)        |                       |
| &emsp;&emsp;total                        |                            | integer(int64)        |                       |
| msg                                      |                            | string                |                       |
| status                                   |                            | integer(int32)        | integer(int32)        |


**响应示例**:
```javascript
{
	"data": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"act_player_count": 0,
				"act_score": 0,
				"act_weight": 0,
				"act_yield": 0,
				"article_count": 0,
				"creator_id": 0,
				"creator_name": "",
				"gid": 0,
				"image_url": "",
				"is_able": "",
				"link_type": [],
				"platform_type": [],
				"player_count": 0,
				"review_count": 0,
				"score": 0,
				"source": 0,
				"sub_count": 0,
				"title": "",
				"types": [],
				"website": "",
				"weight": 0,
				"yield": 0,
				"zh_CN": {
					"act_player_count": 0,
					"act_score": 0,
					"act_weight": 0,
					"act_yield": 0,
					"article_count": 0,
					"creator_id": 0,
					"creator_name": "",
					"gid": 0,
					"image_url": "",
					"is_able": "",
					"link_type": [],
					"platform_type": [],
					"player_count": 0,
					"review_count": 0,
					"score": 0,
					"source": 0,
					"sub_count": 0,
					"title": "",
					"types": [],
					"website": "",
					"weight": 0,
					"yield": 0,
					"zh_CN": {}
				}
			}
		],
		"size": 0,
		"total": 0
	},
	"msg": "",
	"status": 0
}
```






## 二：根据id查询游戏部分详情


**接口地址**:`/openApi/game/searchById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:


**请求参数**:


**请求参数**:


| 参数名称 | 参数说明 | 请求类型 | 是否必须 | 数据类型       | schema |
| -------- | -------- | -------- | -------- | -------------- | ------ |
| id       | id       | query    | true     | integer(int64) |        |


**响应状态**:


| 状态码 | 说明         | schema             |
| ------ | ------------ | ------------------ |
| 200    | OK           | RD«GamePartInfoVo» |
| 401    | Unauthorized |                    |
| 403    | Forbidden    |                    |
| 404    | Not Found    |                    |


**响应参数**:


| 参数名称                | 参数说明 | 类型           | schema         |
| ----------------------- | -------- | -------------- | -------------- |
| data                    |          | GamePartInfoVo | GamePartInfoVo |
| &emsp;&emsp;id          | id       | integer(int64) |                |
| &emsp;&emsp;title       | 游戏名称 | string         |                |
| &emsp;&emsp;token_names | 代币     | array          | string         |
| &emsp;&emsp;types       | 游戏类型 | array          | string         |
| msg                     |          | string         |                |
| status                  |          | integer(int32) | integer(int32) |


**响应示例**:
```javascript
{
	"data": {
		"id": 0,
		"title": "",
		"token_names": [],
		"types": []
	},
	"msg": "",
	"status": 0
}
```








## 三：通过钱包地址查询当前地址关联的用户等级


**接口地址**:`/openApi/infoByPoketAddr`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:


**请求参数**:


**请求参数**:


| 参数名称      | 参数说明 | 请求类型 | 是否必须 | 数据类型       | schema |
| ------------- | -------- | -------- | -------- | -------------- | ------ |
| page          | 页数     | query    | true     | integer(int32) |        |
| size          | 大小     | query    | true     | integer(int32) |        |
| walletAddress | 钱包地址 | query    | false    | string         |        |


**响应状态**:


| 状态码 | 说明         | schema               |
| ------ | ------------ | -------------------- |
| 200    | OK           | RD«IPage«OpenApiVO»» |
| 401    | Unauthorized |                      |
| 403    | Forbidden    |                      |
| 404    | Not Found    |                      |


**响应参数**:


| 参数名称                              | 参数说明 | 类型             | schema                     |
| ------------------------------------- | -------- | ---------------- | -------------------------- |
| data                                  |          | IPage«OpenApiVO» | IPage«OpenApiVO»           |
| &emsp;&emsp;current                   |          | integer(int64)   |                            |
| &emsp;&emsp;pages                     |          | integer(int64)   |                            |
| &emsp;&emsp;records                   |          | array            | OpenApiVO                  |
| &emsp;&emsp;&emsp;&emsp;memberLevel   | 会员等级 | string           | 1青铜，2白银，3黄金，4砖石 |
| &emsp;&emsp;&emsp;&emsp;nickName      | 昵称     | string           |                            |
| &emsp;&emsp;&emsp;&emsp;walletAddress | 钱包地址 | string           |                            |
| &emsp;&emsp;size                      |          | integer(int64)   |                            |
| &emsp;&emsp;total                     |          | integer(int64)   |                            |
| msg                                   |          | string           |                            |
| status                                |          | integer(int32)   | integer(int32)             |


**响应示例**:
```javascript
{
	"data": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"memberLevel": "",
				"nickName": "",
				"walletAddress": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"msg": "",
	"status": 0
}
```







## 四.获取游戏类型列表


**接口地址**:`/openApi/type/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:


**请求参数**:


**请求参数**:


| 参数名称 | 参数说明                         | 请求类型 | 是否必须 | 数据类型 | schema |
| -------- | -------------------------------- | -------- | -------- | -------- | ------ |
| sort     | 排序字段,可用值:gameCount        | query    | false    | string   |        |
| order    | 升序ASC/降序DESC,可用值:ASC,DESC | query    | false    | string   |        |


**响应状态**:


| 状态码 | 说明         | schema                |
| ------ | ------------ | --------------------- |
| 200    | OK           | RD«List«GameTypeDTO»» |
| 401    | Unauthorized |                       |
| 403    | Forbidden    |                       |
| 404    | Not Found    |                       |


**响应参数**:


| 参数名称              | 参数说明             | 类型           | schema         |
| --------------------- | -------------------- | -------------- | -------------- |
| data                  |                      | array          | GameTypeDTO    |
| &emsp;&emsp;gameCount | 游戏数               | integer(int32) |                |
| &emsp;&emsp;id        | id                   | integer(int64) |                |
| &emsp;&emsp;status    | 状态 (0.正常 1.禁用) | integer(int32) |                |
| &emsp;&emsp;typeIcon  | 图标                 | string         |                |
| &emsp;&emsp;typeName  | 类型名称             | string         |                |
| &emsp;&emsp;zh_CN     | 中文                 | GameTypeDTO    | GameTypeDTO    |
| msg                   |                      | string         |                |
| status                |                      | integer(int32) | integer(int32) |


**响应示例**:
```javascript
{
	"data": [
		{
			"gameCount": 0,
			"id": 0,
			"status": 0,
			"typeIcon": "",
			"typeName": "",
			"zh_CN": {
				"gameCount": 0,
				"id": 0,
				"status": 0,
				"typeIcon": "",
				"typeName": "",
				"zh_CN": {}
			}
		}
	],
	"msg": "",
	"status": 0
}
```






## 五.后台搜索可用游戏标签列表


**接口地址**:`/openApi/label/search`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:


**请求参数**:


**请求参数**:


| 参数名称 | 参数说明 | 请求类型 | 是否必须 | 数据类型 | schema |
| -------- | -------- | -------- | -------- | -------- | ------ |
| keyword  | keyword  | query    | true     | string   |        |


**响应状态**:


| 状态码 | 说明         | schema                 |
| ------ | ------------ | ---------------------- |
| 200    | OK           | RD«List«GameLabelDTO»» |
| 401    | Unauthorized |                        |
| 403    | Forbidden    |                        |
| 404    | Not Found    |                        |


**响应参数**:


| 参数名称              | 参数说明 | 类型           | schema         |
| --------------------- | -------- | -------------- | -------------- |
| data                  |          | array          | GameLabelDTO   |
| &emsp;&emsp;addHeat   | 附加热度 | integer(int32) |                |
| &emsp;&emsp;gameCount | 游戏数   | integer(int32) |                |
| &emsp;&emsp;gameHeat  | 总热度   | integer(int32) |                |
| &emsp;&emsp;id        | id       | integer(int64) |                |
| &emsp;&emsp;labelName | 标签名称 | string         |                |
| &emsp;&emsp;realHeat  | 真实热度 | integer(int32) |                |
| &emsp;&emsp;zh_CN     | 中文     | GameLabelDTO   | GameLabelDTO   |
| msg                   |          | string         |                |
| status                |          | integer(int32) | integer(int32) |


**响应示例**:
```javascript
{
	"data": [
		{
			"addHeat": 0,
			"gameCount": 0,
			"gameHeat": 0,
			"id": 0,
			"labelName": "",
			"realHeat": 0,
			"zh_CN": {
				"addHeat": 0,
				"gameCount": 0,
				"gameHeat": 0,
				"id": 0,
				"labelName": "",
				"realHeat": 0,
				"zh_CN": {}
			}
		}
	],
	"msg": "",
	"status": 0
}
```
