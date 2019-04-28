1. 提交

   ```
   git add .
   git commit -m "balabala"
   git status
   撤销readme.txt文件在工作区的修改：git checkout -- readme.txt
   把暂存区的修改回退到工作区：git reset HEAD readme.txt
   
   ```

2. 分支

   ```
   查看分支：git branch
   
   查看远程分支：git branch -r 
   
   查看所属分支：git branch -a
   
   创建分支：git branch <name>
   
   切换分支：git checkout <name>
   
   创建+切换分支：git checkout -b <name>
   
   合并某分支到当前分支：git merge <name>
   
   删除分支：git branch -d <name>
   
   删除远端分支：git push origin --delete <name> 
   ```

3. 本地仓库与远程库关联

   ```
   $ git remote add origin git@github.com:michaelliao/learngit.git
   ```

4. 从远程库克隆到本地
    	```
    $ git clone git@github.com:hanchenchen-DLUT/OJ.git
	```



https://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000

廖雪峰的git教程