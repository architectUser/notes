# git笔记

```
2017.5.25

git笔记：

1.mkdir 创建一个新的根目录，仓库
2.touch 创建一个新的文件（文件格式不限）
3.a>b 将内容a放进b里
4.git init 创建仓库、git add b添加文件和git commit提交信息git log 查看提交历史记录
5.echo 输出，打印信息
6.diff 查看更改信息
7.status 展示现有状态（changed/new/deleted/modefined）
8.gitk --all 查看所有信息，（窗口形式打开）
9.git amend  修改最后提交的信息
10.如果你删除了一个在版本控制之下的文件，那么使用git add .不会在索引中删除这个文件。需要通过带-a选项的git commit命令和-A选项的git add命令来完成
11.rm 删除文件
12.git clone --bare 创建远端仓库
13.git push 推送
14.除了通过完整的URL来访问Git仓库外，还可以通过git remote add命令为仓库添加一个短名称。当你克隆了一个仓库以后，origin表示所克隆的原始仓库。即使我们从零开始，这个名称也存在。
15.git remote 查看已存在的远端仓库
16.git pull 拉取更改
17.git less 查看更改
18.如果错误的修改已经不是最新的commit，则只能使用git revert 还原。
19.
git clean -n
是一次clean的演习, 告诉你哪些文件会被删除. 记住他不会真正的删除文件, 只是一个提醒.

git clean -f
删除当前目录下所有没有track过的文件. 他不会删除.gitignore文件里面指定的文件夹和文件, 不管这些文件有没有被track过.

git clean -f <path>
删除指定路径下的没有被track过的文件.

git clean -df
删除当前目录下没有被track过的文件和文件夹.

git clean -xf
删除当前目录下所有没有track过的文件. 不管他是否是.gitignore文件里面指定的文件夹和文件.
20.你可以提取老版本的代码，通过提交的ID。git log命令可以查看提交ID 。checkout 后加commit id就是把commit的内容复制到index和工作副本中
21.cat主要有三大功能：
1.一次显示整个文件。$ cat filename
2.从键盘创建一个文件。$ cat > filename  
   只能创建新文件,不能编辑已有文件.
3.将几个文件合并为一个文件： $cat file1 file2 > file
参数：
-n 或 --number 由 1 开始对所有输出的行数编号
-b 或 --number-nonblank 和 -n 相似，只不过对于空白行不编号
-s 或 --squeeze-blank 当遇到有连续两行以上的空白行，就代换为一行的空白行
-v 或 --show-nonprinting
22.merge 我们可以合并两个不同分支的结果。Merge通过所谓的三路合并来完成。分别来自两个分支的最新commit和两个分支的最新公共commit。一旦合并发生了冲突，Git会标志出来，开发人员需要手工的去解决这些冲突。解决冲突以后，就可以将文件添加到索引中，然后提交更改
23.创建分支 git branch
   查看分支 git branch -a/git branch
   删除分支 git branch -d
24.push 推送（push）一个分支到远端仓库
25.git mergetool 编辑文件
26.rebase 合并多个commit为一个。
27.Linus为Linux Kernel Project发起的版本控制项目。
HEAD代表当前最新状态。
tag为某个状态的标签。
SHA1为每个提交日志的唯一标识。
 
install:
 
apt-get install git-core
 
 
git clone:
 
git仓库可以使用git clone获得：
git clone git://url
 
也可以通过浏览器浏览。
http://url/gitweb/
 
通过git pull更新仓库，使用git init-db初始化自己的仓库。
 
 
config:
 
开发人员需要为git仓库配置相关信息，这样在提交代码时，这些信息会自动
反映在git仓库的日志中。
 
git config user.name "your name"
git config user.email 

```