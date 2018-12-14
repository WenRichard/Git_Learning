# git上传文件通用步骤
- 首先仓库初始化  
 git init

- 添加远程服务器（个人，组织都可以）   
git remote add origin  **git@github.com:SCU-B418/B418_public_test.git**   

- 不单独上传某个文件 或  单独上传某个文件  
  git add **.**  
  git add **test.txt**  

- 本地提交，-m后面输入的是本次提交的说明，可以输入任意内容，当然最好是有意义的，这样你就能从历史记录里方便地找到改动记录。  
git commit -m"first" 

- 上传到服务器  
git push -u origin master  

- 如果出现错误，用：  
git pull --rebase origin master  
git push -u origin master  
