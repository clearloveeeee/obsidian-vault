# diff与patch
diff查看区别，patch逆操作
# git配置
个人信息，文本编码（UTF-8）
# git 版本控制
**区域**
版本库
工作区
暂存区

**文件状态**
已提交
已修改
已暂存

工作状态与区域相对应
# git命令
## 工程准备
git init 新建仓库
git clone 远端服务器拉取
	注意权限
	通过url下载
	git lfs clone 下载二进制文件
## 文件修改
git add 添加到暂存区
git rm 删除文件
git mv 移动/重命名
## 查看状态
git diff 查看差异
	--name-status 只看文件列表
git status 查看工作目录和暂存区状态
git branch 
	-r 查看远端服务器分支
git checkout 
	均可用于新建分支
	git branch 新建分支后并不会切换
	git checkout -b 新建分支后会自动切换
	
## 提交
git commit 提交到本地
	-m 后接备注
## 日志

git log 
	name-status
	-p
	--pretty
	--graph
## 推送/拉取远端仓库
git push origin branch_name:new_branch_name
git push origin branch_name
git pull origin remote_branch:local_branch
从远端服务器获取某个分支的更新，再与本地指定的进行自动合并
git fetch 
从远端服务器中获取某个分支的更新到本地，并不会进行合并操作，fetch 内容符合预期后，再决定是否手动合并






避免大小写更换名称
