# Sandbox git repo / My test git repo.
this is a test repo for practice with push/pull/clone ect.. with gitbash. 

anyone is free to practice git with this repo PR's will all be accepted. 

*************************************************
Adding directions and bash terminal "info/output"
**************************************************
 # ProTip! Use the URL for this page when adding GitHub as a remote.

***********************************************
helpful links if you have problems pushing code
answers to ERRORS i encountered 

*********************************************************
# Some other helpful commands
echo "# git-Tutorial-repo" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin <url>
git push -u origin master
 OR
git remote add origin https://github.com/singhofen/git-Tutorial-repo.git
git push -u origin master

********************************************************************
https://stackoverflow.com/questions/20939648/issue-pushing-new-code-in-github

https://github.com/rtyley/bfg-repo-cleaner/issues/29

https://stackoverflow.com/questions/24357108/git-updates-were-rejected-because-the-remote-contains-work-that-you-do-not-have/43574620

# Quick git instructions
1. Download zip repo
2. right click on project open via gitbash here
3. make any changes you wish to the project
4. git status to veiw midified files
5. git add . (all) or name of specific file
6. git commit -m 'message to github'
7. git push

*************************************************
# Creating new branch ~ sample terminal ~ what you may see on you local machine.
Dont push your newly created branch to master unsless you are done with changes and making files for current project

$ git checkout -b testBranch
Switched to a new branch 'testBranch'

$ touch testBranch.html

$ git status
On branch testBranch
Untracked files:
  (use "git add <file>..." to include in what will be committed)

        testBranch.html

nothing added to commit but untracked files present (use "git add" to track)

$ git add testBranch.html

$ git status
On branch testBranch
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   testBranch.html

$ git commit -m 'added test branch'
[testBranch 7b2a1a9] added test branch
 1 file changed, 26 insertions(+)
 create mode 100644 testBranch.html

$ git status
On branch testBranch
nothing to commit, working tree clean

$ git push
fatal: The current branch testBranch has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin testBranch

$ git push --set-upstream origin testBranch

$ git status
On branch testBranch
Your branch is up-to-date with 'origin/testBranch'.

$ touch test.txt

$ git status
On branch testBranch
Your branch is up-to-date with 'origin/testBranch'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        test.txt

nothing added to commit but untracked files present (use "git add" to track)

$ git add .

$ git status
On branch testBranch
Your branch is up-to-date with 'origin/testBranch'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   test.txt

$ git commit -m 'added test txt file'
[testBranch c5c7f1c] added test txt file
 1 file changed, 5 insertions(+)
 create mode 100644 test.txt

$ git push

$ git checkout master
Switched to branch 'master'
Your branch is up-to-date with 'origin/master'.

$ git status
On branch master
Your branch is up-to-date with 'origin/master'.

nothing to commit, working tree clean


**************************************************
$ git push -f origin master <--will force push to github but may lose all previous files

# below is a sample list of instructions/commands used for gitflow. You can use it as a snapshot of what is to be expected I/O.

*****************************************
$ touch README.md

$ git add .

$ git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   README.md

$ git commit -m 'edited readme'
[master 95d7c99] edited readme
 1 file changed, 4 insertions(+)
 create mode 100644 README.md

$ git push
fatal: The current branch master has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin master

$ git push --set-upstream origin master
fatal: HttpRequestException encountered.
   

$ git pull
Already up-to-date.

$ touch git-test.html

$ git status
On branch master
Your branch is up-to-date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        git-test.html

nothing added to commit but untracked files present (use "git add" to track)

$ git add .

$ git status
On branch master
Your branch is up-to-date with 'origin/master'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   git-test.html
$ git commit -m 'added git test file'
[master 72d8ea2] added git test file
 1 file changed, 16 insertions(+)
 create mode 100644 git-test.html

$ git push

$ git status
On branch master
Your branch is up-to-date with 'origin/master'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

$ git commit -m 'edited readme file'
On branch master
Your branch is up-to-date with 'origin/master'.

Changes not staged for commit:
        modified:   README.md
no changes added to commit

$ git add .

$ git status
On branch master
Your branch is up-to-date with 'origin/master'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   README.md

$ git commit -m 'edited readme file'
[master 2a0bc00] edited readme file
 1 file changed, 2 insertions(+), 2 deletions(-)

$ git push


