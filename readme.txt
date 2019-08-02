使用git远程仓库
需要将当前的电脑添加到github远程仓库的信任目录中

$ ssh-keygen -t rsa -C "253422477@qq.com"
Generating public/private rsa key pair.
Enter file in which to save the key (/c/Users/Administrator/.ssh/id_rsa):
Created directory '/c/Users/Administrator/.ssh'.
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in /c/Users/Administrator/.ssh/id_rsa.
Your public key has been saved in /c/Users/Administrator/.ssh/id_rsa.pub.
The key fingerprint is:
SHA256:4/oO9XA9DnJCdsOkS3WcHdNF2WxglVRW3ca/SuvdqTI 253422477@qq.com
The key's randomart image is:
+---[RSA 3072]----+
|          o..o*X^|
|         = .o..=X|
|        = +    o.|
|       + o o    .|
|        S + o   .|
|       o O o o . |
|      . . . o o  |
|       o   E o. o|
|      .oo   +o.o.|
+----[SHA256]-----+


创建仓库目录
git init

git add README.md
git commit -m "first commit"
git remote add origin https://github.com/liushaoqiangty/learnGitHub.git
git push -u origin master


查看分支：git branch

创建分支：git branch <name>

切换分支：git checkout <name>

创建+切换分支：git checkout -b <name>

合并某分支到当前分支：git merge <name>//要合并分支的名字

删除分支：git branch -d <name>

