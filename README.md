# how_to_use_git_simply
just for new user to user github

refer to below tutorial:
https://www.jianshu.com/p/c70ca3a02087

Upload the local repository to github.

1. run below command line
    git init
    
    git add README.md
    
    git commit -m "first commit"
    
    git remote add origin git@github.com:Reid00/ping_url.git
    
    git push -u origin masterv
    

2.执行指令：git remote add origin https://github.com/hanyuntao/text.git

    2.1 如果关联出现错误 fatal: remote origin already exists，则执行下列语句再进行关联
  
    2.2 git remote rm origin
  
3.上传本地代码 执行指令：git push -u origin master

    3.1 如果在推送时出现错误 error:failed to push som refs to.......，则执行下列语句
  
    3.2 git pull origin master
  
    3.3 If with this error: fatal: refusing to merge unrelated histories, run the next
  
    3.4 git pull origin master --allow-unrelated-histories
  

使用git clone github的项目到本地和提交项目到github

1.git clone项目到本地

在多人开发中，一般的项目有master和其他分支，那么clone操作就需要你指定对应的分支把项目工程clone到本地，

    1.1 首先新建一个空文件夹，把文件夹进行git初始化操作,在文件夹的根目录下，右键选择git bash here，在弹出的窗体中输入命令：git init
  
    这样就把该文件夹git初始化了
  
    1.2 接下来就是clone操作了，继续输入命令：git clone xx(此处为你的项目的git地址），一般这个命令clone下来的是master分支的项目，你也可以clone指定分  支的工程，命令：git clone -b 分支名 git地址

2.使用git把本地项目提交到github

    2.1 如果该工程没有git初始化，那么在工程根目录下使用git init进行初始化，如果已经初始化，则省略这步
  
    2.2 将项目的文件添加到仓库中使用git add，（git add . ）表示将所有文件都添加，（git add xx(指定文件)）表示将指定文件添加进去
  
    2.3 将add的文件commit到仓库，命令：git commit -m "你想写的注释"
  
      2.3.1 （创建分支）git branch test
      
      2.3.2 （切换分支）git checkout test
      
    2.4 将本地的仓库关联到github上，命令如下：git remote add origin xxx（此处为你的git地址）
  
    2.5 在进行push之前，先进行pull操作，命令如下：git pull origin xxx(此处为你的分支名如test，master或者其他分支名)
  
    2.6 上传代码到github远程仓库，命令如下：git push -u origin xxx（此处为你的分支名），在这个步骤中可能会有弹窗要你输入你的用户名和密码，按照指示操作即可


