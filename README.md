# Portfolio Repository - eduwork-git

## Deskripsi
Repository ini menunjukkan pengalaman saya menggunakan Git dan GitHub, bernama: "eduwork-git", yang di dalamnya termasuk:
- Membuat folder dan branch repository;
- Menambahkan 2 file extensi .txt dan 1 file extensi .php;
- Mengelola riwayat kodingan;
- Menggunakan Git untuk manajemen kode versi.

## Struktur Repository
- **Main branch**: Berisi kode utama.
- **Feature branches**: Branch terpisah untuk pengembangan fitur baru --> dengan nama: "mytask" --> dan sudah dimerge ke main branch.

## Riwayat Pengembangan
1. Membuat repository lokal.
2. Menambahkan branch `mytask` untuk fitur A.
3. Mengintegrasikan perubahan ke branch `main`.

## Teknologi yang Digunakan
- Git
- GitHub

## Riwayat kodingan:
Riwayat kodingan untuk membuat folder dan dokumen repository ini adalah sebagai berikut,

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git
$ git init
Initialized empty Git repository in D:/Automate/eduwork-git/.git/

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (master)
$ ls -a
./  ../  .git/

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (master)
$ git branch -m master main

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (main)
$ git remote -v

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (main)
$ git remote add new-origin https://github.com/rahmileejiyoo/eduwork-git.git

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (main)
$ nano file1.txt

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (main)
$ git add file-1.txt
warning: in the working copy of 'file-1.txt', LF will be replaced by CRLF the next time Git touches it

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (main)
$ git add --renormalize file-1.txt

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (main)
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   file-1.txt


lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (main)
$ git commit -m "upload new file"
[main (root-commit) b7965e2] upload new file
 1 file changed, 1 insertion(+)
 create mode 100644 file-1.txt

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (main)
$ git status
On branch main
nothing to commit, working tree clean

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (main)
$ git push -u origin
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (main)
$ ^C

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (main)
$ git push --set-upstream origin main
fatal: 'origin' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (main)
$ git push -u new-origin
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream new-origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (main)
$ git push --set upstream origin master
error: src refspec origin does not match any
error: src refspec master does not match any
error: failed to push some refs to 'upstream'

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (main)
$ git remote -v
new-origin      https://github.com/rahmileejiyoo/eduwork-git.git (fetch)
new-origin      https://github.com/rahmileejiyoo/eduwork-git.git (push)

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (main)
$ git push --set-upstream new-origin main
To https://github.com/rahmileejiyoo/eduwork-git.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/rahmileejiyoo/eduwork-git.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (main)
$ ^C

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (main)
$ git pull new-origin main --rebase
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 874 bytes | 145.00 KiB/s, done.
From https://github.com/rahmileejiyoo/eduwork-git
 * branch            main       -> FETCH_HEAD
 * [new branch]      main       -> new-origin/main
Successfully rebased and updated refs/heads/main.

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (main)
$ git push new-origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 307 bytes | 307.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/rahmileejiyoo/eduwork-git.git
   a9e7fbc..86ab0b5  main -> main

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (main)
$ git status
On branch main
nothing to commit, working tree clean

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (main)
$ git checkout -b mytask
Switched to a new branch 'mytask'

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (mytask)
$ nano file-2.txt

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (mytask)
$ git add file-2.txt
warning: in the working copy of 'file-2.txt', LF will be replaced by CRLF the next time Git touches it

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (mytask)
$ git add --renormalize file-2.txt

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (mytask)
$ git status
On branch mytask
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   file-2.txt


lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (mytask)
$ ls
README.md  file-1.txt  file-2.txt

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (mytask)
$ git add .

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (mytask)
$ git commit -m "added new file"
[mytask d152b67] added new file
 1 file changed, 1 insertion(+)
 create mode 100644 file-2.txt

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (mytask)
$ git status
On branch mytask
nothing to commit, working tree clean

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (mytask)
$ nano file-3.php

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (mytask)
$ LS
README.md  file-1.txt  file-2.txt  file-3.php

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (mytask)
$ git add .
warning: in the working copy of 'file-3.php', LF will be replaced by CRLF the next time Git touches it

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (mytask)
$ git add -renormalize file-3.php
error: did you mean `--renormalize` (with two dashes)?

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (mytask)
$ git add --renormalize file-3.php

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (mytask)
$ ls
README.md  file-1.txt  file-2.txt  file-3.php

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (mytask)
$ git add .

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (mytask)
$ git commit -m "added new file"
[mytask bc776a0] added new file
 1 file changed, 2 insertions(+)
 create mode 100644 file-3.php

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (mytask)
$ git checkout main
Switched to branch 'main'

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (main)
$ git merge mytask
Updating 86ab0b5..bc776a0
Fast-forward
 file-2.txt | 1 +
 file-3.php | 2 ++
 2 files changed, 3 insertions(+)
 create mode 100644 file-2.txt
 create mode 100644 file-3.php

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (main)
$ git branch
* main
  mytask

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (main)
$ git pull
There is no tracking information for the current branch.
Please specify which branch you want to merge with.
See git-pull(1) for details.

    git pull <remote> <branch>

If you wish to set tracking information for this branch you can do so with:

    git branch --set-upstream-to=new-origin/<branch> main


lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (main)
$ git branch
* main
  mytask

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (main)
$ git checkout mytask
Switched to branch 'mytask'

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (mytask)
$ git checkout main
Switched to branch 'main'

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (main)
$ git merge mytask
Already up to date.

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (main)
$ git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream new-origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (main)
$ git push --set-upstream new-origin main
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (6/6), 590 bytes | 590.00 KiB/s, done.
Total 6 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/rahmileejiyoo/eduwork-git.git
   86ab0b5..bc776a0  main -> main
branch 'main' set up to track 'new-origin/main'.

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (main)
$ git branch
* main
  mytask

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (main)
$ git add .

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (main)
$ git commit -m "Save all changes"
On branch main
Your branch is up to date with 'new-origin/main'.

nothing to commit, working tree clean

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (main)
$ git push new-origin main
Everything up-to-date

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/eduwork-git (main)
$
