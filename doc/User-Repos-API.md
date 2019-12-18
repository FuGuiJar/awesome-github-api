

## 关于User-Repos-API
User-Repos所涉及到的API，包括：

 1. User 某个用户的信息
 2. Repos 某个用户下某个仓库的信息

### 1.User
查询某个用户的信息
#### 1.1 请求说明
| 说明 | URL | 备注|
|--|--|--|
| 请求URL |URL	https://api.github.com/users/{user} ||
| 参数1 |user  | 用户名 |  
|demo|URL	https://api.github.com/users/arvidn||

#### 1.2 返回响应
```
 {
	"login": "arvidn",
	"id": 661450,
	"node_id": "MDQ6VXNlcjY2MTQ1MA==",
	"avatar_url": "https://avatars0.githubusercontent.com/u/661450?v=4",
	"gravatar_id": "",
	"url": "https://api.github.com/users/arvidn",
	"html_url": "https://github.com/arvidn",
	"followers_url": "https://api.github.com/users/arvidn/followers",
	"following_url": "https://api.github.com/users/arvidn/following{/other_user}",
	"gists_url": "https://api.github.com/users/arvidn/gists{/gist_id}",
	"starred_url": "https://api.github.com/users/arvidn/starred{/owner}{/repo}",
	"subscriptions_url": "https://api.github.com/users/arvidn/subscriptions",
	"organizations_url": "https://api.github.com/users/arvidn/orgs",
	"repos_url": "https://api.github.com/users/arvidn/repos",
	"events_url": "https://api.github.com/users/arvidn/events{/privacy}",
	"received_events_url": "https://api.github.com/users/arvidn/received_events",
	"type": "User",
	"site_admin": false,
	"name": "Arvid Norberg",
	"company": "Blockstream",
	"blog": "http://libtorrent.org",
	"location": "Stockholm, Sweden",
	"email": "arvid@libtorrent.org",
	"hireable": null,
	"bio": null,
	"public_repos": 45,
	"public_gists": 0,
	"followers": 551,
	"following": 2,
	"created_at": "2011-03-10T07:42:41Z",
	"updated_at": "2019-12-17T22:30:19Z"
}
```

### 2.Repos
查询某个用户下的某个Repos信息
#### 2.1 请求说明
| 说明 | URL | 备注|
|--|--|--|
| 请求URL | https://api.github.com/repos/{user}/{repos}||
| 参数1 |user  | 某个用户 |  
| 参数2 |repos  | 该用户下的某个仓库名 |  
|demo|https://api.github.com/repos/xingshaocheng/architect-awesome||


#### 2.2 返回响应

```
{
	"id": 128398636,
	"node_id": "MDEwOlJlcG9zaXRvcnkxMjgzOTg2MzY=",
	"name": "architect-awesome",
	"full_name": "xingshaocheng/architect-awesome",
	"private": false,
	"owner": {
		"login": "xingshaocheng",
		"id": 4962837,
		"node_id": "MDQ6VXNlcjQ5NjI4Mzc=",
		"avatar_url": "https://avatars1.githubusercontent.com/u/4962837?v=4",
		"gravatar_id": "",
		"url": "https://api.github.com/users/xingshaocheng",
		"html_url": "https://github.com/xingshaocheng",
		"followers_url": "https://api.github.com/users/xingshaocheng/followers",
		"following_url": "https://api.github.com/users/xingshaocheng/following{/other_user}",
		"gists_url": "https://api.github.com/users/xingshaocheng/gists{/gist_id}",
		"starred_url": "https://api.github.com/users/xingshaocheng/starred{/owner}{/repo}",
		"subscriptions_url": "https://api.github.com/users/xingshaocheng/subscriptions",
		"organizations_url": "https://api.github.com/users/xingshaocheng/orgs",
		"repos_url": "https://api.github.com/users/xingshaocheng/repos",
		"events_url": "https://api.github.com/users/xingshaocheng/events{/privacy}",
		"received_events_url": "https://api.github.com/users/xingshaocheng/received_events",
		"type": "User",
		"site_admin": false
	},
	"html_url": "https://github.com/xingshaocheng/architect-awesome",
	"description": "后端架构师技术图谱",
	"fork": false,
	"url": "https://api.github.com/repos/xingshaocheng/architect-awesome",
	"forks_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/forks",
	"keys_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/keys{/key_id}",
	"collaborators_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/collaborators{/collaborator}",
	"teams_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/teams",
	"hooks_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/hooks",
	"issue_events_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/issues/events{/number}",
	"events_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/events",
	"assignees_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/assignees{/user}",
	"branches_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/branches{/branch}",
	"tags_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/tags",
	"blobs_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/git/blobs{/sha}",
	"git_tags_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/git/tags{/sha}",
	"git_refs_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/git/refs{/sha}",
	"trees_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/git/trees{/sha}",
	"statuses_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/statuses/{sha}",
	"languages_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/languages",
	"stargazers_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/stargazers",
	"contributors_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/contributors",
	"subscribers_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/subscribers",
	"subscription_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/subscription",
	"commits_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/commits{/sha}",
	"git_commits_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/git/commits{/sha}",
	"comments_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/comments{/number}",
	"issue_comment_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/issues/comments{/number}",
	"contents_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/contents/{+path}",
	"compare_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/compare/{base}...{head}",
	"merges_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/merges",
	"archive_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/{archive_format}{/ref}",
	"downloads_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/downloads",
	"issues_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/issues{/number}",
	"pulls_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/pulls{/number}",
	"milestones_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/milestones{/number}",
	"notifications_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/notifications{?since,all,participating}",
	"labels_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/labels{/name}",
	"releases_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/releases{/id}",
	"deployments_url": "https://api.github.com/repos/xingshaocheng/architect-awesome/deployments",
	"created_at": "2018-04-06T13:30:58Z",
	"updated_at": "2019-12-18T09:31:41Z",
	"pushed_at": "2019-12-16T11:53:47Z",
	"git_url": "git://github.com/xingshaocheng/architect-awesome.git",
	"ssh_url": "git@github.com:xingshaocheng/architect-awesome.git",
	"clone_url": "https://github.com/xingshaocheng/architect-awesome.git",
	"svn_url": "https://github.com/xingshaocheng/architect-awesome",
	"homepage": "",
	"size": 2472,
	"stargazers_count": 40383,
	"watchers_count": 40383,
	"language": null,
	"has_issues": true,
	"has_projects": true,
	"has_downloads": true,
	"has_wiki": true,
	"has_pages": false,
	"forks_count": 12692,
	"mirror_url": null,
	"archived": false,
	"disabled": false,
	"open_issues_count": 52,
	"license": null,
	"forks": 12692,
	"open_issues": 52,
	"watchers": 40383,
	"default_branch": "master",
	"permissions": {
		"admin": false,
		"push": false,
		"pull": true
	},
	"temp_clone_token": "",
	"network_count": 12692,
	"subscribers_count": 2906
}
```
