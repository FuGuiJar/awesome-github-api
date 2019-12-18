
## 关于我的-API
我的页面所涉及到的API，包括：

 1. 我的主页
 2. 我的关注
 3. 我的仓库
 4. 我的粉丝


### 1.我的个人主页
#### 1.1 请求说明
| 说明 | URL | 备注|
|--|--|--|
| 请求URL | https://api.github.com/user?access_token={token值} ||
| 参数 | access_token |

#### 1.2 返回响应

```
{
	"login": "crazyandcoder",
	"id": 12810244,
	"node_id": "MDQ6VXNlcjEyODEwMjQ0",
	"avatar_url": "https://avatars2.githubusercontent.com/u/12810244?v=4",
	"gravatar_id": "",
	"url": "https://api.github.com/users/crazyandcoder",
	"html_url": "https://github.com/crazyandcoder",
	"followers_url": "https://api.github.com/users/crazyandcoder/followers",
	"following_url": "https://api.github.com/users/crazyandcoder/following{/other_user}",
	"gists_url": "https://api.github.com/users/crazyandcoder/gists{/gist_id}",
	"starred_url": "https://api.github.com/users/crazyandcoder/starred{/owner}{/repo}",
	"subscriptions_url": "https://api.github.com/users/crazyandcoder/subscriptions",
	"organizations_url": "https://api.github.com/users/crazyandcoder/orgs",
	"repos_url": "https://api.github.com/users/crazyandcoder/repos",
	"events_url": "https://api.github.com/users/crazyandcoder/events{/privacy}",
	"received_events_url": "https://api.github.com/users/crazyandcoder/received_events",
	"type": "User",
	"site_admin": false,
	"name": null,
	"company": "中国平安",
	"blog": "http://crazyandcoder.work/",
	"location": "ShangHai China",
	"email": null,
	"hireable": null,
	"bio": "公众号：programming-world\r\n",
	"public_repos": 23,
	"public_gists": 0,
	"followers": 270,
	"following": 56,
	"created_at": "2015-06-09T07:55:57Z",
	"updated_at": "2019-12-18T03:04:32Z",
	"private_gists": 0,
	"total_private_repos": 0,
	"owned_private_repos": 0,
	"disk_usage": 222238,
	"collaborators": 0,
	"two_factor_authentication": false,
	"plan": {
		"name": "free",
		"space": 976562499,
		"collaborators": 0,
		"private_repos": 10000
	}
}
```

### 2.我的关注 Following
#### 2.1 请求说明
| 说明 | URL | 备注|
|--|--|--|
| 请求URL | https://api.github.com/users/{user}/following||
| 参数1 | page |int类型|
| 参数2 | user |某个用户|
| 例如 | https://api.github.com/users/crazyandcoder/following?page=1 |需要分页处理|


#### 2.2 返回响应
备注：结果返回一个数组
```
[{
	"login": "taowen",
	"id": 40541,
	"node_id": "MDQ6VXNlcjQwNTQx",
	"avatar_url": "https://avatars3.githubusercontent.com/u/40541?v=4",
	"gravatar_id": "",
	"url": "https://api.github.com/users/taowen",
	"html_url": "https://github.com/taowen",
	"followers_url": "https://api.github.com/users/taowen/followers",
	"following_url": "https://api.github.com/users/taowen/following{/other_user}",
	"gists_url": "https://api.github.com/users/taowen/gists{/gist_id}",
	"starred_url": "https://api.github.com/users/taowen/starred{/owner}{/repo}",
	"subscriptions_url": "https://api.github.com/users/taowen/subscriptions",
	"organizations_url": "https://api.github.com/users/taowen/orgs",
	"repos_url": "https://api.github.com/users/taowen/repos",
	"events_url": "https://api.github.com/users/taowen/events{/privacy}",
	"received_events_url": "https://api.github.com/users/taowen/received_events",
	"type": "User",
	"site_admin": false
}, {
	"login": "JakeWharton",
	"id": 66577,
	"node_id": "MDQ6VXNlcjY2NTc3",
	"avatar_url": "https://avatars0.githubusercontent.com/u/66577?v=4",
	"gravatar_id": "",
	"url": "https://api.github.com/users/JakeWharton",
	"html_url": "https://github.com/JakeWharton",
	"followers_url": "https://api.github.com/users/JakeWharton/followers",
	"following_url": "https://api.github.com/users/JakeWharton/following{/other_user}",
	"gists_url": "https://api.github.com/users/JakeWharton/gists{/gist_id}",
	"starred_url": "https://api.github.com/users/JakeWharton/starred{/owner}{/repo}",
	"subscriptions_url": "https://api.github.com/users/JakeWharton/subscriptions",
	"organizations_url": "https://api.github.com/users/JakeWharton/orgs",
	"repos_url": "https://api.github.com/users/JakeWharton/repos",
	"events_url": "https://api.github.com/users/JakeWharton/events{/privacy}",
	"received_events_url": "https://api.github.com/users/JakeWharton/received_events",
	"type": "User",
	"site_admin": false
}]

```

