## git操作

克隆代码
git clone https://github.com/jiejuepy/firstgit.git


git branch 查看分支
git branch name 创建新分支name

git branch -D删除本地分支，在其他分支里面执行
git push origin --delete 分支名 删除远程的分支

touch 名字 创建文件名
vim 名字 编辑文件
rm 名字  删除文件

git checkout -b 分支名whf
-- 在master里面创建whf分支


vim readme.md

git add . 添加修改的所有文件到缓存区
git status查看状态
(git add 修改的文件名 name1 name2...)
git commit -m'增加注解'
git push origin 分支名 上传到远程分支上

提醒输入用户名和密码
上传成功

设置全局变量
git config --global user.email
"sss@qq.com"

git config --global uer.name
'xx'

合并add和commit操作
git commit -am'增加注解'

创建秘钥
ssh-keygen -t rsa -C xxxx@qq.com（账号）

git pull origin master如果在github上面删除文件夹了，要先pull下来，再push你的代码上去

git diff 分支1 分支2 对比两个分支是否相同

git merge name1 name2分支合并

### 版本号操作
git tag -a 版本号 -m 注解
git push origin 版本号 上传版本号
git tag -d 版本号 本地删除版本号
git push origin --delete 版本号  删除远程的版本号


### stash操作
git stash 缓存本地修改的代码S
git stash list 查看本地缓存的片段
发现有缓存列表,刚才缓存的记录为stash@{0}:xxx
git stash apply stash@{0}

git stash clear 删除缓存
git log查看日志

git reset 版本号 返回之前的版本