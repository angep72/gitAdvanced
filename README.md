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
