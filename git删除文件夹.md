**github只能删除repository，不能里面单个删除的文件夹**  
方法：  
在从Github下拉的项目的根目录下右击点击'Git Bash Here'，打开Git Bash后输入：  
* git rm -r --cached graph  
--cached不会把本地的graph文件夹删除，但是要保证根目录不存在要删除的那个文件夹  
* git commit -m 'delete graph文件夹'   
单引号里为Commit时需要提交的说明  
* git push -u origin master    
若需要对其他分支进行操作，则把master换为对应分支，如:git push -u origin dev
