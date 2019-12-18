

## 关于Trending-API
Trending所涉及到的API，包括：

 1. Trending-Repositories
 2. Trending-Developers

### 1.Trending-Repositories
#### 1.1 请求说明
| 说明 | URL | 备注|
|--|--|--|
| 请求URL |https://github-trending-api.now.sh/repositories?since={} ||
| 参数1 |since  | 参考值有daily-weekly-monthly |  
|demo|https://github-trending-api.now.sh/repositories?since=daily||

#### 1.2 返回响应
返回一个数组
```
[
{
	"author": "xingshaocheng",
	"name": "architect-awesome",
	"avatar": "https://github.com/xingshaocheng.png",
	"url": "https://github.com/xingshaocheng/architect-awesome",
	"description": "后端架构师技术图谱",
	"stars": 40365,
	"forks": 12684,
	"currentPeriodStars": 455,
	"builtBy": [{
		"username": "xingshaocheng",
		"href": "https://github.com/xingshaocheng",
		"avatar": "https://avatars3.githubusercontent.com/u/4962837"
	}, {
		"username": "liukgg",
		"href": "https://github.com/liukgg",
		"avatar": "https://avatars0.githubusercontent.com/u/8112340"
	}, {
		"username": "sorenduan",
		"href": "https://github.com/sorenduan",
		"avatar": "https://avatars0.githubusercontent.com/u/34806814"
	}, {
		"username": "BeoneMan",
		"href": "https://github.com/BeoneMan",
		"avatar": "https://avatars3.githubusercontent.com/u/38913093"
	}, {
		"username": "eazow",
		"href": "https://github.com/eazow",
		"avatar": "https://avatars1.githubusercontent.com/u/1249362"
	}]
}
]
```

### 2.Trending-Developers
#### 2.1 请求说明
| 说明 | URL | 备注|
|--|--|--|
| 请求URL | https://github-trending-api.now.sh/developers?since={} ||
| 参数1 |since  | 参考值有daily-weekly-monthly |  
|demo|https://github-trending-api.now.sh/developers?since=daily||


#### 2.2 返回响应
返回结果是一个数组
```
[
{
	"username": "natario1",
	"name": "Mattia Iavarone",
	"type": "user",
	"url": "https://github.com/natario1",
	"avatar": "https://avatars0.githubusercontent.com/u/15526561",
	"repo": {
		"name": "CameraView",
		"description": "📸 A well documented, high-level Android interface that makes capturing pictures and videos easy, addressing all of the common issues and needs. Real-time filters, gestures, watermarks, frame processing, RAW, output of any size.",
		"url": "https://github.com/natario1/CameraView"
	}
}
]
```
