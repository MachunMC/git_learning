# 一、常用操作

## 1. 代码提交

```bash
git add xxx xxx					# 添加xxx到暂存区，添加所有修改用"."表示
git commit -m "commit log"		# 将暂存区的内容，提交到版本库
git log							# 查看本地提交记录
```





## 2. 版本回退

```bash
git reset --hard HEAD^  	  # 返回上一次提交
git reset --hard commit_id    # 版本回退到某一次提交
git checkout -- file		  # 撤销某个未添加到工作区的文件的修改
							  # 如果文件已经添加到工作区，则使用git reset
```





## 3. git和github

```bash
git pull      				# 将远端更新拉取到本地
git push origin master		# 将本地master分支的提交推送到远端（origin表示远端仓库）
```





## 4. 分支管理

```bash
git branch					# 查看本地分支（-a表示查看本地和远端的分支）
git branch	dev				# 创建dev分支
git checkout dev			# 从master分支切换到dev分支
git branch -d dev			# 删除dev分支
git merge dev				# 将dev分支合并到当前分支
```





## 5. tag标签

```bash
git tag							 # 查看本地tag
git tag v1.0			    	 # 创建v1.0 tag
git tag v1.1 commit_id			 # 基于某次提交，创建tag
git tag -a v1.2 -m "commit log"	 # 创建v1.2 tag，并添加评论
git tag -d v1.1					 # 删除v1.1 tag
git show v1.1					 # 显示v1.1 tag的信息
git push origin v1.1			 # 将本地v1.1 tag推送到远端服务器
```

