# git分支提交  
### 目的：拉取分支，提交分支，删除分支，协同开发  

* #### 创建本地分支
  git branch test    (test是分支的名称，可以随便取)

* #### 查看分支创建是否成功，下面的命令可以得到现在仓库中的分支列表
  git branch

* #### master分支是仓库默认的主分支，把工作从master分支下切换到test分支下
  git checkout test

* #### 将新分支push到github
  git push origin test

* #### 提交当前分支信息
  注：可通过 ls 查看目录，cat查看文件具体信息
  git add 1.txt
  git commit -m"update"

* #### 切回master分支
  git checkout master

* #### 因为是合作开发项目，这时远程仓库中的内容有可能已经发生了变化，所以我们需要将远程仓库中的内容和本地分支中的内容进行合并
  git pull origin master

* #### 接下来要做的是将test分支合并到master上
  git merge test

* #### 最后一步，我们把修改的内容提交到主分支上
  git push origin master

* #### 删除分支
  git push origin :test
