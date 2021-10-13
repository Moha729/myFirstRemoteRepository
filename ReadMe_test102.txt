Testing testing.

Microsoft Windows [Version 10.0.19043.1237]
(c) Microsoft Corporation. Alle rettigheder forbeholdes.

C:\Users\Dell 7480>cd Desktop

C:\Users\Dell 7480\Desktop>mkdir
The syntax of the command is incorrect.

C:\Users\Dell 7480\Desktop>mkdir test_repo

C:\Users\Dell 7480\Desktop>cd test_repo

C:\Users\Dell 7480\Desktop\test_repo>git init
Initialized empty Git repository in C:/Users/Dell 7480/Desktop/test_repo/.git/

C:\Users\Dell 7480\Desktop\test_repo>git commit
On branch master

Initial commit

nothing to commit (create/copy files and use "git add" to track)

C:\Users\Dell 7480\Desktop\test_repo>git add ReadMe_Repo_test101
fatal: pathspec 'ReadMe_Repo_test101' did not match any files

C:\Users\Dell 7480\Desktop\test_repo>git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        ReadMe_Repo_test101.txt

nothing added to commit but untracked files present (use "git add" to track)

C:\Users\Dell 7480\Desktop\test_repo>git add ReadMe_Repo_test101
fatal: pathspec 'ReadMe_Repo_test101' did not match any files

C:\Users\Dell 7480\Desktop\test_repo>git add ReadMe_Repo_test101
fatal: pathspec 'ReadMe_Repo_test101' did not match any files

C:\Users\Dell 7480\Desktop\test_repo>git add ReadMe_Repo_test101.txt

C:\Users\Dell 7480\Desktop\test_repo>git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   ReadMe_Repo_test101.txt


C:\Users\Dell 7480\Desktop\test_repo>git commit -m"added ReadMe_Repo_test101.txt"
[master (root-commit) 8feff65] added ReadMe_Repo_test101.txt
 1 file changed, 1 insertion(+)
 create mode 100644 ReadMe_Repo_test101.txt

C:\Users\Dell 7480\Desktop\test_repo>git status
On branch master
nothing to commit, working tree clean

C:\Users\Dell 7480\Desktop\test_repo>git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   ReadMe_Repo_test101.txt

no changes added to commit (use "git add" and/or "git commit -a")

C:\Users\Dell 7480\Desktop\test_repo>git add .

C:\Users\Dell 7480\Desktop\test_repo>git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   ReadMe_Repo_test101.txt


C:\Users\Dell 7480\Desktop\test_repo>git commit -m "made changes"
[master 83c0f51] made changes
 1 file changed, 3 insertions(+), 1 deletion(-)

C:\Users\Dell 7480\Desktop\test_repo>git checkout -b newBranch1
Switched to a new branch 'newBranch1'

C:\Users\Dell 7480\Desktop\test_repo>git add .

C:\Users\Dell 7480\Desktop\test_repo>git commit -m "first commit on newBranch1"
[newBranch1 e4063dd] first commit on newBranch1
 1 file changed, 3 insertions(+), 1 deletion(-)

C:\Users\Dell 7480\Desktop\test_repo>git chechout master
git: 'chechout' is not a git command. See 'git --help'.

The most similar command is
        checkout

C:\Users\Dell 7480\Desktop\test_repo>git chechout master
git: 'chechout' is not a git command. See 'git --help'.

The most similar command is
        checkout

C:\Users\Dell 7480\Desktop\test_repo>git checkout master
Switched to branch 'master'

C:\Users\Dell 7480\Desktop\test_repo>git add .

C:\Users\Dell 7480\Desktop\test_repo>git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   ReadMe_test102.txt


C:\Users\Dell 7480\Desktop\test_repo>git commit -m "Created second file"
[master 5678d1c] Created second file
 1 file changed, 1 insertion(+)
 create mode 100644 ReadMe_test102.txt

C:\Users\Dell 7480\Desktop\test_repo>git checkout newBranch
error: pathspec 'newBranch' did not match any file(s) known to git

C:\Users\Dell 7480\Desktop\test_repo>git checkout newBranch1
Switched to branch 'newBranch1'

C:\Users\Dell 7480\Desktop\test_repo>git merge master
Merge made by the 'recursive' strategy.
 ReadMe_test102.txt | 1 +
 1 file changed, 1 insertion(+)
 create mode 100644 ReadMe_test102.txt

C:\Users\Dell 7480\Desktop\test_repo>git checkout master
Switched to branch 'master'

C:\Users\Dell 7480\Desktop\test_repo> git merge newBranch1
Updating 5678d1c..7d549b1
Fast-forward
 ReadMe_Repo_test101.txt | 4 +++-
 1 file changed, 3 insertions(+), 1 deletion(-)

C:\Users\Dell 7480\Desktop\test_repo>git status
On branch master
nothing to commit, working tree clean

C:\Users\Dell 7480\Desktop\test_repo>