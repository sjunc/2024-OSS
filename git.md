
109-1@109-1-05 MINGW64 /c/2024-git-master
$ git config --system  core.autocrif true

109-1@109-1-05 MINGW64 /c/2024-git-master
$ git config --global core.autocrif true

109-1@109-1-05 MINGW64 /c/2024-git-master
$ git config --global core.autocrlf true

109-1@109-1-05 MINGW64 /c/2024-git-master
$ git config --global core.safecrlf false

109-1@109-1-05 MINGW64 /c/2024-git-master
$ git config --global core.editor'core --wait'
error: invalid key: core.editorcore --wait

109-1@109-1-05 MINGW64 /c/2024-git-master
$ git config --global core.editor'core--wait'

109-1@109-1-05 MINGW64 /c/2024-git-master
$ git config --global core.editor'core --wait'
error: invalid key: core.editorcore --wait

109-1@109-1-05 MINGW64 /c/2024-git-master
$ git config --global user.name sjunc

109-1@109-1-05 MINGW64 /c/2024-git-master
$ git config --global core.editor ‘code --wait’

109-1@109-1-05 MINGW64 /c/2024-git-master
$ git config --global user.email tjdwns4248@gmail.com

109-1@109-1-05 MINGW64 /c/2024-git-master
$ init.defaultBranch main
bash: init.defaultBranch: command not found

109-1@109-1-05 MINGW64 /c/2024-git-master
$ git config --global init.defaultBranch main

109-1@109-1-05 MINGW64 /c/2024-git-master
$ git init gfirst
Initialized empty Git repository in C:/2024-git-master/gfirst/.git/

109-1@109-1-05 MINGW64 /c/2024-git-master
$ git init gfirst
Initialized empty Git repository in C:/2024-git-master/gfirst/.git/

109-1@109-1-05 MINGW64 /c/2024-git-master
$

109-1@109-1-05 MINGW64 /c/2024-git-master
$ git config --global --edit
hint: Waiting for your editor to close the file... error: cannot spawn ‘code: No such file or directory
error: unable to start editor '‘code'

109-1@109-1-05 MINGW64 /c/2024-git-master
$ git config --global --edit
hint: Waiting for your editor to close the file... error: cannot spawn ‘code: No such file or directory
error: unable to start editor '‘code'

109-1@109-1-05 MINGW64 /c/2024-git-master
$ ^C

109-1@109-1-05 MINGW64 /c/2024-git-master
$ git config --global core.editor ‘code --wait’

109-1@109-1-05 MINGW64 /c/2024-git-master
$ git config --global --edit
hint: Waiting for your editor to close the file... error: cannot spawn ‘code: No such file or directory
error: unable to start editor '‘code'

109-1@109-1-05 MINGW64 /c/2024-git-master
$ git config --global core.editor 'code --wait'
warning: core.editor has multiple values
error: cannot overwrite multiple values with a single value
       Use a regexp, --add or --replace-all to change core.editor.

109-1@109-1-05 MINGW64 /c/2024-git-master
$ git config --global --edit
hint: Waiting for your editor to close the file... error: cannot spawn ‘code: No such file or directory
error: unable to start editor '‘code'

109-1@109-1-05 MINGW64 /c/2024-git-master
$ git init gfirst
Initialized empty Git repository in C:/2024-git-master/gfirst/.git/

109-1@109-1-05 MINGW64 /c/2024-git-master
$ cd gfirts
bash: cd: gfirts: No such file or directory

109-1@109-1-05 MINGW64 /c/2024-git-master
$ cd gfirst

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ echo A > basic

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ cat basic
A

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git add basic

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git status --short
A  basic

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   basic


109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git commit -m 1
[main (root-commit) 2725633] 1
 1 file changed, 1 insertion(+)
 create mode 100644 basic

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git log
commit 27256335e83b32db44fba16c186f39758ba84205 (HEAD -> main)
Author: sjunc <tjdwns4248@gmail.com>
Date:   Mon Oct 7 16:06:13 2024 +0900

    1

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git log --patch
commit 27256335e83b32db44fba16c186f39758ba84205 (HEAD -> main)
Author: sjunc <tjdwns4248@gmail.com>
Date:   Mon Oct 7 16:06:13 2024 +0900

    1

