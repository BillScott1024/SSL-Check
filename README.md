# Check Your SSL Every Day ! 
🔒无后端每日检查特定网站的SSL证书状况
利用Travis-CI定时检测SSL状态并输出

# 开始

1. Fork 本项目，修改 `.travis.yml` 第12行，在 `  - ./checker.sh ` 后面跟上需要检测的网址,多个网址请用空格隔开.
2. 若需要检测页面绑定域名,则修改第14行,默认指向我的域名,请替换 `ssl.cyfan.top` 为你的域名，若不需要，则将14行删除
3. 若第二步绑定域名，请前往NS添加CNAME。
4. 新建一个GithubToken，权限至少要拥有写入Repo
5. 登入 https://travis-ci.org 勾开此项目，添加三个变量：

- GITHUB_TOKEN：你的GithubToken，**必填**
- GITHUB_EMAIL：你的Github邮箱
- GITHUB_USER：你的github用户名

6. Trigger这个项目
7. 进入Github项目，勾开GithubPage服务
8. 进入Trvis-ci，设置Cron Jobs为每日部署

# Demo：https://ssl.cyfan.top
