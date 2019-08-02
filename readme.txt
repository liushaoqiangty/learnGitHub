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


本地秘钥
ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQCbOspNhqmrcQDfFLuK/kCZJ+NBtUUQHIUtisgvagcW9VtKMbMC2/tuu8+aA0Pcdydssi/xabom5GZlbE0IvUbOnFeyaKb9GIvKzSR2yDU9I4YoXBPAFd4f/AUAZGwmApyfZhCynqHUGlRPwxpEIOEwEtHGYb5rTGh1XT2jHDRK4oYyoyXdWABuDP8Vzzhr0pkqzefTfTBgeVBUx/ltaJk03sHq+fqGCNbwSeFjHEgMfhrBtXjDRuevpEtDNTab5AZKqWhm6jYW25oCldLywjeuirdvdjnooUWEOIMe8AtFVSIjbg/hTCXUXh4+6e1N6yMKGjqGqsEIh16UCy+P5uEsYdCGP93x4ti1Vvr4auQe+z1uL01aeJyxElerg5Vk+ASFLRS9SjQGkNIdleShQYMr7ts2rezvOrycMKUgrYD/TcjixQ6rQ4zy9wLBmrXmN7RqhAofqgMmhzzQUJfWxkGQKNWxkhrFW3I5EYOx3AAeJgqH/JQGyhkCrn+4u9MEQc8= 253422477@qq.com

创建仓库目录
git init

git add README.md
git commit -m "first commit"
git remote add origin https://github.com/liushaoqiangty/learnGitHub.git
git push -u origin master