diff --git a/basic b/basic
new file mode 100644
index 0000000..f70f10e
--- /dev/null
+++ b/basic
@@ -0,0 +1 @@
+A

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git diff

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git diff --staged HEAD

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git diff HEAD

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git log --oneline
2725633 (HEAD -> main) 1

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ echo B >> basic

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ cat basic
A
B

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git commit -am 2
[main b40f082] 2
 1 file changed, 1 insertion(+)

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git log
commit b40f082f984396f8c414395e58dd575e6e9abd74 (HEAD -> main)
Author: sjunc <tjdwns4248@gmail.com>
Date:   Mon Oct 7 16:10:43 2024 +0900

    2

commit 27256335e83b32db44fba16c186f39758ba84205
Author: sjunc <tjdwns4248@gmail.com>
Date:   Mon Oct 7 16:06:13 2024 +0900

    1

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git log --patch
commit b40f082f984396f8c414395e58dd575e6e9abd74 (HEAD -> main)
Author: sjunc <tjdwns4248@gmail.com>
Date:   Mon Oct 7 16:10:43 2024 +0900

    2

diff --git a/basic b/basic
index f70f10e..35d242b 100644
--- a/basic
+++ b/basic
@@ -1 +1,2 @@
 A
+B

commit 27256335e83b32db44fba16c186f39758ba84205
Author: sjunc <tjdwns4248@gmail.com>
Date:   Mon Oct 7 16:06:13 2024 +0900

    1

diff --git a/basic b/basic
new file mode 100644
index 0000000..f70f10e
--- /dev/null
+++ b/basic
@@ -0,0 +1 @@
+A

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ echo C >> basic

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ echo C >> basic

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ cat basic
A
B
C

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git diff
diff --git a/basic b/basic
index 35d242b..b1e6722 100644
--- a/basic
+++ b/basic
@@ -1,2 +1,3 @@
 A
 B
+C

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git diff HEAD
diff --git a/basic b/basic
index 35d242b..b1e6722 100644
--- a/basic
+++ b/basic
@@ -1,2 +1,3 @@
 A
 B
+C

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git diff --staged HEAD

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git add basic

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git diff

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git diff --staged HEAD
diff --git a/basic b/basic
index 35d242b..b1e6722 100644
--- a/basic
+++ b/basic
@@ -1,2 +1,3 @@
 A
 B
+C

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git diff HEAD
diff --git a/basic b/basic
index 35d242b..b1e6722 100644
--- a/basic
+++ b/basic
@@ -1,2 +1,3 @@
 A
 B
+C

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git commit -m 3
[main 93685a3] 3
 1 file changed, 1 insertion(+)

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git diff HEAD

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git diff --staged HEAD

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git log
commit 93685a324e95f0ca4da72b70f9f1407b413511c5 (HEAD -> main)
Author: sjunc <tjdwns4248@gmail.com>
Date:   Mon Oct 7 16:18:08 2024 +0900

    3

commit b40f082f984396f8c414395e58dd575e6e9abd74
Author: sjunc <tjdwns4248@gmail.com>
Date:   Mon Oct 7 16:10:43 2024 +0900

    2

