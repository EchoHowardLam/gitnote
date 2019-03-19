Concepts
---
1. Repository is a data storage for code
2. Your computer has a LOCAL repo
3. The git server holds a REMOTE repo
4. Modification to files does not update LOCAL repo until you tell git to do so
5. HEAD is a pointer pointing at the branch you are currently in

---

Branch manipulations
---
```
# You should see a list of branches, master is main branch,
# * means you are in that branch, so HEAD and * points to same branch
git branch

# Create new branch, does not move to that new branch
git branch NewBranchName

# Set HEAD to BranchName, meaning moving to that branch
git checkout BranchName
```

Update local repo's HEAD branch based on the modified files
---
```
git add -A
git commit -m 'Type your commit message here'
```

Sync local repo to remote repo (pull all branch, push HEAD branch)
---
```
# Make sure that you already updated ALL LOCAL repo based on modified files
git pull
git push origin
```

Oh no, I screw up
---
```
# see which commit you wish to go back
git log --oneline

# if you only screw up the "git commit" and want to keep your file modifications
git reset [the target commit's hash value]

# else if you screw up the file modification too and want to reset file contents too
git reset [the target commit's hash value] --hard
```

Check current status
---
```
# See which file is modified but not updated to local repo
git status

# See history of commits
git log
```
