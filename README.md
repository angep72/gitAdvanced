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
ca6ecf1 (ft/test.md) HEAD@{13}: rebase (start): checkout HEAD




### Part2 
## challenge 1
HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)
$ git checkout -b ft/new-feature
Switched to a new branch 'ft/new-feature'

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/new-feature)

## Challenge 2

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/new-feature)
$ git commit -m "Implemented core functionality for new feature"
[ft/new-feature 49a428c] Implemented core functionality for new feature
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 feature.txt

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/new-feature)

## Chalenge3 
P@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/new-feature)
$ git checkout main 
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)
$ git checkout -b readme.txt
Switched to a new branch 'readme.txt'

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (readme.txt)
$ git checkout main 
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)
$ git branch -d readme.txt
Deleted branch readme.txt (was 8567ece).

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)
$ git add readme.txt

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)
$ git commit -m "Updated project readme"
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Readme.txt

nothing added to commit but untracked files present (use "git add" to track)

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)
$ git add readme.txt

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)
$ git add Readme.txt

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)
$ git commit -m "Updated project readme"
[main ae31a66] Updated project readme
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 Readme.txt

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)
$ git push 
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 250 bytes | 250.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/angep72/gitAdvanced.git
   8567ece..ae31a66  main -> main

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)

## Chalenge 4 
HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/new-feature)
$     git push --set-upstream origin ft/new-feature
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (5/5), 527 bytes | 527.00 KiB/s, done.
Total 5 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/new-feature' on GitHub by visiting:
remote:      https://github.com/angep72/gitAdvanced/pull/new/ft/new-feature
remote:
To https://github.com/angep72/gitAdvanced.git
 * [new branch]      ft/new-feature -> ft/new-feature
branch 'ft/new-feature' set up to track 'origin/ft/new-feature'.

## Challenge 5 
HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)
$ git branch -d ft/new-feature
Deleted branch ft/new-feature (was e1c100b).

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)
$
## Chalenge 6

commit ddcc06a54e1db11179e643b639b6b792b4ab7d78

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)
$ git checkout -b ft/new-branch-from-commit 18a37249823d15b09d61020d7e234f2c492eb073
Switched to a new branch 'ft/new-branch-from-commit'

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/new-branch-from-commit)
$ git status 
On branch ft/new-branch-from-commit
nothing to commit, working tree clean

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/new-branch-from-commit)
$ git status
On branch ft/new-branch-from-commit
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        t.js

nothing added to commit but untracked files present (use "git add" to track)

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/new-branch-from-commit)
$ git add . 

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/new-branch-from-commit)
$ git commit -m "helo"
[ft/new-branch-from-commit a7d4796] helo
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 t.js

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/new-branch-from-commit)
$ git push 
fatal: The current branch ft/new-branch-from-commit has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/new-branch-from-commit

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/new-branch-from-commit)
$ git push --set-upstream origin ft/new-branch-from-commit
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 228 bytes | 228.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/new-branch-from-commit' on GitHub by visiting:
remote:      https://github.com/angep72/gitAdvanced/pull/new/ft/new-branch-from-commit
remote:
To https://github.com/angep72/gitAdvanced.git
 * [new branch]      ft/new-branch-from-commit -> ft/new-branch-from-commit
branch 'ft/new-branch-from-commit' set up to track 'origin/ft/new-branch-from-commit'.

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/new-branch-from-commit)
$

## Challenge 7 

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)
$ git pull 
Updating 675744e..875afc1
Fast-forward
 t.js | 0
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 t.js

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)
 
 ##Challenge 8
 HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/new-branch-from-commit)
$ git rebase -i HEAD~1
Stopped at a7d4796...  helo
You can amend the commit now, with

  git commit --amend 

Once you are satisfied with your changes, run

  git rebase --continue

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/new-branch-from-commit|REBASE 1/1)
$ git rebase --continue 
Successfully rebased and updated refs/heads/ft/new-branch-from-commit.

## Challenge 9 
HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)
$ git branch -m ft/new-branch-from-commit ft/improved-branch-name

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)
$ git branch 
  ft/branch
  ft/improved-branch-name
  ft/test.md
* main
## Challenge 10 
HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)
$ git checkout 957125e052116f2f621809acd376f6296a19ee8b
Note: switching to '957125e052116f2f621809acd376f6296a19ee8b'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at 957125e Challenge8 part2 done

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced ((957125e...))

### Part 3 
Challenge 1 

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)
$ git stash
Saved working directory and index state WIP on main: e3f90df Challenge 10 part 2 done

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)
$ 
 ## Chalenge 2 
 HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)
$ git stash pop
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
Dropped refs/stash@{0} (e0c943bf04050706aa5bd175f21d7e4a3ed3898d)
 

 ## Challenge 3 
 HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/new-feature)
$ git merge
Updating f128378..7d2da53
Fast-forward
 helloeee.js | 2 +-
 1 file changed, 1 insertion(+), 1 deletion(-)

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/new-feature)

## Challenge 4

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)
$ git mergetool

This message is displayed because 'merge.tool' is not configured.
See 'git mergetool --tool-help' or 'git help config' for more details.
'git mergetool' will now attempt to use one of the following tools:
opendiff kdiff3 tkdiff xxdiff meld tortoisemerge gvimdiff diffuse diffmerge ecmerge p4merge araxis bc codecompare smerge emerge vimdiff nvimdiff       
No files need merging.

## Challenge 5
HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/new-feature)
$ git checkout ft/test.md
Switched to branch 'ft/test.md'
Your branch and 'origin/ft/test.md' have diverged,
and have 2 and 9 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

  ## Challenge 6
  itAdvanced (main)
$ git add test.gitignore

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)
$ git commit -m "git ignore"
[main c992cd8] git ignore
 1 file changed, 1 insertion(+)
 create mode 100644 test.gitignore

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)
$ git push 
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 273 bytes | 91.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0  
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/angep72/gitAdvanced.git
   1392bb4..c992cd8  main -> main

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)
$

### Challenge 7
itAdvanced (main)
$ git tag v1.0

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)

## Challenge 8 
HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)       
$ git tag 
v1.0
HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)       
$ git tag -d v1.0
Deleted tag 'v1.0' (was de06127)

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)
$ 

## Challenge 9 
HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)       
$ git push 
$ git push
Writing objects: 100% (3/3), 386 bytes | 193.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/angep72/gitAdvanced.git
   87d9d62..6d3fca8  main -> main
   ## Challenge 10 
   


