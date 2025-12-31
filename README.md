✅ EXPERIMENT – 1 : Basic Git Commands
git init
git status
git add file.txt
git commit -m "Initial commit"
git log
git config --global user.name "ABC"
git config --global user.email "ABC@gmail.com"
git config --list

✅ EXPERIMENT – 2 : Creating & Managing Branches
Create Branch
git branch feature
git branch

Switch Branch
git checkout feature

Merge Feature into Master
git checkout master
git merge feature

Check Merged / Not Merged Branches
git branch --merged
git branch --no-merged

✅ EXPERIMENT – 3 : Ignore Files, Checkout, Cherry-Pick
Ignore Files using .gitignore
touch a.txt b.txt Customer.java
mkdir logs
touch logs/server.log
notepad .gitignore


.gitignore content

*.txt
logs/
.*

git status

Checkout Difference
git checkout feature
git checkout -b newbranch

Cherry-Pick Commit
git log --oneline
git checkout f1
git cherry-pick <commit-id>

✅ EXPERIMENT – 4 : Clone & Merge Conflict (GitHub)
Clone Repository
git clone https://github.com/octocat/Hello-World.git
cd Hello-World


(Merge conflict is resolved on GitHub UI — no command required)

✅ EXPERIMENT – 5 : Revert, Merge, Rebase
Git Revert
echo "first line" > newfile.txt
git add newfile.txt
git commit -m "commit 1"

echo "second line" > newfile.txt
git add newfile.txt
git commit -m "commit 2"

git log --oneline
git revert HEAD

Git Merge
git checkout master
git merge f1

Git Rebase
git checkout f1
git rebase master

✅ EXPERIMENT – 6 : Push to GitHub
Push to Master
git remote add origin <repo-url>
git push -u origin master

Push to Particular Branch
git checkout feature
git push origin feature

Push New Branch
git branch bug-fixes
git checkout bug-fixes
git push -u origin bug-fixes

✅ EXPERIMENT – 7 : Tags & Reset
Create Tag
git tag version1.0
git tag

Delete Tag
git tag -d version1.0
git push origin --delete version1.0

Git Reset
git reset --soft <commit-id>
git reset --mixed <commit-id>
git reset --hard <commit-id>

✅ EXPERIMENT – 8 : Stash & Show Commit
Git Stash
git stash
git stash list
git stash show
git stash pop
git stash apply
git stash drop stash@{0}
git stash clear

Show Commit Details
git log --oneline
git show <commit-id>
