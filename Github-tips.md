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
## 获取diff格式与patch格式的文件  
对于长期投身于软件开发的人来说，有时可能会希望以diff格式文件和patch格式的文件来处理Pull Requeset。  
举个例子，假设Pull Request的URL如下所示。  
`https://github.com/用户名/仓库名/pull/28`  
如果想获取diff格式的文件，只要像下面这样在URL末尾，添加`.diff` 即可。  
`https://github.com/用户名/仓库名/pull/28.diff`  
同理，想要patch格式的文件，只要在URL末尾添加`.patch` 即可.  
`https://github.com/用户名/仓库名/pull/28.patch`  
## 引用评论  
在Conversation中人们通过添加评论进行对话，这里用一个简单的方法可以帮助你引用某个人的评论，选中想要引用的评论然后按R键，被选择的部分就会自动以评论语法写入评论文本框中，该快捷键在issue中同样有效。  
 
## 添加表情符号  
[emoji表情符号速查](https://www.webpagefx.com/tools/emoji-cheat-sheet/)    
## pull request中文件的改动  
- file changed 标签页中可以查看当前pull request 更改的文件内容以及前后的差别，标签上的数字表示新建及被改动的文件数。默认情况下系统会将空格的不同也高亮显示，所以在空格用改动的情况下会难以阅读。这时候只要在URL的末尾添加`？w=1`就可以不显示空格的差别。  
- 将鼠标指针放在被更改行号的左侧，我们会看到一个加号。点击这个加号可以在代码中插入评论，这样，评论是针对哪行代码的就一目了然了。 这个插入评论的功能让针对代码的评论变得十分顺畅。特别是在多人协作的软件开发中，这个功能更加不可或缺。  
## 在WIKI中显示侧边栏  
所有wiki页面都可以显示侧边栏。做法很简单，只要创建名为`_sidebar`的页面即可。`_sidebar`页不会显示在page的页面一览中。在编辑个页面时页面下部会附加Sidebar段。  
## pulse  
pulse 是体现该仓库软件开发活跃度的功能，根据这个页面，用户可以判断目前这个软件是否正在被积极开发，或者持有仓库修改权限的人是否在认真的进行BUG修正等维护工作。在挑选Github上的开发的软件时，它可以作为一个重要的衡量标准。  




