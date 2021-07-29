1、Git结构

2、Git和代码托管中心

代码托管中心的任务：维护远程库

> 局域网环境下：GitLab服务器
>
> 外网环境下：GitHub、马云

git远程操作

```shell
1、添加远程仓库地址
git remote add [shortname] [url]
例子：git remote add origin git@github.com:tianqixin/runoob-git-test.git

2、使用以下命令生成 SSH Key：
#your_email@youremail.com 改为自己的邮箱，之后会要求确认路径和输入密码，我们这使用默认的一路回车就行。成功的话会在 ~/ 下生成 .ssh 文件夹，进去，打开 id_rsa.pub，复制里面的 key。
ssh-keygen -t rsa -C "youremail@example.com" 

3、在github或gitee上添加ssh公钥
# Account => Settings（账户配置）=>SSH and GPG keys=> New SSH key。

4、验证是否成功，输入以下命令：
ssh -T git@github.com

5、提交到 Github
git push -u origin master
```

