╭╴㉿ david at …/Git/Previous/gitflow_practice
🕙 09:51:25 PM
╰─ git clone git@github.com:daafonsecato/flow-pr-test.git
Cloning into 'flow-pr-test'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.

╭╴㉿ david at …/Git/Previous/gitflow_practice
🕙 09:53:06 PM
╰─ cd flow-pr-test

╭╴㉿ david at …/flow-pr-test on  main ( )
🕙 09:53:10 PM
╰─ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

╭╴㉿ david at …/flow-pr-test on  main ( )
🕙 09:53:14 PM
╰─ git branch -a
* main
  remotes/origin/HEAD -> origin/main
  remotes/origin/main

╭╴㉿ david at …/flow-pr-test on  main ( )
🕙 09:53:20 PM
╰─ git flow init

Which branch should be used for bringing forth production releases?
   - main
Branch name for production releases: [main]
Branch name for "next release" development: [develop]

How to name your supporting branch prefixes?
Feature branches? [feature/]
Bugfix branches? [bugfix/]
Release branches? [release/]
Hotfix branches? [hotfix/]
Support branches? [support/]
Version tag prefix? []
Hooks and filters directory? [/mnt/c/Users/dafonseca/OneDrive - ENDAVA/Documents/Intership/Git/Previous/gitflow_practice/flow-pr-test/.git/hooks]

╭╴㉿ david at …/flow-pr-test on  develop () took 7s
🕙 09:53:35 PM
╰─ git flow feature start f1
Switched to a new branch 'feature/f1'

Summary of actions:
- A new branch 'feature/f1' was created, based on 'develop'
- You are now on branch 'feature/f1'

Now, start committing on your feature. When done, use:

     git flow feature finish f1


╭╴㉿ david at …/flow-pr-test on  feature/f1 ()
🕙 09:53:53 PM
╰─ git status
On branch feature/f1
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        f1.txt

nothing added to commit but untracked files present (use "git add" to track)

╭╴㉿ david at …/flow-pr-test on  feature/f1 ( )
🕙 09:54:18 PM
╰─ git add .

╭╴㉿ david at …/flow-pr-test on  feature/f1 (++(1))
🕙 09:54:21 PM
╰─ git commit -m "Hello, f1 added"
[feature/f1 4ffa6bd] Hello, f1 added
 1 file changed, 1 insertion(+)
 create mode 100644 f1.txt

╭╴㉿ david at …/flow-pr-test on  feature/f1 ()
🕙 09:54:31 PM
╰─ git flow feature start f2
Switched to a new branch 'feature/f2'

Summary of actions:
- A new branch 'feature/f2' was created, based on 'develop'
- You are now on branch 'feature/f2'

Now, start committing on your feature. When done, use:

     git flow feature finish f2


╭╴㉿ david at …/flow-pr-test on  feature/f2 ()
🕙 09:54:49 PM
╰─ git flow feature finish f1
Switched to branch 'develop'
Updating 7227106..4ffa6bd
Fast-forward
 f1.txt | 1 +
 1 file changed, 1 insertion(+)
 create mode 100644 f1.txt
Deleted branch feature/f1 (was 4ffa6bd).

Summary of actions:
- The feature branch 'feature/f1' was merged into 'develop'
- Feature branch 'feature/f1' has been locally deleted
- You are now on branch 'develop'


╭╴㉿ david at …/flow-pr-test on  develop ( )
🕙 09:55:24 PM
╰─ git checkout feature/f2
Switched to branch 'feature/f2'

╭╴㉿ david at …/flow-pr-test on  feature/f2 ( )
🕙 09:55:43 PM
╰─ git commit -m "Hello, f2 added"
On branch feature/f2
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        f2.txt

nothing added to commit but untracked files present (use "git add" to track)

╭╴㉿ david at …/flow-pr-test on  feature/f2 ( )
🕙 09:55:54 PM
╰─ git commit -am "Hello, f2 added"
On branch feature/f2
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        f2.txt

nothing added to commit but untracked files present (use "git add" to track)

╭╴㉿ david at …/flow-pr-test on  feature/f2 ( )
🕙 09:56:01 PM
╰─ git add .

