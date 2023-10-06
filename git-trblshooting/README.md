# Git troubleshooting  

### Merge Conflicts:  
Merge conflicts occur when Git cannot automatically merge changes from one branch into another due to conflicting changes in the same code. You need to resolve the conflicts manually.  
```
# Create a conflict by changing the same lines in two branches
git checkout main
echo "Change in main" >> file.txt
git commit -am "Change in main"
git checkout feature-branch
echo "Change in feature" >> file.txt
git commit -am "Change in feature"
git merge main
```
You will see a conflict marker in file.txt. Resolve the conflict, commit, and then complete the merge.  

### Detached HEAD State:  
The detached HEAD state occurs when you check out a specific commit instead of a branch. It's not recommended for making changes.  
```
# Check out a commit directly, putting the repo in a detached HEAD state
git checkout commit-hash
```
To work in a branch, create a new branch or checkout an existing one.  

### Push Rejected:  
Push rejection happens when you try to push changes that conflict with the remote repository. You may need to pull changes first.  
```
git push origin main
# If rejected, pull changes and then push
git pull origin main
git push origin main
```

### Untracked Files:  
Untracked files are files that Git doesn't manage. To start tracking them:
```
# Add untracked files to staging
git add file.txt
```

### Accidental Commit:  
If you accidentally commit something, you can amend the last commit:  
```
git commit --amend
```

### Deleted Branch:  
If you accidentally delete a branch, you can usually recover it using the reflog:  
```
# Find the commit where the branch was deleted
git reflog
# Restore the branch
git checkout -b branch-name commit-hash
```

### Reverting a Commit:  
To undo a previous commit, you can use git revert:  
```
# Revert the last commit
git revert HEAD
```
This creates a new commit that undoes the changes made by the previous commit.  

### Resetting to a Previous Commit:  
To reset your branch to a previous commit (use with caution):  
```
# Reset to a previous commit
git reset --hard commit-hash
```