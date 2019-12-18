
## 关于All activity-API
All activity所涉及到的API，包括：


### 1.All activity
#### 1.1 请求说明
| 说明 | URL | 备注|
|--|--|--|
| 请求URL | https://api.github.com/users/{user}/received_events?name={}&page=1 ||
| 参数1 |user  |
| 参数2 | name |
| 参数3 |page  |
|demo|https://api.github.com/users/crazyandcoder/received_events?name=crazyandcoder&page=1||

#### 1.2 返回响应
返回一个数组
```
[
{
	"id": "11114461291",
	"type": "WatchEvent",
	"actor": {
		"id": 2010104,
		"login": "wo417989",
		"display_login": "wo417989",
		"gravatar_id": "",
		"url": "https://api.github.com/users/wo417989",
		"avatar_url": "https://avatars.githubusercontent.com/u/2010104?"
	},
	"repo": {
		"id": 58596246,
		"name": "crazyandcoder/citypicker",
		"url": "https://api.github.com/repos/crazyandcoder/citypicker"
	},
	"payload": {
		"action": "started"
	},
	"public": true,
	"created_at": "2019-12-18T08:43:41Z"
}
]
```
