## 分页获取板块内主题

baseURL:https://formless.me/api

**接口地址**:`/forum/topic/page`


**请求方式**:`POST`


**请求数据类型**:`application/x-www-form-urlencoded,application/json`


**响应数据类型**:`*/*`


**接口描述**:


**请求示例**:


```javascript
{
  "forumLabelId": 0,
  "forumModuleId": 0,
  "keyword": "",
  "page": 0,
  "size": 0,
  "sort": ""
}
```


**请求参数**:


**请求参数**:


| 参数名称                  | 参数说明                                                     | 请求类型 | 是否必须 | 数据类型         | schema           |
| ------------------------- | ------------------------------------------------------------ | -------- | -------- | ---------------- | ---------------- |
| forumTopicPageVO          | ForumTopicPageVO                                             | body     | true     | ForumTopicPageVO | ForumTopicPageVO |
| &emsp;&emsp;forumLabelId  | 论坛标签id(子版块)                                           |          | false    | integer(int64)   |                  |
| &emsp;&emsp;forumModuleId | 论坛板块id                                                   |          | true     | integer(int64)   |                  |
| &emsp;&emsp;keyword       | 搜索关键字                                                   |          | false    | string           |                  |
| &emsp;&emsp;page          | 页数                                                         |          | true     | integer(int32)   |                  |
| &emsp;&emsp;size          | 每页条数                                                     |          | true     | integer(int32)   |                  |
| &emsp;&emsp;sort          | 排序方式(HOT热门,REPLYTIME恢复时间,CREATETIME发布时间),可用值:CREATETIME,HOT,REPLYTIME |          | false    | string           |                  |


**响应状态**:


| 状态码 | 说明         | schema                  |
| ------ | ------------ | ----------------------- |
| 200    | OK           | RD«Page«ForumTopicDTO»» |
| 201    | Created      |                         |
| 401    | Unauthorized |                         |
| 403    | Forbidden    |                         |
| 404    | Not Found    |                         |


**响应参数**:


| 参数名称                                           | 参数说明                     | 类型                | schema              |
| -------------------------------------------------- | ---------------------------- | ------------------- | ------------------- |
| data                                               |                              | Page«ForumTopicDTO» | Page«ForumTopicDTO» |
| &emsp;&emsp;countId                                |                              | string              |                     |
| &emsp;&emsp;current                                |                              | integer(int64)      |                     |
| &emsp;&emsp;maxLimit                               |                              | integer(int64)      |                     |
| &emsp;&emsp;optimizeCountSql                       |                              | boolean             |                     |
| &emsp;&emsp;orders                                 |                              | array               | OrderItem           |
| &emsp;&emsp;&emsp;&emsp;asc                        |                              | boolean             |                     |
| &emsp;&emsp;&emsp;&emsp;column                     |                              | string              |                     |
| &emsp;&emsp;pages                                  |                              | integer(int64)      |                     |
| &emsp;&emsp;records                                |                              | array               | ForumTopicDTO       |
| &emsp;&emsp;&emsp;&emsp;collectCount               | 收藏数                       | integer             |                     |
| &emsp;&emsp;&emsp;&emsp;commentCount               | 评论数                       | integer             |                     |
| &emsp;&emsp;&emsp;&emsp;commentTime                | 最后评论时间                 | string              |                     |
| &emsp;&emsp;&emsp;&emsp;comments                   | 主题回复                     | array               | ForumCommentDTO     |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;childComments  |                              | array               | ForumCommentDTO     |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;commentCount   | 评论数                       | integer             |                     |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;content        | 回复内容                     | string              |                     |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;createTime     | 创建时间                     | string              |                     |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;formatDate     |                              | string              |                     |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;forumCommentId | 所属评论id                   | integer             |                     |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;forumTopocId   | 论坛主题id                   | integer             |                     |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;id             | 论坛评论id                   | integer             |                     |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;isUp           | 该用户是否点赞该记录         | integer             |                     |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;toUserHeadImg  | 回复用户图像                 | string              |                     |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;toUserId       | 回复用户id                   | integer             |                     |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;toUserName     | 回复用户名称                 | string              |                     |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;upCount        | 点赞数                       | integer             |                     |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;userHeadImg    | 用户头像                     | string              |                     |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;userId         | 用户id                       | integer             |                     |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;userName       | 用户名称                     | string              |                     |
| &emsp;&emsp;&emsp;&emsp;content                    | 帖子内容                     | string              |                     |
| &emsp;&emsp;&emsp;&emsp;contentText                | 帖子纯文本内容               | string              |                     |
| &emsp;&emsp;&emsp;&emsp;createTime                 | 创建时间                     | string              |                     |
| &emsp;&emsp;&emsp;&emsp;formatDate                 | 格式化时间                   | string              |                     |
| &emsp;&emsp;&emsp;&emsp;forumModuleId              | 论坛板块id                   | string              |                     |
| &emsp;&emsp;&emsp;&emsp;gameId                     | 游戏id                       | integer             |                     |
| &emsp;&emsp;&emsp;&emsp;gameImages                 | 游戏图像                     | string              |                     |
| &emsp;&emsp;&emsp;&emsp;gameTitle                  | 游戏标题                     | string              |                     |
| &emsp;&emsp;&emsp;&emsp;id                         | 主题id                       | integer             |                     |
| &emsp;&emsp;&emsp;&emsp;isGreat                    | 是否精华(1.是 0.否)          | integer             |                     |
| &emsp;&emsp;&emsp;&emsp;isTop                      | 是否置顶(1.是 0.否)          | integer             |                     |
| &emsp;&emsp;&emsp;&emsp;isUp                       | 该用户是否点赞该记录1.是0.否 | integer             |                     |
| &emsp;&emsp;&emsp;&emsp;labelId                    | 论坛子板块id                 | integer             |                     |
| &emsp;&emsp;&emsp;&emsp;labelName                  | 论坛子板块名称               | string              |                     |
| &emsp;&emsp;&emsp;&emsp;title                      | 帖子标题                     | string              |                     |
| &emsp;&emsp;&emsp;&emsp;topicCount                 | 论坛帖子数                   | integer             |                     |
| &emsp;&emsp;&emsp;&emsp;upCount                    | 点赞数                       | integer             |                     |
| &emsp;&emsp;&emsp;&emsp;userHeadImg                | 发帖用户头像                 | string              |                     |
| &emsp;&emsp;&emsp;&emsp;userId                     | 用户id                       | integer             |                     |
| &emsp;&emsp;&emsp;&emsp;userName                   | 发帖用户名称                 | string              |                     |
| &emsp;&emsp;&emsp;&emsp;viewCount                  | 浏览数                       | integer             |                     |
| &emsp;&emsp;searchCount                            |                              | boolean             |                     |
| &emsp;&emsp;size                                   |                              | integer(int64)      |                     |
| &emsp;&emsp;total                                  |                              | integer(int64)      |                     |
| msg                                                |                              | string              |                     |
| status                                             |                              | integer(int32)      | integer(int32)      |


**响应示例**:
```javascript
{
	"data": {
		"countId": "",
		"current": 0,
		"maxLimit": 0,
		"optimizeCountSql": true,
		"orders": [
			{
				"asc": true,
				"column": ""
			}
		],
		"pages": 0,
		"records": [
			{
				"collectCount": 0,
				"commentCount": 0,
				"commentTime": "",
				"comments": [
					{
						"childComments": [
							{
								"childComments": [
									{}
								],
								"commentCount": 0,
								"content": "",
								"createTime": "",
								"formatDate": "",
								"forumCommentId": 0,
								"forumTopocId": 0,
								"id": 0,
								"isUp": 0,
								"toUserHeadImg": "",
								"toUserId": 0,
								"toUserName": "",
								"upCount": 0,
								"userHeadImg": "",
								"userId": 0,
								"userName": ""
							}
						],
						"commentCount": 0,
						"content": "",
						"createTime": "",
						"formatDate": "",
						"forumCommentId": 0,
						"forumTopocId": 0,
						"id": 0,
						"isUp": 0,
						"toUserHeadImg": "",
						"toUserId": 0,
						"toUserName": "",
						"upCount": 0,
						"userHeadImg": "",
						"userId": 0,
						"userName": ""
					}
				],
				"content": "",
				"contentText": "",
				"createTime": "",
				"formatDate": "",
				"forumModuleId": "",
				"gameId": 0,
				"gameImages": "",
				"gameTitle": "",
				"id": 0,
				"isGreat": 0,
				"isTop": 0,
				"isUp": 0,
				"labelId": 0,
				"labelName": "",
				"title": "",
				"topicCount": 0,
				"upCount": 0,
				"userHeadImg": "",
				"userId": 0,
				"userName": "",
				"viewCount": 0
			}
		],
		"searchCount": true,
		"size": 0,
		"total": 0
	},
	"msg": "",
	"status": 0
}
```





