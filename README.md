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


