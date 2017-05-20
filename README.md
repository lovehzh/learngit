# learngit
## 1
Learn git demo


## 2
在服务器添加完公钥后报错


sign_and_send_pubkey: signing failed: agent refused operation

这个时候我们只要执行下

eval "$(ssh-agent -s)"

ssh-add
就可以了

## 3

> 提示：更新被拒绝，因为您当前分支的最新提交落后于其对应的远程分支。
> 提示：再次推送前，先与远程变更合并（如 'git pull ...'）。详见
> 提示：'git push --help' 中的 'Note about fast-forwards' 小节。

引起这个问题是远程仓库和本地不同步引起的

解决方案：需要先获取远端更新并与本地合并,再git push
具体操作如下:

> git fetch origin    //获取远程更新
> merge origin/master //把更新的内容合并到本地分支
