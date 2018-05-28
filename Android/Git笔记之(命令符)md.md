## git 命令 ##
##**移除已经添加到git远程仓库的文件以及文件夹步骤**

- 1） git rm -rf 文件夹名
- 2） git commit -m "移除误操作的文件"
- 3） git push origin master
	
##上传项目到gitlab##
**（一）c盘下的：C/admin/.ssh下生成的id_rsa和id_rsa.pub 把id.rsa.pub放入gitlab生成的 Add an SSH Key 中**

- git config --global user.name "椰子"
- git config --global user.email "995852922@qq.com"
- ssh-keygen -t rsa -C "995852922@qq.com"




**（二）上传项目到gitlab命令**

- git config --global user.name "椰子"
- git config --global user.email "995852922@qq.com"
- git init
- git remote add origin ssh://git@42.123.127.93:10022/tyshawn/sdap1.git
- git add .
- git commit -m "程序源代码"
- git push -u origin master