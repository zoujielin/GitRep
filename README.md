
# git命令学习
## 如何push到远程仓库
 1.git init   
 2.git add    
 3.git commit -m""  
 4.git remote add origin git@github.com:fang-king/Selenium.git 关联远程github上刚创建的库  
 5.git pull --rebase origin master或· git pull origin master //把远程信息拉倒本地并且合并  
 6.git push -u origin master  
 7.git push -f origin master 强制push  
 8.git 上传文件到仓库上提示：origin does not to be a git repository  
 重新输入一次：git remote add origin git@github.com:yourusername/test.git  
 然后再push   
 git remote add origin git@github.com:fang-king/Selenium.git 关联远程github上刚创建的库  
 yourusername/test.git为clone连接   

## 解决push或pull反复输入账号密码
如果我们git clone的下载代码的时候是连接的https://而不是git@git (ssh)的形式，   
当我们操作git pull/push到远程的时候，总是提示我们输入账号和密码才能操作成功，频繁的输入账号和密码会很麻烦。   
解决办法：   
git bash进入你的项目目录，  
输入：  
git config --global credential.helper store  
然后你会在你本地生成一个文本，  
上边记录你的账号和密码。当然这些你可以不用关心。  
然后你使用上述的命令配置好之后，    
再操作一次git pull，然后它会提示你输入账号密码，这一次之后就不需要再次输入密码了。  
分支：  
## 创建分支命令  
git branch 分支名  //创建分支不切换  
git checkout -b 分支名   //创建分支并且切换到新分支  
git ckeckout 分支名 //切换为远程分支,本地自动创建同名分支
git push origin :分支名 //删除远程仓库分支（注意origin后有空格  
git branch -a，//列出所有分支名称本地以及远程   
git checkout -b dev origin/dev，//作用是checkout远程的dev分支，在本地起名为dev分支，并切换到本地的dev  
git branch //
git branch -D master //删除本地分支  

## 文本编辑命令 
:wq保存  
vim编辑  
i插入  
esc退出  
touch 创建文件名

