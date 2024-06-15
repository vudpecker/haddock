roblox@SELNK1350100682:/mnt/c/Users/msabanay/Documents/Project/haddock$ git commit -m "updated invetory"
[master bb02a01] updated invetory
 1 file changed, 13 deletions(-)

roblox@SELNK1350100682:/mnt/c/Users/msabanay/Documents/Project/haddock$ git push . Head
Everything up-to-date
roblox@SELNK1350100682:/mnt/c/Users/msabanay/Documents/Project/haddock$ git push . HEAD
Everything up-to-date




roblox@SELNK1350100682:/mnt/c/Users/msabanay/Documents/Project/haddock$ git status
On branch master
Your branch and 'main' have diverged,
and have 4 and 1 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

nothing to commit, working tree clean


roblox@SELNK1350100682:/mnt/c/Users/msabanay/Documents/Project/haddock$ git pull
From .
 * branch            main       -> FETCH_HEAD
hint: You have divergent branches and need to specify how to reconcile them.
hint: You can do so by running one of the following commands sometime before
hint: your next pull:
hint:
hint:   git config pull.rebase false  # merge (the default strategy)
hint:   git config pull.rebase true   # rebase
hint:   git config pull.ff only       # fast-forward only
hint:
hint: You can replace "git config" with "git config --global" to set a default
hint: preference for all repositories. You can also pass --rebase, --no-rebase,
hint: or --ff-only on the command line to override the configured default per
hint: invocation.
fatal: Need to specify how to reconcile divergent branches.
roblox@SELNK1350100682:/mnt/c/Users/msabanay/Documents/Project/haddock$ git log
commit bb02a01c3c23fa4cb3c3509d0f1c49ee28d5cc62 (HEAD -> master)
Author: Murugaraja <murugaraja@gmail.com>
Date:   Thu Jun 13 14:47:39 2024 +0200

    updated invetory

commit a4c525dbb50ecb2e1a56ca971d2aac0824e1e74d (origin/master)
Author: Murugaraja <murugaraja@gmail.com>
Date:   Thu Jun 13 13:52:05 2024 +0200

    added inventories

commit 1f8a7be31d84b01e17b051fa11bbc3d6fb4dcd24
Author: Murugaraja <murugaraja@gmail.com>
Date:   Wed Jun 12 10:10:54 2024 +0200

    add loops

commit 28549e04b88498e2ef7f356f8ec7059574bbd1bf
Author: Murugaraja <murugaraja@gmail.com>
Date:   Tue Jun 11 15:19:01 2024 +0200

    initial commit
roblox@SELNK1350100682:/mnt/c/Users/msabanay/Documents/Project/haddock$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
roblox@SELNK1350100682:/mnt/c/Users/msabanay/Documents/Project/haddock$ ls
README.md
roblox@SELNK1350100682:/mnt/c/Users/msabanay/Documents/Project/haddock$
roblox@SELNK1350100682:/mnt/c/Users/msabanay/Documents/Project/haddock$ git branch
* main
  master
roblox@SELNK1350100682:/mnt/c/Users/msabanay/Documents/Project/haddock$ git pull
Already up to date.
roblox@SELNK1350100682:/mnt/c/Users/msabanay/Documents/Project/haddock$ git merge master
fatal: refusing to merge unrelated histories
roblox@SELNK1350100682:/mnt/c/Users/msabanay/Documents/Project/haddock$ git cherry-pick 28549e04b
[main fd8ffd0] initial commit
 Date: Tue Jun 11 15:19:01 2024 +0200
 3 files changed, 23 insertions(+)
 create mode 100644 Ansible/ansible-for-beginners.pdf
 create mode 100644 Ansible/books/condition_age.yml
 create mode 100644 Ansible/books/condition_register.yml
roblox@SELNK1350100682:/mnt/c/Users/msabanay/Documents/Project/haddock$ git cherry-pick 1f8a7be31
[main a815a35] add loops
 Date: Wed Jun 12 10:10:54 2024 +0200
 1 file changed, 10 insertions(+)
 create mode 100644 Ansible/books/loops_exerc-yml
roblox@SELNK1350100682:/mnt/c/Users/msabanay/Documents/Project/haddock$ git cherry-pick a4c525dbb
[main 1610844] added inventories
 Date: Thu Jun 13 13:52:05 2024 +0200
 2 files changed, 69 insertions(+)
 create mode 100644 Ansible/books/inventory.yml
 create mode 100644 Ansible/books/inventory_parent_child.yml
roblox@SELNK1350100682:/mnt/c/Users/msabanay/Documents/Project/haddock$ git cherry-pick bb02a01c3
[main 754c9be] updated invetory
 Date: Thu Jun 13 14:47:39 2024 +0200
 1 file changed, 13 deletions(-)




roblox@SELNK1350100682:/mnt/c/Users/msabanay/Documents/Project/haddock$ git status
On branch main
Your branch is ahead of 'origin/main' by 4 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean




roblox@SELNK1350100682:/mnt/c/Users/msabanay/Documents/Project/haddock$ git push
Enumerating objects: 24, done.
Counting objects: 100% (24/24), done.
Delta compression using up to 12 threads
Compressing objects: 100% (23/23), done.
Writing objects: 100% (23/23), 4.69 MiB | 2.83 MiB/s, done.
Total 23 (delta 4), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (4/4), done.
To github.com:vudpecker/haddock.git
   f45fb18..754c9be  main -> main
roblox@SELNK1350100682:/mnt/c/Users/msabanay/Documents/Project/haddock$ git branch
* main
  master
roblox@SELNK1350100682:/mnt/c/Users/msabanay/Documents/Project/haddock$ git pull
Already up to date.
roblox@SELNK1350100682:/mnt/c/Users/msabanay/Documents/Project/haddock$ git branch
* main
  master
roblox@SELNK1350100682:/mnt/c/Users/msabanay/Documents/Project/haddock$