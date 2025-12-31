

 EXPERIMENT – 4 : Clone & Merge Conflict (GitHub)
Clone Repository
git clone https://github.com/octocat/Hello-World.git
cd Hello-World


(Merge conflict is resolved on GitHub UI — no command required)

 EXPERIMENT – 5 : Revert, Merge, Rebase
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

 EXPERIMENT – 6 : Push to GitHub
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
