# learngit
## 1
学习如何使用git

在远程创建仓库后,克隆到本地
git remote add origin git@github.com:lovehzh/learngit.git

### 把本地仓库推送到远程仓库上
> git push -u origin master

把本地库的内容推送到远程，用git push命令，实际上是把当前分支master推送到远程。

由于远程库是空的，我们第一次推送master分支时，加上了-u参数，Git不但会把本地的master分支内容推送的远程新的master分支，还会把本地的master分支和远程的master分支关联起来，在以后的推送或者拉取时就可以简化命令。
### 从现在起，只要本地作了提交，就可以通过命令：
> git push origin master


## 2
在服务器添加完公钥后报错


sign_and_send_pubkey: signing failed: agent refused operation

这个时候我们只要执行下

eval "$(ssh-agent -s)"

ssh-add
就可以了

## 3

> 提示：更新被拒绝，因为您当前分支的最新提交落后于其对应的远程分支。

> 提示：再次推送前，先与远程变更合并（如 'git pull ...'）。详见'git push --help' 中的 'Note about fast-forwards' 小节。

引起这个问题是远程仓库和本地不同步引起的

解决方案：需要先获取远端更新并与本地合并,再git push
具体操作如下:

> git fetch origin    //获取远程更新

> git merge origin/master //把更新的内容合并到本地分支

## nano 常用命令

Ctrl + O     保存文件
Ctrl + X     退出编辑器
Ctrl + K     剪切行
Ctrl + U     粘贴
Ctrl + /       替换
Ctrl + W    查找
Ctrl + Y     上一屏幕
Ctrl + V     下一屏幕
Ctrl + P     向上移动一行
Ctrl + N     向下移动一行
Ctrl + F     向前移动光标一格
Ctrl + B     向后移动光标一格
Ctrl + G     调用帮助菜单