╭╴㉿ david at …/flow-pr-test on  feature/f2 (++(1))
🕙 09:56:08 PM
╰─ git commit -m "Hello, f2 added"
[feature/f2 a43cc45] Hello, f2 added
 1 file changed, 1 insertion(+)
 create mode 100644 f2.txt

╭╴㉿ david at …/flow-pr-test on  feature/f2 ()
🕙 09:56:10 PM
╰─ git flow feature publish f2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 300 bytes | 27.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'feature/f2' on GitHub by visiting:
remote:      https://github.com/daafonsecato/flow-pr-test/pull/new/feature/f2
remote:
To github.com:daafonsecato/flow-pr-test.git
 * [new branch]      feature/f2 -> feature/f2
branch 'feature/f2' set up to track 'origin/feature/f2'.
Already on 'feature/f2'
Your branch is up to date with 'origin/feature/f2'.

Summary of actions:
- The remote branch 'feature/f2' was created or updated
- The local branch 'feature/f2' was configured to track the remote branch
- You are now on branch 'feature/f2'


╭╴㉿ david at …/flow-pr-test on  feature/f2 ( ) took 6s
🕙 09:56:35 PM
╰─ git add .

╭╴㉿ david at …/flow-pr-test on  feature/f2 (++(1) )
🕙 09:57:22 PM
╰─ git commit -m "Hello, f2 fixed"
[feature/f2 e8b76da] Hello, f2 fixed
 1 file changed, 1 insertion(+), 1 deletion(-)

╭╴㉿ david at …/flow-pr-test on  feature/f2 (⇡1)
🕙 09:57:27 PM
╰─ git flow feature finish f2
Branches 'feature/f2' and 'origin/feature/f2' have diverged.
And local branch 'feature/f2' is ahead of 'origin/feature/f2'.
Switched to branch 'develop'
Merge made by the 'ort' strategy.
 f2.txt | 1 +
 1 file changed, 1 insertion(+)
 create mode 100644 f2.txt
To github.com:daafonsecato/flow-pr-test.git
 - [deleted]         feature/f2
Deleted branch feature/f2 (was e8b76da).

Summary of actions:
- The feature branch 'feature/f2' was merged into 'develop'
- Feature branch 'feature/f2' has been locally deleted; it has been remotely deleted from 'origin'
- You are now on branch 'develop'


╭╴㉿ david at …/flow-pr-test on  develop () took 8s
🕙 09:59:28 PM
╰─ git flow release start v1.0
Switched to a new branch 'release/v1.0'

Summary of actions:
- A new branch 'release/v1.0' was created, based on 'develop'
- You are now on branch 'release/v1.0'

Follow-up actions:
- Bump the version number now!
- Start committing last-minute fixes in preparing your release
- When done, run:

     git flow release finish 'v1.0'


╭╴㉿ david at …/flow-pr-test on  release/v1… ()
🕙 10:04:33 PM
╰─ vim ~/.config/starship.toml

╭╴㉿ david at …/flow-pr-test on  release/v1.0 () took 7s
🕙 10:05:30 PM
╰─

╭╴㉿ david at …/flow-pr-test on  release/v1.0 ()
🕙 10:05:31 PM
╰─

╭╴㉿ david at …/flow-pr-test on  release/v1.0 ()
🕙 10:05:32 PM
╰─ git add .

╭╴㉿ david at …/flow-pr-test on  release/v1.0 (++(1))
🕙 10:07:39 PM
╰─ git commit -m "Ready for the release"
[release/v1.0 78c2a38] Ready for the release
 1 file changed, 2 insertions(+), 1 deletion(-)

╭╴㉿ david at …/flow-pr-test on  release/v1.0 ()
🕙 10:07:52 PM
╰─ git flow release finish v1.0
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
Merge made by the 'ort' strategy.
 README.md | 3 ++-
 f1.txt    | 1 +
 f2.txt    | 1 +
 3 files changed, 4 insertions(+), 1 deletion(-)
 create mode 100644 f1.txt
 create mode 100644 f2.txt
Already on 'main'
Your branch is ahead of 'origin/main' by 6 commits.
  (use "git push" to publish your local commits)
fatal: no tag message?
Fatal: Tagging failed. Please run finish again to retry.

