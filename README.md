# Git exercise

## Bundle 3

### Exercise 1

```bash


vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (main)
$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/team-page)
$ git status
On branch ft/team-page
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/team-page)
$ git add team.html

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/team-page)
$ git commit -m "create team page"
[ft/team-page df5adee] create team page
 1 file changed, 15 insertions(+)
 create mode 100644 team.html

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/team-page)
$ git push
fatal: The current branch ft/team-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/team-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/team-page)
$ git push --set-upstream origin ft/team-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 476 bytes | 476.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/Niyonyungu/Git-exercise-solution/pull/new/ft/team-ge
remote:
To https://github.com/Niyonyungu/Git-exercise-solution.git
 * [new branch]      ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/team-page)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (main)
$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/contact-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/team-page)
$ git log
commit df5adee23f840d954e81907bd2635b4d9d4ea89a (HEAD -> ft/team-page, origin/ft/tm-page)
Author: Michel vainqueur <vainqueurmg@gmail.com>
Date:   Wed May 17 23:06:39 2023 +0200

    create team page

commit a0433816918efc3a5d3a5bb5d8b8aaaf40574efa (origin/main, main, ft/contact-pag
Author: Michel vainqueur <vainqueurmg@gmail.com>
Date:   Wed May 17 23:01:35 2023 +0200

    readme file

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/team-page)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/contact-page)
$ git cherry-pick df5adee23f840d954e81907bd2635b4d9d4ea89a
[ft/contact-page 06ed6db] create team page
 Date: Wed May 17 23:06:39 2023 +0200
 1 file changed, 15 insertions(+)
 create mode 100644 team.html

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/contact-page)
$ git log
commit 06ed6db2089c05ea837aa4453cfe6496d34ad12b (HEAD -> ft/contact-page)
Author: Michel vainqueur <vainqueurmg@gmail.com>
Date:   Wed May 17 23:06:39 2023 +0200

    create team page

commit a0433816918efc3a5d3a5bb5d8b8aaaf40574efa (origin/main, main)
Author: Michel vainqueur <vainqueurmg@gmail.com>
Date:   Wed May 17 23:01:35 2023 +0200

    readme file

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/contact-page)
$ git status
On branch ft/contact-page
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        contact.html

nothing added to commit but untracked files present (use "git add" to track)

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/contact-page)
$ git add contact.html

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/contact-page)
$ git commit -m "added contact page"
[ft/contact-page abdf0bc] added contact page
 1 file changed, 16 insertions(+)
 create mode 100644 contact.html

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/contact-page)
$ git push
fatal: The current branch ft/contact-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/contact-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/contact-page)
$  git push --set-upstream origin ft/contact-page
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 757 bytes | 378.00 KiB/s, done.
Total 6 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), done.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/Niyonyungu/Git-exercise-solution/pull/new/ft/conta-page
remote:
To https://github.com/Niyonyungu/Git-exercise-solution.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/contact-page)
$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/faq-page)
$ git status
On branch ft/faq-page
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        faq.html

nothing added to commit but untracked files present (use "git add" to track)

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/faq-page)
$ git add faq.html

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/faq-page)
$ gitggggggggoooo
bash: gitggggggggoooo: command not found

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/faq-page)
$ git commit -m "added faq page"
[ft/faq-page 458c98b] added faq page
 1 file changed, 15 insertions(+)
 create mode 100644 faq.html

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/faq-page)
$ git push
fatal: The current branch ft/faq-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/faq-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/faq-page)
$ git push --set-upstream origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 454 bytes | 454.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/Niyonyungu/Git-exercise-solution/pull/new/ft/faq-pe
remote:
To https://github.com/Niyonyungu/Git-exercise-solution.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/faq-page)
$ git log
[ft/faq-page 7934f04] Qa!                               BBBBBBBBBBNNG
 1 file changed, 15 deletions(-)
 delete mode 100644 team.html
z
vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/faq-page)
$ git log
commit 7934f0498cfcbfdcd68d8ab8d83b04d5156275ed (HEAD -> ft/faq-page)
Author: Michel vainqueur <vainqueurmg@gmail.com>
Date:   Wed May 17 23:38:07 2023 +0200

    Qa!
                                  ^B^B^B^B^B^B^B^BBBBBBBBBBBNNG

commit 458c98be257c2fed6956011185abbea529b7ebc0 (origin/ft/faq-page)
Author: Michel vainqueur <vainqueurmg@gmail.com>
Date:   Wed May 17 23:32:13 2023 +0200

    added faq page

commit abdf0bcafad14037f6c98a6740635b6a4e5347a0 (origin/ft/contact-page, ft/contact-page)
Author: Michel vainqueur <vainqueurmg@gmail.com>
Date:   Wed May 17 23:26:35 2023 +0200

    added contact page

commit 06ed6db2089c05ea837aa4453cfe6496d34ad12b
Author: Michel vainqueur <vainqueurmg@gmail.com>
Date:   Wed May 17 23:06:39 2023 +0200
:...skipping...
commit 7934f0498cfcbfdcd68d8ab8d83b04d5156275ed (HEAD -> ft/faq-page)
Author: Michel vainqueur <vainqueurmg@gmail.com>
Date:   Wed May 17 23:38:07 2023 +0200

    Qa!
                                  ^B^B^B^B^B^B^B^BBBBBBBBBBBNNG

commit 458c98be257c2fed6956011185abbea529b7ebc0 (origin/ft/faq-page)
Author: Michel vainqueur <vainqueurmg@gmail.com>
Date:   Wed May 17 23:32:13 2023 +0200

    added faq page

commit abdf0bcafad14037f6c98a6740635b6a4e5347a0 (origin/ft/contact-page, ft/contac
Author: Michel vainqueur <vainqueurmg@gmail.com>
Date:   Wed May 17 23:26:35 2023 +0200

    added contact page

commit 06ed6db2089c05ea837aa4453cfe6496d34ad12b
Author: Michel vainqueur <vainqueurmg@gmail.com>
Date:   Wed May 17 23:06:39 2023 +0200

    create team page

commit a0433816918efc3a5d3a5bb5d8b8aaaf40574efa (origin/main, main)
Author: Michel vainqueur <vainqueurmg@gmail.com>
Date:   Wed May 17 23:01:35 2023 +0200

    readme file
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
a
vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/faq-page)
$ git push
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 235 bytes | 235.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Niyonyungu/Git-exercise-solution.git
   458c98b..7934f04  ft/faq-page -> ft/faq-page

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/faq-page)
$


```

