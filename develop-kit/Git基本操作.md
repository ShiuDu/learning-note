git初始化
配置全局用户信息（分布式版本控制）  
$ git config  --global user.name  “用户名”  
$ git config --global  user.email  “邮箱”  
设置默认的编辑器  
$ git config --global core.editor "编辑器运行程序的路径"  
查看git的配置信息  
$ git config --list  
查看git的命令手册  
$ git help  

Git仓库（repository）  
初始化版本库：git init  
添加文件到版本库  
$git add  文件名  
$git commit  -m "提交的说明"  
查看git仓库状态  
$git status  

添加远程仓库  
$git remote add origin http地址  
第一次提交的时候会默认创建master分支(pwd 展示当前目录信息,mkdir 创建文件夹)  
推送到远端  
$git push  
检出项目到本地(默认把分支已经和远端关联上)  
$git clone http地址  

回到过去  
将版本库中内容覆盖到暂存区（工作区不会变化，如果要使工作区变化）  
$git reset head  
将版本库中内容重置（缓存、版本库、本地都会变化）  
$git reset  --hard hash码 
清空本地文件    
$git rm 文件名  

标签管理（建立里程碑）  
查看所有标签： $git tag  
创建标签：$git tag name  
指定提交信息:git tag -a name -m "comment"   
删除标签:git tag -d name (删除标签名为)  
标签发布：git push origin name  

分支管理  
git branch name 创建name的分支  
git checkout name 切换分支  
git branch 查看分支，查看当前在哪个分支上  
切换到master分支上：git checkout master 
*代表你所在那个分支上  
合并分支代码到master（需要先把分支切换到master分支上）：git merge 分支名  
删除分支（合并分支后，分支就没有作用）：git branch -d 分支名  

工作流  
Git 有三种状态，你的文件可能处于其中之一：已提交（committed）、已修改（modified）和已暂存（staged）。 已提交表示数据已经安全的保存在本地数据库中。 已修改表示修改了文件，但还没保存到数据库中。 已暂存表示对一个已修改文件的当前版本做了标记，使之包含在下次提交的快照中。
由此引入 Git 项目的三个工作区域的概念：Git 仓库、工作目录以及暂存区域。

创建GitHUb远程仓库
ssh-keygen -t rsa -C "注册的邮箱"   
ssh -T git@github.com 判断本地仓库和远程仓库是否连通    
git remote add origin git@github.com "添加远程仓库"  
git push -u origin master "第一次连接远程仓库推送"（默认把本地master和远程master关联）   
git pull origin <分支名> "把远程分支拉取回来到本地，同时把本地代码和远程代码合并  
origin 一般是源，认为是远程仓库  

总结
工作流： 工作区——》暂存区——》版本库  
初始化  git init ——》git add ——》gitcommit  
远程仓库：Git remote add ——>git pull(拉去最新的代码)——》git push ——>git clone  
分支管理：git branch ——>git checkout  

关于多人合作的经验  
  多用客户端和工具，少用命令行，除非在Linux服务器上直接开发  
  每次提交前，diff自己的代码，以免提交错误的代码  
 下班回家前整理好自己的工作区。  
 并行的项目，使用分支开发  
 遇到冲突时，搞明白冲突的原因，千万不要随意丢弃别人的代码  
 产品发布后，记得打Tag，免得不知道线上的版本，方便将来拉分支修复BUG  
 推送前使用git pull合并远程变化的代码  

附加信息
Ls -a 把隐藏和不隐藏的文件都显示  
Echo "git repo2" >> text.txt 管道追加(>>追加，echo是输出)  
