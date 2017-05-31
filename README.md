# 玩转git命令行  
## git基础篇  
- workspace:    工作区  
- Index/Stage: 暂存区  
- Repository:  仓库区/本地仓库  
- Remote:  远程仓库  
## git命令篇
git  config  --global user.name "你的注册名"                                          #设置初次使用Git时的名字 (名字请用英文)    
git config  --global  user.email  "你的注册邮箱"                                      #设置初次使用Git时的邮箱    


## git技巧篇

1.如何修改远程仓库地址    
- 修改命令：`git remote set-url origin [url]`
- 先删后加： `git remote rm origin `      `git remote add origin [url]`  
- 直接修改config文件 ` git config -e [--global]

2.如何提交文件夹到github远程仓库  
- $ git add floder_name/`*.*`       
- $ git add floder_name/*  

3.如何撤销一个合并   
- $ git merge  --abort  

4. 查看图片的差别       
[图片差别](https://github.com/blog/817-behold-image-view-modes)

