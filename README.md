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
