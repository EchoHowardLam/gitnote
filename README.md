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

---

Update local repo's HEAD branch based on the modified files
---
```
git add -A
git commit -m 'Type your commit message here'
```

---

Sync local repo to remote repo (pull all branch, push HEAD branch)
---
```
# Make sure that you already updated ALL LOCAL repo based on modified files
git pull
git push origin
```
---
