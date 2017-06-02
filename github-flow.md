## Github Flow的流程   
整个开发的流程大致如下：  

1.令master分支时常保持可以部署的状态  

2.进行新的作业时要从master分支创建新分支，新分支名称要具体可描述性
（所谓可描述性的名称，是指该名称可以直观正确地表达这个分支的特性，比如：user-content-cache-key 、submodules-init-task、redis2-transition 这样子做的目的是能够让其他人清楚地知道该分支正在进行什么工作）  

3.在2中新建的本地仓库分支进行提交  

4.在Github端仓库创建同名分支，定期push  
（由于除了master分支之外都是作业中的分支，所以push作业分支时不需要太多顾虑。在开发过程中，建议定期将本地仓库中创建的分支以同名的形式push到Github端的远程仓库）

5.需要帮助或反馈时创建pull request ，以pull request进行交流  

6.让其他开发者进行审查，确认作业完成后与master分支合并  

7.与master分支何并后立即部署  
（代码合并至master分支后且通过所有自动测试之后，需要立刻进行部署。在部署之后，需要确认刚刚合并的代码是否存在问题）  

####  具有代表性的部署工具  
|名称 | URL | 备注 |  
|--------|   -------- |  --------- | 
| [Capistrano](https://github,com/capistrano/capistrano) | https://github,com/capistrano/capistrano| Ruby开发的代表性部署工具|  
|[Mina](https://github.com/nadarei/mina)|https://github.com/nadarei/mina|Ruby开发的部署工具|  
|[Fabric](http://fabfile.org)|http://fabfile.org|Python开发的部署工具|  
|[Cinnamon](https://github.com/kentaro/cinnamon)|https://github.com/kentaro/cinnamon|Perl开发的部署工具|    
|[Webistrano*](https://github.com/kentaro/webistrano)|https://github.com/kentaro/webistrano|可通过web执行capistrano的工具|   
|[Strano](https://github.com/joelmoss/strano)|https://github.com/joelmoss/strano|可通过web执行capistrano的工具，与webistrano采用的中间件不同|     

备注：[github是如何工作的](http://zachholman.com/posts/how-github-works/)



