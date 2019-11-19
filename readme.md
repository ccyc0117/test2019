第一个仓库
1、git init 初始化仓库

2、新建一个readme.md文件

3、git add 文件名 添加文件到本地仓库
git add .  //添加所有文件

4、添加用户名和邮箱（第一次的时候需要）
git config --global uesr.email ‘你的邮箱’
git config --global user.name ‘你的用户名’

5、提交
git commit -m '注释'  //注释是对本次提交的说明

6、添加远程仓库地址
git remote add origin git@github.com:ccyc0117/2019.git

7、将本地提交的文件推送到远程仓库
git push 远程仓库名的别名 master
git push abc master

8、没有权限，先生成ssh key
ssh-keygen -t rsa -C ‘邮箱’

执行完上一条命令后会在  ~/.ssh/文件夹下生成两个文件 公钥文件id_rse.pub
将公钥文件中得内容放在GitHub中
settings->SSH and GPG keys ->new ssh key
ttile：仓库名
key ： id_rsa.pub 的内容