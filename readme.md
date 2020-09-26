
Learning Git 


akd70 (master #) learning_git
$ touch index.html
akd70 (master #) learning_git
$ touch app.js
akd70 (master #) learning_git
$ git init
Initialized empty Git repository in C:/Users/akd70/OneDrive/Desktop/learning_git/.git/
akd70 (master #) learning_git
$ git config --global user.name 'Ankit Dixit'

akd70 (master #) learning_git
$ git config --global user.email 'tiknazen@gmail.com'
akd70 (master #) learning_git
$ git add index.html
akd70 (master +) learning_git
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   index.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        app.js

akd70 (master +) learning_git
$ git rm --cached index.html
rm 'index.html'
akd70 (master #) learning_git
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        app.js
        index.html

nothing added to commit but untracked files present (use "git add" to track)
akd70 (master #) learning_git

Adds all the file of extension of .html to the staging area:
$ git add *.html
akd70 (master +) learning_git
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   index.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        app.js


Remove the Fles from the staging area:
akd70 (master +) learning_git
$ git rm --cached index.html
rm 'index.html'


Adds all the file in the staging area: 
akd70 (master +) learning_git
$ git add .
akd70 (master +) learning_git
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   app.js
        new file:   index.html

After modifying the html file checking the status:
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   app.js
        new file:   index.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   index.html



akd70 (master *+) learning_git
$ git add .
akd70 (master +) learning_git
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   app.js
        new file:   index.html

2 Types of commit:
By adding comment within the command:
$ git commit -m 'Changed app.js'
[master 7dbe459] Changed app.js
 1 file changed, 1 insertion(+)
By the default code editor opened when the git commit command is typed and we give the comment in the code editor.

If we don’t want to use any file we use git ignore:
We will add the log.txt in the .gitignore and can see the output as followed.
akd70 (master) learning_git
$touch .gitignore
akd70 (master) learning_git
$ touch log.txt
akd70 (master) learning_git
$ git add .
akd70 (master +) learning_git
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   .gitignore
After creating 2 folders dir1 and dir2 with respective files app1.js and app2.js. We add the dir2 folder in the git ignore and save it.
akd70 (master *+) learning_git
$ git add .
akd70 (master +) learning_git
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   .gitignore
        new file:   dir1/appp1.js


akd70 (master +) learning_git
$ git branch login
akd70 (master +) learning_git
$ git commit -m 'added git ignore,dir1,dir2,txt'
[master 66b3331] added git ignore,dir1,dir2,txt
 2 files changed, 3 insertions(+)
 create mode 100644 .gitignore
 create mode 100644 dir1/appp1.js
akd70 (master) learning_git
$ git checkout login
Switched to branch 'login'
akd70 (login) learning_git
$ touch login.html
akd70 (login) learning_git
$ git add .
akd70 (login +) learning_git
$ git commit -m 'login form'
[login 10feee6] login form
 4 files changed, 3 insertions(+)
 create mode 100644 dir2/app2.js
 create mode 100644 log.txt
 create mode 100644 login.html
akd70 (login) learning_git
$ git checkout master
Switched to branch 'master'
akd70 (master) learning_git
$ git merge login
hint: Waiting for your editor to close the file...
Merge made by the 'recursive' strategy.
 dir2/app2.js | 1 +
 index.html   | 1 +
 log.txt      | 1 +
 login.html   | 0
 4 files changed, 3 insertions(+)
 create mode 100644 dir2/app2.js
 create mode 100644 log.txt
 create mode 100644 login.html





Github:
After making a repository in github
akd70 (master) learning_git
$ git remote
akd70 (master) learning_git
$ git remote add origin https://github.com/tiknazendev/learninggit.git
akd70 (master) learning_git
$ git remote
origin

akd70 (master) learning_git
$ git push -u origin master
Enumerating objects: 19, done.
Counting objects: 100% (19/19), done.
Delta compression using up to 8 threads
Compressing objects: 100% (12/12), done.
Writing objects: 100% (19/19), 1.55 KiB | 396.00 KiB/s, done.
Total 19 (delta 4), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (4/4), done.
To https://github.com/tiknazendev/learninggit.git
 * [new branch]      master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.
akd70 (master) learning_git
$ touch readme.md

