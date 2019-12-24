1、本地创建工程工作空间。例如（workspace）
2、进入工程的workspace，右键，选择git base here，执行以下操作
	a) git config --global user.name 'xx'  注：xx为公司邮箱前缀
	b) git config --global user.email 'xxx'  注：xx为公司邮箱
	c) git init 注：将当前目录用git进行管理
d) git remote add origin http://git.yonyou.com/yygov/A/fa/fa-8.5.git  注：将本地和   gitlab关联git remote add origin
e) git clone http://git.yonyou.com/yygov/A/fa/fa-8.5.git 注：克隆目录结构
f)  cd fa-8.5 注：切换到fa-8.5目录下
	g) git checkout -b develop 注：创建develop分支并进入该分支
	h) git pull origin develop 注：将git上的项目拉到本地

2.操作git
	a)git status 查看当前文件状态
	b)git add . 将当前文件夹中的内容加到本地git缓存
	c)git commit -m 'message' 将本地git缓存中的数据加到本地git仓库
	e)git push origin develop 将本地的develop分支推送到gitlab的develop分支




一般如果想要把某个文件下的文件上传到githup
 1，右键  git base here
 2,git init
 3,git config user.name 'githup的账号'
 4,git config user.email 'githup注册的邮箱'
 5,git remote add origin 远程仓库地址
 6,git add *
 7,git commit -m 'xxx'
 8,git push --set-upstream origin master