## 获取游戏详情


**接口地址**:`/game/info/{gid}`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>根据id获取游戏详情页</p>



**请求参数**:


**请求参数**:


| 参数名称 | 参数说明                    | 请求类型 | 是否必须 | 数据类型       | schema |
| -------- | --------------------------- | -------- | -------- | -------------- | ------ |
| gid      | gid                         | path     | true     | integer(int64) |        |
| language | language,可用值:en_US,zh_CN | query    | false    | string         |        |


**响应状态**:


| 状态码 | 说明         | schema         |
| ------ | ------------ | -------------- |
| 200    | OK           | RD«GameInfoVO» |
| 401    | Unauthorized |                |
| 403    | Forbidden    |                |
| 404    | Not Found    |                |


**响应参数**:


| 参数名称                            | 参数说明                            | 类型               | schema           |
| ----------------------------------- | ----------------------------------- | ------------------ | ---------------- |
| data                                |                                     | GameInfoVO         | GameInfoVO       |
| &emsp;&emsp;comment_allowed         | 允许评论,可用值:FALSE,TRUE          | string             |                  |
| &emsp;&emsp;community               |                                     | string             |                  |
| &emsp;&emsp;current_stage           | 当前阶段                            | string             |                  |
| &emsp;&emsp;description             | 介绍                                | string             |                  |
| &emsp;&emsp;detail                  | 游戏详情                            | string             |                  |
| &emsp;&emsp;developer               | 开发商                              | string             |                  |
| &emsp;&emsp;events                  | 游戏事件                            | array              | GameEventDTO     |
| &emsp;&emsp;&emsp;&emsp;end_time    | 结束日期                            | string             |                  |
| &emsp;&emsp;&emsp;&emsp;link        | 平台链接                            | string             |                  |
| &emsp;&emsp;&emsp;&emsp;name        | 事件名                              | string             |                  |
| &emsp;&emsp;&emsp;&emsp;start_time  | 起始日期                            | string             |                  |
| &emsp;&emsp;forum_img_url           | 论坛背景                            | string             |                  |
| &emsp;&emsp;forum_module_id         | 论坛板块id                          | string             |                  |
| &emsp;&emsp;gid                     | 游戏id                              | integer(int64)     |                  |
| &emsp;&emsp;image_url               |                                     | string             |                  |
| &emsp;&emsp;images                  | 图片信息                            | array              | MediaInfoDTO     |
| &emsp;&emsp;&emsp;&emsp;fid         | 文件id                              | integer            |                  |
| &emsp;&emsp;&emsp;&emsp;issue_id    |                                     | integer            |                  |
| &emsp;&emsp;&emsp;&emsp;poster      |                                     | string             |                  |
| &emsp;&emsp;&emsp;&emsp;sort        |                                     | integer            |                  |
| &emsp;&emsp;&emsp;&emsp;type        | 媒体类型,可用值:IMAGE,VIDEO         | string             |                  |
| &emsp;&emsp;&emsp;&emsp;url         | 媒体链接地址                        | string             |                  |
| &emsp;&emsp;languages               | 语言                                | array              | string           |
| &emsp;&emsp;link_type               | 链类型                              | array              | string           |
| &emsp;&emsp;link_url                | 游戏链接                            | string             |                  |
| &emsp;&emsp;milestones              | 里程碑                              | array              | GameMilestoneDTO |
| &emsp;&emsp;&emsp;&emsp;description | 里程碑描述                          | string             |                  |
| &emsp;&emsp;&emsp;&emsp;time        | 时间 yyyy-MM-dd                     | string             |                  |
| &emsp;&emsp;not_show_detail         | 是否显示详情,可用值:FALSE,TRUE      | string             |                  |
| &emsp;&emsp;platform_type           | 支持平台列表                        | array              | string           |
| &emsp;&emsp;publish_date            | 发布日期                            | string(date)       |                  |
| &emsp;&emsp;server_time             | 服务器时间                          | string(date-time)  |                  |
| &emsp;&emsp;sort_name               |                                     | string             |                  |
| &emsp;&emsp;status                  | 游戏状态,可用值:ONLINE,RESERVE,TEST | string             |                  |
| &emsp;&emsp;tags                    | 游戏标签                            | array              | string           |
| &emsp;&emsp;team_introduce          | 团队介绍                            | string             |                  |
| &emsp;&emsp;telegram                |                                     | string             |                  |
| &emsp;&emsp;title                   | 标题                                | string             |                  |
| &emsp;&emsp;token_economy           | 代币经济                            | string             |                  |
| &emsp;&emsp;token_names             | 币种名称                            | array              | string           |
| &emsp;&emsp;twitter                 |                                     | string             |                  |
| &emsp;&emsp;types                   | 游戏类型                            | array              | string           |
| &emsp;&emsp;videos                  | 视频                                | array              | MediaInfoDTO     |
| &emsp;&emsp;&emsp;&emsp;fid         | 文件id                              | integer            |                  |
| &emsp;&emsp;&emsp;&emsp;issue_id    |                                     | integer            |                  |
| &emsp;&emsp;&emsp;&emsp;poster      |                                     | string             |                  |
| &emsp;&emsp;&emsp;&emsp;sort        |                                     | integer            |                  |
| &emsp;&emsp;&emsp;&emsp;type        | 媒体类型,可用值:IMAGE,VIDEO         | string             |                  |
| &emsp;&emsp;&emsp;&emsp;url         | 媒体链接地址                        | string             |                  |
| &emsp;&emsp;website                 | 游戏官方网站                        | string             |                  |
| &emsp;&emsp;yield                   | 收益率                              | number(bigdecimal) |                  |
| &emsp;&emsp;youtube                 |                                     | string             |                  |
| msg                                 |                                     | string             |                  |
| status                              |                                     | integer(int32)     | integer(int32)   |


