# Part1
## Challenge 1  
P@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (main)
$ git checkout -b ft/test.md
Switched to a new branch 'ft/test.md'

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/test.md)
$ git add test1.md

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/test.md)
$ git add test2.md

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/test.md)
$ git add test3.md

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/test.md)
$ git commit -m "create initial file "
[ft/test.md (root-commit) 3bbe5c7] create initial file
 3 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test1.md
 create mode 100644 test2.md
I have added test4 file 
 create mode 100644 test3.md

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/test.md)
$ git status
On branch ft/test.md
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        test4.md

nothing added to commit but untracked files present (use "git add" to track)

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/test.md)
$ git add test4.md

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/test.md)
$ git commit --amend
[ft/test.md 69fdcbc] I have added test4 file
 Date: Tue May 21 11:57:15 2024 +0200
 4 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test1.md
 create mode 100644 test2.md
 create mode 100644 test3.md
 create mode 100644 test4.md

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/test.md)
$ git push 
fatal: The current branch ft/test.md has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/test.md

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/test.md)
$ git push --set-upstream origin ft/test.md
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 239 bytes | 119.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/angep72/gitAdvanced.git
 * [new branch]      ft/test.md -> ft/test.md
branch 'ft/test.md' set up to track 'origin/ft/test.md'.

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/test.md)

## Challenge2
HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/test.md)
$ git push
Everything up-to-date

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/test.md)
$ git rebase  HEAD~2
Current branch ft/test.md is up to date.

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/test.md)
$ git rebase  -i HEAD~2
Successfully rebased and updated refs/heads/ft/test.md.

HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/test.md)


## challenge 3
HP@DESKTOP-1CTEVNT MINGW64 ~/OneDrive/Desktop/TheGym/gitAdvanced (ft/test.md)
$ git rebase -i HEAD~3
[detached HEAD 92b1c04] first-challenge
 Date: Tue May 21 12:07:15 2024 +0200
 1 file changed, 70 insertions(+)
 create mode 100644 README.md
Successfully rebased and updated refs/heads/ft/test.md.
