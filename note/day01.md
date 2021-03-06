## 项目描述
    1). 这是一个关于哪方面的项目?
    2). 有哪些功能模块, 你负责哪些?
    3). 技术栈是哪些?
    4). 开发方式的特点?

## 技术选型
    1). 前台数据处理/交互/组件化
    2). 前后台交互
    3). 模块化
    4). 项目构建/工程化
    5). css预编译器
    6). 其它

## 接口相关理解
    1). 接口
    2). 接口文档
    3). 对/调/测接口 / 联调
    4). 前后台分离
    5). mock数据/接口

## git版本控制的基本操作
1). 创建本地仓库(代码在本地仓库中)
    创建.gitignore文本, 并配置好
    git init
    git add .
    git commit -m "init app"

2). 创建远程仓库
    New Repo
    指定仓库名
    创建		

3). 将本地仓库的代码推送到远程仓库
    git remote add origin url (在本地记录远程仓库的地址)
    git push origin master

4). 如果本地代码有修改, 要提交到本地仓库, 推送到仓库
    git add .
    git commit -m "xxx"
    git push origin master

    git config --global credential.helper store (记住用户和密码)

5). 如果远程代码有修改, 要拉取到本地仓库
    git pull origin master

6). 将远程仓库的代码clone到本地(生成仓库)
    git clone url

## 分支操作
1). 创建本地分支, 并推送到远程
    git checkout -b dev
    git push origin origin dev
2). 拉取远程新分支到本地
    git pull  (如果分支是在clone后创建的才需要执行)
    git checkout -b dev origin/dev
3). 本地dev分支代码修改
    git add .
    git commit -m "xxx"
    git push origin dev
4). 将dev分支合并到master
    git checkout master
    git merge dev

## 做的事件比较复杂的原因?
		1). 逻辑性比强(情况比较多) ==> 分析清楚所有情况分别处理
		2). 流程比较长(流程操作很多)  ==> 整体少量大的流程步骤在心里
	
## 使用脚手架创建项目并运行
    1). 使用vue-cli3/4
    2). 开发环境运行
    3). 生产环境打包运行

## 一些配置
		1). 关闭eslint配置: vue.config.js   lintOnSave: false/'warning'
		2). @路径提示: jsconfig.json

## 引入vue-router
    1). 下载vue-router
		2). 确定整体路由结构:
				上: Header
				中: router-view
				下: Footer
		3). 定义一级路由组件: Home/Search/Register/Login
		4). 创建路由器, 配置路由, 配置路由器

		5). 组件中路由相关的2个对象 (面试问题)
				$router: 路由器对象, 包含一些用于路由跳转的方法: push()/replace()/back()
				$route: 当前路由信息对象, 包含当前路由相关数据的对象: path/name/query/params/meta