commit 27256335e83b32db44fba16c186f39758ba84205
Author: sjunc <tjdwns4248@gmail.com>
Date:   Mon Oct 7 16:06:13 2024 +0900

    1

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git log -oneline
fatal: unrecognized argument: -oneline

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git log --oneline
93685a3 (HEAD -> main) 3
b40f082 2
2725633 1

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git checkout HEAD~2
Note: switching to 'HEAD~2'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at 2725633 1

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst ((2725633...))
$ cat basic
A

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst ((2725633...))
$ get log
bash: get: command not found

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst ((2725633...))
$ git log
commit 27256335e83b32db44fba16c186f39758ba84205 (HEAD)
Author: sjunc <tjdwns4248@gmail.com>
Date:   Mon Oct 7 16:06:13 2024 +0900

    1

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst ((2725633...))
$ git log --oneline
2725633 (HEAD) 1

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst ((2725633...))
$

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst ((2725633...))
$ git log --oneline --all
93685a3 (main) 3
b40f082 2
2725633 (HEAD) 1

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst ((2725633...))
$ git config --global alias.co checkout

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst ((2725633...))
$ git co main
Previous HEAD position was 2725633 1
Switched to branch 'main'

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ cat basic
A
B
C

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git co HEAD~1
Note: switching to 'HEAD~1'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at b40f082 2

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst ((b40f082...))
$ cat basic
A
B

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst ((b40f082...))
$ git co HEAD^
Previous HEAD position was b40f082 2
HEAD is now at 2725633 1

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst ((2725633...))
$ git log --oneline --all
93685a3 (main) 3
b40f082 2
2725633 (HEAD) 1

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst ((2725633...))
$ cat basic
A

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst ((2725633...))
$ git log --all
commit 93685a324e95f0ca4da72b70f9f1407b413511c5 (main)
Author: sjunc <tjdwns4248@gmail.com>
Date:   Mon Oct 7 16:18:08 2024 +0900

    3

commit b40f082f984396f8c414395e58dd575e6e9abd74
Author: sjunc <tjdwns4248@gmail.com>
Date:   Mon Oct 7 16:10:43 2024 +0900

    2

commit 27256335e83b32db44fba16c186f39758ba84205 (HEAD)
Author: sjunc <tjdwns4248@gmail.com>
Date:   Mon Oct 7 16:06:13 2024 +0900

    1

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst ((2725633...))
$ git co main
Previous HEAD position was 2725633 1
Switched to branch 'main'

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git config --global alias.la 'log --all'

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ la
bash: la: command not found

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git la
commit 93685a324e95f0ca4da72b70f9f1407b413511c5 (HEAD -> main)
Author: sjunc <tjdwns4248@gmail.com>
Date:   Mon Oct 7 16:18:08 2024 +0900

    3

commit b40f082f984396f8c414395e58dd575e6e9abd74
Author: sjunc <tjdwns4248@gmail.com>
Date:   Mon Oct 7 16:10:43 2024 +0900

    2

commit 27256335e83b32db44fba16c186f39758ba84205
Author: sjunc <tjdwns4248@gmail.com>
Date:   Mon Oct 7 16:06:13 2024 +0900

    1

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git config --global edit
error: key does not contain a section: edit

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git config --global --edit
hint: Waiting for your editor to close the file... error: cannot spawn ‘code: No such file or directory
error: unable to start editor '‘code'

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git config --global --edit
hint: Waiting for your editor to close the file... error: cannot spawn ‘code: No such file or directory
error: unable to start editor '‘code'

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git config -- global -- edit
error: key does not contain a section: global

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git config --global alias.lal '--all --oneline'

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git config --global alias.lgl '--oneline'

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git lgl
unknown option: --oneline
usage: git [-v | --version] [-h | --help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--no-lazy-fetch]
           [--no-optional-locks] [--no-advice] [--bare] [--git-dir=<path>]
           [--work-tree=<path>] [--namespace=<name>] [--config-env=<name>=<envvar>]
           <command> [<args>]

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git lal
unknown option: --all
usage: git [-v | --version] [-h | --help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--no-lazy-fetch]
           [--no-optional-locks] [--no-advice] [--bare] [--git-dir=<path>]
           [--work-tree=<path>] [--namespace=<name>] [--config-env=<name>=<envvar>]
           <command> [<args>]

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$ git log --oneline --graph
* 93685a3 (HEAD -> main) 3
* b40f082 2
* 2725633 1

109-1@109-1-05 MINGW64 /c/2024-git-master/gfirst (main)
$
