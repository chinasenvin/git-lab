1.  
git config --global user.email "mail@email.com"   //github's registration email address e.g. mail@163.com  
git config --global user.name "username"  //github's registration user name

2.  
create new repository on https://github.com/  
```
git remote add origin https://github.com/chinasenvin/git-lab.git  
git push -u origin master
```

3.  
chinasenvin@pc MINGW32 /d/git  
$ git init git-lab  
Initialized empty Git repository in D:/git/git-lab/.git/  
$ git remote -v  
fatal: Not a git repository (or any of the parent directories): .git  
$ cd git-lab  
$ git remote -v  
$ git remote add origin https://github.com/chinasenvin/git-lab.git  
$ git remote -v  
origin https://github.com/chinasenvin/git-lab.git (fetch)  
origin https://github.com/chinasenvin/git-lab.git (push)  

4.  
$ git push -u origin master  
error: src refspec master does not match any.  
error: failed to push some refs to 'https://github.com/chinasenvin/git-lab.git'  
>原因分析
>引起该错误的原因是，目录中没有文件，空目录是不能提交上去的

5.  
$ git add create_repository.md  
$ git commit -m 'create_repository.md commit'  
[master (root-commit) 8457f88] create_repository.md commit  
 1 file changed, 23 insertions(+)  
 create mode 100644 create_repository.md  
$ git push -u origin master  
fatal: unable to access 'https://github.com/chinasenvin/git-lab.git/': Failed to connect to github.com port 443: Timed out  


