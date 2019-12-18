

## 关于搜索-API
搜索所涉及到的API，包括：

 1. 搜索整个GitHub仓库内容
 

### 1.搜索
搜索整个GitHub仓库内容
#### 1.1 请求说明
| 说明 | URL | 备注|
|--|--|--|
| 请求URL |https://api.github.com/search/repositories?q={content} ||
| 参数1 |q  | 搜索的内容 |  
|demo|https://api.github.com/search/repositories?q=citypicker||

#### 1.2 返回响应
```
 {
	"total_count": 211,
	"incomplete_results": false,
	"items": [{
		"id": 58596246,
		"node_id": "MDEwOlJlcG9zaXRvcnk1ODU5NjI0Ng==",
		"name": "citypicker",
		"full_name": "crazyandcoder/citypicker",
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
		"html_url": "https://github.com/crazyandcoder/citypicker",
		"description": "citypicker城市选择器，详细的省市区地址信息，支持仿iOS滚轮实现，仿京东样式，一级或者三级列表展示方式。",
		"fork": false,
		"url": "https://api.github.com/repos/crazyandcoder/citypicker",
		"forks_url": "https://api.github.com/repos/crazyandcoder/citypicker/forks",
		"keys_url": "https://api.github.com/repos/crazyandcoder/citypicker/keys{/key_id}",
		"collaborators_url": "https://api.github.com/repos/crazyandcoder/citypicker/collaborators{/collaborator}",
		"teams_url": "https://api.github.com/repos/crazyandcoder/citypicker/teams",
		"hooks_url": "https://api.github.com/repos/crazyandcoder/citypicker/hooks",
		"issue_events_url": "https://api.github.com/repos/crazyandcoder/citypicker/issues/events{/number}",
		"events_url": "https://api.github.com/repos/crazyandcoder/citypicker/events",
		"assignees_url": "https://api.github.com/repos/crazyandcoder/citypicker/assignees{/user}",
		"branches_url": "https://api.github.com/repos/crazyandcoder/citypicker/branches{/branch}",
		"tags_url": "https://api.github.com/repos/crazyandcoder/citypicker/tags",
		"blobs_url": "https://api.github.com/repos/crazyandcoder/citypicker/git/blobs{/sha}",
		"git_tags_url": "https://api.github.com/repos/crazyandcoder/citypicker/git/tags{/sha}",
		"git_refs_url": "https://api.github.com/repos/crazyandcoder/citypicker/git/refs{/sha}",
		"trees_url": "https://api.github.com/repos/crazyandcoder/citypicker/git/trees{/sha}",
		"statuses_url": "https://api.github.com/repos/crazyandcoder/citypicker/statuses/{sha}",
		"languages_url": "https://api.github.com/repos/crazyandcoder/citypicker/languages",
		"stargazers_url": "https://api.github.com/repos/crazyandcoder/citypicker/stargazers",
		"contributors_url": "https://api.github.com/repos/crazyandcoder/citypicker/contributors",
		"subscribers_url": "https://api.github.com/repos/crazyandcoder/citypicker/subscribers",
		"subscription_url": "https://api.github.com/repos/crazyandcoder/citypicker/subscription",
		"commits_url": "https://api.github.com/repos/crazyandcoder/citypicker/commits{/sha}",
		"git_commits_url": "https://api.github.com/repos/crazyandcoder/citypicker/git/commits{/sha}",
		"comments_url": "https://api.github.com/repos/crazyandcoder/citypicker/comments{/number}",
		"issue_comment_url": "https://api.github.com/repos/crazyandcoder/citypicker/issues/comments{/number}",
		"contents_url": "https://api.github.com/repos/crazyandcoder/citypicker/contents/{+path}",
		"compare_url": "https://api.github.com/repos/crazyandcoder/citypicker/compare/{base}...{head}",
		"merges_url": "https://api.github.com/repos/crazyandcoder/citypicker/merges",
		"archive_url": "https://api.github.com/repos/crazyandcoder/citypicker/{archive_format}{/ref}",
		"downloads_url": "https://api.github.com/repos/crazyandcoder/citypicker/downloads",
		"issues_url": "https://api.github.com/repos/crazyandcoder/citypicker/issues{/number}",
		"pulls_url": "https://api.github.com/repos/crazyandcoder/citypicker/pulls{/number}",
		"milestones_url": "https://api.github.com/repos/crazyandcoder/citypicker/milestones{/number}",
		"notifications_url": "https://api.github.com/repos/crazyandcoder/citypicker/notifications{?since,all,participating}",
		"labels_url": "https://api.github.com/repos/crazyandcoder/citypicker/labels{/name}",
		"releases_url": "https://api.github.com/repos/crazyandcoder/citypicker/releases{/id}",
		"deployments_url": "https://api.github.com/repos/crazyandcoder/citypicker/deployments",
		"created_at": "2016-05-12T01:21:33Z",
		"updated_at": "2019-12-18T08:43:40Z",
		"pushed_at": "2019-11-14T06:26:55Z",
		"git_url": "git://github.com/crazyandcoder/citypicker.git",
		"ssh_url": "git@github.com:crazyandcoder/citypicker.git",
		"clone_url": "https://github.com/crazyandcoder/citypicker.git",
		"svn_url": "https://github.com/crazyandcoder/citypicker",
		"homepage": "",
		"size": 1739,
		"stargazers_count": 2609,
		"watchers_count": 2609,
		"language": "Java",
		"has_issues": true,
		"has_projects": true,
		"has_downloads": true,
		"has_wiki": true,
		"has_pages": false,
		"forks_count": 548,
		"mirror_url": null,
		"archived": false,
		"disabled": false,
		"open_issues_count": 10,
		"license": null,
		"forks": 548,
		"open_issues": 10,
		"watchers": 2609,
		"default_branch": "master",
		"permissions": {
			"admin": true,
			"push": true,
			"pull": true
		},
		"score": 165.37094
	}
}]
}
```
