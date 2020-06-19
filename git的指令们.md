### 指令
1. git init :初始化
2. git config --global user.name xxx : 设置全局用户名。
3. git config --global user.email xxx : 设置全局用户邮箱。
4. git config --list : 查看全局配置信息。
5. git add xxx(文件名) :将xxx文件放入暂存区
6. git commit -m:提交一次版本
   - 后面要写此次提交版本的描述信息 -m，例：git commit -m 'project init'
7. git add . : 全部文件放入暂存区
8. git status : 查看当前的状态
9. git log : 提交的若干版本的信息。
10. git diff : 查看两版本的差异。
11. git diff HEAD : 比较工作区与本地版本库中最近一次commit的内容
12. git reflog : 查看历史操作记录。
13. git reset --(hard | soft | mixed) HEAD : 版本回退。  
    - hard: 回退全部至完整的上一个版本，包括HEAD,index,woking tree；
    - mixed: 暂存区和工作目录回退至上一个版本；
    - soft: 只回退暂存区内容。
    
14. git branch xxx : 创建新分支。
15. git checkout -b xxx : 创建并切换分支。
16. git merge <branch> : 无冲突合并。
17. git checkout -- <file> : 撤销工作区修改
18. git reset HEAD <file> : 撤销暂存区(缓存)文件，不覆盖工作区。
19. git reset --hard HEAD^ : 回退到上一次commit的状态。

### github
1. git remote add xxx : 添加远程的仓库(名字xxx)
2. git push xxx 'branch':代码提交到远程仓库xxx中的<分支>。
3. git pull xxx 'branch' : 更新本地文件(获取服务器端最新版本文件)
4. git clone ... : 复制下载某地址的项目

5. dir : 查看分支内所有文件
6. git rm -r --cached xxx : 删除远程仓库中的xxx文件或文件夹(执行完后要执行 commit提交和push更新 这两个命令才能生效)

#### 关联远程仓库
1. 命令行中：ssh-keygen,会产生一个秘钥，若本次关联操作之前已有生成的秘钥，则可省略此步。
    - 在执行此步后，系统会在C盘本机用户文件夹内生成文件夹.ssh，内有文件id_rsa.pub，记录生成的秘钥。
2. 打开GitHub中的settings设置，找到菜单：SSH and GPG keys选项，点击"New SSH key"新创建一个key，复制粘贴生成的key，添加。
3. 回到远程仓库界面，复制ssh地址，命令行切换至master分支，输入命令：git remote add xxx，后面加上2步骤中复制的地址，就完了。

       

#### 一个学习github的网站
&lt;https://learngitbranching.js.org/?locale=zh_CN&gt;


 