### 3.我的粉丝 Followers
#### 3.1 请求说明
| 说明 | URL | 备注|
|--|--|--|
| 请求URL |https://api.github.com/users/{user}/followers?page=1 |支持分页|
| 参数1 | page |int类型|
| 参数2 | user |我的用户loginName|
| 例如 | https://api.github.com/users/crazyandcoder/followers?page=1 |需要分页处理|


#### 3.2 返回响应
结果返回一个数组
```
[{
	"login": "BearEgg",
	"id": 10806820,
	"node_id": "MDQ6VXNlcjEwODA2ODIw",
	"avatar_url": "https://avatars0.githubusercontent.com/u/10806820?v=4",
	"gravatar_id": "",
	"url": "https://api.github.com/users/BearEgg",
	"html_url": "https://github.com/BearEgg",
	"followers_url": "https://api.github.com/users/BearEgg/followers",
	"following_url": "https://api.github.com/users/BearEgg/following{/other_user}",
	"gists_url": "https://api.github.com/users/BearEgg/gists{/gist_id}",
	"starred_url": "https://api.github.com/users/BearEgg/starred{/owner}{/repo}",
	"subscriptions_url": "https://api.github.com/users/BearEgg/subscriptions",
	"organizations_url": "https://api.github.com/users/BearEgg/orgs",
	"repos_url": "https://api.github.com/users/BearEgg/repos",
	"events_url": "https://api.github.com/users/BearEgg/events{/privacy}",
	"received_events_url": "https://api.github.com/users/BearEgg/received_events",
	"type": "User",
	"site_admin": false
}, {
	"login": "hookliu",
	"id": 22365014,
	"node_id": "MDQ6VXNlcjIyMzY1MDE0",
	"avatar_url": "https://avatars2.githubusercontent.com/u/22365014?v=4",
	"gravatar_id": "",
	"url": "https://api.github.com/users/hookliu",
	"html_url": "https://github.com/hookliu",
	"followers_url": "https://api.github.com/users/hookliu/followers",
	"following_url": "https://api.github.com/users/hookliu/following{/other_user}",
	"gists_url": "https://api.github.com/users/hookliu/gists{/gist_id}",
	"starred_url": "https://api.github.com/users/hookliu/starred{/owner}{/repo}",
	"subscriptions_url": "https://api.github.com/users/hookliu/subscriptions",
	"organizations_url": "https://api.github.com/users/hookliu/orgs",
	"repos_url": "https://api.github.com/users/hookliu/repos",
	"events_url": "https://api.github.com/users/hookliu/events{/privacy}",
	"received_events_url": "https://api.github.com/users/hookliu/received_events",
	"type": "User",
	"site_admin": false
}]

```

### 4.我的仓库 Repositories
#### 4.1 请求说明
| 说明 | URL | 备注|
|--|--|--|
| 请求URL | https://api.github.com/user/repos?affiliation=owner&direction=asc&page=1&sort=full_name&visibility=all||
| 参数1 | affiliation | 隶属关系，固定值owner |
| 参数2 | direction | 排序方式，asc升序，desc降序 |
| 参数3 | page | 分页 |
| 参数4|  |sort  |排序
| 参数5 |visibility  |  |