### Exercise 2

```bash

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (main)
$ checkout ft/faq-page
bash: checkout: command not found

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (main)
$ git checkout ft/faq-page
Switched to branch 'ft/faq-page'
Your branch is up to date with 'origin/ft/faq-page'.

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/faq-page)
$ git checkout -b ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/home-page-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (main)
$ ls
README.md

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (main)
$ git add README.md

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md


vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (main)
$ git commit -m "changed sthg in readme"
[main b9b12b7] changed sthg in readme
 1 file changed, 5 insertions(+)

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 295 bytes | 295.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Niyonyungu/Git-exercise-solution.git
   8ba8aa8..b9b12b7  main -> main

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (main)
$ checkout ft/home-page-redesign
bash: checkout: command not found

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (main)
$ git checkout ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/home-page-redesign)
$ git rebase main
Successfully rebased and updated refs/heads/ft/home-page-redesign.

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/home-page-redesign)
$ git log
commit 5a4d6a22e1d89f84c7624340963b7acbb34b615d (HEAD -> ft/home-page-redesign)
Author: Michel vainqueur <vainqueurmg@gmail.com>
Date:   Wed May 17 23:38:07 2023 +0200

    Qa!
                                  ^B^B^B^B^B^B^B^BBBBBBBBBBBNNG

commit 87955b12197bcb06accb09b2c6923179abd3bb44
Author: Michel vainqueur <vainqueurmg@gmail.com>
Date:   Wed May 17 23:32:13 2023 +0200

    added faq page

commit ed53faf1963ecf5a4d75ea8bc803c0191ee245f7
Author: Michel vainqueur <vainqueurmg@gmail.com>
Date:   Wed May 17 23:26:35 2023 +0200

    added contact page

commit e93b3d5fcb92f8289689f17f9eb8f54126545da7
Author: Michel vainqueur <vainqueurmg@gmail.com>
Date:   Wed May 17 23:06:39 2023 +0200

    create team page

commit b9b12b7946a8183af969bb864316485c0320b419 (origin/main, main)
Author: Michel vainqueur <vainqueurmg@gmail.com>
Date:   Thu May 18 00:05:24 2023 +0200

    changed sthg in readme

commit 8ba8aa86d1072b711f4106e3698568409edb851e
Author: Michel vainqueur <vainqueurmg@gmail.com>
Date:   Wed May 17 23:59:06 2023 +0200

    final exercise 1

commit a0433816918efc3a5d3a5bb5d8b8aaaf40574efa
Author: Michel vainqueur <vainqueurmg@gmail.com>
Date:   Wed May 17 23:01:35 2023 +0200

    readme file

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/home-page-redesign)
$ git status
On branch ft/home-page-redesign
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html

nothing added to commit but untracked files present (use "git add" to track)

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/home-page-redesign)
$ git add home.html

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/home-page-redesign)
$ git commit -m "modified home page"
[ft/home-page-redesign 731bf27] modified home page
 1 file changed, 16 insertions(+)
 create mode 100644 home.html

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/home-page-redesign)
$ git push
fatal: The current branch ft/home-page-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/home-page-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/home-page-redesign)
$ git push --set-upstream origin ft/home-page-redesign
Enumerating objects: 15, done.
Counting objects: 100% (15/15), done.
Delta compression using up to 4 threads
Compressing objects: 100% (14/14), done.
Writing objects: 100% (14/14), 1.48 KiB | 759.00 KiB/s, done.
Total 14 (delta 7), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (7/7), done.
remote:
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/Niyonyungu/Git-exercise-solution/pull/new/ft/home-page-redesign
remote:
To https://github.com/Niyonyungu/Git-exercise-solution.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
branch 'ft/home-page-redesign' set up to track 'origin/ft/home-page-redesign'.

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Bundle-3&4 (ft/home-page-redesign)
$


```
