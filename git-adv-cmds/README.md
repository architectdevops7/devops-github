# Git advanced commands

### Git Rebase:   
git rebase is used to move or combine a sequence of commits to a new base commit. It's often used to integrate changes from one branch into another while maintaining a linear commit history. Here's how it works:  

**Start with a feature branch and switch to it**  
git checkout feature-branch  

**Rebase the feature branch onto the main branch**  
git rebase main  

In this example, the changes made in feature-branch are reapplied on top of the latest changes in main. This results in a linear commit history.  

### Git Cherry-Pick:  
git cherry-pick is used to apply a specific commit from one branch onto another branch. It's helpful when you want to selectively bring in changes without merging entire branches. Here's an example:  

**Check out the branch where you want to apply the commit**  
git checkout target-branch  

**Cherry-pick a specific commit from another branch**  
git cherry-pick commit-hash  

This command applies the changes from the specified commit (commit-hash) onto the current branch (target-branch).  

### Git Stash:  
git stash allows you to temporarily save changes that you're not ready to commit yet, so you can work on something else or switch branches without committing half-done work. Here's how to use it:  

**Stash changes**  
git stash save "Work in progress"  

**Switch to a different branch or perform other operations**  
git checkout other-branch  

**Apply the stashed changes back**  
git stash apply  

You can also use git stash pop to apply and remove the most recent stash.  

These Git commands are useful for managing changes, rebasing branches, selectively applying commits, and temporarily saving your work in progress.  s