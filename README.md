# Sandbox git repo / My test git repo.
this is a test repo for practice with push/pull/clone ect.. with gitbash. 

anyone is free to practice git with this repo PR's will all be accepted. 

*****************************
Adding directions and bash terminal "info/output"

***********************************************
helpful links if you have problems pushing code
 answers to ERRORS i encountered 

https://stackoverflow.com/questions/20939648/issue-pushing-new-code-in-github

https://github.com/rtyley/bfg-repo-cleaner/issues/29

https://stackoverflow.com/questions/24357108/git-updates-were-rejected-because-the-remote-contains-work-that-you-do-not-have/43574620



**************************************************
$ git push -f origin master
fatal: HttpRequestException encountered.
   An error occurred while sending the request.
Username for 'https://github.com': singhofen
Counting objects: 23, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (23/23), done.
Writing objects: 100% (23/23), 10.96 KiB | 273.00 KiB/s, done.
Total 23 (delta 18), reused 0 (delta 0)
remote: Resolving deltas: 100% (18/18), done.
To https://github.com/singhofen/git-Tutorial-Test-repo.git
 + 2f65c14...9df37f9 master -> master (forced update)

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
   An error occurred while sending the request.
Username for 'https://github.com': singhofen
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 397 bytes | 79.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/singhofen/git-Tutorial-Test-repo.git
   9df37f9..95d7c99  master -> master
Branch master set up to track remote branch master from origin.

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
fatal: HttpRequestException encountered.
   An error occurred while sending the request.
Username for 'https://github.com': singhofen
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 651 bytes | 130.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/singhofen/git-Tutorial-Test-repo.git
   95d7c99..72d8ea2  master -> master

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
fatal: HttpRequestException encountered.
   An error occurred while sending the request.
Username for 'https://github.com': singhofen
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 342 bytes | 85.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/singhofen/git-Tutorial-Test-repo.git
   72d8ea2..2a0bc00  master -> master