╭╴㉿ david at …/flow-pr-test on  main (⇡6) took 10s
🕙 10:08:18 PM
╰─ git flow release finish v1.0
Branches 'main' and 'origin/main' have diverged.
And local branch 'main' is ahead of 'origin/main'.
Already on 'main'
Your branch is ahead of 'origin/main' by 6 commits.
  (use "git push" to publish your local commits)
Switched to branch 'develop'
Merge made by the 'ort' strategy.
 README.md | 3 ++-
 1 file changed, 2 insertions(+), 1 deletion(-)
Deleted branch release/v1.0 (was 78c2a38).

Summary of actions:
- Release branch 'release/v1.0' has been merged into 'main'
- The release was tagged 'v1.0'
- Release tag 'v1.0' has been back-merged into 'develop'
- Release branch 'release/v1.0' has been locally deleted
- You are now on branch 'develop'


╭╴㉿ david at …/flow-pr-test on  develop () took 26s
🕙 10:08:52 PM
╰─ git tree
*   8194bd2 - (11 seconds ago) Merge tag 'v1.0' into develop - David Fonseca (HEAD -> develop)
|\
| *   a37670f - (50 seconds ago) Merge branch 'release/v1.0' - David Fonseca (tag: v1.0, main)
| |\
| | * 78c2a38 - (67 seconds ago) Ready for the release - David Fonseca
| |/
|/|
* |   eb754ca - (10 minutes ago) Merge branch 'feature/f2' into develop - David Fonseca
|\ \
| * | e8b76da - (12 minutes ago) Hello, f2 fixed - David Fonseca
| * | a43cc45 - (13 minutes ago) Hello, f2 added - David Fonseca
| |/
* / 4ffa6bd - (14 minutes ago) Hello, f1 added - David Fonseca
|/
* 7227106 - (46 minutes ago) Initial commit - daafonsecato (origin/main, origin/HEAD)

╭╴㉿ david at …/flow-pr-test on  develop ()
🕙 10:08:59 PM
╰─ git push --all origin
Enumerating objects: 18, done.
Counting objects: 100% (18/18), done.
Delta compression using up to 8 threads
Compressing objects: 100% (12/12), done.
Writing objects: 100% (16/16), 1.55 KiB | 36.00 KiB/s, done.
Total 16 (delta 4), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (4/4), done.
To github.com:daafonsecato/flow-pr-test.git
   7227106..a37670f  main -> main
 * [new branch]      develop -> develop

╭╴㉿ david at …/flow-pr-test on  develop ()
🕙 10:09:57 PM
╰─ git push origin --tags
Enumerating objects: 1, done.
Counting objects: 100% (1/1), done.
Writing objects: 100% (1/1), 179 bytes | 29.00 KiB/s, done.
Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:daafonsecato/flow-pr-test.git
 * [new tag]         v1.0 -> v1.0

╭╴㉿ david at …/flow-pr-test on  develop ()
🕙 10:11:47 PM
╰─ git flow feature start f3
Switched to a new branch 'feature/f3'

Summary of actions:
- A new branch 'feature/f3' was created, based on 'develop'
- You are now on branch 'feature/f3'

Now, start committing on your feature. When done, use:

     git flow feature finish f3


╭╴㉿ david at …/flow-pr-test on  feature/f3 ()
🕙 10:16:41 PM
╰─ git add .

╭╴㉿ david at …/flow-pr-test on  feature/f3 (++(1))
🕙 10:17:15 PM
╰─ git commit -m "f3 added"
[feature/f3 433aa8f] f3 added
 1 file changed, 1 insertion(+)
 create mode 100644 f3.txt

╭╴㉿ david at …/flow-pr-test on  feature/f3 ()
🕙 10:17:26 PM
╰─ git push origin HEAD
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 293 bytes | 29.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'feature/f3' on GitHub by visiting:
remote:      https://github.com/daafonsecato/flow-pr-test/pull/new/feature/f3
remote:
To github.com:daafonsecato/flow-pr-test.git
 * [new branch]      HEAD -> feature/f3

