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
4.创建省份标示
	$ git config --global user.email "431592711@qq.com"
	$ git config --global user.name "Regius"

