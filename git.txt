Github create and push remote repo

$ git init
Initialized empty Git repository in /home/network/

$ git add README.md

$ git commit -m "first commit"
[master (root-commit) adc1a5a] first commit
 1 file changed, 1 insertion(+)
 create mode 100644 README.md

$ git remote add origin git@github.com:howard6066/network.git
                        
$ git push -u origin master
Enter passphrase for key '/root/.ssh/id_rsa': 
Counting objects: 3, done.
Writing objects: 100% (3/3), 218 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To git@github.com:howard6066/network.git
 * [new branch]      master -> master
Branch master set up to track remote branch master from origin.



Git 命令整理

git add 新增檔案
#git add . 新增目錄下所有檔案

git commit 提交檔案
#git commit -m 'message' 直接提交，不進入編輯器
#git commit 提交檔案，進入編輯器
#git commit --amend 編輯已提交的註釋

git reset 回復檔案
#git reset 放棄add，保留修改
#git reset --hard 放棄所有修改，回到上個提交的狀態
#git reset --hard HEAD 回到最新提交的版本
#git reset --hard HEAD^ 回到前一個提交的版本

git branch 分支
#git branch 列出所有branch
#git branch -a 列出所有本地和遠端的branch
#git branch <new-branch> 依目前branch，建立新的branch

git checkout 切換
#git checkout <branch> 切換branch
#git checkout master 切換到master
#git checkout <new-branch> master 從master建立新的branch，並切換到新的branch
#git checkout -b <new-branch> 依目前branch建立新的branch，並切換到新的branch
#git checkout <file> 重新checkout此檔案

git log
#git log 列出所有log

git pull
#git pull 將遠端的檔案更新到本地

git push
#git push 將本地檔案更新到遠端