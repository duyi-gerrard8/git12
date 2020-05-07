####指令
1. git init :初始化
2. git add xxx(文件名) :将xxx文件放入暂存区
3. git commit -m:提交一次版本
   - 后面要写此次提交版本的描述信息 -m，例：git commit -m 'project init'
4. git add . : 全部文件放入暂存区
5. git status : 查看当前的状态
6. git log : 提交的若干版本的信息。
7. git diff : 查看两版本的差异。
8. git diff HEAD : 比较工作区与本地版本库中最近一次commit的内容
9. git reflog : 查看历史操作记录。
10. git reset --(hard | soft | mixed) HEAD : 版本回退。  
    - hard: 回退全部至完整的上一个版本，包括HEAD,index,woking tree；
    - mixed: 暂存区和工作目录回退至上一个版本；
    - soft: 只回退暂存区内容。
    
11. git branch xxx : 创建新分支。
12. git checkout -b xxx : 创建并切换分支。

####github
1. git remote add xxx : 添加远程的仓库(名字xxx)
2. git push xxx :代码提交到远程仓库xxx。


 

