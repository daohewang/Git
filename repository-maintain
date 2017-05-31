## 仓库的维护  
fork或clone来的仓库，一旦放置不管就会离最新的源代码越来越远。如果不以最新的源代码为基础进行开发，编写代码也可能是无用功。  
通常来说clone来的仓库实际上与原仓库没有任何关系，所以我们需要将原仓库设置为远程仓库，从该仓库获取（fetch）数据与本地仓库进行合并（merge），让本地仓库的源代码保持最新状态。  
**步骤：**

1. 仓库的Fork与clone    
将你想要fork的仓库作为原仓库，在Github上进行fork，然后clone至本地仓库  
> `git clone url地址`  

2. 给仓库设置名称   
我们给原仓库设置`upstream`的名称，将其作为远程仓库。  
> `git remote add upstream url地址`  

今后，我们的这个仓库将以`upstream`作为原仓库的标识符，这个环境下只需要设定一次即可。  

3. 获取最新的数据  
我们从远成仓库实际获取（fetch） 最新源代码，与自己仓库的分支进行合并。要让仓库维持最新状态，只需要重复这一操作即可。  
> `$ git fetch upstream  `   
> `$ git merge upstream/master `    

我们通过git    fetch 命令获取最新的数据，将`upstream/master`分支与当前分支（master）合并。这样一来，当前分支（ master）就获得了最新的源代码。一般情况下master分支都会获得最新代码，很少需要fork的开发者亲自进行修正。

 
 
