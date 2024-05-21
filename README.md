## Challenge 1
HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/test.md)
$ git rebase -i HEAD~3
[detached HEAD 92b1c04] first-challenge
 Date: Tue May 21 12:07:15 2024 +0200
 1 file changed, 70 insertions(+)
 create mode 100644 README.md
Successfully rebased and updated refs/heads/ft/test.md.

## Challeng 2
HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/test.md)
$ git commit --amend
[ft/test.md 69fdcbc] I have added test4 file
 Date: Tue May 21 11:57:15 2024 +0200
 4 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test1.md
 create mode 100644 test2.md
 create mode 100644 test3.md
 create mode 100644 test4.md
 ## Challenge 3
HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/test.md)
$ git push 
pick 10d9855 first-challenge
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 310 bytes | 310.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/angep72/gitAdvanced.git
   10d9855..5dae88d  ft/test.md -> ft/test.md

## Challenge 4

edit c501f93 splitting
$ git rebase -i HEAD~2
fatal: It seems that there is already a rebase-merge directory, and
I wonder if you are in the middle of another rebase.  If that is the
case, please try
        git rebase (--continue | --abort | --skip)
If that is not the case, please
        rm -fr ".git/rebase-merge"
and run me again.  I am stopping in case you still have something
valuable there.


HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/test.md|REBASE 1/5)
$ git rebase --abort

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/test.md)
$ git rebase -i HEAD~2
Stopped at c501f93...  splitting
You can amend the commit now, with

  git commit --amend

Once you are satisfied with your changes, run

  git rebase --continue

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/test.md|REBASE 1/6)
$ git reset HEAD^
Unstaged changes after reset:
M       README.md

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/test.md|REBASE 1/6)
$ git status
interactive rebase in progress; onto 578a3c3
Last command done (1 command done):
   edit c501f93 splitting
Next commands to do (5 remaining commands):
   pick ac7d1ec challenge three codes
   pick 10d9855 first-challenge
  (use "git rebase --edit-todo" to view and edit)
You are currently splitting a commit while rebasing branch 'ft/test.md' on '578a3c3'.
  (Once your working directory is clean, run "git rebase --continue")

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        test5.md
        test6.md

no changes added to commit (use "git add" and/or "git commit -a")

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/test.md|REBASE 1/6)
$ git add test5.md

## challenge 5
P@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)
$ git rebase -i HEAD~3
hint: Waiting for your editor to close the file...       0 [sig] bash 3870! sigpacket::process: Suppressing signal 18 to win32 process (pid 18516)     
                                                                                                                                                   226010 [sig] bash 3870! sigpacket::process: Suppressing signal 18 to win32 process (pid 18516)
[detached HEAD c61800e] Challege 3 and Challenge 4 squashe
 Date: Tue May 21 13:39:06 2024 +0200
 1 file changed, 74 insertions(+), 1 deletion(-)
Successfully rebased and updated refs/heads/main..
## Chalenge 6 

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/test.md)
$ git rebase -i HEAD~2
Successfully rebased and updated refs/heads/ft/test.md.

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/test.md)
$ git status
On branch ft/test.md
Your branch is behind 'origin/ft/test.md' by 1 commit, and can be fast-forwarded.
  (use "git pull" to update your local branch)

nothing to commit, working tree clean


## Challenge 7 

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/test.md)
$ git rebase -i HEAD~4
Successfully rebased and updated refs/heads/ft/test.md.

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/test.md)
$ git checkout main 
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)

## Challenge 8
HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)
$ git cherry-pick d019c3c35544d9b8b3d9d155eb07c01dd1b44a95
[main 5df3651] implemented test 5
 Date: Tue May 21 15:24:01 2024 +0200
 1 file changed, 1 insertion(+)
 create mode 100644 test5.md
 HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)

## Challenge 9
commit c336f56a26c1ccb308275383b8a77fa8b56140d8 (HEAD -> main, origin/main)
| Author: angep72 <p.umunyana@alustudent.com>
| Date:   Tue May 21 15:31:46 2024 +0200
|
|     challenge 8
|
* commit 5df36512329ef00e254e0cd1ac9aa43d2a05826b
| Author: angep72 <p.umunyana@alustudent.com>
| Date:   Tue May 21 15:24:01 2024 +0200
|
|     implemented test 5
|
* commit 0330cacdeaab34a70a84e2de9393b37d42524114
| Author: angep72 <p.umunyana@alustudent.com>
:
## Challenge 10 
HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)
$ git reflog 
54ac0df (HEAD -> main, origin/main) HEAD@{0}: commit: challenge 9 done
c336f56 HEAD@{1}: commit: challenge 8
5df3651 HEAD@{2}: cherry-pick: implemented test 5
0330cac HEAD@{3}: checkout: moving from ft/branch to main
d019c3c (ft/branch) HEAD@{4}: checkout: moving from main to ft/branch
0330cac HEAD@{5}: checkout: moving from ft/branch to main
d019c3c (ft/branch) HEAD@{6}: checkout: moving from main to ft/branch
0330cac HEAD@{7}: checkout: moving from ft/branch to main
d019c3c (ft/branch) HEAD@{8}: commit: implemented test 5
0330cac HEAD@{9}: checkout: moving from main to ft/branch
0330cac HEAD@{10}: commit: challenge 7
7ca6559 HEAD@{11}: checkout: moving from ft/test.md to main
ca6ecf1 (ft/test.md) HEAD@{12}: rebase (finish): returning to refs/heads/ft/test.md
ca6ecf1 (ft/test.md) HEAD@{13}: rebase (start): checkout HEAD~4




### Part2 
## challenge 1
HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)
$ git checkout -b ft/new-feature
Switched to a new branch 'ft/new-feature'

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/new-feature)