## 文件相关操作  
一般文件的左侧会显示该文件的行号，加入我们点击第10行的行号，这一行就会被高亮标记为黄色，同时URL末尾会自动添加"#L10"。使用这个URL，程序猿们在交流时,
就可以将讨论明确指向某一行。另外，如果将“#L10”改成"#L10-15",则会标记该文件的第10~15行。
## 查看分支之间的差别 
比如我们想要查看[Ruby on Rails](https://github.com/rails/rails) 4-0-stable分支和3-2-stable分支之间的差别，可以像下面这样将分支名加到URL里面。  
`https://github.com/rails/rails/compare/4.0-stable...3-2.stable`    
这样子就能查看两个分支之间的差别了  
## 查看与几天之前的差别  
假如我们想查看master分支在最近七天内的差别，可以像下面这样将时间加入URL  
`https://github.com/rails/rails/compare/master@{7.day.ago}...master`  
这样就就能查看这段期间内的差别了。    
- day  
- week  
- month  
- year  
指定期间可以使用以下四个时间单位，如果差别过大则不会列出所有提交，只显示最近的一部分。  
## 查看与指点日期之间的差别  
加入我们想查看master分支2013年1月1日与现在的区别，可以将日期加入URL  
`https://github.com/rails/rails/compare/master@{2013-01-01}...master`  