#### 4.2 返回响应
结果返回一个数组
```
[
{
	"id": 195318990,
	"node_id": "MDEwOlJlcG9zaXRvcnkxOTUzMTg5OTA=",
	"name": "awesome-flutter",
	"full_name": "crazyandcoder/awesome-flutter",
	"private": false,
	"owner": {
		"login": "crazyandcoder",
		"id": 12810244,
		"node_id": "MDQ6VXNlcjEyODEwMjQ0",
		"avatar_url": "https://avatars2.githubusercontent.com/u/12810244?v=4",
		"gravatar_id": "",
		"url": "https://api.github.com/users/crazyandcoder",
		"html_url": "https://github.com/crazyandcoder",
		"followers_url": "https://api.github.com/users/crazyandcoder/followers",
		"following_url": "https://api.github.com/users/crazyandcoder/following{/other_user}",
		"gists_url": "https://api.github.com/users/crazyandcoder/gists{/gist_id}",
		"starred_url": "https://api.github.com/users/crazyandcoder/starred{/owner}{/repo}",
		"subscriptions_url": "https://api.github.com/users/crazyandcoder/subscriptions",
		"organizations_url": "https://api.github.com/users/crazyandcoder/orgs",
		"repos_url": "https://api.github.com/users/crazyandcoder/repos",
		"events_url": "https://api.github.com/users/crazyandcoder/events{/privacy}",
		"received_events_url": "https://api.github.com/users/crazyandcoder/received_events",
		"type": "User",
		"site_admin": false
	},
	"html_url": "https://github.com/crazyandcoder/awesome-flutter",
	"description": "关于flutter的一切，从入门到精通。",
	"fork": false,
	"url": "https://api.github.com/repos/crazyandcoder/awesome-flutter",
	"forks_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/forks",
	"keys_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/keys{/key_id}",
	"collaborators_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/collaborators{/collaborator}",
	"teams_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/teams",
	"hooks_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/hooks",
	"issue_events_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/issues/events{/number}",
	"events_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/events",
	"assignees_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/assignees{/user}",
	"branches_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/branches{/branch}",
	"tags_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/tags",
	"blobs_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/git/blobs{/sha}",
	"git_tags_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/git/tags{/sha}",
	"git_refs_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/git/refs{/sha}",
	"trees_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/git/trees{/sha}",
	"statuses_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/statuses/{sha}",
	"languages_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/languages",
	"stargazers_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/stargazers",
	"contributors_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/contributors",
	"subscribers_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/subscribers",
	"subscription_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/subscription",
	"commits_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/commits{/sha}",
	"git_commits_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/git/commits{/sha}",
	"comments_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/comments{/number}",
	"issue_comment_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/issues/comments{/number}",
	"contents_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/contents/{+path}",
	"compare_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/compare/{base}...{head}",
	"merges_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/merges",
	"archive_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/{archive_format}{/ref}",
	"downloads_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/downloads",
	"issues_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/issues{/number}",
	"pulls_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/pulls{/number}",
	"milestones_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/milestones{/number}",
	"notifications_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/notifications{?since,all,participating}",
	"labels_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/labels{/name}",
	"releases_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/releases{/id}",
	"deployments_url": "https://api.github.com/repos/crazyandcoder/awesome-flutter/deployments",
	"created_at": "2019-07-05T01:26:41Z",
	"updated_at": "2019-11-15T01:51:35Z",
	"pushed_at": "2019-11-15T01:51:33Z",
	"git_url": "git://github.com/crazyandcoder/awesome-flutter.git",
	"ssh_url": "git@github.com:crazyandcoder/awesome-flutter.git",
	"clone_url": "https://github.com/crazyandcoder/awesome-flutter.git",
	"svn_url": "https://github.com/crazyandcoder/awesome-flutter",
	"homepage": "",
	"size": 78,
	"stargazers_count": 2,
	"watchers_count": 2,
	"language": "Dart",
	"has_issues": true,
	"has_projects": true,
	"has_downloads": true,
	"has_wiki": true,
	"has_pages": false,
	"forks_count": 1,
	"mirror_url": null,
	"archived": false,
	"disabled": false,
	"open_issues_count": 4,
	"license": null,
	"forks": 1,
	"open_issues": 4,
	"watchers": 2,
	"default_branch": "master",
	"permissions": {
		"admin": true,
		"push": true,
		"pull": true
	}
}
]

```