**响应示例**:
```javascript
{
	"data": {
		"comment_allowed": "",
		"community": "",
		"current_stage": "",
		"description": "",
		"detail": "",
		"developer": "",
		"events": [
			{
				"end_time": "",
				"link": "",
				"name": "",
				"start_time": ""
			}
		],
		"forum_img_url": "",
		"forum_module_id": "",
		"gid": 0,
		"image_url": "",
		"images": [
			{
				"fid": 0,
				"issue_id": 0,
				"poster": "",
				"sort": 0,
				"type": "",
				"url": ""
			}
		],
		"languages": [],
		"link_type": [],
		"link_url": "",
		"milestones": [
			{
				"description": "",
				"time": ""
			}
		],
		"not_show_detail": "",
		"platform_type": [],
		"publish_date": "",
		"server_time": "",
		"sort_name": "",
		"status": "",
		"tags": [],
		"team_introduce": "",
		"telegram": "",
		"title": "",
		"token_economy": "",
		"token_names": [],
		"twitter": "",
		"types": [],
		"videos": [
			{
				"fid": 0,
				"issue_id": 0,
				"poster": "",
				"sort": 0,
				"type": "",
				"url": ""
			}
		],
		"website": "",
		"yield": 0,
		"youtube": ""
	},
	"msg": "",
	"status": 0
}
```





## 根据虚拟货币名称获取价格信息


**接口地址**:`/crypto/getByNames`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:


**请求参数**:


**请求参数**:


| 参数名称 | 参数说明         | 请求类型 | 是否必须 | 数据类型 | schema |
| -------- | ---------------- | -------- | -------- | -------- | ------ |
| names    | 虚拟货币名称列表 | query    | true     | string   |        |


**响应状态**:


| 状态码 | 说明         | schema                         |
| ------ | ------------ | ------------------------------ |
| 200    | OK           | RD«Set«CryptoCurrencyPriceVO»» |
| 401    | Unauthorized |                                |
| 403    | Forbidden    |                                |
| 404    | Not Found    |                                |


**响应参数**:


| 参数名称                                 | 参数说明                    | 类型               | schema                |
| ---------------------------------------- | --------------------------- | ------------------ | --------------------- |
| data                                     |                             | array              | CryptoCurrencyPriceVO |
| &emsp;&emsp;coinLogo                     | logo                        | string             |                       |
| &emsp;&emsp;high24h                      | 24小时高价                  | number(bigdecimal) |                       |
| &emsp;&emsp;id                           | 主键id                      | integer(int64)     |                       |
| &emsp;&emsp;low24h                       | 24小时低价                  | number(bigdecimal) |                       |
| &emsp;&emsp;name                         | 名称                        | string             |                       |
| &emsp;&emsp;quotes                       | 关联价格信息(对USD,BTC,ETH) | array              | CryptoCurrencyQuoteVO |
| &emsp;&emsp;&emsp;&emsp;cryptoCurrencyId | 虚拟货币id                  | integer            |                       |
| &emsp;&emsp;&emsp;&emsp;name             | 货币名称                    | string             |                       |
| &emsp;&emsp;&emsp;&emsp;percentChange1h  | 1小时变化百分比             | number             |                       |
| &emsp;&emsp;&emsp;&emsp;percentChange24h | 24小时变化百分比            | number             |                       |
| &emsp;&emsp;&emsp;&emsp;percentChange7d  | 7天变化百分比               | number             |                       |
| &emsp;&emsp;&emsp;&emsp;price            | 相对价格                    | number             |                       |
| &emsp;&emsp;symbol                       | 符号                        | string             |                       |
| msg                                      |                             | string             |                       |
| status                                   |                             | integer(int32)     | integer(int32)        |


**响应示例**:
```javascript
{
	"data": [
		{
			"coinLogo": "",
			"high24h": 0,
			"id": 0,
			"low24h": 0,
			"name": "",
			"quotes": [
				{
					"cryptoCurrencyId": 0,
					"name": "",
					"percentChange1h": 0,
					"percentChange24h": 0,
					"percentChange7d": 0,
					"price": 0
				}
			],
			"symbol": ""
		}
	],
	"msg": "",
	"status": 0
}
```





## 获取热门游戏标签


**接口地址**:`/game/lable/hot`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:


**请求参数**:


**请求参数**:


| 参数名称 | 参数说明                    | 请求类型 | 是否必须 | 数据类型 | schema |
| -------- | --------------------------- | -------- | -------- | -------- | ------ |
| language | language,可用值:en_US,zh_CN | query    | false    | string   |        |


**响应状态**:


| 状态码 | 说明         | schema                    |
| ------ | ------------ | ------------------------- |
| 200    | OK           | RD«List«GameLabelListVO»» |
| 401    | Unauthorized |                           |
| 403    | Forbidden    |                           |
| 404    | Not Found    |                           |


**响应参数**:


| 参数名称              | 参数说明 | 类型           | schema          |
| --------------------- | -------- | -------------- | --------------- |
| data                  |          | array          | GameLabelListVO |
| &emsp;&emsp;gameHeat  | 总热度   | integer(int32) |                 |
| &emsp;&emsp;id        | id       | integer(int64) |                 |
| &emsp;&emsp;labelName | 标签名称 | string         |                 |
| msg                   |          | string         |                 |
| status                |          | integer(int32) | integer(int32)  |


**响应示例**:
```javascript
{
	"data": [
		{
			"gameHeat": 0,
			"id": 0,
			"labelName": ""
		}
	],
	"msg": "",
	"status": 0
}
```
