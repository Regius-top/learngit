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
