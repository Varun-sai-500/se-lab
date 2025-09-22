# se-lab
PS C:\Users\fs\Desktop\git> git config --global user.name "
PS C:\Users\fs\Desktop\git> git config --global user.email PS C:\Users\fs\Desktop\git> git clone https://github.com/Varemote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (3/3), done.
Receiving objects: 100% (4/4), done.
PS C:\Users\fs\Desktop\git> cd se-lab
PS C:\Users\fs\Desktop\git\se-lab> git add .
PS C:\Users\fs\Desktop\git\se-lab> git commit -m "new commi
[main bc91bfd] new commit
 1 file changed, 1 insertion(+)
 create mode 100644 hi.cpp
PS C:\Users\fs\Desktop\git\se-lab> git push origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 321 bytes | 321.00 KiB/s, done
To https://github.com/Varun-sai-500/se-lab
PS C:\Users\fs\Desktop\git\se-lab> git checkout -b new-feat
PS C:\Users\fs\Desktop\git\se-lab> git add .
PS C:\Users\fs\Desktop\git\se-lab> git commit -m "new branc
[new-feature 5ec3678] new branch
 1 file changed, 4 insertions(+)
 create mode 100644 new.cpp
PS C:\Users\fs\Desktop\git\se-lab> git push origin new-feat
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 316 bytes | 158.00 KiB/s, done
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 
remote: Resolving deltas: 100% (1/1), completed with 1 loca
remote:
remote: Create a pull request for 'new-feature' on GitHub b
remote:      https://github.com/Varun-sai-500/se-lab/pull/n
remote:
To https://github.com/Varun-sai-500/se-lab
 * [new branch]      new-feature -> new-feature
Already up to date.
Everything up-to-date
commit 5ec3678563d56d99b142f93d80bb5c5727da5bd8 (HEAD -> neDate:   Mon Sep 22 14:12:18 2025 +0530

    new branch
main)
Date:   Mon Sep 22 14:10:12 2025 +0530

    new commit
commit e8982b0edea0dfe4a46c0a8664c513eee5e9d5f4
# f, fixup [-C | -c] <commit> = like "squash" but keep only
#                    commit's log message, unless -C is use#                    keep only this commit's message; -c is
# f, fixup [-C | -c] <commit> = like "squash" but keep only
#                    commit's log message, unless -C is use#                    keep only this commit's message; -c is
Date:   Mon Sep 22 13:09:26 2025 +0530
    Initial commit
PS C:\Users\fs\Desktop\git\se-lab> git merge new-feature
Already up to date.
PS C:\Users\fs\Desktop\git\se-lab> git history
git: 'history' is not a git command. See 'git --help'.
PS C:\Users\fs\Desktop\git\se-lab> git add child.cpp
fatal: pathspec 'child.cpp' did not match any files
PS C:\Users\fs\Desktop\git\se-lab> git add chid.cpp
PS C:\Users\fs\Desktop\git\se-lab> git commit -m "child"   
[new-feature 190e9db] child
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 chid.cpp
PS C:\Users\fs\Desktop\git\se-lab> git add parent.cpp
PS C:\Users\fs\Desktop\git\se-lab> git commit "parent"
error: pathspec 'parent' did not match any file(s) known to
PS C:\Users\fs\Desktop\git\se-lab> git commit -m "parent"
[new-feature 8bbb18e] parent
 1 file changed, 1 insertion(+)
 create mode 100644 parent.cpp
