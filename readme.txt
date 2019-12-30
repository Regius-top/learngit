1.创建git的版本库
	$ mkdir learngit
	$ cd learngit 
2.讲创建的目录改为git可以管理的仓库
	$ git init
	$ ls -ah
3.把文件添加到版本库 
第一步：用命令 git add <ffile> 告诉git，把文件添加到仓库       
	$ git add readme.txt
第二步：用命令 git commit -m <message> 告诉git，把文件提交到仓库
	$ git commit -m "wrote a readme file"
4.创建身份标识
	$ git config --global user.email "431592711@qq.com"
	$ git config --global user.name "Regius"
5.查看工作区的状态
	$ git status
  查看修改的内容
	$ git diff readme.txt
6.历史记录
	1）查看历史记录
	$ git log
	2)查看日志记录——简化成时间线
	$ git log --pretty=oneline
	3)回到上一个版本
	$ git reset --hard HEAD^
	4)回到某个版本
	$ git reset --hard af52(版本号)
	5）记录每一次命令
	$ git reflog
	6)
	场景1：当你改乱了工作区某个文件的内容，想直接丢弃工作区的修改时，用命令git checkout -- file。

	场景2：当你不但改乱了工作区某个文件的内容，还添加到了暂存区时，想丢弃修改，分两步，第一步用命令git reset 		HEAD <file>，就回到了场景1，第二步按场景1操作。

	场景3：已经提交了不合适的修改到版本库时，想要撤销本次提交，参考版本回退一节，不过前提是没有推送到远程库。



























