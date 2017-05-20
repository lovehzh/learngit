# learngit
Learn git demo

在服务器添加完公钥后报错


sign_and_send_pubkey: signing failed: agent refused operation

这个时候我们只要执行下

eval "$(ssh-agent -s)"

ssh-add
就可以了