PS C:\Users\fs\Desktop\git\se-lab> git rebase -i HEAD~4
Successfully rebased and updated refs/heads/new-feature.
PS C:\Users\fs\Desktop\git\se-lab> git rebase -i HEAD~2
Successfully rebased and updated refs/heads/new-feature.
PS C:\Users\fs\Desktop\git\se-lab> git log
commit 8bbb18ec04dbb75e216e1464012bf7d134f8b17c (HEAD -> ne
Author: varunsai <varunsaip2005@gmail.com>
Date:   Mon Sep 22 14:20:06 2025 +0530

    parent

commit 190e9db37931b1bde43a58f73341baef3b218790
Author: varunsai <varunsaip2005@gmail.com>
Date:   Mon Sep 22 14:19:34 2025 +0530

    child

commit 5ec3678563d56d99b142f93d80bb5c5727da5bd8 (origin/new
Author: varunsai <varunsaip2005@gmail.com>
Date:   Mon Sep 22 14:12:18 2025 +0530

    new branch

commit bc91bfd125a0fb8a757565346fca3e33fb2e7d30 (origin/mai
main)
Author: varunsai <varunsaip2005@gmail.com>
Date:   Mon Sep 22 14:10:12 2025 +0530

    new commit

commit e8982b0edea0dfe4a46c0a8664c513eee5e9d5f4
Author: Varun Sai <varunsaip2005@gmail.com>
Date:   Mon Sep 22 13:09:26 2025 +0530

    Initial commit
...skipping...

                   SUMMARY OF LESS COMMANDS

      Commands marked with * may be preceded by a number, N
      Notes in parentheses indicate the behavior if N is gi
      A key preceded by a caret indicates the Ctrl key; thu

  h  H                 Display this help.
  q  :q  Q  :Q  ZZ     Exit.
 -----------------------------------------------------------

                           MOVING

  e  ^E  j  ^N  CR  *  Forward  one line   (or N lines).
  y  ^Y  k  ^K  ^P  *  Backward one line   (or N lines).
  f  ^F  ^V  SPACE  *  Forward  one window (or N lines).
  b  ^B  ESC-v      *  Backward one window (or N lines).
  z                 *  Forward  one window (and set window 
  w                 *  Backward one window (and set window 
  ESC-SPACE         *  Forward  one window, but don't stop 
  d  ^D             *  Forward  one half-window (and set ha  u  ^U             *  Backward one half-window (and set ha  ESC-)  RightArrow *  Right one half screen width (or N po
  ESC-(  LeftArrow  *  Left  one half screen width (or N po
HELP -- Press RETURN for more, or q when done...skipping...
Author: varunsai <varunsaip2005@gmail.com>
Date:   Mon Sep 22 14:19:34 2025 +0530
    child

commit 5ec3678563d56d99b142f93d80bb5c5727da5bd8 (origin/new-feature)
Author: varunsai <varunsaip2005@gmail.com>
Date:   Mon Sep 22 14:12:18 2025 +0530

    new branch

n, origin/HEAD, main)
Author: varunsai <varunsaip2005@gmail.com>
Date:   Mon Sep 22 14:10:12 2025 +0530

    new commit

commit e8982b0edea0dfe4a46c0a8664c513eee5e9d5f4
Author: Varun Sai <varunsaip2005@gmail.com>
Date:   Mon Sep 22 13:09:26 2025 +0530

    Initial commit
PS C:\Users\fs\Desktop\git\se-lab>
PS C:\Users\fs\Desktop\git\se-lab> git apply patching.patch

error: No valid patches in input (allow with "--allow-empty")
PS C:\Users\fs\Desktop\git\se-lab> git push origin main    
To https://github.com/Varun-sai-500/se-lab
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/Varun-sai-500/se-lab'
k that you do not
hint: have locally. This is usually caused by another reposhint: the same ref. If you want to integrate the remote changes, use
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
PS C:\Users\fs\Desktop\git\se-lab> git pull
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 
0 (from 0)
Unpacking objects: 100% (3/3), 983 bytes | 35.00 KiB/s, done.
From https://github.com/Varun-sai-500/se-lab
   bc91bfd..2503e4b  main       -> origin/main
See git-pull(1) for details.


If you wish to set tracking information for this branch you can do so with:

    git branch --set-upstream-to=origin/<branch> new-feature

PS C:\Users\fs\Desktop\git\se-lab> git rebase -i HEAD~2    
error: cannot rebase: You have unstaged changes.
error: Please commit or stash them.
PS C:\Users\fs\Desktop\git\se-lab> git commit -m "commitd" 
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   hi.cpp

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        patching.patch

t -a")
PS C:\Users\fs\Desktop\git\se-lab> git apply patching.patch

error: No valid patches in input (allow with "--allow-empty")
To https://github.com/Varun-sai-500/se-lab
 ! [rejected]        main -> main (non-fast-forward)       
error: failed to push some refs to 'https://github.com/Varun-sai-500/se-lab'
hint: Updates were rejected because a pushed branch tip is 
behind its remote
hint: counterpart. If you want to integrate the remote changes, use 'git pull'
hint: before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
PS C:\Users\fs\Desktop\git\se-lab> git pull
Please specify which branch you want to merge with.        
See git-pull(1) for details.
 have to commit

    git pull <remote> <branch>

If you wish to set tracking information for this branch you

    git branch --set-upstream-to=origin/<branch> new-feature

PS C:\Users\fs\Desktop\git\se-lab> git pull fill.cpp       
fatal: 'fill.cpp' does not appear to be a git repository   
fatal: Could not read from remote repository.

Please make sure you have the correct access rights        
and the repository exists.
PS C:\Users\fs\Desktop\git\se-lab> git pull 
See git-pull(1) for details.

If you wish to set tracking information for this branch you can do so with:
    git branch --set-upstream-to=origin/<branch> new-feature

PS C:\Users\fs\Desktop\git\se-lab> git pull origin main    
From https://github.com/Varun-sai-500/se-lab
 * branch            main       -> FETCH_HEAD
 fill.cpp | 1 +
 1 file changed, 1 insertion(+)
 create mode 100644 fill.cpp
PS C:\Users\fs\Desktop\git\se-lab> git push origin main    
To https://github.com/Varun-sai-500/se-lab
 ! [rejected]        main -> main (non-fast-forward)       
error: failed to push some refs to 'https://github.com/Varun-sai-500/se-lab'
hint: Updates were rejected because a pushed branch tip is 
behind its remote
hint: counterpart. If you want to integrate the remote chanhint: before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
PS C:\Users\fs\Desktop\git\se-lab> git apply patching.patch

error: No valid patches in input (allow with "--allow-empty")
PS C:\Users\fs\Desktop\git\se-lab> git checkout mian       
PS C:\Users\fs\Desktop\git\se-lab> git checkout main       
M       hi.cpp
Your branch is behind 'origin/main' by 1 commit, and can be fast-forwarded.
  (use "git pull" to update your local branch)
PS C:\Users\fs\Desktop\git\se-lab> git push origin main    
To https://github.com/Varun-sai-500/se-lab
hint: Updates were rejected because the tip of your currenthint: its remote counterpart. If you want to integrate the 
remote changes,
hint: use 'git pull' before pushing again.
p' for details.
PS C:\Users\fs\Desktop\git\se-lab> git pull origin main    
From https://github.com/Varun-sai-500/se-lab
Updating bc91bfd..2503e4b
Fast-forward
 fill.cpp | 1 +
 1 file changed, 1 insertion(+)
 create mode 100644 fill.cpp
PS C:\Users\fs\Desktop\git\se-lab> git push origin main    
Everything up-to-date
pick 2503e4b Create fill.cpp

error: No valid patches in input (allow with "--allow-empty")
PS C:\Users\fs\Desktop\git\se-lab> git applt patching.patch --allow-empty      
git: 'applt' is not a git command. See 'git --help'.       

        apply
PS C:\Users\fs\Desktop\git\se-lab> git apply patching.patch --allow-empty
PS C:\Users\fs\Desktop\git\se-lab> git add .
PS C:\Users\fs\Desktop\git\se-lab> git push origin main    
Everything up-to-date
PS C:\Users\fs\Desktop\git\se-lab> git rebase -i HEAD~2    
error: cannot rebase: Your index contains uncommitted changes.
error: Please commit or stash them.
PS C:\Users\fs\Desktop\git\se-lab> git commit -m "commit"  
[main 45024d9] commit
 2 files changed, 7 insertions(+), 1 deletion(-)
 create mode 100644 patching.patch
PS C:\Users\fs\Desktop\git\se-lab> git rebase -i HEAD~2    
hint: Waiting for your editor to close the file...
sh: line 1: man: command not found

shell returned 127

Press ENTER or type command to continue
Successfully rebased and updated refs/heads/main.
PS C:\Users\fs\Desktop\git\se-lab> git rebase -i HEAD~2    
Successfully rebased and updated refs/heads/main.
PS C:\Users\fs\Desktop\git\se-lab> git commit --amend -m "N[main 79089df] New commit message here
 Date: Mon Sep 22 15:06:57 2025 +0530
 2 files changed, 7 insertions(+), 1 deletion(-)
 create mode 100644 patching.patch
commit 79089dfdce264206f23a3e21f925c55402fccdeb (HEAD -> main)
Author: varunsai <varunsaip2005@gmail.com>
Date:   Mon Sep 22 15:06:57 2025 +0530
    New commit message here

commit 2503e4ba44f9a28937b7add16f5aa2fc40efe370 (origin/main, origin/HEAD)
Author: Varun Sai <varunsaip2005@gmail.com>
Date:   Mon Sep 22 14:46:47 2025 +0530

    Create fill.cpp

commit bc91bfd125a0fb8a757565346fca3e33fb2e7d30
Author: varunsai <varunsaip2005@gmail.com>
Date:   Mon Sep 22 14:10:12 2025 +0530

    new commit

commit e8982b0edea0dfe4a46c0a8664c513eee5e9d5f4
Author: Varun Sai <varunsaip2005@gmail.com>
Date:   Mon Sep 22 13:09:26 2025 +0530

    Initial commit
PS C:\Users\fs\Desktop\git\se-lab> git log oneline
fatal: ambiguous argument 'oneline': unknown revision or path not in the working tree.
Use '--' to separate paths from revisions, like this:
PS C:\Users\fs\Desktop\git\se-lab> git log --oneline
79089df (HEAD -> main) New commit message here
2503e4b (origin/main, origin/HEAD) Create fill.cpp
bc91bfd new commit
e8982b0 Initial commit
PS C:\Users\fs\Desktop\git\se-lab> git checkout bc91bfd
Note: switching to 'bc91bfd'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at bc91bfd new commit
PS C:\Users\fs\Desktop\git\se-lab> git checkout main
Previous HEAD position was bc91bfd new commit
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)
PS C:\Users\fs\Desktop\git\se-lab> 