╭╴㉿ david at …/flow-pr-test on  feature/f3 ()
🕙 10:17:35 PM
╰─ git flow feature publish f3
branch 'feature/f3' set up to track 'origin/feature/f3'.
Everything up-to-date
Already on 'feature/f3'
Your branch is up to date with 'origin/feature/f3'.

Summary of actions:
- The remote branch 'feature/f3' was created or updated
- The local branch 'feature/f3' was configured to track the remote branch
- You are now on branch 'feature/f3'


╭╴㉿ david at …/flow-pr-test on  feature/f3 ( ) took 5s
🕙 10:17:49 PM
╰─ git add .

╭╴㉿ david at …/flow-pr-test on  feature/f3 (++(1) )
🕙 10:18:34 PM
╰─ git commit -m "f3 modified"
[feature/f3 ea2ae9e] f3 modified
 1 file changed, 2 insertions(+), 1 deletion(-)

╭╴㉿ david at …/flow-pr-test on  feature/f3 (⇡1)
🕙 10:18:41 PM
╰─ git tree
* ea2ae9e - (32 seconds ago) f3 modified - David Fonseca (HEAD -> feature/f3)
* 433aa8f - (2 minutes ago) f3 added - David Fonseca (origin/feature/f3)
*   8194bd2 - (10 minutes ago) Merge tag 'v1.0' into develop - David Fonseca (origin/develop, develop)
|\
| *   a37670f - (11 minutes ago) Merge branch 'release/v1.0' - David Fonseca (tag: v1.0, origin/main, origin/HEAD, main)
| |\
| | * 78c2a38 - (11 minutes ago) Ready for the release - David Fonseca
| |/
|/|
* |   eb754ca - (20 minutes ago) Merge branch 'feature/f2' into develop - David Fonseca
|\ \
| * | e8b76da - (22 minutes ago) Hello, f2 fixed - David Fonseca
| * | a43cc45 - (23 minutes ago) Hello, f2 added - David Fonseca
| |/
* / 4ffa6bd - (25 minutes ago) Hello, f1 added - David Fonseca
|/
* 7227106 - (56 minutes ago) Initial commit - daafonsecato

╭╴㉿ david at …/flow-pr-test on  feature/f3 (⇡1)
🕙 10:19:13 PM
╰─ git flow feature finish f3
Branches 'feature/f3' and 'origin/feature/f3' have diverged.
And local branch 'feature/f3' is ahead of 'origin/feature/f3'.
Switched to branch 'develop'
Merge made by the 'ort' strategy.
 f3.txt | 2 ++
 1 file changed, 2 insertions(+)
 create mode 100644 f3.txt
To github.com:daafonsecato/flow-pr-test.git
 - [deleted]         feature/f3
Deleted branch feature/f3 (was ea2ae9e).

Summary of actions:
- The feature branch 'feature/f3' was merged into 'develop'
- Feature branch 'feature/f3' has been locally deleted; it has been remotely deleted from 'origin'
- You are now on branch 'develop'


╭╴㉿ david at …/flow-pr-test on  develop () took 8s
🕙 10:19:34 PM
╰─ git tree
*   8eeca1b - (22 seconds ago) Merge branch 'feature/f3' into develop - David Fonseca (HEAD -> develop)
|\
| * ea2ae9e - (70 seconds ago) f3 modified - David Fonseca
| * 433aa8f - (2 minutes ago) f3 added - David Fonseca
|/
*   8194bd2 - (11 minutes ago) Merge tag 'v1.0' into develop - David Fonseca (origin/develop)
|\
| *   a37670f - (12 minutes ago) Merge branch 'release/v1.0' - David Fonseca (tag: v1.0, origin/main, origin/HEAD, main)
| |\
| | * 78c2a38 - (12 minutes ago) Ready for the release - David Fonseca
| |/
|/|
* |   eb754ca - (21 minutes ago) Merge branch 'feature/f2' into develop - David Fonseca
|\ \
| * | e8b76da - (22 minutes ago) Hello, f2 fixed - David Fonseca
| * | a43cc45 - (24 minutes ago) Hello, f2 added - David Fonseca
| |/
* / 4ffa6bd - (25 minutes ago) Hello, f1 added - David Fonseca
|/
* 7227106 - (57 minutes ago) Initial commit - daafonsecato